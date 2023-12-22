[![fmAutoMate logo][fmAutoMate logo]][fmAutoMate home]

# fmAutoMate
[Towards a FileMaker IDE]

A tool for FileMaker developers which extends and automates your script workspace and FileMaker environment to provide you with some awesome functions to boost developer productivity (including, in some cases, making the impossible possible 😜).

[Copyright](LICENSE) © 2021-2024 MrWatson of www.mrwatson.de 

## Welcome to the closest thing to a FileMaker IDE you can get

Have you ever wanted

- more developer power at your finger tips in FileMaker?
- a context menu full of useful developer functions in the Filemaker Script Workspace? (search and replace, anybody?)
- Hot Keys to apply functions in FileMaker at the press of a key or two?
- functions in the calculation editor to format code or change case? (or calculate layout object coordinates, anyone?)
- a FileMaker Integrated Developer Environment, more like Visual Studio Code?

Yeah? Well, you have it now right in front of you!

Not sure yet? Then take a peek at the [Inspiring functionality](#inspiring-functionality) to get hooked.

Have fun!

MrWatson

![mrwatson.de logo][mrwatson.de logo]
 
## Quickstart

1. Check the requirements in [dependencies](#dependencies), below
2. Install the `MBS-Plugin``
   - If you don't have one, get yourself the latest [MBS-Plugin][MBS-Plugin].
3. Install the fmAutomate folder
   - Download `fmAutoMate.zip` from the [latest release on Github][fmAutoMate releases]
     > Note: The release zip contains pretty Mac file icons, which the `Code > Download zip file` lacks, however, if you want cutting edge functions that have not yet made it into a release, then you may want the `Code > Download zip file` anyhow.
   -  Unzip and rename the folder to `fmAutoMate`, if necessary.
   - Move/copy the `fmAutoMate`` folder to your Applications folder, or to anywhere on your drive.
   > Note: If you have [fmWorkMate][fmWorkMate home] and would like to be able to start fmAutoMate from the fmWorkMate toolbox, place the fmAutoMate folder *next to* the fmWorkMate folder!
5. Install & Test the fmAutoMate functionality
   - Open fmAutoMate in FileMaker Pro
   - Press the `[fmAutoMate]` button to define your fmAutoMate context menu
   - Test fmAutoMate Script Workspace context menu
      - Open up a script in your Script Workspace
      - Select some steps,
      - Right-click to get your fmAutoMate context menu!
      - Click a menu item and have fun developing in an increasingly integrated environment!
   - Test fmAutomate Extended Hot Keys dialog
     - Press `⌃⌘K` to open the Extended Hot Key function dialog.
     - Choose a function (or type the keys & press return) to apply a function.
6. Install & Test fmAutoMate Services
   - For extra functions in the calculation editor (or any text editor, or even field) [install the fmAutoMate-Service extensions](fmAutoMate-Services/README.md).
7. Review & Install Integration, as needed
   - See [Integrations](#integrations) below.

## Dependencies

Like most tools from MrWatson, fmAutoMate builds on fantastic MBS-Plugin functions on Mac. It also integrates with MrWatson's fmIDE module for maximum integration and developer fun, so…

- Required
  - **A Mac**
    - Sorry Win-guys, there's nothing I can do to change this.
  - **FileMaker**
    - but, of course, you already have that.
  - [MBS-Plugin][MBS-Plugin]
    - Version 0.13 of fmAutoMate needs at least MBS Plugin version 11.2.0.07 to improve the search function to find the correct line - even when the script has multi-line comments.
    - However, I recommend simply keeping your MBS Plugin up to date, because fmAutoMate and the MBS Plugin develop at a faster rate than this documentation. :)

See [Integrations](#integrations) below for further optional dependencies.

## Integrations

fmAutoMate integrates with several of MrWatson's other tools to bring you powerful functions saving you hours of work.

- Optional (recommended)
  - [fmIDE Module][fmIDE]
    - If you wish to have *really cool integrations*, you'll need / want to install the [fmIDE Module][fmIDE] in your Database files.
    - fmIDE is required for all the functions in the fmIDE sub menu
    - This module allows fmAutoMate to open scripts in the FileMaker script workspace
  - [fmCheckMate-XSLT Library][fmCheckMate-XSLT]
    - The fmCheckMate XSLT-Library is a free library of functions from MrWatson that, above all, add functionality to the FileMaker clipboard
    - If you want the *mega cool* Paste FileMaker Pseudocode functions, you'll need to download this library and place it in your Documents folder.
  - [fmWorkMate][fmWorkMate home] (inc. fmCheckMate)
    - fmWorkMate is a free toolbox of FileMaker power tools, above all containing MrWatson's fmCheckMate tool for editing, changing, transforming and transporting FileMaker code via the FileMaker clipboard.
- Optional
  - [fmScriptWorkspace Module][fmScriptWorkspace home]
    - The fmScriptWorkspace Module is the predecessor of fmIDE, so you probably won't need it.



## Inspiring functionality

- Search and Replace (variable names, field names, table names, etc...)
- Open Scripts in *other* files (you know, that thing that ⌘+Click *should* do - but doesn't)
- Copy script steps *directly* between local and remote databases (using Xut, Xopy & PaXte)
- [Insert a history comment](https://github.com/mrwatson-de/fmAutoMate/wiki/How-to#insert-a-history-comment) that 
  - *automatically enters the date and author*
  - in *your* desired format?
  - and that remembers it ready for the next script!
- [Insert pseudo-code](https://github.com/mrwatson-de/fmAutoMate/wiki/How-to#insert-pseudocode)
  ```
  $r=0
  $i=1
  $n=10
  Loop
    Exit Loop If [ $i > $n ]
    $r=$r+$i
    $i=$i+1
  End Loop
  Set Field [ _fmAutoMate::_gResult ; $r ]
  ```
  - Take a look at the [original twitter footage](https://twitter.com/mrwatson_de/status/1495553400347533313) of this function
- Save/load/insert code snippets
- Generate code automatically
  - by 'multiplying' steps by the values on the clipboard (seeing is believing!)
  - Refactor code
  - Perform code analysis, changes or transformations using [fmCheckMate][fmCheckMate home]
- Copy variable names, field names or calculations *without* having to open the script step / calculation editor
- Copy layout buttons and insert their steps into a script *directly* (really? Hell, yeah! 😎👍)
- Maybe even add the necessary parameters to a Perform Script call - completely automatically? (*)
- Oh yeah, and what about "Dock Window to Script Workspace" for those annoying floating windows you get from the debugger? 🤩 Wouldn't that just be phenomenal?
- Copy the current column of data from the active field?
  - Just type ⌘⌃K cc ⏎


...all of which is open source?

...*and* extensible?

- with a built in context-menu editor
- and a calculation editor
  - with calculation syntax highlighting and syntax-checking
  - with built-in help for MBS functions and MBS menu-calls
  - with support for code-blocks, parameters and If / Else blocks in calculations

(*) Note: experimental / uses a DDR / success depends on your parameter passing conventions / customizable / demonstrates the possibilities / really exciting

## Tips & Tricks

These might help you take your second steps with fmWorkmate
- [Turn HotKeys On after Restarting FileMaker](https://github.com/mrwatson-de/fmAutoMate/wiki/How-to#turn-hotkeys-on-after-restarting-filemaker)
- [Turn HotKeys Off, if they cause Interference](https://github.com/mrwatson-de/fmAutoMate/wiki/How-to#turn-hotkeys-off-if-they-cause-interference)
- [Roll your own functions](https://github.com/mrwatson-de/fmAutoMate/wiki/How-to#roll-your-own-functions)

## P.S.

Since fmAutoMate has now been in successful use for several years(*) I consider it no longer a proof-of-concept thing, but rather a beta, which means...

- You are welcome to contribute - menu items - ideas - code!
- There are still issues - see the [wiki][fmAutoMate wiki].

(*) at least by me, and possibly even somebody else ;-)

## Links

- [fmAutoMate home][fmAutoMate home]
- [fmAutoMate wiki][fmAutoMate wiki]
- [fmAutoMate repo][fmAutoMate repo]
- [fmAutoMate latest release][fmAutoMate releases]
- [fmIDE]



[fmAutoMate home]:https://www.fmworkmate.com/fmautomate
[fmAutoMate wiki]:https://github.com/mrwatson-de/fmAutoMate/wiki
[fmAutoMate releases]:https://github.com/mrwatson-de/fmAutoMate/releases
[fmAutoMate repo]:https://github.com/mrwatson-de/fmAutoMate
[fmAutoMate logo]:fmAutoMate_Logo_256_sm.png
[fmCheckMate home]:https://www.fmworkmate.com/fmcheckmate
[fmCheckMate-XSLT]:https://github.com/mrwatson-de/fmCheckMate-XSLT

[fmIDE]:https://github.com/fmIDE/fmIDE
[fmScriptWorkspace home]:https://www.fmworkmate.com/fmscriptworkspace
[fmWorkMate home]:https://www.fmworkmate.com
[MBS-Plugin]:https://www.monkeybreadsoftware.com/filemaker/
[mrwatson.de logo]:www.mrwatson.de_neon_128.png
[mrwatson.de]:http://www.mrwatson.de
