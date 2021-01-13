[![fmAutoMate logo][fmAutoMate logo]][fmAutoMate home]

# fmAutoMate
[Towards a FileMaker IDE]

A tool for FileMaker developers from MrWatson which extends and automates your script workspace using the MBS-Plugin and MrWatsons fmScriptWorkspace Module

[Copyright](LICENSE) © 2021 MrWatson of www.mrwatson.de 

## Welcome

Ever wanted an integrated Filemaker Script Workspace? 

Now you have it! Have fun!

MrWatson

![mrwatson.de logo][mrwatson.de logo]

P.S. Since fmAutoMate has been in successful use for over a year(*) I consider it no longer a proof-of-concept thing, but rather a beta, which means...

- You are welcome to contribute - menu items - ideas - code!
- There are still issues - see the [wiki][fmAutoMate wiki].

(*) at least by me, and possibly even somebody else ;-]

## Quickstart

1. First up, get yourself the latest [MBS-Plugin][MBS-Plugin]
2. Download fmAutoMate from [Github][fmAutoMate repo]
3. Open fmAutoMate in FileMaker Pro
4. Press the fmAutoMate button to define your fmAutoMate context menu
5. Open up a script in your Script Workspace, for example, by pressing the [Edit Test Script] button :D
6. Select some code,
7. Right-click to get your fmAutoMate context menu!

Click a menu item and have fun developing in an increasingly integrated environment!

## Tips & Tricks

These might help you take your second steps with fmWorkmate

### Turn HotKeys On after Restarting FileMaker

After closing and restarting FileMaker the fmAutoMate menu is still there, but the HotKeys have been forgotten.

To turn the HotKeys back on

- Right Click on a script step
- Choose fmAutoMate > HotKeys On

or

  - Open fmAutoMate
  - Click the [fmAutoMate] Button on the start page

### Turn HotKeys off, if they cause Interference

fmAutoMate HotKeys are currently defined globally on your computer, not just in FileMaker / Script Workspace.

If this interferes with your other apps

Turn HotKeys off 

  - Right Click on a script step
  - Choose fmAutoMate > HotKeys On

or

  - Open fmAutoMate
  - Click the [X HotKeys Off] Button on the start page

### Roll your own functions

It's not that difficult.

Basically,

- an fmAutoMate function is just the guts of a let statement (without the Let and the result bit)
- you can use MBS functions to do almost anthing you want
- there's a bunch of code blocks you can use that expand to 
- you can store blocks of text or stuff in parameters and then reference them from within the code (saves hours of escaping text!)

The best way to learn is by looking at the existing functions.


## Links

- [fmAutoMate home][fmAutoMate home]
- [fmAutoMate wiki][fmAutoMate wiki]
- [fmAutoMate repo][fmAutoMate repo]



[fmAutoMate home]:https://www.fmworkmate.com/fmautomate
[fmAutoMate wiki]:https://github.com/mrwatson-de/fmAutoMate/wiki
[fmAutoMate repo]:https://github.com/mrwatson-de/fmAutoMate
[fmAutoMate logo]:fmAutoMate_Logo_256_sm.png
[MBS-Plugin]:https://www.monkeybreadsoftware.com/filemaker/
[mrwatson.de logo]:www.mrwatson.de_neon_128.png
[mrwatson.de]:http://www.mrwatson.de
