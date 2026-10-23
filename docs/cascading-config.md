[Nano](../README.md) __|__ __[Documentation](README.md)__

---

# Creating a Configuration that Cascades   


> *Using a cascading style configuration encourages experimentation and learning*

---

## In this Document

- [What it is](#what-it-is)
- [Set up](#set-up)

## What it is

Most config types follow a system where the last defined setting is the one that is used. 

## Set Up

The set up generally leverages configuration systems that allow for `include` statements. Fortunately Nano Does!

## Cascading Color Scheme

Lets say we have a few color files

- `editor.nanorc` - The first config
- `text.nanorc` - The second Config, editor `include`s `text`
- `specificlanguage.nanorc` - The 3rd `specificlanguage.nanorc` is `inlcude`d at the ottom of `editor`

When all these files are included they add up to look like this:

```text
#editor

set textcolor = black

#text

set textcolor = white

#specificlanguage

set textcolor = blue

```

---

__(Ɔ) 2026__ [8rents](https://github.com/8rents) under the [MIT License](../LICENSE.md)