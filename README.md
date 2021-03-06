# pawn-humanize

Pawn-humanize is a library inspired by [go-humanize](https://github.com/dustin/go-humanize) that makes stuff computers can read easily, more readable for humans.

## Installation (Sampctl)
Simply install to your project:

```bash
sampctl package install thecodeah/pawn-humanize
```

Include in your code and begin using the library:

```pawn
#include <humanize>
```

# Features

## Commas
```
0 -> 0
100 -> 100
1000 -> 1,000
1000000 -> 1,000,000
-100000 -> -100,000
```
```C
HumanizeComma(integer, dest[], maxLength = sizeof dest)
```

## Colors
```
0xA86420FF -> "Chocolate Brown"
0x42F44EFF -> "Lime Green"
0x137A8EFF -> "Teal"
```
```C
HumanizeColor(color, dest[], maxLength = sizeof dest)
```

## Ordinals
```
0 -> 0th
1 -> 1st
2 -> 2nd
3 -> 3rd
4 -> 4th
etc...
```
```C
HumanizeOrdinal(number, dest[], maxLength = sizeof dest)
```