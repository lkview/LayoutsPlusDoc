# LindenPlus
This is about parameterized Linden layouts. 
It uses the system plug-in called **LindenPlus**. 
It requires that variables be defined in the private dropbox folder called **_CoDVariables**. The naming convention is as follows:

    account id_-variables.csv

For example, 

    corvettemods-variables.csv

There is no forgiveness in the naming of the variables, or for missing variables. The job will immediately give an error if a variable is missing or misspelled.

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
* A — This shows the SKU number in bold on the left, and the price on the right. A thin rule is above both.
* B —  Not invented yet
* C —  Not invented yet 

**MaxImageHeight** — This is the maximum height of the images in inches. It is also the height of the image box, even if the image is not this tall.

**MaxNameHeight** — This is the maximum height of the product name in inches. If the text wraps beyond this height, it will be truncated with the ellipsis (...).

**NameLRMg** — The left & right margin of the product name in inches. 

**NameFontSize** — The font size of the product name in points. This can be a decimal number.

**NameLeading** — The leading of the product name in points. This can be a decimal number.

**SKUWidth** — The width of the box containing the SKU number, in inches. The SKU number is left-aligned.

**PriceWidth** — The width of the box containing the price, in inches. The price is right-aligned.

**SKUFontSize** — Font size of the SKU number.

**PriceFontSize** — Font size of the price.

**Currency** — Currency symbol

**SpaceCurrency** — Must be true or false, indicating whether there should be a space after the currency symbol.

**PriceStyle** — The choices are:
* Simple — The symbol, left side, and right side are all the same size
* Superior — The symbol and the right side are half size, and top aligned

**PriceFormat** — *not yet available* The choices are:

    #,###.##
    #.###,##
    # ###.##
    # ###,##
    #'###.##
    #,##,###.##
    #.###
    #,###.###

