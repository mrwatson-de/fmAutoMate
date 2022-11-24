[![fmAutoMate logo][fmAutoMate logo]][fmAutoMate home]

# fmAutoMate
[Towards a FileMaker IDE]

A tool for FileMaker developers from MrWatson which extends and automates your script workspace using the MBS-Plugin [and MrWatson's fmScriptWorkspace Module]
 
[Copyright](LICENSE) © 2021 MrWatson of www.mrwatson.de 

## Welcome to the closest thing to a FileMaker IDE you can get

Ever wanted an Integrated Developer Environment for your Filemaker Script Workspace? 

Or a menu in the script workspace where you can:

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


...all of which is open source?

...*and* extensible?

- with a built in context-menu editor
- and a calculation editor
  - with calculation syntax highlighting and syntax-checking
  - with built-in help for MBS functions and MBS menu-calls
  - with support for code-blocks, parameters and If / Else blocks in calculations

Yeah?

Well, now you have it!

Not only that, but also [fmAutoMate-Service extensions](fmAutoMate-Service/README.md) for your calculation editor!

Have fun!

MrWatson

![mrwatson.de logo][mrwatson.de logo]

(*) Note: experimental / uses a DDR / success depends on your parameter passing conventions / customizable / demonstrates the possibilities / really exciting

P.S. Since fmAutoMate has been in successful use for over a year(*) I consider it no longer a proof-of-concept thing, but rather a beta, which means...

- You are welcome to contribute - menu items - ideas - code!
- There are still issues - see the [wiki][fmAutoMate wiki].

(*) at least by me, and possibly even somebody else ;-]

## Quickstart

1. First up, get yourself the latest [MBS-Plugin][MBS-Plugin]
2. Download `fmAutoMate.zip` from the [latest release on Github][fmAutoMate releases]
   > Note: The release zip contains the pretty Mac file icons, which the `Code > Download zip file` lacks
4. Unzip and copy the fmAutoMate folder to your Applications folder, or to anywhere on your drive
   > Note: If you have [fmWorkMate][fmWorkMate home] and would like to be able to start fmAutoMate from the fmWorkMate toolbox, place the fmAutoMate folder *next to* the fmWorkMate folder!
5. Open fmAutoMate in FileMaker Pro
6. Press the fmAutoMate button to define your fmAutoMate context menu
7. Open up a script in your Script Workspace, for example, by pressing the [Edit Test Script] button :D
8. Select some code,
9. Right-click to get your fmAutoMate context menu!

Click a menu item and have fun developing in an increasingly integrated environment!

## Dependencies

- A Mac (Required)
  - Sorry Win-guys, there's nothing I can do to change this.
- FileMaker (Required)
- [MBS-Plugin][MBS-Plugin] (Required)
  - Version 0.13 of fmAutoMate now uses MBS Plugin version 11.2.0.07 to improve the search function to find the correct line - even when the script has multi-line comments - so make sure you are up to date!
- [fmScriptWorkspace Module][fmScriptWorkspace home] (Optional)
  - If you wish to have *really cool integration*, you'll need / want to install the [fmScriptWorkspace Module][fmScriptWorkspace home] in your Database files.
  - This module allows fmAutoMate to open scripts in the FileMaker script workspace

## Tips & Tricks

These might help you take your second steps with fmWorkmate
- [Turn HotKeys On after Restarting FileMaker](https://github.com/mrwatson-de/fmAutoMate/wiki/How-to#turn-hotkeys-on-after-restarting-filemaker)
- [Turn HotKeys Off, if they cause Interference](https://github.com/mrwatson-de/fmAutoMate/wiki/How-to#turn-hotkeys-off-if-they-cause-interference)
- [Roll your own functions](https://github.com/mrwatson-de/fmAutoMate/wiki/How-to#roll-your-own-functions)


## Links

- [fmAutoMate home][fmAutoMate home]
- [fmAutoMate wiki][fmAutoMate wiki]
- [fmAutoMate repo][fmAutoMate repo]
- [fmAutoMate latest release][fmAutoMate releases]



[fmAutoMate home]:https://www.fmworkmate.com/fmautomate
[fmAutoMate wiki]:https://github.com/mrwatson-de/fmAutoMate/wiki
[fmAutoMate releases]:https://github.com/mrwatson-de/fmAutoMate/releases
[fmAutoMate repo]:https://github.com/mrwatson-de/fmAutoMate
[fmAutoMate logo]:fmAutoMate_Logo_256_sm.png
[fmCheckMate home]:https://www.fmworkmate.com/fmcheckmate
[fmScriptWorkspace home]:https://www.fmworkmate.com/fmscriptworkspace
[fmWorkMate home]:https://www.fmworkmate.com
[MBS-Plugin]:https://www.monkeybreadsoftware.com/filemaker/
[mrwatson.de logo]:www.mrwatson.de_neon_128.png
[mrwatson.de]:http://www.mrwatson.de
