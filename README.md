# Blitz Basic 2  Expérimentation

All source can be compiled with Blitz Basic 2 - I suggest [Ultimate Blitz Basic 2.1]([Source](1-background-with-rainbowcopper.bba)).

I also suggest the [VSCode Blitz Basic Extension](https://marketplace.visualstudio.com/items?itemName=mickgyver.amiga-blitzbasic2) to type code, run code and package code for floppy, harddisk, CDTV and CD32 (Disclaimer : I am a contributor of the plugin).

## 1 - Bitmap with rainbow copper effect

Simple example using the copper to generate a vertical rainbow behind a bitmap. The rainbow can use color not in the palette (You get extra color).

[Source](1-background-with-rainbowcopper.bba)

## 2 - Adding dual playfield for parallax effect

2 bitmaps with 3 bitplans (8 colors each).

Foreground bitmap using 0 to 7 palette.

Background bitmap using 8 to 15 palette.

[Source](2-adding-dual-payfield.bba)

## 3 - Adding a lot of rain effect using sprite multiplexing - 16 colors sprites

Inpired from the trick from Agony game for the rain effect : https://codetapper.com/amiga/sprite-tricks/agony/

Using code from previous step to add a sprite multiplexing using Copper based on [@earok](https://github.com/earok/BlitzBasicDemos/blob/master/SpriteMultiplex/main.bb) code.

Limitation is I didn't figure out how to get this effect with the copper rainbow background.

[Source](3-adding-rain-sprites-multiplexing-copper.bba)

Required to have BB2OBJTYPES.RES in resident libs in compiler Option

## 3b - Adding a lot of rain effect using sprite multiplexing - 4 colors sprites

Same as 3 but in 4 color sprites so up to 7 sprites per line (last channel is for smooth scrolling).

Still got a color issue on odd channel.

[Source](3b-adding-rain-sprites-multiplexing-copper-4colorsprite.bba)

Required to have BB2OBJTYPES.RES in resident libs in compiler Option

## 4 - Rain effect using CustomSprites Blitz Basic 2 native sprite multiplexing - 4 colors sprites

Inpired from the trick from Agony game for the rain effect : https://codetapper.com/amiga/sprite-tricks/agony/

Using CustomSprites instruction for Blitz Basic 2.

Limitation is I didn't figure out how to get this effect with the copper rainbow background. (Still using copper)

[Source](4-adding-rain-sprites-multiplexing-customsprites.bba)

Required to have BB2OBJTYPES.RES in resident libs in compiler Option