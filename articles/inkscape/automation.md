# Inkscape - automatic layout and components creation

## Overview

While **Inkscape** itself could help a lot with game designing tasks, when combined with extensions dedicated for board games creation you will get one of best tools you could ever use to create your layouts in minutes! In this tutorial we will not only generate layouts, but also create cards, which uses as much vector graphics as possible and use raster images only as illustration. 

In next tutorial we will take already created raster (for example in png format) components and arrange them on the page.(TODO)

Goal of this how-to is to take our components and generate all layouts and files we need.

----------------------------------------------------------

**Note**: You may wonder if this is best approach to automation, there are other tools dedicated to creating cards (or maybe other components). Choice is yours, but here is why I think this is the best combination:

 * **Inkscape** is open source, forever free, amazing vector designing program which will be there next 50 years. ;-)
 * **countersheetsextension** is open source, forever free, advanced tool, dedicated to board games creation. It is written by **Pelle Nilsson** board game designer who understand how it should work, it has many advanced features and good documentation. Github commits starts in 2010 which means there is **more then 10 years of development**.
 * This is multiplatform solution, so works on **Linux**, **MacOS** and **Windows**.
 * It is universal, you need **tokens**, **cards**, **dices**, **standies**, ... you can create/arrange them all using the same tools.
 * It is **easy**, but **powerful**. You can start quick and small, but tool allows you to set many options if you need them. It will grow with you.
 * **You are in control**. After you generate components - you will get ordinary **svg file**, which you can edit as you like. This allows you to customize output as you want it to be, even if extension doesn't (yet) do exactly what you need.
 * **Automatic PDF generation**.

## Why every game creator should use automation?

I really believe, that everyone should automatically generate their layouts and components. Here are reasons why:

 * **Easy iterative changes.** Fix typo, change icon, click twice, done. New version ready to release (in multiple layouts).
 * **Quick experiments and easy cooperation.** Do you want to try new graphic element? Change it, click and check out all your components.
 * **Much faster workflow.** After following this tutorial you will create your games much faster!
 * **Easy translation.** All texts are in one file editable with Libreoffice Calc or MS Excel.
 * **Professional output** Automation allows you create and maintain multiple layouts for different styles of game builds without additional work.

## Software used

* **Inkscape** - core of all our work.
* **countersheetsextension** - Inkscape extension.
* **Libreoffice Calc** - to manipulate csv files. You can use **MS Excel** or any other editor you want, but all info here is for **Calc**.

## Before reading

For **Inkscape** I would recommend to read **Before reading** section in [previous Inkscape tutorial](gutter-foud-without-template.md) if you are not familiar with Inkscape.
For **countersheetsextension** installation go to [official wiki](https://github.com/lifelike/countersheetsextension/wiki/Install). Just install it (copy to extension folder) and go back here.
For **Libreoffice**, just go to [official site](https://www.libreoffice.org/) to download it, or install it as you normally install your programs (package manager).

## How automation works?

We will have our layout and our components design in svg file. We will use data entered in spreadsheet to generate final svg file. We will also have other graphic files with parts of our design, which will be embedded into main layout svg file. After we generate everything, we will export it into pdf.

## Preparing components

Let's create basic card. Open **Inkscape**, in **File - Document properties ...** make sure we have **A4** **portrait** set (to not worry we will take care of US Letter later).

With **Rectangle tool** [**R**] create rectangle of any size. Open **Fill and stroke** panel [**CTRL+SHIFT+F**], on **Stroke style** tab switch to **millimeters** and set **Width** to **0.001**. On **Stroke** tab set color to black and on **Fill** tab click on **cross** to disable fill. Press [**S**] to switch to **Select and transform tool** and in toolbar switch to **millimeters** set width to **63.5** and height to **88.9** ([**Enter**] will confirm value) - those are poker card dimensions. Move our card out of page if it is on it.

Now press [**CTRL+D**] to duplicate rectangle, on the bottom color toolbar click on some color, f.e: red(#FF0000). This will be our card border at the end, we will change it's color for different cards. Hold **SHIFT** and click on bottom color toolbar on X to disable stoke. To open **Transform** panel press [**CRTL+SHIFT+M**] switch to **Scale** tab and add bleed by adding 2mm on all sides, so switch to **mm** and set width to **67.5**, height to **92.9** and hit **Apply**. Then send this rectangle to the bottom by pressing [**End**].

Press [**Tab**] to switch to our previous rectangle (or click on it when zoomed in). Open Object panel by pressing [**CTRL+SHIFT+O**] and change ID to "card" and click **Set** (I will explain it later).

Press [**CTRL+D**] to duplicate rectangle, click on 2.5% gray (#F9F9F9FF) and then hold **Shift** and click on X symbol on bottom color toolbar. Press [**CTRL+SHIFT+M**] and on **Scale** tab click on **Clear**, set **mm** and width to **53.5** and height **78.9**. This is our card main area.

Now with **Rectangle tool** [**R**] create some rectangle next to our card (but not on it), with **Select tool** [**S**] set it to 3mm x 3mm. Set color to f.e. green (#abc837ff). Press [**CTRL+D**] to duplicate, drag duplicated square down, click on it to get rotation handles, hold [**CTRL**] drag corner to rotate by 3 "jumps", so it will be rotated by 45°. Change color to orange (#FF6600). Create circle [**E**], make it blue () with no stroke (**Shift** and click on X) and [**S**] to set size to 3x3 millimeters. Press [**SHIFT+8**] for **Stars and polygons tool**, in toolbar set **Regular polygon** and **3** corners. Draw triangle holding **CTRL** (bottom should be horizontal), on toolbar click on **lock** icon (between width an height) and set width to **4.243mm**, change color to pink (#FF2A7FFF).


Press [**CTRL+SHIFT+O**] click on all 4 symbols one by one and name them **ssquare**, **sdiamond**, **scircle**, **striangle**, do not forget to press **Set** every time you write it to **ID** box.

_**NOTE**: as it is easy to get lost in object names, I am using convention, where all objects which serve the same function, in other words - will be placed on component on the same spot - are prefixed with the same letter(-s). 
<br>In this case, all symbols are prefixed with "s"._

Select green rectangle and make clone of it by **Edit - Clone - Create clone** [**ALT+D**], shortcut may not work under Linux. Open **Object properties** [**CTRL+SHIFT+O**] and set **ID** to **symbol**, press **Set**. Enable snapping [**%**] if not already enabled and make sure you have **Snap to cusp nodes, incl. rectangle corners** enabled. Take clone and snap it to the left upper corner of the card, to the inner corner of the red edge. Press [**CTRL+SHIFT+M**] to open transform panel and on **Move** tab make sure **Relative move** is checked, set horizontal to **-0.5** and vertical to **-0.5**, press **Apply**. Switch to **Text tool**, click somewhere out of anything, write **2** and set font and size (I've used **Dejavu Sans Mono** and **8** size). Press [**CTRL+SHIFT+O**], set **ID** to **number** press **Set** button. Switch to **Select tool** and holding **Shift** click on clone (so number 2 and cloned image is selected), press [**CTRL+SHIFT+A**], set **Relative to** to **Last selected** and click on **Center on vertical axis** and **Center on horizontal axis**.

Let's download some graphics. 

## Special object names

### Special layers:

**cs_layout** layer - when named **cs_layout** layer will dictate space availabile for components. Every rectangle will be used as place for components. Bleed doesnt count as occupied space.

**cs_background_front** layer - this layer will be added to all pages containing components fronts. You can use it to add additional elements or cutting helpers to the page.

**cs_background_back** layer - this layer will be added to all pages containing components backs.

All three layers supports suffixes, so instead **cs_layout** you can have **cs_layout_mysuffix**(where **mysuffix** is suffix entered in plugin configuration).


### Special objects


**cs_regstyle** line - 
**cs_foldstyle** line - 

## CSV Cheatsheet

There may be **multiple** tables in one csv file! Just leave **one empty line** between tables. 
**ID** means **object ID** in Inkscape, which is set after **[CTRL+SHIFT+O]**.

column1 header  | column2 header
----------------|----------------
column1 value 1 | column2 value 1
column1 value 2 | column2 value 2

**"x"** below means object ID , not literal x!

Special **header** symbols:
 
 * **first column header** - is always template ID.  
 * **@x** - hide template defining rectangle. Used very often. 
 * **BACK** - if you name column like that, it will mean, that component have a back. There must be **y** as value in column.
 * **+** - by default back use the same template as front,if you name column simply **'+'** you can define different template for backs. Put **x** or **@x** as value, where **x** is ID of template. 
 * **partx*** or ***partx** - means wildcard. **partx** means part of object ID. Values in this column will change multiple objects, like **x1**, **x2**, **xten** or in second case **1x**, **2x**, **tenx**.
 * **x[style:fill]** or **x[style:stroke]** - allows to set **fill** or **stroke** color for element called **x**. You can set also: **stroke-width** and many others. You can find more in [spreadsheetextension wiki](https://github.com/lifelike/countersheetsextension/wiki/Set-Style). You can also use this header to copy style of other object (value in column must be \<id), [more](https://github.com/lifelike/countersheetsextension/wiki/Copy-Style).

Special **column** values:

 * **number in first column** - how many of this components will be generated. You can also use **number+**(fill whole row with tokens), **number++** fill entire box, **number+++** current page. **number** determines minimal ammount, f.e. **3++** creates at least 3 components and continues creating them until they fill whole box (rectangle in **cs_layout** layer).
 * **=somevalue** - set default value for this column. Default is used if there is no value given for this row.
 * **\<x** - combined with header **x[style:x]** copies given style from **\<x** object.
 * **@x** - hide template defining rectangle.
 * **<<filename.txt** - read given text file.
 * **\*bold*** and **_/italics/_** - use **star**(\*) to make text **bold** and **slash**(/) to make text _italics_.
 * **{filename.png}** - place image inside text.
 * **%autonumber%** - if you put **%autonumber%** into text, it will be replaced by number (automatic sequence 1,2,3,...).

## TODO:

A4 sizing:

`cs_layout_duplex` : 190 x 277 

`cs_layout_gutter` : 90 x 277

