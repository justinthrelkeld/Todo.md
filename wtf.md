todo.md is a markdown based todo list file, combining and expanding on the ideas of GitHub Flavored Markdown and Todo.txt. The aim is to create a human and machine readable file for storing projects, todos, and assignments in a way that is conducive to both individuals and teams.

Components
1. File/structure specification
2. Full file parser
3. Command line interface
4. Web application
5. Desktop application
6. Mobile application

# File Specification
Example file
```
- [ ] This is a top level task @someone #tagOrReference :project +due [http://link.com]
	- [ ] this indented item inherits everything from the top item, unless you specify something different.
	- [x] To mark something as complete, put an x in the box. Upper or lowercase should work
	- [ ] Due dates should be stored in a manner that elminates any potential ambiguity. The method will likely vary between implimentations.
	- [ ] Todos can contain !, !!, and !!!, which are rendered as priority tags


# Description

The todo file should be easy to read and should work with, not against the user's natural workflow.

Exclaimation points must always be treated as priority tags, with the number of marks coresponding directly to the priority level. If 0 is lowest priority, ! is level 1, !! is level 2, and !!! is level three. Except for when enclosed in quotes ! should always indicate priority, regardless of whether an application makes a distinction between one priority level and another.

Ideally, a distributed team based version would utilize some form of version control (i.e., Git) and some form of accessible sync (i.e. Dropbox).

required syntax to define a todo is `- [ ]`

Elements can indent infinitely(?) and children inherit all properties of their parent unless overridden their own property

# An update
After heavy use of the wonderful and amazing project management app Asana, I've been wondering how you could create a system like Asana that, at the end of the day, was based on todo.md.
This file would have a very low number of minimum elements but could scale to fit just about any need.
