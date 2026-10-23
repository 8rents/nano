[Nano](../README.md) __|__ [Documentation](../docs/README.md)

# Nano Binary Folder

> *Scripts you can run to help you with this repository*

---

## Scripts

All scripts need to be made executable before they can be used:

### Making nano scripts executable

```bash
chmod 755  bin/*.sh
```

### Running scripts from the `bin` folder

From the `nano` directory:

```bash
./bin/install.sh
```

This runs the install script

### Linking Scripts to your Path

```bash
ln -s ~/.config/nano/bin/nano-syntax.sh ~/bin/nano-syntax
```

Now you can just run:

```bash
nano-syntax *
```

## Nano Language Syntaxes

Will list the languages and ask which you want to install. It will also clone the submodule if it hasn't been cloned yet.

### List available Syntaxes

```bash
nano-syntax -l
```

### Adding a syntax's syntax

```
nano-syntax <filename (without .nanorc)>
```

#### Example

```bash
# Adds html Syntax
nano-syntax html
```

### Options / Flags

- `-l` - list language files
- `-e` - edit language syntax

---

__(Ɔ) 2026__ [8rents](https://github.com/8rents) under the [MIT License](../LICENSE.md)
