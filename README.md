__Nano__ ng  __|__ [Documentag[tion](docs/README.md)

# (Pimp my) Nano

> *Modernizing the most dissed editor on the command line...*

---

## *Now with!*

- More Modern key bindings
- New & Improved color schemes
- A Better, cooler looking, and more functional interface
- Only the best options enabled

---

## *What it looks like*

![screenshot](https://raw.githubusercontent.com/8rents/nano/refs/heads/main/screenshot.png)

---

## Installation

When cloning this repo, include the `--recursive` flag on the `clone` command. Install it to `$XDG_CONFIG_HOME/nano`, which likely is `~/.config/nano`.

```bash
cd ~/.config
git clone --recursive https://github.com/8rents/nano
```

### If you've already cloned it

If you've already cloned this repo, initialize and update submodules with the `submodule` command.

```bash
git submodule update --init --recursive
```

That should download and configure each of them.

### Submodules Included in this repo

The following are included in this package as submodules: 

#### [8rents/nano-syntax-highlighting](https://github.com/8rents/nano-syntax-highlighting)

Improved syntax highlighting for nano. Actively updated and growing. 

> **Forked from: [galenguyer/nano-syntax-highlighting](https://github.com/galenguyer/nano-syntax-highlighting)**

---

## Repository Development

Where this repository is going and where it's been

- [List of Past Changes by Version (Changelog)](../CHANGELOG.md)
- [List of Upcoming Changes (To Do List)](../TODO.md)

---

## Documentation, Guides & Articles

Articles to help you better understand configuring nano

- [Mutlibuffer& Workflow Tips](docs/multibuffer-and-tips/README.md)
- [Creating a Cascading Configuration](docs/cascading-config.md)
- [Working with colors in Nano](docs/colors/README.md)
- [Notable Options](docs/notable-options/README.md) 
- [Functions in Nano and binding them to create a more modern feel](docs/function-binding/README.md)


---

## Links / Sources

Some of the sources that I've found helpful while putting together this repository

- [Reddit/Ask Linux - What does your nanorc look like?](https://www.reddit.com/r/linux/comments/1f3jeoo/what_does_your_nanorc_look_like)
- [davidhcefx/nanorc - Modern Nano Keybindings](https://github.com/davidhcefx/Modern-Nano-Keybindings)
- [scopatz/nanorc - Improved Nano Syntax Highlighting Files](https://github.com/scopatz/nanorc)

---

__(Ɔ) 2026__ [8rents](https://github.com/8rents) under the [MIT License](LICENSE.md)