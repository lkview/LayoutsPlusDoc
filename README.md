# LindenPlus
This is about parameterized Linden layouts. 
It uses the system plug-in called **LindenPlus**. 
It requires that variables be defined in the private dropbox folder called **_CoDVariables**. The naming convention is as follows:

    account id_-variables.csv

For example, 

    corvettemods-variables.csv

Any undefined variable will be assigned its default.

### Product layout: *ImageAboveName*
This layout was originally developed to support corvettemods. It displays:
* product image
* product name
* SKU number
* price

In order to support this layout, the variable.csv file must contain all of the parameter labels shown in this sample csv. The labels are required as shown. The values (to the right of the comma) are explained below.

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

**SpaceCurrency** — Must be true or false, indicating whether there should be a space after the currency symbol. (Default is false)

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

