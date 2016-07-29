# XRead Python Text Editor
## V1.1.2 +WE 1.1
## By poikNplop

A Python 3 and Tkinter Text Editor.

## Usage

To run:

   - $ python3 XRead.py

OR - $ chmod +x XRead.py && ./XRead.py

in the bash terminal. You may also need to replace `python3` in
the first command with `python` if you only have python 3 and not
python 2.

XRead works like a standard plain-text editor. Don't try and open
OpenOffice or Microsoft Word files. It won't work.

## Web Editor

The web editor is used as two things:

Another application (in the command replace `XRead.py` with
`XReadWeb.py`)

An addon to XRead.py allowing you to use xml/html importing and
exporting with the special tree style of writing. It works like
this (notice the tabs and double spaces):

`<a it='cheese'><b>text<c/></b>stuff<d><e>hmm<e/><f/></d>la</a>`

`
a '#'  '#'  '#' {'it':'cheese'}

	b '#' text '#' stuff '#' {}

		c '#'  '#'  '#' {}

	d '#'  '#' la '#' {}

		e '#'  '#'  '#' {}

		f '#'  '#'  '#' {}
`
Basically the system is:

`tagname '#' text '#' tailtext '#' {'attrib':'utes'}`

An emptier one:

`tagname '#'  '#'  '#' {}`

if the 5 was a space:

`tagname5'#'55'#'55'#'5{}`

This is also described in Help/Style in Web Editor or
Help/Web Editor Style in standard XRead.
