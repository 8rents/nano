# Using Nano's File Browser & Opening Multiple Files at Once

> *...and other helpful tips*

---

## This Documents Table of Contents

- [Opening multiple files in Nano from the Command Line](#opening-multiple-files-from-the-command-line)
- [Cycle Through Files in Nano](#cycle-through-files-in-nano)
- [Opening Files Within Nano](#opening-files-within-nano)
- [Cut & Paste a Selection](#cut-&-paste-a-selection)
- [Run a Spell Check](#run-a-spellcheck)
- [Lint a File](#lint-a-file)
- [Reformat a File](#reformat-a-file)

---

This document contains advanced nano workflow tips and tricks.

## Opening multiple files from the Command Line

First make sure `set multibuffer` is in your nanorc. It's enabled on this repository's `nanorc`.

You can open as many files at once from your shell by adding them after the first.

```
nano file1.txt file2.txt
```

### Cycle through files in nano

Once you have multiple buffers open in Nano, you can cycle through them with `alt` + `,` or  `.`.

- **next file:** `alt + .`
- **prev file:** `alt + ,`

### Opening Files from within Nano

Once you're already in Nano you can still open up additional files in additional buffers (windows) using the file menu.

- **Open file by name** - `ctrl + r`
  > *You can `tab` complete the names*

## Selecting Text

One of those things we take for granted with modern editors

### Making a Selection

There's more than one way to make a selection

- `ctrl + m` to sticky selection on
- `shift + arrows` - guide selection
- `^a` - select all 

### Using the Selection

- `^c` - copy
- `^x` - cut. 
- `^v` - paste.

---

## Advanced Editing with External Programs

Nano has limited but some capability to use external programs to edit your documents.

### Run a Spellcheck

*working on this*

### Lint a File

*working on this too*

### Reformat a File

*and working on this as well...*


---

__(Ɔ) 2026__ [8rents](https://github.com/8rents) under the [MIT License](../LICENSE.md)