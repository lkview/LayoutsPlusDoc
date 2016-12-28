The following are the "Primary Layouts", which refer to the overall look of the product presentation. Within a Primary Layout, there is the ability to select and configure price presentation. 

The Primary Layouts available so far are:

[ImageAboveName](#imageabovename)  
[NameWrapAroundImage](#namewraparoundimage)

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
    SKU_LType,A
    MaxImageHeight,0.5
    MaxNameHeight,0.45
    NameLRMg,0.1
    NameFontSize,9
    NameLeading,10.8
    SKUWidth,0.8
    PriceWidth,0.8
    SKUFontSize,9
    PriceFontSize,9
    Currency,$
    SpaceCurrency,false
    PriceStyle,simple
    PriceFormat,#,###.##
    PriceColor,FF0000
    NumericCharWidth,0.145


**ImageDesc_LType** — The value must be set to **ImageAboveName**.

**SKU_LType** — The choices are:
* A — This shows the SKU number in bold on the left, and the price on the right. A thin rule is above both. (Default is A)
* B —  Not invented yet
* C —  Not invented yet 

**MaxImageHeight** — This is the maximum height of the images in inches. It is also the height of the image box, even if the image is not this tall. (Default is 0.5)

**MaxNameHeight** — This is the maximum height of the product name in inches. If the text wraps beyond this height, it will be truncated with the ellipsis (...). (Default is 0.45)

**NameLRMg** — The left & right margin of the product name in inches. (Default is 0.1)

**NameFontSize** — The font size of the product name in points. This can be a decimal number. (Default is 9)

**NameLeading** — The leading of the product name in points. This can be a decimal number. (Default is 10.8)

**SKUWidth** — The width of the box containing the SKU number, in inches. The SKU number is left-aligned. (Default is 0.8)

**PriceWidth** — The width of the box containing the price, in inches. The price is right-aligned. (Default is 0.8)

**SKUFontSize** — Font size of the SKU number. (Default is 9)

**PriceFontSize** — Font size of the price. (Default is 9)

**Currency** — Currency symbol (Default is $)

**SpaceCurrency** — If there should be a space after the currency symbol and before the price, this value must be "yesspace". (Default is "nospace")

**PriceStyle** — The choices are:
* Simple — The symbol, left side, and right side are all the same size
* Superior — The symbol and the right side are half size, and top aligned

**PriceFormat** — *Not yet available*. Default is #,###.## 
The choices are:

    #,###.##
    #.###,##
    # ###.##
    # ###,##
    #'###.##
    #,##,###.##
    #.###
    #,###.###

**PriceColor** — Express as RGB hex. Default is FF0000

**NumericCharWidth** —  This is required only if **PriceStyle** is set to _Superior_. The value is the width of one numeric character at the **PriceFontSize**.



## *NameWrapAroundImage*
This layout displays:
* Product name, wrapped around the product image
* SKU number
* Price (either simple or superior)

**Example #1: _Name Wrap Around Image_ with _simple_ price format**
image not yet available

**Example #2: _Name Wrap Around Image_ with _superior_ price format**
<img src="http://app.catalog-on-demand.com/images/linden_layouts/linden-image-over-prodname-superior-price.PNG" width="600">

In order to support this layout, the variable.csv file must contain all of the parameter labels shown in this sample csv. The values (to the right of the comma) are the defaults.

Sample csv:

    ImageDesc_LType,NameWrapAroundImage
    SKU_LType,A
    MaxImageHeight,0.5
    MaxImageWidth,1.4
    NameLRMg,0.1
    NameFontSize,9
    NameLeading,10.8
    SKUWidth,0.8
    PriceWidth,0.8
    SKUFontSize,9
    PriceFontSize,9
    Currency,$
    SpaceCurrency,false
    PriceStyle,simple
    PriceFormat,#,###.##
    PriceColor,FF0000
    NumericCharWidth,0.145


**ImageDesc_LType** — The value must be set to NameWrapAroundImage

**SKU_LType** — Same as _ImageAboveName_

**MaxImageHeight** — Same as _ImageAboveName_

**MaxNameHeight** — This is the maximum height of the product name in inches. If the text wraps beyond this height, it will be truncated with the ellipsis (...). (Default is 0.45)

**NameLRMg** — The left & right margin of the product name in inches. (Default is 0.1)

**NameFontSize** — The font size of the product name in points. This can be a decimal number. (Default is 9)

**NameLeading** — The leading of the product name in points. This can be a decimal number. (Default is 10.8)

**SKUWidth** — The width of the box containing the SKU number, in inches. The SKU number is left-aligned. (Default is 0.8)

**PriceWidth** — The width of the box containing the price, in inches. The price is right-aligned. (Default is 0.8)

**SKUFontSize** — Font size of the SKU number. (Default is 9)

**PriceFontSize** — Font size of the price. (Default is 9)

**Currency** — Currency symbol (Default is $)

**SpaceCurrency** — If there should be a space after the currency symbol and before the price, this value must be "yesspace". (Default is "nospace")

**PriceStyle** — The choices are:
* Simple — The symbol, left side, and right side are all the same size
* Superior — The symbol and the right side are half size, and top aligned

**PriceFormat** — *Not yet available*. Default is #,###.## 
The choices are:

    #,###.##
    #.###,##
    # ###.##
    # ###,##
    #'###.##
    #,##,###.##
    #.###
    #,###.###

**PriceColor** — Express as RGB hex. Default is FF0000

**NumericCharWidth** —  This is required only if **PriceStyle** is set to _Superior_. The value is the width of one numeric character at the **PriceFontSize**.



