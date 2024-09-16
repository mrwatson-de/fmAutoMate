# fmAutoMate-Services

fmAutoMate-Services are extensions for your FileMaker calculation editor - indeed *for any text editor or field*. (That's because fmAutoMate-Services are macOS Services and integrate seamlessly into your entire Mac system.)

fmAutoMate-Services are optional, so make sure you press the `Install fmAutoMate-Services` button on the fmAutomate start page first! (See [Installing fmAutoMate-Services](Installing-fmAutoMate-Services.md) for more.)


## Using fmAutoMate-Services

Is a snip!

- Open the calculation editor in FileMaker and select some lines of code
- Right Click the text to show the context menu
- Choose one of the fmAutoMate-Services under `Services > fmAutoMate > ...`


## fmAutoMate-Services Reference


### Services > fmAutoMate > Clipboard

 `Services > fmAutoMate > Clipboard > Retype`

Retypes whatever is on the clipboard. Similar to pasting, but a tab character will jump to the next field.


### Services > fmAutoMate > Selected Text

`Services > fmAutoMate > Selected Text …`

Displays a toolbox of functions to apply to the currently selected text.

- Case functions:
  - `lowercase` - Changes the selected text to **lowercase**
  - `UPPERCASE` - Changes the selected text to **UPPERCASE**
  - `Title Case` - Changes the selected text to **Title Case**
  - `Normal case` - Changes the selected text to **Normal case**
  - -
  - `lowerCamelCase` - Changes the selected *words* to **lowerCamelCase**
  - `UpperCamelCase` - Changes the selected *words* to **UpperCamelCase**
  - `split⁁Camel⁁Case` - Splits the selected *CamelCasePhrase* into *words* by adding a space before each uppercase letter
  - -
  - `lower_snake_case` - Changes the selected text to **lower_snake_case**
  - `SCREAMING_SNAKE_CASE` - Changes the selected text to **SCREAMING_SNAKE_CASE**
  - `lower-kebab-case` - Changes the selected text to **lower-kebab-case**
  - `SCREAMING-KEBAB-CASE` - Changes the selected text to **SCREAMING-KEBAB-CASE**
- EOL functions:
  - `Remove line breaks` - Removes line breaks entirely from the selected text
  - `Replace line breaks with space` - Replace line breaks within the selected text with a space
  - `Show line breaks` - Displays <CR> and <LF> in within the selected text to make line breaks visible
  - `Unshow line breaks` - Reinstates the original text by removeing the <CR> and <LF> markers from the selected text again
  - -
  - `CR` - Changes all line breaks in the selected text to **CR** (Carriage Return)
  - `CRLF` - Changes all line breaks in the selected text to **CRLF** (Carriage Return and Line Feed)
  - `LF` - Changes all line breaks in the selected text to **LF** (Line Feed)
- Calculation functions:
  - `Calculate (JavasSript)` - Displays a small Javascript calculator dialog
  - `Evaluate (JavaScript)` - Evaluates the selected text as Javascript
- fmIDE functions:
  - `fmIDE > Encode for URL` - Encodes the selected text as a URL parameter
  - `fmIDE > Link to Script` - Creates an fmIDE link to a script using the selected text as script name
- Line functions:
  - `Add line numbers` - Adds line numbers to the selected lines 
  - `Add Json Array Prefix` - Adds a JSON Array Prefix to the selected lines (`[0].`, `[1].`, etc.)
  - `Remove line numbers` - Removes the line numbers from the selected lines 
  - `Remove Json Array Prefix` - Removes the JSON Array Prefix to the selected lines

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
