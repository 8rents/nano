[Nano](../README.md) __|__ __[Documentation](README.md)__

---

# Working with colors in Nano

> *Simplifiying and streamlining the process of working efficently and expressively with colors in Nano*

---

## Nano Color Explained

Colors in Nano come in 2 main variaties: **Basic & Extended**

### Your Terminal Colorscheme defines the "Basic Colors"

Basic colors are the 8 (16) colors that you have in your terminal at your disposal. Each of these colors is a label and can have the actual color value changed to match a broader theme.

**Basic color names are the most compatible and will always be supported. They will also inherently match a users terminal theme.**

> ### Viewing the basic colors with neofetch
> 
> if you run `neofetch` in the terminal at the bottom of the system profile you'll see 2 rows of 8 colored blocks. These are the basic colors. 
> 
> ![Neofetch color blocks](https://raw.githubusercontent.com/8rents/_/refs/heads/i/screenshots/neofetch-colors.png)

#### Basic Normal Colors (0-7)

You can see the normal 8 colors on the first row of neofetch. WWhat hex they are defined to in your terminal setting will change their appearance.

*Valid basic color names are:*

`black`, `red`, `green`, `yellow`, `blue`, `magenta`, `cyan`, `white` & `normal`

or `color0` - `color7` in XTERM terms.

#### Basic Bright Colors (8-15)

In addition to the 8 listed above there are the "Bright" variants. These are the same colors except with the word `bright` in front of them. `brightyellow`, `brightgreen` etc.

#### And a couple of special extra colors...

These are the 16 basic colors (0-15). You actually get 18 to 19 basic colors. `background`, `foreground` and `cursor`. are also valid names if set in the terminal profiles.

---

## Nano Extended Colors 

Extended colors are less compatible and might not be supported with all devices, terminals or Nano installations. Extended colors do not draw from your 16 terminal colors. They are defined with their own hex codes. There;s 24 extended colors and with the 2 different variants (`bright` or `light` & `dark`). 

**Valid extended color names are:** `pink`, `purple`, `mauve`, `lagoon`, `mint`, `lime`, `peach`, `orange`, `latte`, `rosy`, `beet`, `plum`, `sea`, `sky`, `slate`, `teal`, `sage`, `brown`, `ocher`, `sand`, `tawny`, `brick`, `crimson` and of course, `normal`

Color name prefixes like  `bright`, `dark` and `light` can also be applied to extended colors. **like:** `brightslate`, or the extra moody `darksea`.

---

## Interface Elements Styling Syntax in Nano

The syntax for adding color to elements in Nano is

> ### color settings syntax
> 
> ```
> <setoption> [italic,][bold,]<foregound>,<background>
> ```
>
> - Don't put any spaces into the setting string. Except after the option name.
> - `<>` - denotes that the text inside the brackets is variable and should be something else. Don't add the brackets to the actual code. The options generally begin with `set` or `unset`,
>   `<setoption>` could be: `setminibar` or `unsetstatusbar`
> - `[bold,][italic,]` - Items in straight bracket denotes that the word isn't variable and should't change, but is optional. 
>   For these two keys, you can put both, one, or either or, but they always go in that order when used together. The comma has to be included with the word.
> - `<foreground>` | `<background>` - Replace either of these words with a color code. `black`, `sage`, `brightred` would all work.

```conf
# The minibar has bold black text on a pink background
set minibar bold,black,pink

# The minibar has italic white text on a grey background
set minibar bold,black,brightred
```

The above two minibar settings render the same way. One is using the much preferred, basic 16 colors.


---

__(Ɔ) 2026__ [8rents](https://github.com/8rents) under the [MIT License](../LICENSE.md)