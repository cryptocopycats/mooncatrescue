
![](https://github.com/cryptocopycats/awesome-mooncatrescue-bubble/raw/master/i/design-000x3.png)
![](https://github.com/cryptocopycats/awesome-mooncatrescue-bubble/raw/master/i/design-001x3.png)
![](https://github.com/cryptocopycats/awesome-mooncatrescue-bubble/raw/master/i/design-002x3.png)
![](https://github.com/cryptocopycats/awesome-mooncatrescue-bubble/raw/master/i/design-003x3.png)
![](https://github.com/cryptocopycats/awesome-mooncatrescue-bubble/raw/master/i/design-056x3.png)
![](https://github.com/cryptocopycats/awesome-mooncatrescue-bubble/raw/master/i/design-057x3.png)
![](https://github.com/cryptocopycats/awesome-mooncatrescue-bubble/raw/master/i/design-058x3.png)
![](https://github.com/cryptocopycats/awesome-mooncatrescue-bubble/raw/master/i/design-059x3.png)


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

### mooncats.csv  -  25 440 MoonCats by ID with Design, Pose, Facing, Face, Fur, Color, Mint, Timestamp, Block

Mooncats dataset in comma-separated values (CSV) format
in blocks of a thousand cats each
(e.g.
`00.csv` incl. 0x0000020886-0x000a05b9ac,
`01.csv` incl. 0x000a0a11c8-0x0013b68a2f,
`02.csv` incl. 0x0013b72770-0x001e26e929,
and so on).
The data records for cats
incl. id, palette, design, pose, facing, face, fur, color, hue, row and mint serial number, rescue block and timestamp,
and more.
Example - [`00.csv`](00.csv):


```
row, id,           palette, design, pose, facing, face, fur, color,    ... mint
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


Design (0 to 127)

128 patterns from 0 to 127 - composed of 4 (pose) x 4 (face) x 4 (fur)
x 2 (facing) designs.


<!--
Pattern (0 to 63)

64 patterns from 0 to 63 - composed of 4 (pose) x 4 (face) x 4 (fur) designs.

Note: Left and right facing cats are combined under the same pattern, that is,
NOT counted as distinct patterns.
-->

Pose (4)

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

- Red (345 to 359° & 0 to 14° degrees): 2 251 cats
- Orange (15 to 44° degrees): 2 233 cats
- Yellow (45 to 74° degrees): 2 137 cats
- Chartreuse (75 to 104° degrees): 1 903 cats
- Green (105 to 134° degrees): 1 920 cats
- Teal (135 to 164° degrees): 1 934 cats
- Cyan (165 to 194° degrees): 2 191 cats
- Sky Blue (195 to 224° degrees): 2 199 cats
- Blue (225 to 254° degrees): 2 223 cats
- Purple (255 to 284° degrees): 2 179 cats
- Magenta (285 to 314° degrees): 2 058 cats
- Fuchsia (315 to 344° degrees): 2 116 cats

Note: The 96 genesis cats (ids starting with `ff`) are either Black or White
with 48 cats each.


Mint (25 440)

Mint sequence number - cats sorted by by rescue / mint order starting with 0; see Row squence number for sorted by id


Timestamp

The timestamp the cat got rescued / released. By year:

- 2017:  3 365 cats
- 2018:  2 319 cats
- 2019:  71 cats
- 2020:  3 cats
- 2021: 19 682 cats

Note: Almost all cats in 2021 got rescued on MoonCat Rescue Day on March 12th.



Block

The block number the cat got rescued / released




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

Update:

> The community has spoken. With a final outcome of YES: 944 NO: 367,
> the devs will destroy their private key to the MoonCatRescue contract.
> The contract will be left as found.
> The remaining Genesis MoonCats will never be released and will continue to live happily on the moon.
>
>  -- [Ponderware](https://twitter.com/ponderware/status/1373992233180004358)




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
