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
    1. Ignore the Layout Type setting (this will be overridden by LayoutsPlus)
1. The settings under Layout Options > SKU table may or may not be used. See the documentation for the LayoutsPlus Primary Layout that you use.
1. Under Miscellaneous > Plug-Ins, select the following:
    1. Linden with LayoutsPlus
    1. LayoutsPlus

### Ironwood
1. Select either Ironwood Brochure or Ironwood Catalog
1. The settings under **Layout Options > Product** will be ignored in favor of settings for LayoutsPlus.
1. The settings under **Layout Options > SKU table** may or may not be used. See the documentation for the LayoutsPlus Primary Layout.
1. Under **Miscellaneous > Plug-Ins**, select the following:
    1. LayoutsPlus
    1. Also one of the following: (see note below)
      1. Ironwood HTML - One Column
      1. Ironwood HTML - Two Column
      1. Ironwood HTML - Three Column

      **_Note:_** *If you have entered "None" for your primary layout, then only select the LayoutsPlus plug-in. Do not select any of the Ironwood HTML plug-ins.*

## II. Create and upload a LayoutsPlus parameter csv file

1. Create a csv per the specifications
1. Place the csv in the images/codvariables ftp folder

### Naming convention for the csv file
The naming convention is as follows:  
**_account id_-variables.csv**

For example,  
**corvettemods-variables.csv**

### Naming convention for the csv file if you need more than one
If you require additional csv files for the same customer, you need to specify a suffix. An example might be "namewrap".

The naming convention is as follows:  
**_account id_-_suffix_-variables.csv**

For example,  
**corvettemods-namewrap-variables.csv**

## III. Development tips

### Use the HTML button in jobs manager
Click this button to see the HTML that was used for the description for the first product in the render. When you are just getting started with using LayoutsPlus, this can be more useful than looking at the PDF.

### Use the "HTML-only" feature when in Development
Do you want instant feedback on exactly what the plug-in did?  

Then use the HTML-only feature when you submit a job. Doing so allows you to instantly see the HTML in jobs manager, and does not submit a job to the publishing system. This gives you super-fast turnaround for testing parameter settings. To use the feature, enter the following before the Job ID when you submit a job: _5ty83bvx_  

(Note: use a text expander to enter this (I used *rnn*))
