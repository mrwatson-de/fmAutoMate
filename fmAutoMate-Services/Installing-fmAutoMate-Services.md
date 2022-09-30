# fmAutoMate-Services

fmAutoMate-Services are extensions for your FileMaker calculation editor - indeed for any text editor or even text field(*). That's because fmAutoMate-Services are macOS Services  and integrate seamlessly into your entire Mac system.

- Installing
- Using
- Deinstalling
- fmAutoMate-Services Reference

Once you have installed fmAutoMate in your FileMaker



## Installing fmAutoMate-Services

Installing fmAutoMate-Services…

- …from the fmAutoMate start page
- …from the fmAutoMate menu
- …from the Finder
- …optionally by default


### Installing fmAutoMate-Services from fmAutoMate

If you have already installed fmAutoMate in FileMaker you can install the Services directly from the fmAutoMate context menu:

- Open a script in the Script Workspace
- Right click on a step to get the fmAutoMate context menu
- Choose `fmAutoMate > Services > Install fmAutoMate-Services` menu to install the Services for your user.



### Installing fmAutoMate-Services from Finder

If you would like more control over which Services are installed fmAutoMate-Services can be installed individually from the Finder.

The Services files are in the fmAutoMate-Services / fmAM-Services folder

Just 

- double-click the file to automatically install it.

Note:

- This will *move* the file to the Services folder (~/Library/Services).
- If you would like to keep a copy of the file, then 
  1. First copy the files you want to install to a subfolder,
  2. and then double click them


### Installing fmAutoMate-Services by default

If you turn on the `Install fmAM-Services` setting in the fmAutoMate settings menu, the fmAutoMate-Services are installed automatically.

Note:

- This simply copies the files to the ~/Library/Services/ folder, and *overwites the files there*.

## Using an fmAutoMate-Service

Just

- Select and right click some text
- Select the Services menu
- Choose the function you need

Note:

- (*) The Services menu *does not* appear in normal FileMaker fields.

## Deinstalling fmAutoMate-Services

fmAutoMate-Services not what you need?

Then just…

- Open the Services folder (~/Library/Services).
- Delete any files you don't want
  - or move them back to the fmAutoMate-Service folder

## Using fmAutoMate-Services

- Open the calculation editor in FileMaker and type or select some lines of code(*)
- Right Click the selected text to show the context menu
- Choose one of the fmAutoMate-Services under `Services > fmAutoMate > ...`


## fmAutoMate-Services Reference



 `Services > fmAutoMate > Clipboard > Retype`

Retypes whatever is on the clipboard. Similar to pasting, but a tab character will jump to the next field.

`Services > fmAutoMate > Selected Text > Align Ampersand`

Aligns the first occurence of '&' in the selected lines by adding space before the term.

`Services > fmAutoMate > Selected Text > Align Comments > Block Comments`

Aligns the first occurence of '/*' in the selected lines by adding space before the term.


`Services > fmAutoMate > Selected Text > Align Comments > Line Comments`

Aligns the first occurence of '//' in the selected lines by adding space before the term.

`Services > fmAutoMate > Selected Text > Align Equals Sign`

Aligns the first occurence of '=' in the selected lines by adding space before the term.


`Services > fmAutoMate > Selected Text > Align Semi-Colon`

Aligns the first occurence of ';' in the selected lines by adding space before the term.

`Services > fmAutoMate > Selected Text > Sort`

Sorts the selected lines.
