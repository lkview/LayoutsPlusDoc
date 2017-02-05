# Introduction to LayoutsPlus
The next generation of layouts builds on the new HTML-based layout functionality in Catalog-on-Demand. It offers the following advantages over the previous layout model:
* Compatible with both composition models:
 * Ironwood (dynamic composition)
 * Linden (grid-based composition)
* More flexibility with placement and behavior of elements inside each layout via configurable parameters for each layout
* Sub-layouts to configure certain elements, such as prices or tables
* Faster to create new layouts.

To use LayoutsPlus, you will need to first create a configuration. Next you will create and upload a parameter file. You can edit either one at any time.

## I. Create a configuration
Your next steps depend on whether you are going to use LayoutsPlus with Linden or Ironwood.
### Linden
1. Select either Linden Brochure or Linden Catalog
1. Under Layout Options > Product:
    1. Set up the grid as usual
    1. Ignore the Layout Type setting (this will be overridden by LindenPlus)
1. The settings under Layout Options > SKU table may or may not be used. See the documentation for the LayoutsPlus Primary Layout that you use.
1. Under Miscellaneous > Plug-Ins, select the following:
    1. Settings for LindenPlus
    1. LayoutsPlus

### Ironwood
1. Select either Ironwood Brochure or Ironwood Catalog
1. The settings under **Layout Options > Product** will be ignored in favor of settings for LayoutsPlus.
1. The settings under **Layout Options > SKU table** may or may not be used. See the documentation for the LayoutsPlus Primary Layout.
1. Under **Miscellaneous > Plug-Ins**, select the following:
    1. LayoutsPlus
    1. Also one of the following:
      1. Ironwood HTML - One Col
      1. Ironwood HTML - Two Col
      1. Ironwood HTML - Three Col

## II. Create and upload a LayoutsPlus parameter file

1. Create a csv per the specifications
1. Place the csv in the images/codvariables ftp folder

## Naming convention for the csv file
The naming convention is as follows:  
**_account id_-variables.csv**

For example,  
**corvettemods-variables.csv**

## Naming convention for the csv file if you need more than one
If you require additional csv files for the same customer, you need to specify a suffix. An example might be "namewrap".

The naming convention is as follows:  
**_account id_-_suffix_-variables.csv**

For example,  
**corvettemods-namewrap-variables.csv**
