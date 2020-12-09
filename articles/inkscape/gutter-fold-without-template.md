# Inkscape - creating layout from scratch

## Overview

In this tutorial we will create component layout from scratch, without using template. There will be no automation, we will just use bare Inkscape.

I hope to make video later (will be linked here), which will show more.

## Before reading

* Install Inkscape, make sure it is running ok. I have version 1.0, so try to use latest version availabile, but do not worry too much about it.

```
Note: Text in square brackets means keyboard key or combination of keys pressed together. 
So [A] means: press A key on keyboard.
```

* Familiarize yourself with following Inkscape tools:
    - Select and transform tool [**S**],
    - Bezier Pen [**B**],
    - Rectangle tool [**R**],
    - Gradient tool [**G**],
    - Text tool [**T**].
* Enable and familiarize yourself with panels:
    - Layer - Layers...
    - Object - Fill and Stroke...[**CTRL+SHIFT+F**]
    - Object - Transform...[**CTRL+SHIFT+M**]
    - Object - Align and Distribute...[**CTRL+SHIFT+A**]
    - Object - Arrange...

If you want, go watch **Logos by Nick**. They are brief and excellent.

[![Inkscape Explained in 5 Minutes](https://img.youtube.com/vi/pa6a7oz7vEE/hqdefault.jpg)](https://www.youtube.com/watch?v=pa6a7oz7vEE)

[![All 21 Inkscape Tools Explained in 10 Minutes](https://img.youtube.com/vi/qq7HsMvEVmU/hqdefault.jpg)](https://www.youtube.com/watch?v=qq7HsMvEVmU)

Then try all of mentioned tools/panels. OK, let's go!

## Create page with double-sided tokens

We have double-sided square tokens for your fictional game to arrange. For this tutorial, we will create very primitive placeholder tokens as part of tutorial, but you can use your own tokens (in vectors or **File - Import..**. raster graphics).

We are using **A4** page size and **milimeters** as units. I would recommend to stick with that for now. Also page is "universal" it will print fine on **letter** format page.

In following tutorial we will create **gutter fold** layout, but you can use the same steps for creating **duplex printing** layout, where first page will contain fronts without central line (you can probably fit there 2 lines of tokens more) and second page with backs. In Inkscape every page is separate file. They can be merged to create one pdf file, but this is covered in separate tutorial.

### Prepare our example token

1. <ins>Create token background</ins>
    * With **Rectangle tool** [**R**] draw rectangle, open **Fill and Stroke** [**CTRL+SHIFT+F**], on **Stroke paint** tab click on **No paint**, on **Stroke style** set *Width* to 0, on **Fill** tab choose *Linear gradient*. 
    * Select **Gradient tool** [**G**]. Choose color for the first gradient node and click on some light color on the bottom, for other node choose other light color. 
    * Press [**S**], in toolbar switch to **milimeters** and enter 34 in **W**idth and in **H**eight boxes, confirm new values by pressing [**Enter**]. Out tokens will be 3cm by 3cm, but we need bleed.
2. <ins>Place some text on token</ins>
    * Press [**T**] for **Text tool**. Click somewhere outside our token and write "My token", select font and size in toolbar. 
    * Press [**CTRL+SHIFT+A**]. Press [**S**] and select our text object if not already selected, hold **SHIFT** key and click on square. In **Align and distribute** panel set *Relative to:* to **Last selected**. Click on icons: **Center on horizontal axis** and **Center on vertical axis**.
3. <ins>Group token</ins>
    * While having square and text selected press [**CTRL+G**] to group objects. Then in toolbar click on **Move gradients** icon (it is one before last) or checkbox.

Great! We have our token done!

### Create layout based on grid

1. <ins>Document Properties</ins>
    * **Open File - Document Properties**. 
    * Select **A4**, **portrait**.
    * Switch to **Grids** tab. Choose **Rectangular grid** and click **New**. Set **Grid units** to **milimeters**. Set *Align to page* to center point. Set **Spacing X** and **Spacing Y** to 8.5, **Major grid line every** leave at 5. 
    * Close dialog.
2. <ins>Create Center (folding) line</ins>.
    * Press [**B**], click, hold **CTRL**, second click at the end, press [**Enter**] - you will draw horizontal line almost as wide as page (leave at least **5mm** from edge).
    * Press [**CTRL+SHiFT+A**] and set *Relative to:* to **Page** and click on:  **Center on horizontal axis** and **Center on vertical axis**.
    * Press [**CTRL+SHIFT+F**], select **Stroke style** tab, set units to millimeters and set *Width* to **0.150**. 
    * Line should lay on grid line.
3. <ins>Create token back</ins>
    * Press [**S**] and select our token. Press [**CTRL+D**] to duplicate it, then click and drag new token somewhere close to original token. 
    * Hold **CTRL** and double click on duplicated token text. Change it to: **"My token[Enter] back"** where "back" is on second line. In toolbar set **Text alignment** to **Center**. Press [**ESC**].
    * Press [**S**]. Click on duplicated token then [**CTRL+SHIFT+G**] to un-group it. Press [**ESC**], click on text, then hold **SHIFT** and click on square background. Press [**CTRL+SHIFT+A**] set *Relative to:* to **Last selected** and center on both axes. Press [**CTRL+G**] to group it back. 
    * Press **CTRL+]** (CTRL + square bracket) twice to rotate it upside down.
4. <ins>Place token and its back</ins> 
    * Enable snapping by pressing [**SHIFT+5**], make sure that **Snap to grids** is enabled. 
    * Snap token above our center line (one grid square away from line) and two grid square from the left page edge.
    * Place token back under center line one grid square from line and two grid squares from the left page edge.
5. <ins>Create page of tokens</ins>
    * Select (holding **SHIFT**) token front and back, press [**CTRL+D**] to duplicate and move them to the right, so they are touching tokens on the left side. 
    * Select all 4 elements (2 fronts and 2 backs), again duplicate [**CTRL+D**], move, etc. 
    * Using that technique create 5 tokens on a row. Then duplicate whole rows of fronts and backs.
6. If you want to have universal page printable on letter paper you should have 3 by 5 of fronts and the same amount of backs.

Layout done!

### Cutting marks

1. <ins>Creating lines horizontal lines</ins>
    * Make sure snapping is enabled [**SHIFT+5**] and enable: **Snap to cusp nodes, incl. rectangle corners** (it is in the middle of snapping toolbar) and **Snap to grids**.
    * Press [**B**] click somewhere on the grid intersection and create horizontal line by clicking on other intersection, press [**Enter**], you will create 8.5mm long line. Press [**CTRL+SHIFT+F**], on **Stroke style** set width to 0.1mm. Drag line so right end will snap to the **top-left** corner of the most top-left token. 
    * Disable **Snap to grids** in snapping toolbar. Duplicate line [**CTRL+D**] and move new line to the bottom-left corner of the same token.
    * Continue duplicating lines and moving them down 2 more times. Now you have 4 lines, all touching token corners.
2. <ins>Creating vertical lines</ins>
    * Press [**S**] and select one line. Press [**CTRL+D**] to duplicate it, press **CTRL+]** to rotate it. Move line so bottom end will snap to **top-left** corner of most top-left token.
    * Duplicate line by pressing [**CTRL+D**] and move new line to the **top-right** corner of the same token.
    * Continue duplicating and moving 4 more times as with horizontal lines. All corners would have line.
3. <ins>Move lines to right places</ins>
    * Select 2 horizontal lines in the middle (not upper and bottom ones). Press [**CTRL+D**] to duplicate them. Hold **SHIFT** and add top line to selection (now you have 3 lines selected). Press [**CTRL+SHIFT+M**] and **Transform** panel will open. On **Move** tab check **Relative move** and make sure **Apply to each object separately** is **unchecked**, set units to millimeters, set **Vertical** to **2** and press **Apply** button. Press [**ESC**]
    * Select again the same 2 lines in the middle and bottom line. In **Transform** panel on **Move** tab change vertical from 2 to **-2** and press **Apply**.
    * Apply the same logic to vertical lines. Select all 4 middle lines (without first and last), [**CTRL+D**], hold **SHIFT** and click on the first line. In **Transform** panel on **Move** tab set **Vertical** to **0** and **Horizontal** to **2**, press **Apply**.
    * Select the same 4 middle lines and last line. In **Transform** panel on **Move** tab change **Horizontal** to **-2**. Press **Apply**.
4. <ins>Copy cutting lines where needed.</ins>
    * Make sure, that snapping is enabled [**SHIFT+5**], enable **Snap to paths** and **Snap midpoints of line segments** (first and last icons in **Snap nodes, paths, and handles** section).
    * Select all 6 horizontal lines. Press [**CTRL+D**], hold **CTRL** and drag lines to the right edge of page, so left lines ends will snap into the right tokens edges.
    * Select all 10 vertical lines. Press [**CTRL+D**] and holding **CTRL** snap them to the folding line, so they will be divided be folding line by half.
    * Press [**CTRL+D**] again and move duplicated lines holding **CTRL** to the bottom of last token backs row. Snap lines top end to the bottom tokens edge.
    * Select all 12 horizontal lines (on both sides of tokens), duplicate them [**CTRL+D**], move them down holding [**CTRL**], so bottom line will snap to the most bottom corner. Press [**CTRL+SHIFT+M**] and on **Move** tab set **Horizontal** to **0** and **Vertical** to **-2**, click **Apply**.

**Congratulations! You have just created finished product!**

You can export it to PDF with **File - Save a copy ...**. You can use this as a template for next pages, just **File - Save as ...** different file, delete token fronts with [**DEL**] and replace them by new ones.
