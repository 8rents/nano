# Functions in Nano and binding them

> *With the built in functions that Nano provides, we will be able to bind all the well tread, predictable keyboard shortcuts to the proper functions to make Nano modern and easy to use.*

---

The following is a list of built in functions in nano. They each or multiple ones can be bound to a specific keyboard shortcut. 

## Modernizing Nano's keyboard shortcuts

Following consistency with other major browsers and environments.

## The Useful functions that deserve bindings

- __`help`__ - `^?`-  Invokes the help viewer.
- __`cancel^d`__ - `esc` - Cancels the current command.
- __`exit`__ - `^w` - Exits from the program (or from the help viewer or file browser).
- __`writeout`__ - `^S` -  Writes the current buffer to disk, asking for a name.
- __`savefile`__ - `^s` - Writes the current file to disk without prompting.
- __`whereis`__ - `^f` - Starts a 2forward search for text in the c22urrent buffer — or for filenames matching a string in the current list in the file browser.
- __`wherewas`__ - `^!F` - Starts a backward search for text in the current buffer — or for filenames matching a string in the current list in the file browser.
- __`findprevious`__ - `^!f` -  Searches the next occurrence in the backward direction.
- __`findnext`__ - `^g` -  Searches the next occurrence in the forward direction.
- __`replace`__ - `^!@f` -  Interactively replaces text within the current buffer.
- __`cut`__ - `^x` -  Cuts and stores the current line (or the marked region).
- __`copy`__ - `^c` - Copies the current line (or the marked region) without deleting it.
- __`paste`__ - `^v` - Pastes the currently stored text into the current buffer at the current cursor position.
- __`mark`__ - `^m` - Sets the mark at the current position, to start selecting text. Or, when it is set, unsets the mark.
- __`zero`__ - `^k` - Toggles the presence of title bar and status bar.
- __`softwrap`__ - `^!w` - Toggles the displaying of overlong lines on multiple screen lines.
- __`linenumbers`__ - `^!l` - Toggles the display of line numbers in front of the text.
- __`nosyntax`__ - `^k` - Toggles syntax highlighting.
- __`firstfile`__ - `^a`  Goes to the first file in the list when using the file browser.
- __`lastfile`__ - `^e` - Goes to the last file in the list when using the file browser.
- __`nohelp`__ - `^?` - Toggles the presence of the two-line list of key bindings at the bottom of the screen. (This toggle is special: it is available in all menus except the help viewer and the linter. All further toggles are available in the main menu only.)

## All Valid function names to be bound are:

> ### Keyboard shortcut symbnols
>
> - `^` - Control
> - `!` - Shift
> - `@` - Alt

- __`help`__ - `^?`-  Invokes the help viewer.
- __`cancel^d`__ - `esc` - Cancels the current command.
- __`exit`__ - `^w` - Exits from the program (or from the help viewer or file browser).
- __`writeout`__ - `^S` -  Writes the current buffer to disk, asking for a name.
- __`savefile`__ - `^s` - Writes the current file to disk without prompting.
- __`insert`__ - Inserts a file into the current buffer (at the current cursor position), or into a new buffer when option multibuffer is set.
- __`whereis`__ - `^f` - Starts a 2forward search for text in the c22urrent buffer — or for filenames matching a string in the current list in the file browser.
- __`wherewas`__ - `^!F` - Starts a backward search for text in the current buffer — or for filenames matching a string in the current list in the file browser.
- __`findprevious`__ - `^!f` -  Searches the next occurrence in the backward direction.
- __`findnext`__ - `^g` -  Searches the next occurrence in the forward direction.
- __`replace`__ - `^!@f` -  Interactively replaces text within the current buffer.
- __`cut`__ - `^x` -  Cuts and stores the current line (or the marked region).
- __`copy`__ - `^c` - Copies the current line (or the marked region) without deleting it.
- __`paste`__ - `^v` - Pastes the currently stored text into the current buffer at the current cursor position.
- __`zap`__ - Throws away the current line (or the marked region). (This function is bound by default to `Meta+Delete`.)
- __`chopwordleft`__ - Deletes from the cursor position to the beginning of the preceding word. This function is bound by default to `^!+Delete`. If your terminal produces ^H for `^+Backspace`, you can make `^+Backspace`delete the word to the left of the cursor by rebinding ^H to this function.
- __`chopwordright`__ - Deletes from the cursor position to the beginning of the next word. (This function is bound by default to `^+Delete`.)
- __`cutrestoffile`__ - Cuts all text from the cursor position till the end of the buffer.
- __`mark`__ - `^m` - Sets the mark at the current position, to start selecting text. Or, when it is set, unsets the mark.
- __`location`__ - Reports the current position of the cursor in the buffer: the line, column, and character positions.
- __`wordcount`__ - Counts and reports on the status bar the number of lines, words, and characters in the current buffer (or in the marked region).
- __`execute`__ - Prompts for a program to execute. The program’s output is inserted into the current buffer — or into a new buffer when M-F is toggled. When the program’s name is preceded by a pipe symbol (|), then the current buffer (or the marked region) is piped to the program, and the output of the program replaces the buffer (or the marked region).
- __`speller`__ - `^e`- Invokes a spell-checking program, either the default hunspell(1) or GNU spell(1), or the one defined by --speller or set speller.
- __`formatter`__ - `^L` - Invokes a full-buffer-processing program (if the active syntax defines one). (The current buffer is written out to a temporary file, the program is run on it, and then the temporary file is read back in, replacing the contents of the buffer.)
- __`linter`__ - `^l` - Invokes a syntax-checking program (if the active syntax defines one). If this program produces lines of the form "filename:linenum:charnum: some message", then the cursor is put at the indicated position in the mentioned file while showing "some message" on the status bar. You can move from message to message with <PgUp> and <PgDn>, and leave linting mode with ^C or <Enter>.
- __`justify`__ - Justifies the current paragraph (or the marked region). A paragraph is a group of contiguous lines that, apart from possibly the first line, all have the same indentation. The beginning of a paragraph is detected by either this lone line with a differing indentation or by a preceding blank line.
- __`fulljustify`__ - Justifies the entire current buffer (or the marked region).
- __`indent`__ - Indents (shifts to the right) the current line or the marked lines.
- __`unindent`__ - Unindents (shifts to the left) the current line or the marked lines.
- __`comment`__ - `^!m` - Comments or uncomments the current    line or the marked lines, using the comment style specified in the active syntax.
- __`complete`__ - Completes (when possible) the fragment before the cursor to a full word found elsewhere in the current buffer.
- __`left`__ - Goes left one position (in the editor or browser).
- __`right`__ - Goes right one position (in the editor or browser).
- __`up`__ - Goes one line up (in the editor or browser).
- __`down`__ - Goes one line down (in the editor or browser).
- __`scrollup`__ - Scrolls the viewport up one row (meaning that the text slides down) while keeping the cursor in the same text position, if possible. (This function is bound by default to `Alt+Up`. If `Alt+Up` does nothing on your Linux console, see the FAQ: <https://nano-editor.org/dist/latest/faq.html#4.1>
- __`scrolldown`__ - Scrolls the viewport down one row (meaning that the text slides up) while keeping the cursor in the same text position, if possible. (This function is bound by default to <Alt+Down>.)
- __`center`__ - Scrolls the line with the cursor to the middle of the viewport.
- __`cycle - Scrolls the line with the cursor first to the middle of the viewport, then to the top, then to the bottom.
- __`prevword`__ - Moves the cursor to the beginning of the previous word.
- __`nextword`__ - Moves the cursor to the beginning of the next word.
- __`home`__ - Moves the cursor to the beginning of the current line.
- __`end`__ - Moves the cursor to the end of the current line.
- __`beginpara`__ - Moves the cursor to the beginning of the current paragraph.
- __`endpara`__ - Moves the cursor to the end of the current paragraph.
- __`prevblock`__ - Moves the cursor to the beginning of the current or preceding block of text. (Blocks are separated by one or more blank lines.)
- __`nextblock`__ - Moves the cursor to the beginning of the next block of text.
- __`toprow`__ - Moves the cursor to the first row in the viewport.
- __`bottomrow`__ - Moves the cursor to the last row in the viewport.
- __`pageup`__ - Goes up one screenful.
- __`pagedown`__ - Goes down one screenful.
- __`firstline`__ - `^A` - Goes to the first line of the file.
- __`lastline`__ - `^E` - Goes to the last line of the file.
- __`gotoline`__ - `^l` - Goes to a specific line (and column if given). A negative number counts from the end of the buffer (and end of the line). Putting ++ or -- before the first number will jump the given number of lines forward or backward.
- __`findbracket`__ - Moves the cursor to the bracket (or brace or parenthesis, etc.) that matches (pairs) with the one under the cursor. See set matchbrackets.
- __`anchor`__ - Places an anchor at the current line, or removes it when already present. (An anchor is visible when line numbers are activated.)
- __`prevanchor`__ - Goes to the first anchor before the current line.
- __`nextanchor`__ - Goes to the first anchor after the current line.
- __`prevbuf`__ - Switches to editing/viewing the previous buffer when multiple buffers are open.
- __`nextbuf`__ - Switches to editing/viewing the next buffer when multiple buffers are open.
- __`verbatim`__ - Inserts the next keystroke verbatim into the file, or begins Unicode input when a hexadecimal digit is typed.
- __`tab`__ - Inserts a tab at the current cursor location.
- __`enter`__ - Inserts a new line below the current one.
- __`delete`__ - Deletes the character under the cursor.
- __`backspace`__ - Deletes the character before the cursor.
- __`recordmacro`__ - Starts the recording of keystrokes — the keystrokes are stored as a macro. When already recording, the recording is stopped.
- __`runmacro`__ - Replays the keystrokes of the last recorded macro.
- __`undo`__ - `^z` - Undoes the last performed text action (add text, delete text, etc).
- __`redo`__ - `^!z`- Redoes the last undone action (i.e., it undoes an undo).
- __`refresh`__ - `^!r` - Refreshes the screen.
- __`suspend`__ - Suspends the editor and returns control to the shell (until you tell the process to resume execution with fg).
- __`casesens`__ - Toggles whether searching/replacing ignores or respects the case of the given characters.
- __`regexp`__ - Toggles whether searching/replacing uses literal strings or regular expressions.
- __`backwards`__ - Toggles whether searching/replacing goes forward or backward.
- __`older`__ - Retrieves the previous (earlier) entry at a prompt.
- __`newer`__ - Retrieves the next (later) entry at a prompt.
- __`flipreplace`__ - Toggles between searching for something and replacing something.
- __`flipgoto`__ - Toggles between searching for text and targeting a line number.
- __`flipexecute`__ - Switches from inserting a file to executing a command.
- __`flippipe`__ - When executing a command, toggles whether the current buffer (or marked region) is piped to the command.
- __`flipnewbuffer`__ - Toggles between inserting into the current buffer and into a new empty buffer.
- __`flipconvert`__ - When reading in a file, toggles between converting and not converting it from DOS/Mac format. Converting is the default.
- __`dosformat`__ - When writing a file, switches to writing a DOS format (CR/LF).
- __`macformat`__ - When writing a file, switches to writing a Mac format.
- __`append`__ - When writing a file, appends to the end instead of overwriting.
- __`prepend`__ - When writing a file, "prepends" (writes at the beginning) instead of overwriting.
- __`backup`__ - When writing a file, creates a backup of the current file.
- __`discardbuffer`__ - When about to write a file, discard the current buffer without saving. (This function is bound by default only when option `--saveonexit` is in effect.)
- __`browser`__ - `^o` - Starts the file browser (in the Read File and Write Out menus), allowing to select a file from a list.
- __`gotodir`__ - Goes to a directory to be specified, allowing to browse anywhere in the filesystem.
- __`firstfile`__ - `^a`  Goes to the first file in the list when using the file browser.
- __`lastfile`__ - `^e` - Goes to the last file in the list when using the file browser.
- __`nohelp`__ - `^?` - Toggles the presence of the two-line list of key bindings at the bottom of the screen. (This toggle is special: it is available in all menus except the help viewer and the linter. All further toggles are available in the main menu only.)
- __`zero`__ - `^k` - Toggles the presence of title bar and status bar.
- __`constantshow`__ - Toggles the constant reporting (on the status bar) of the current line, column, and character positions.
- __`softwrap`__ - `^!w` - Toggles the displaying of overlong lines on multiple screen lines.
- __`linenumbers`__ - `^!l` - Toggles the display of line numbers in front of the text.
- __`whitespacedisplay`__ - Toggles the showing of whitespace.
- __`nosyntax`__ - `^k` - Toggles syntax highlighting.
- __`smarthome`__ - Toggles the smartness of the Home key.
- __`autoindent`__ - Toggles whether a newly created line will contain the same amount of leading whitespace as the preceding line — or as the next line if the preceding line is the beginning of a paragraph.
- __`cutfromcursor`__ - Toggles whether cutting text cuts the whole line or just from the current cursor position to the end of the line.
- __`breaklonglines`__ Toggles whether the overlong part of a line is hard-wrapped to the next line.
- __`tabstospaces`__ - Toggles whether typed tabs are converted to spaces.
- __`mouse`__  - Toggles mouse support

## Valid menu sections are:

- __`main`__  - The main editor window where text is entered and edited.
- __`help`__  - The help-viewer menu.
- __`search`__  - The search menu (AKA whereis).
- __`replace`__  - The ’search to replace’ menu.
- __`replacewith`__  - The ’replace with’ menu, which comes up after ’search to replace’.
- __`yesno`__  - The ’yesno’ menu, where the Yes/No/All/Cancel question is asked.
- __`gotoline`__  - The ’goto line (and column)’ menu.
- __`writeout`__  - The ’write file’ menu.
- __`insert`__  - The ’insert file’ menu.
- __`browser`__  - The ’file browser’ menu, for selecting a file to be opened or inserted or written to.
- __`whereisfile`__  - The ’search for a file’ menu in the file browser.
- __`gotodir - The ’go to directory’ menu in the file browser.
- __`execute`__  - The menu for inserting the output from an external command, or for filtering the buffer (or the marked region) through an external command, or for executing one of several tools.
- __`spell`__  - The menu of the integrated spell checker where the user can edit a misspelled word.
- __`linter`__  - The linter menu, which allows jumping through the linting messages.
- __`all`__ - A special name that encompasses all menus. For bind it means all menus where the specified function exists; for unbind it means all menus where the specified key exists.


### EXAMPLES

To make `Ctrl+Z` suspend nano:

```
bind ^Z suspend main
```

To make `Shift+Alt+C` copy the marked region to the system’s clipboard:

```
bind Sh-M-C "{execute}| xsel -ib {enter}{undo}" main
```