# LindenPlus
This is about parameterized Linden layouts. 
It uses the system plug-in called **LindenPlus**. 
It requires that variables be defined in the private dropbox folder called **_CoDVariables**. The naming convention is as follows:

    account id_-variables.csv

For example, 

    corvettemods-variables.csv

There is no forgiveness in the naming of the variables, or for missing variables. The job will immediately give an error if a variable is missing or misspelled.

## Layout #1: *ImageAboveName*
This layout was originally developed to support corvettemods. It displays:
* product image
* product name
* SKU number
* price

The variable files must contain the following:

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

#### ImageDesc_LType
The value must be set to _ImageAboveName_.

#### SKU_LType

