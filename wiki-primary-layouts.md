The following are the "Primary Layouts", which refer to the overall look of the product presentation. Within a Primary Layout, there is the ability to select and configure SKU and price presentation.

The Primary Layouts available so far are:

[ImageAboveName](#imageabovename)  
[NameWrapAroundImage](#namewraparoundimage)  
[NameAboveImageOnLeft](#nameaboveimageonleft)

## *ImageAboveName*
This layout displays:
* product image
* product name
* SKU number
* price (either simple or superior)


**Example #1: _Image Above Name_ with _simple_ price format**
<img src="http://app.catalog-on-demand.com/images/linden_layouts/linden-image-over-prodname-simple-price.PNG" width="600">


In order to support this layout, the variable.csv file must contain all of the parameter labels shown in this sample csv. The values (to the right of the comma) are the defaults.

Sample csv:

    ImageDesc_LType,ImageAboveName
    FontFamily,HelveticaNeue
    MaxImageHeight,0.5
    MaxNameHeight,0.45
    StyleProdName,none
    NameLRMg,0.1
    NameFontSize,9
    NameLeading,10.8
    DescFontSize,9
    DescLeading,10.8
    MaxDescHeight,1.0


## *NameWrapAroundImage*
This layout displays:
* Product name, wrapped around the product image
* SKU number
* Price (either simple or superior)

**Example #1: _Name Wrap Around Image_ with _superior_ price format**
<img src="http://app.catalog-on-demand.com/images/linden_layouts/linden-prodname-wrap-image-superior-price.PNG" width="600">

In order to support this layout, the variable.csv file must contain all of the parameter labels shown below. The values (to the right of the comma) are the defaults.

    ImageDesc_LType,NameWrapAroundImage
    FontFamily,HelveticaNeue
    StyleProdName,none
    MaxImageHeight,0.5
    MaxImageWidth,1.4
    NameLRMg,0.1
    NameFontSize,9
    NameLeading,10.8
    DescFontSize,9
    DescLeading,10.8
    MaxDescHeight,1.0


## *NameAboveImageOnLeft*

This layout displays:
* *Left side:* Product name above the image
* *Right side:* Description above either (a) the SKU/item info; or (b)&nbsp;a SKU table

**Example #1: _Name above image on left_ with _single SKU_**
<img src="http://app.catalog-on-demand.com/images/layoutsplus/NameAboveImageOnLeft-singlesku.PNG" width="600">

<hr>

**Example #2: _Name above image on left_ with _table_**
<img src="http://app.catalog-on-demand.com/images/layoutsplus/NameAboveImageOnLeft-table.PNG" width="600">

In order to support this layout, the variable.csv file must contain all of the parameter labels shown in this sample csv. The values (to the right of the comma) are the defaults.

Sample csv:

    ImageDesc_LType,NameAboveImageOnLeft
    LayoutWidth,7.3
    FontFamily,HelveticaNeue
    MaxImageHeight,0.5
    MaxImageWidth,1.4
    StyleProdName,none
    NameLRMg,0.1
    NameFontSize,9
    NameLeading,10.8
    DescFontSize,9
    DescLeading,10.8
    MaxDescHeight,1.0

# Parameter definitions

**ImageDesc_LType** — The options are:
* [ImageAboveName](#imageabovename)
* [NameWrapAroundImage](#namewraparoundimage)
* [NameAboveImageOnLeft](#nameaboveimageonleft)

**FontFamily** — The choices are:
* HelveticaNeue (default)
* HelveticaNeueCondensed
* MyriadPro
* ProximaNova
* Arial

**StyleProdName** — The choices are:
* none — No style will be applied to the product name
* bold — This will cause the product name to appear bold

**SKU_LType** — [See Configuration of SKU/Price Sub-layouts](../wiki/Configuration-of-SKU-Price-Sub-layouts)

**MaxImageHeight** — This is the maximum height of the images in inches. It is also the height of the image box, even if the image is not this tall. (Default is 0.5)

**MaxImageWidth** — This is the maximum width of the product image in inches. (Default is 1.4)

**MaxNameHeight** — This is the maximum height of the product name in inches. If the text wraps beyond this height, it will be truncated with the ellipsis (...). (Default is 0.45)

**NameLRMg** — The left & right margin of the product name in inches. (Default is 0.1)

**NameFontSize** — The font size of the product name in points. This can be a decimal number. (Default is 9)

**NameLeading** — The leading of the product name in points. This can be a decimal number. (Default is 10.8)

**ImageDesc_LType** — The value must be set to _NameWrapAroundImage_

**LayoutWidth** — This is the width of the layout in inches. Only full width layouts are supported at this time. (Default is 7.3)

**MaxImageWidth** — This is the maximum width of the product image in inches. (Default is 1.4)

**DescFontSize** — Font size of the description in points. This can be a decimal number. (Default is 9)

**DescLeading** — The leading of the product description in points. This can be a decimal number. (Default is 10.8)

**MaxDescHeight** — This is the maximum height of the product description in inches. If the text wraps beyond this height, it will be truncated with the ellipsis (...). (Default is 2.0)
