[Nano](../README.md) __|__ __[Documentation](README.md)__

---

# How to create new keybindings for nano

> *With the built in functions that Nano provides, we will be able to bindthe well tread, predictable keyboard shortcuts to the proper functions to make Nano modern and easy to use again*

---

## Table of Contents

- [List of Functions to Rebind](#list-of-functions-to-rebind) - These are the important Nano functions I'm going to focus on to create a better experience.
- [Complete List of Valid Function Names in Nano](#complete-list-of-valid-function-names-in-nano) - The entire list of built in fucntion names from which to choose from.
- [Valid Nano Menu Sections](#valid-nano-menu-selections) - When binding a key to a function you need to include a menu to use. This is the complete list of menus.
- [Binding a Function and Menu to a Key Command](#binding-a-function-and-menu-to-a-key) - A practical example of binding a new key command.

---


## Links

- [Nano Manpage](https://man.archlinux.org/man/nanorc.5.en)


## Keybinding Syntax

bind keys function menu

### Keybinding Example  

```
bind ^O browser whereisfile # Opens file browser
```

The `bind` keyword followed by the keyboard shortcut: 

- `^` ctrl
- `M` alt/meta 
- `Sh` shift

Then the function name (browser)

and then the menu: `whereisfile`

### Do Not Rebind the following

- `^M` (Enter) - not good idea
- `^I` (Tab) - not good idea
- `^[` (Esc) is not possible,

## Functions that can be bound to a key combo

The following is the complete list of [function names thst can be bound in nano](https://man.archlinux.org/man/nanorc.5.en)

## Function Menus

The function menu is declared right after the fuction name.

- `main` - The main editor window where text is entered and edited.
- `help` - The help-viewer menu.
- `search` - The search menu (AKA whereis).
- `replace` - The 'search to replace' menu.
- `replacewith` - The 'replace with' menu, which comes up after 'search to replace'
- `yesno` - The  'yesno' menu, where the Yes/No/All/Cancel question is asked.
- `gotoline` - The 'goto line (and column)' menu.
- `writeout` - The 'write file' menu.
- `insert` - The 'insert file' menu.
- `browser` - The 'file browser' menu, for selecting a file to be opened or inserted or written to.
- `whereisfile` - The 'search for a file' menu in the file browser.
- `gotodir` - The 'go to directory' menu in the file browser.
- `execute` - The menu for inserting the output from an external command, or for filtering the buffer (or the marked region) through an external command, or for executing one of several tools.
- `spell` - The menu of the integrated spell checker where the user can edit a misspelled word.
- `linter` - The linter menu, which allows jumping through the linting messages.
- `all` - A special name that encompasses all menus. For bind it means all menus where the specified function exists; for unbind it means all menus where the specified key exists

To make `Shift+Alt+C` copy the marked region to the system’s clipboard:

```
bind Sh-M-C "{execute}| xsel -ib {enter}{undo}" main
```

---

__(Ɔ) 2026__ [8rents](https://github.com/8rents) under the [MIT License](../LICENSE.md)