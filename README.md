# MoonCatRescue on the Blockchain


## Datasets

### mooncats.csv  -  25 440 MoonCats by ID with Design, Pose, Facing, and Colors in RGB and HSL (Hue, Sat, Lum)

Mooncats dataset in comma-separated values (CSV) format
in blocks of a thousand cats each
(e.g.
`00.csv` incl. 0x0000020886-0x000a05b9ac,
`01.csv` incl. 0x000a0a11c8-0x0013b68a2f,
`02.csv` incl. 0x0013b72770-0x001e26e929,
and so on).
The data records for cats
incl. id, palette, design, pose, facing, colors in rbg and hsl (hue, sat, lum), row and mint serial number,
and more.
Example - [`00.csv`](00.csv):


```
row, id,          palette, design, pose, facing, color, r, g, b, hue, sat, lum, mint
0,   0x0000020886, Normal, 0, Standing, Left, Sky Blue,   2,   8, 134, 237.27, ... 2679
1,   0x000002f63e, Normal, 0, Standing, Left, Green,      2, 246,  62, 134.75, ... 13869
2,   0x000004683b, Normal, 0, Standing, Left, Lime Green, 4, 104,  59, 153.00, ... 24457
3,   0x0000048998, Normal, 0, Standing, Left, Cyan,       4, 137, 152, 186.08, ... 22386
4,   0x000006ce5d, Normal, 0, Standing, Left, Green,      6, 206,  93, 146.10, ... 7933
...

```



Notes about some fields:

Row (25 440)

Row sequence number (starting with 0) - cats sorted by id; see Mint sequence number for sorted by rescue / mint order


Palette (2)

- Normal
- Inverted

Design (0 to 127)

128 designs from 0 to 127

Poses (4)

- Standing: 6 175 cats
- Sleeping: 6 063 cats
- Pouncing: 6 711 cats
- Stalking: 6 491 cats

Facing (2)

- Left: 12 825 cats
- Right: 12 615 cats

Color

Derived from hues by degrees.

- Red (0 to 29 degrees): 2 270 cats
- Orange (30 to 59 degrees): 2 186 cats
- Yellow (60 to 89 degrees): 2 042 cats
- Chartreuse (90 to 119 degrees): 1 869 cats
- Green (120 to 149 degrees): 1 882 cats
- Lime Green (150 to 179 degrees): 2 066 cats
- Cyan (180 to 209 degrees): 2 256 cats
- Sky Blue (210 to 239 degrees): 2 173 cats
- Blue (240 to 269 degrees): 2 263 cats
- Purple (270 to 299 degrees): 2 052 cats
- Magenta (300 to 329 degrees): 2 085 cats
- Fuscia (330 to 359 degrees): 2 200 cats

Note: The 96 genesis cats (ids starting with `ff`) are either Black or White
with 48 cats each.


Mint (25 440)

Mint sequence number - cats sorted by by rescue / mint order starting with 0; see Row squence number for sorted by id





### Your Tool Here

Do you have a tool for the mooncats dataset? Let us know! Add your tool here.





## License

![](https://publicdomainworks.github.io/buttons/zero88x31.png)

The mooncatrescue on the blockchain dataset
is dedicated to the public domain.
Use it as you please with no restrictions whatsoever.



## Questions? Comments?

Post them on the [mooncatrescue reddit](https://www.reddit.com/r/mooncatrescue). Thanks.
