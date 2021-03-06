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
            * [Cards](#cards)
            * [Circle components](#circle-components)
         * [Low-ink version](#low-ink-version)
         * [Color space](#color-space)
      * [Layouts](#layouts)
         * [Common rules for all layouts](#common-rules-for-all-layouts)
            * [Crop(cutting) marks.](#cropcutting-marks)
            * [Bleed](#bleed)
               * [What is bleed?](#what-is-bleed)
         * [Page size A4 vs U.S. Letter](#page-size-a4-vs-us-letter)
            * [Usable space](#usable-space)
            * [If you prepare only one version](#if-you-prepare-only-one-version)
            * [If you are hero and prepare both versions](#if-you-are-hero-and-prepare-both-versions)
         * [Duplex printing vs gutter fold layouts.](#duplex-printing-vs-gutter-fold-layouts)
            * [Duplex printing layout](#duplex-printing-layout)
               * [When duplex printing is used?](#when-duplex-printing-is-used)
               * [Do we need cutting lines on both sides of components (backs and fronts)?](#do-we-need-cutting-lines-on-both-sides-of-components-backs-and-fronts)
            * [Gutter fold](#gutter-fold)
               * [Remember when preparing](#remember-when-preparing)
               * [Double cutting lines (bleed between components)](#double-cutting-lines-bleed-between-components)
               * [When gutter fold layout is used?](#when-gutter-fold-layout-is-used)
      * [Instructions for game users](#instructions-for-game-users)
      * [Biggest mistakes](#biggest-mistakes)
      * [Practical tutorials](#practical-tutorials)
      * [Feedback](#feedback)
      * [TODO](#todo)

<!-- Added by: ernie, at: Mon Apr 12 09:48:51 AM CEST 2021 -->

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

- download and install Inkscape,
- prepare your components (as a vector or raster graphics) in Inkscape,
- choose which layouts you will provide, usually duplex layout and gutter fold layout,
- look at [Practical tutorials](#practical-tutorials) - WIP there will be more ;-). 

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

#### Cards

There is many sizes in the wild, but for normal cards I would consider poker card size as most commonly used:

Poker size:  88.9mm x 63.5mm (3.5in x 2.5in)

Second common size is bridge cards which are narrower. It may be beneficial to use this size if player has to keep many cards in hand.

Bridge size: 88.9mm x 56mm (3.5in x 2.25in)

#### Circle components

There are no standards I would know about. 

You can take into account, that NT IC-1500P rottary cutter (which would not punch hole in the middle of the cicrle) can cut 18mm-170mm circles (I would say 19mm in reality).
I personally have 22mm and 29mm punches, but that means nothing. ;-) I will fill in more sizes, based on available coin protectors or sizes from common games.

Other components are up to you.

TODO: expand this section to offer more sizes. A lot of research needed.

### Low-ink version

If you want to increase chance that game will be playtested it is good idea to provide low-ink version. Sometimes author are
also providing B&W (greyscale) versions and they are not necessary low-ink.

If you are not going to prepare greyscale version maybe just try to print your game greyscale and check how it looks. Maybe
it will be usable if you only make few elements darker or lighter? It can even improve readability of your normal (color) version.

### Color space

For home printers choose sRGB (default in many graphic tools). You can eventually consider Adobe RGB, but not every printer supports it
and colors would be compressed. Forget about CMYK. ;-)

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

Should there be cutting marks between components?

It depends, if you take into account bleed - they may be helpful when cutting, but from my experience, they are not necessary. If you have space to add them without interfering with bleed - go for it. 

```
Note: Proper bleed prevents cutting marks beeing too close to component.
```

#### Bleed

##### What is bleed?

Bleed is part of graphics which extends behind component. In practice, if component is made by image, part of that images (all edges) will be cut off final component. If there is one color edge on the component it is just additional space taken by that color added to all edges of the component.
In example, if you have poker sized card (63.5x88.9mm) with 2mm bleed it will take 67.5x92.9mm of space on page..

Characteristics:

1. Bleed is necessary to allow slight cutting/alignment errors.
2. Bleed should be 2-3mm.
3. Best when created during component design phase.
4. You need to have bleed area around every edge of the component.

**Fake bleed**

Fake bleed is bleed added later, not at design phase, to provide area for cutting/alignment errors. I would distinguish two types of fake bleed:

- **graphical** - tries to continue graphic design from components (usually created by cloning some parts of original design). It is quite hard to do and sometimes impossible to do well, but when done right results may be very good.
- **one color** - to add bleed it is needed to modify component itself. If component originally doesn't have one color edge, it is added to the component (usually covering 2-3mm of the component) and then extended to form additional 2-3mm bleed (so lets say you have 6mm one color edge total). This is worst type of situation, but sometimes necessary (I saw this kind of bleed on gamecrafter). 

NOTE: You can not just add one color around component and call it bleed. It will still create bad looking edges on any misalignment.


![alt text][bleed]

### Page size A4 vs U.S. Letter

```
NOTE: Remember that A3 (legal) printers are rare, while you can provide A3 board you should
provide also 2xA4 alternative.
```

In centimeters (cm):

| Format | Width | Height |
|--------|-------|--------|
| A4     | 21    | 29.7   |
| letter | 21.59 | 27.94  |

**Margins**
Use at least **5mm** (0.5cm, 0.2inch) margin on every side. If you want be safe, use **10mm** (1cm, 0.4inch) margin.

#### Usable space
Let's assume you have 3mm cutting marks + 2mm bleed + 5mm margin. 

**A4**
Usable space is **190x277mm** moved 10mm right and down from the left upper corner of the page.

**Letter**
Usable space is **190.59x259.4mm** moved 10mm right and down from left upper corner of the page.

```
NOTE: Please let me know if your printer can't print so close to the edge! I will update info here.
```

#### If you prepare only one version

If you use **A4** leave extra **18mm** (1.8cm) margin at the **bottom** of the page. So you need **23mm** (2.3cm) space at the bottom. You can set your guide in Inkscape to **274mm**.

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

Also remember that duplex printing layout should contain always page with fronts, then page with backs, and so on. Even if you feel, that your file is bigger then it could. This way you will allow for quick printing without investigation which backs are for which components.

There is also very good addition to duplex format - outline. This element was introduced to me by countersheet Inkscape extension and I find it briliant. It is outline around whole page and it allows to cut along it. When someone prints fronts and backs on separate pages outline allows to align fronts and backs much better then shown in linked Polish tutorial. It eliminates priner drift.

Example page from my unpublished prototype with outline:

![duplex-outline][duplexoutline]

##### When duplex printing is used?

* For every form of "quick printing". When someone wants to play as soon as possible and do not care about perfect build. Also when someone wants to print only fronts of your components.
* If someone has:
  - double-sided photo paper,
  - linen or other decorated thick paper.
* When someone has no other option. It is still possible to glue front and back (usually with cardboard between) quite precisely,
  but it is much harder comparing to gutter fold layout.

Precision of duplex printing depends heavily on printer. Usually there will be some shift so bleed is necessary. 
It works best if cut from back side of component.

##### Do we need cutting lines on both sides of components (backs and fronts)?

Yes, we do. :-)

If someone is gluing fronts and backs together they need them to align fronts with backs.

If you are interested how this can be done, let me know, for now I will leave you with article in polish ;-), sorry for that, 
but it is the only source I know, which describe process clearly. Just look at the pictures.

http://piotrnowinski.pl/wlasne-projekty/gry-planszowe/jak-profesjonalnie-przygotowac-karty-do-gry

Here is link for google-translated version:
https://translate.google.com/translate?hl=&sl=pl&tl=en&u=http%3A%2F%2Fpiotrnowinski.pl%2Fwlasne-projekty%2Fgry-planszowe%2Fjak-profesjonalnie-przygotowac-karty-do-gry

#### Gutter fold

This is very good layout for PNP, lets see why.

![alt-text][gutterfold]

1. We have bleed.
2. Cutting marks are perfect.
3. Fronts and backs are aligned perfectly - always!
4. Usually we do not loose any paper space.

Gutter fold allows for best quality components because there will be no shift between backs and fronts.

##### Remember when preparing

1. **Folding line** should be at least **5mm** from (almost 1/4inch) bleed.
   Sometimes even bigger space would be beneficial if components are meant to be thick (f.e.: 2mm cardboard used as core). 
   With thicker core material there is risk of fold not being in the center, which will result in misalignment. More space
   should prevent that (*TODO: really? I need to experiment more with that*).
2. Backs have to be upside down.

##### Double cutting lines (bleed between components)

I would recommend using double cutting lines, this will ensure bleed area is around all components edges. As with duplex printing layout, it is very important have bleed if your edges are different color or have any sort of pattern/gradient.

My layout of **Barry Skinner** [DNGN](https://boardgamegeek.com/thread/2475283/wip-dngn-minimalist-style-euro-inspired-dungeon-cr/page/1):
![Gutter fold layout with bleed everywhere][gfbleed]

##### When gutter fold layout is used?

Always ... well almost always. If someone wants to have best looking game, she/he would use this layout provided by author or created by user. There is no better layout known to mankind yet. :-D


## Instructions for game users

It is always good idea to provide short instructions how to print and cut your game.

Here are instructions which you can include inside your files or alongside them.

[Gutter fold instruction - source](articles/gutter-fold-howto.md)
 * ![PDF A4 Portait][gA4port]
 * ![PDF A4 Landscape][gA4land]
 * ![PDF Letter Portait][gLetterport]
 * ![PDF Letter Landscape][gLetterland]

![Whole directory][ginst]


## Biggest mistakes

* **Lines around component.** Usually they are there to simplify cutting, but in reality, they are nightmare. You always end up with ugly black lines around some edges of the component. It will be quite random and they will ruin your build.
* **No cutting helpers at all.** How one should cut it? ;-)
* **No bleed** We are not perfect. Some people are really manually talented, others are not experienced cutters or they are using non-optimal equipment. By providing bleed you can even they chances to have nice looking game. I had seen people solving no bleed by cutting into component, which may ruin you design.

* ****

## Practical tutorials

Do you want to learn how to create layouts with Inkscape? Here you go:

* [Inkscape - create layout without template](articles/inkscape/gutter-fold-without-template.md)


## Feedback

I would love to hear any critics you have for this text. English is not my first language, so it would be great if we can iron out wording and grammar here. :-)

You can create issue (or PR!) on github or contact me by **geekmail**:

https://boardgamegeek.com/geekmail/compose?touser=ernierasta

## TODO

This how-to is not considered complete without:

- more tools to create/edit pdf (need to investigate their availability under Windows OS),
- short how-to print&cut in form of svg and pdf which game designers can distribute along their files or included in files.
- example article (or/and video) how to prepare both layouts in Inkscape.
- example how to automate layout creation using Inkscape extensions.

[introcards]: images/intro.png
[cuttingmarksgood]: images/crop-marks-good.png "Good crop marks"
[cuttingmarksbad]: images/crop-marks-bad.png "Bad crop marks"
[bleed]: images/bleed.png "Bleed example"
[duplex]: images/the-shooting-party_duplex.png "Duplex example"
[duplexbleed]: images/twin-stars_duplex-bleed.png "Duplex with bleed"
[duplexoutline]: images/duplex-outline.png "Duplex with outline"
[gutterfold]: images/the-shooting-party_gutter-fold.png "Gutter fold example"
[gfbleed]: images/gf-with-bleed.png
[ginst]: articles/gutter-fold-howto
[gA4land]: articles/gutter-fold-howto/A4-landscape.pdf
[gA4port]: articles/gutter-fold-howto/A4-portait.pdf
[gLetterport]: articles/gutter-fold-howto/letter-portait.pdf
[gLetterland]: articles/gutter-fold-howto/letter-landscape.pdf


