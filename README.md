
![](https://github.com/cryptocopycats/awesome-mooncatrescue-bubble/raw/master/i/design-000x3.png)
![](https://github.com/cryptocopycats/awesome-mooncatrescue-bubble/raw/master/i/design-001x3.png)
![](https://github.com/cryptocopycats/awesome-mooncatrescue-bubble/raw/master/i/design-002x3.png)
![](https://github.com/cryptocopycats/awesome-mooncatrescue-bubble/raw/master/i/design-003x3.png)


# MoonCatRescue on the Blockchain


> What is a mooncat? Just another cryptokitty? How are they selling for so much?
>
> Mooncats are scarce and verifiable. You can bring a mooncat anywhere in the world,
> airplane or boat, proving itself to be a truer store of value than gold itself.
>
> Only 25 thousand mooncats. 21 million bitcoins. Do the math.
>
> Spent over $20,000 on mooncat id 0xff0b000ca7 ... one of the first genesis batch.
>
> Someone took Jeff Bezos crown today [as the richest man on earth].
> Top mooncat holder owns 1,144 cats. LOL.
>
> -- March 13, 2021 - Moon Cat Rescue Day



## Datasets

### mooncats.csv  -  25 440 MoonCats by ID with Pattern, Pose, Facing, Face, Fur and Colors in RGB and HSL (Hue, Sat, Lum)

Mooncats dataset in comma-separated values (CSV) format
in blocks of a thousand cats each
(e.g.
`00.csv` incl. 0x0000020886-0x000a05b9ac,
`01.csv` incl. 0x000a0a11c8-0x0013b68a2f,
`02.csv` incl. 0x0013b72770-0x001e26e929,
and so on).
The data records for cats
incl. id, palette, pattern, pose, facing, face, fur, colors in rbg and hsl (hue, sat, lum), row and mint serial number,
and more.
Example - [`00.csv`](00.csv):


```
row, id,           palette, pattern, pose, facing, face, fur, color,    ... mint
0,   0x0000020886, Normal, 0, Standing, Left, Smile, Solid, Sky Blue,   ... 2679
1,   0x000002f63e, Normal, 0, Standing, Left, Smile, Solid, Green,      ... 13869
2,   0x000004683b, Normal, 0, Standing, Left, Smile, Solid, Lime Green, ... 24457
3,   0x0000048998, Normal, 0, Standing, Left, Smile, Solid, Cyan,       ... 22386
4,   0x000006ce5d, Normal, 0, Standing, Left, Smile, Solid, Green,      ... 7933
...
```



Notes about some fields:

Row (25 440)

Row sequence number (starting with 0) - cats sorted by id; see Mint sequence number for sorted by rescue / mint order


Palette (2)

- Normal (`0`): 13 080 cats
- Inverted (`1`): 12 360 cats


Pattern (0 to 63)

64 patterns from 0 to 63 - composed of 4 (pose) x 4 (face) x 4 (fur) designs.

Note: Left and right facing cats are combined under the same pattern, that is,
NOT counted as distinct patterns.


Poses (4)

- Standing (`00`): 6 175 cats
- Sleeping (`01`): 6 063 cats
- Pouncing (`10`): 6 711 cats
- Stalking (`11`): 6 491 cats

Facing (2)

- Left (`0`): 12 825 cats
- Right (`1`): 12 615 cats

Face (4)

- Smile (`00`): 6 313 cats
- Frown, Look Down (`01`): 6 212 cats
- Frown, Look Up (`10`): 6 336 cats
- Flat Whiskers (`11`): 6 579 cats

Fur (4)

- Solid (`00`): 6 511 cats
- Striped (`01`): 6 179 cats
- Eyepatch (`10`):  6 172 cats
- Half/Half (`11`): 6 578 cats


Color

Derived from hues by degrees.

- Red (0 to 29° degrees): 2 270 cats
- Orange (30 to 59° degrees): 2 186 cats
- Yellow (60 to 89° degrees): 2 042 cats
- Chartreuse (90 to 119° degrees): 1 869 cats
- Green (120 to 149° degrees): 1 882 cats
- Lime Green (150 to 179° degrees): 2 066 cats
- Cyan (180 to 209° degrees): 2 256 cats
- Sky Blue (210 to 239° degrees): 2 173 cats
- Blue (240 to 269° degrees): 2 263 cats
- Purple (270 to 299° degrees): 2 052 cats
- Magenta (300 to 329° degrees): 2 085 cats
- Fuscia (330 to 359° degrees): 2 200 cats

Note: The 96 genesis cats (ids starting with `ff`) are either Black or White
with 48 cats each.


Mint (25 440)

Mint sequence number - cats sorted by by rescue / mint order starting with 0; see Row squence number for sorted by id





### Frequently Asked Questions (F.A.Q.s) and Answers

Q: Why 25 440 and not 25 600 cats? The MoonCatRescue website states
 "with the latest in litterbox technology, that can fit up to 25 600 MoonCats"?

Note: Genesis cats are not "rescued" but rather "released" by the contract owners.
If those original project owners re-emerge,
they'd have the ability to release more genesis cats.

To quote the re-emerged contract owner (Ponderware):

> As for the remaining 160 genesis cats. We are trying to work out the best course
> to maintain the ethos of the project,
> and maximize the enjoyment of all mooncat rescuers.
> Note: we don't receive any compensation for new genesis cats.
>  We were supposed to but, well, check the FAQ.
>
>  -- [Ponderware](https://twitter.com/ponderware/status/1370945005641158659)




### Your Tool Here

Do you have a tool for the mooncats dataset? Let us know! Add your tool here.





## Thanks

Big thank you to [Brooks Boyd](https://github.com/MidnightLightning) (a.k.a Midnight Lightning)
who not only posted the `mooncats.json` dataset on the MoonCatRescue reddit but also
named all colors and patterns (pose, face, fur, etc.) and much more -
generously answered all questions in amazing details
incl. posting info graphics about the 360° color wheel
, how to decode the magic `k` mooncat value or showing all patterns
or color variations.




## License

![](https://publicdomainworks.github.io/buttons/zero88x31.png)

The mooncatrescue on the blockchain dataset
is dedicated to the public domain.
Use it as you please with no restrictions whatsoever.



## Questions? Comments?

Post them on the [mooncatrescue reddit](https://www.reddit.com/r/mooncatrescue). Thanks.
