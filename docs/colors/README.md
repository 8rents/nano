[Home](../../README.md) __|__ [Todo](../../TODO.md) __|__ __[Additional Docs](../README.md)__

# Working with colors in Nano

> *Simplifiying and streamlining the process of working efficently and expressively with colors in Nano*

---

## Color Explained

Colors come in 2 main vaiaties: Basic & Extended

### Basic Colors

Basic colors are the 8 colors that you have in your terminal at your disposal. Each of these colors is a label and can have the actual color value changed to match a broader theme.

Basic color names are the most compatible and will always be supported. They will also inherently match a users terminal theme.

### Viewing colors with neofetch

if you run `neofetch` in the terminal at the bottom of the system profile you'll see 2 rows of 8 colored blocks. These are the basic colors. 

![Neofetch color blocks](https://raw.githubusercontent.com/8rents/_/refs/heads/i/screenshots/neofetch-colors.png)

From left to right on the top row:

1. black
2. red
3. green
4. yellow
5. blue
6. magenta
7. cyan
8. white

In addition to the 8 listed above there are the "Bright" variants. These are the same colors except with the word "bright" in front of them. brightyellow, brightgreen etc.

## Extendeded Colors 

Extended colors are less compatible and might not be supported with all devices, terminals or Nano installations.

Valid extended color names in Nano are:

1. pink
2. purple
3. mauve
4. lagoon
5. mint
6. lime
7. peach
8. orange
9. latte
10. rosy
11. beet
12. plum
13. sea
14. sky
15. slate
16. teal
17. sage
18. brown
19. ocher
20. sand
21. tawny
22. brick
23. crimson
24. normal

Color name prefixes like  "bright", "dark" and "light" can also be applied to extended colors.

## Styling Interface Elements in Nano

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
# The minibar has bold white text on a magenta backgrond
set minibar bold,white,magenta

# The minibar has italic white text on a grey background
set minibar italic,white,brightblack
```

---

