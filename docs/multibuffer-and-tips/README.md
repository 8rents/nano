# Using Nano's File Browser 

> *...and other helpful tips*

---

This document contains advanced nano workflow tips and tricks.

## In this document

- [Opening multiple files](#opening-multiple-files)
- [Cycle through files in nano](#cycle-through-files-in-nano)
- [Opening files within nano](#opening-files-within-nano)
- [Cut & paste a selection](#cut-&-paste-a-selection)
- [Run a spell check](#run-a-spellcheck)
- [Lint a File](#lint-a-file)
- [Reformat a File](#reformat-a-file)

## Opening multiple files

First make sure `set multibuffer' is in your nanorc. It's enabled on this repositorys.

You can open as many files at once from your shell bt adding them aftrr the first.

```
nano file1.txt file2.txt
```

## Cycle through files in nano

- **next file:** `alt + .`
- **prev file:** `alt + ,`

## Opening files within nano

- **Open file by name** - `ctrl + r`
  > *You can `tab` complete the names*

## Cut & paste a selection

- **Make a selection** - `ctrl + 6` to set a mark. navigate to end point. `ctrl + k` to cut. `ctrl + u` to paste.

## Run a spellcheck

## lint a file

## reformat a file