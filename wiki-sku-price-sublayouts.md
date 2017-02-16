# Layout "A"
Features:
* SKU number on the left
* Price on the right

Options:
* Price can be any of the [StylePrice](../wiki/Configuration-of-SKU-Price-Sub-layouts) options

You need these parameters in your csv:

    SKU_LType,A
    SKUWidth,0.8
    PriceWidth,0.8
    SKUFontSize,9
    PriceFontSize,9
    Currency,$
    SpaceCurrency,false
    PriceFormat,#,###.##
    PriceColor,FF0000
    TextBeforeItemNum,Part #
    StyleItemNumber,bold
    StylePrice,simple

# Layout "B"
Features:
* Shopping cart icon on the left — linked to the corresponding product page on the e-commerce site
* SKU number in the middle
* Price on the right

Options:
* Price can be any of the [StylePrice](../wiki/Configuration-of-SKU-Price-Sub-layouts) options

You need these parameters in your csv:

    SKU_LType,B
    Other parameters are the same as Layout A

# Layout "Table"
Features:
* SKU table, one row per SKU
* Uses column hide/show settings
* Uses column sizing settings

You need these parameters in your csv:

    SKU_LType,Table
    TableHeaderFontSize,8  
    TableHeaderLeading,9  
    TableDataFontSize,8  

# Layout "CustomTable_v1"
Features:
* SKU table, one row per SKU
* Control font color and background color per data cells
* Control relative column width
* Does NOT use these settings from the UI:
  * Column hide/show settings
  * Column sizing settings

You need these parameters in your csv:
```
    SKU_LType,CustomTable_v1
    TableHeaderFontSize,8  
    TableHeaderLeading,9  
    TableDataFontSize,8  
    CustomTable,
    AdditionalAttrMap,pprofit_sale#$#_Sale#$$#xyz#$#_xyz
```


# Reference for all sub-layouts

**SKUWidth** — The width of the box containing the SKU number, in inches. The SKU number is left-aligned. (Default is 0.8)

**PriceWidth** — The width of the box containing the price, in inches. The price is right-aligned. (Default is 0.8)

**SKUFontSize** — Font size of the SKU number. (Default is 9)

**PriceFontSize** — Font size of the price. (Default is 9)

**Currency** — Currency symbol (Default is $)

**SpaceCurrency** — If there should be a space after the currency symbol and before the price, this value must be "yesspace". (Default is "nospace")

**PriceFormat** — *Not yet available*. Default is #,###.##
The [choices](http://www.thefinancials.com/Default.aspx?SubSectionID=curformat) are:

    #,###.##
    #.###,##
    # ###.##
    # ###,##
    #'###.##
    #,##,###.##
    #.###
    #,###.###


**PriceColor** — Express as RGB hex. Default is FF0000

**TextBeforeItemNum** — Any text you want to appear before the item number (SKU number), such as _Part #_. Default is null.

**StyleItemNumber** — The choices are:
* none — No style will be applied to the item number
* bold — This will cause the item number to appear bold

**StylePrice** — The choices are:
* Simple — The symbol, left side of the price, and right side of the price are all the same size
* Simple-bold —  Same as Simple, except the symbol and price (both left and right sides) are bolded
* Superior — The symbol and the right side are half size, and top aligned

**CustomTable** — This specifies the properties of the table. There is one row for each table column. Rows are separated by #$$#. The properties are separated by #$#.

1. Column label — The label that will appear for that column in the table header.
1. Attribute name — The name of the attribute as it comes from the database.
1. Column width — The percentage width of the column. The percentages for all columns must add up to 100.
1. Alignment - The alignment of the data cell. Must be *left*, *right*, or *center*.
1. Data cell font color — The RGB hex value of the color of the font that appears in the data cell.
1. Data cell background color — The RGB hex value of the color of the background of the data cell.

**AdditionalAttrMap** — This is to convert "additional attributes" (which come from FJF files) into regular item attributes so that they can be used in the HTML table. This value consists of rows of two values. Each row requires:  
  1. the additional attribute name (e.g., ```pprofit_sale```); and  
  1. the regular attribute name (e.g., ```_Sale```).

Rows are separated by #$$#. The values are separated by #$#. An example value is:
```
pprofit_sale#$#_Sale#$$#xyz#$#_xyz
```
