# Board game: how to prepare files for printing

by Leszek Cimała

![alt-text][introcards]

**Table of Contents**
<!--ts-->
   * [Board game: how to prepare files for printing](#board-game-how-to-prepare-files-for-printing)
      * [Intro](#intro)
      * [Quickstart](#quickstart)
      * [How games are made?](#how-games-are-made)
      * [Components](#components)
         * [Size](#size)
      * [Layouts](#layouts)
         * [Common rules for all layouts](#common-rules-for-all-layouts)
            * [Crop(cutting) marks.](#cropcutting-marks)
            * [Bleed](#bleed)
         * [Page size A4 vs U.S. Letter](#page-size-a4-vs-us-letter)
            * [If you prepare only one version](#if-you-prepare-only-one-version)
            * [If you are hero and prepare both versions](#if-you-are-hero-and-prepare-both-versions)
         * [Duplex printing vs gutter fold layouts.](#duplex-printing-vs-gutter-fold-layouts)
            * [Duplex printing layout](#duplex-printing-layout)
               * [When duplex printing is used?](#when-duplex-printing-is-used)
            * [Gutter fold](#gutter-fold)
      * [Biggest mistakes](#biggest-mistakes)
      * [Software needed](#software-needed)
      * [Feedback](#feedback)

<!-- Added by: ernie, at: Sat 14 Nov 2020 09:56:23 PM CET -->

<!--te-->

## Intro 

As a word of warning - I am not expert in printing, nor artist, just guy who likes to make games which looks good. Usually people have hard times believing that game is home-made.

Also this article is about preparing games for home printing. For professional printing there are more things to consider, but general idea will be mostly the same.

Why should you care about well prepared files?

1. if you look for playtesters/feedback, by preparing files you will increase probability people will print your game.
2. if you want your game to look good on people tables.

I am shocked how much time and love people can put into their graphic design just to ruin it by wrong component layout.
But in my opinion even simple minimalistic graphic is nice and deserve to be cut well.

When preparing this how-to I was looking at my downloaded PNP-s (60+ games), and if not counting about 10 R&W, max 5 of them
were well done.

## Quickstart

If you want to quickstart your files do following:

- download and install Gimp and Inkscape,
- prepare your components (as a vector or raster graphics) to separate files (for cards poker size, mini-poker),
- choose which layouts you will provide, usually duplex layout and gutter fold layout. 

## How games are made?

To understand how to prepare files for PNP you should know how people make cards and other components.

For now I will send you to:
**Dining Table Print & Play**  youtube channel. It is excellent source of information and I would call this channel as "classic" in PNP space.

How to make **cards**:
https://www.youtube.com/watch?v=WyMVRJu5yQ4

He presents 3 methods, you are aiming for "The awesome one", look at timestamp:

https://www.youtube.com/watch?v=WyMVRJu5yQ4&t=1183s

This is, ladies and gentlemen, *gutter fold* method. He just should crease more aggressively, then folding is much quicker.

And **tokens**:
https://www.youtube.com/watch?v=iqqFvPZe4qs

Depending on tokens you plan to use, you can skip to part which is interesting for you. 
If you are going to use hex tokens, it is crucial to put them in layout you will see there.

## Components

### Size

If you did not decided yet which size of your components you want to use, I would recommend to stick with standard sizes.
What are standard sizes? Who knows. :-)

There is many sizes in the wild, but for normal cards I would consider poker card size as most commonly used:

Poker size:  88.9mm x 63.5mm (3.5in x 2.5in)

Second common size is bridge cards which are narrower. It may be beneficial to use this size if player has to keep many cards in hand.

Bridge size: 88.9mm x 56mm (3.5in x 2.25in)

Other components are usually up to you, just remember that A3 (legal) printers are rare, while you can provide A3 board you should
provide also 2xA4 alternative.

### Low-ink version

If you want to increase chance that game will be playtested it is good idea to provide low-ink version. Sometimes author are
also providing B&W (greyscale) versions and they are not necessary low-ink.

If you are not going to prepare greyscale version maybe just try to print your game greyscale and check how it looks. Maybe
it will be usable if you only make few elements darker or lighter? It can even improve readability of your normal (color) version.

## Layouts

### Common rules for all layouts

#### Crop(cutting) marks.

1. Allows to position cutting ruler precisely.
2. Will never be visible on components.

Example of good crop marks:

![alt text][cuttingmarksgood]

Example of bad crop marks:

![alt text][cuttingmarksbad]

Usually my crop marks are 0.15mm wide, it seems very narrow, but you can see them well
and they allow for precise cutting.

#### Bleed

1. Bleed is necessary to allow slight cutting/alignment errors.
2. Bleed should be 2-3mm.
3. Best when created in component design phase.
4. You need to have bleed area around every edge of the component.

![alt text][bleed]

### Page size A4 vs U.S. Letter

In centimeters (cm):

| Format | Height | Width |
|--------|--------|-------|
| A4     | 29.7   | 21    |
| letter | 27.94  | 21.59 |

**Margins**
Use at least **5mm** (0.5cm, 0.2inch) margin on every side. If you want be safe, use **10mm** (1cm, 0.4inch) margin.

```
NOTE: Please let me know if your printer can't print so close to the edge! I will update info here.
```

#### If you prepare only one version

If you use **A4** leave extra **18mm** (1.8cm) margin at the **bottom** of the page.

If you use **letter** size leave extra **6mm** (0.6cm) margin on **right side** of the paper.

Don't center components on the page unless you know, mentioned space will be there.

#### If you are hero and prepare both versions

Problem using "wrong" paper size is, how printing software/printers behave, if user is not careful they may resize content which is not what we want.

It is much better to prepare files for both paper sizes if you can.

### Duplex printing vs gutter fold layouts.

This part is the reason why whole article even exists. This is important!

#### Duplex printing layout

Example of well prepared duplex printing layout, **The shooting party** by **John Kean**.

1. page - front, 2. page - back
![alt-text][duplex]

When preparing duplex printing layout remember that components are mirrored. Look where on page card nr 1 front is placed
and where back for it is.

As you can see, there are cutting marks and they are ok. There is also bleed (very light pink) - perfect. 

Whole file is well done with only one exception - <span style="color: red">it is marked red<span>. This card and 2 cards around it has no bleed.
This is the only card with different border and that is potential place, where even small aligning or cutting
error would result in ugly card edge.

How to solve situations like that?

You should make double cutting marks in places where 2 different borders meets and make space for bleed area for both cards.
Here is example of what I mean (**Twin Stars** by  **Mike Mullins, Jason Tagmire**):

![alt-text][duplexbleed]

Notice, that card edges are different color (and they are not one unified color), so author solved the problem by making two cutting lines. There is plenty of bleed, so cards will always look good.

##### When duplex printing is used?

* For every form of "quick printing". When someone wants to play as soon as possible and do not care about perfect build.
* If someone has:
  - double-sided photo paper,
  - linen or other decorated thick paper.
* When someone has no other option. It is still possible to glue front and back (usually with cardboard between) quite precisely,
  but it is much harder then with gutter fold layout.

Precision of duplex printing depends heavily on printer. Usually there will be some shift so bleed is necessary. 
It works better for backs, which are created by repeating pattern.

##### Do we need cutting lines on both sides of components (backs and fronts)?

Yes, we do. :-)

If someone is gluing fronts and backs together they need them to align fronts with backs.

If you are interested how this can be done, let me know, for now I will leave you with article in polish ;-), sorry for that, 
but it is the only source I know, which describe process clearly. Just look at the pictures.

http://piotrnowinski.pl/wlasne-projekty/gry-planszowe/jak-profesjonalnie-przygotowac-karty-do-gry

Here is link for google-translated version:
https://translate.google.com/translate?hl=&sl=pl&tl=en&u=http%3A%2F%2Fpiotrnowinski.pl%2Fwlasne-projekty%2Fgry-planszowe%2Fjak-profesjonalnie-przygotowac-karty-do-gry

#### Gutter fold

This is the best layout for PNP, lets see why.

![alt-text][gutterfold]

1. We have bleed.
2. Cutting marks are perfect.

## Biggest mistakes

* **Lines around component.** Usually they are there to simplify cutting, but in reality, they are nightmare. You always end up with ugly black lines around some edges of the component. It will be quite random and they will ruin your build.
* **No cutting helpers at all.** How one should cut it? ;-)
* ****

## Software needed

GIMP, Inkscape.


## Feedback

I would love to hear any critics you have for this text. English is not my first language, so it would be great if we can iron out wording and grammar here. :-)

You can create issue (or PR!) on github or contact me by **geekmail**:

https://boardgamegeek.com/geekmail/compose?touser=ernierasta

[introcards]: images/intro.png
[cuttingmarksgood]: images/crop-marks-good.png "Good crop marks"
[cuttingmarksbad]: images/crop-marks-bad.png "Bad crop marks"
[bleed]: images/bleed.png "Bleed example"
[duplex]: images/the-shooting-party_duplex.png "Duplex example"
[duplexbleed]: images/twin-stars_duplex-bleed.png "Duplex with bleed"
[gutterfold]: images/the-shooting-party_gutter-fold.png "Gutter fold example"
