# Forest Atlas Style Guide

These resources are intended to expedite the production and deployment of Forest Atlas maps. This repository includes the following assets.

* Esri ArcGIS .style files—one for each of the Forest Atlas map themes
* URL for *Standard WRI* data taxonomy spreadsheet, which details all of the different layers
* URL for *Forest Atlas Style Guide* spreadsheet, which includes styling rules for the Forest Atlas maps

### [Standard WRI Spreadsheet](https://docs.google.com/spreadsheets/d/1vRLRplGwL2MEPyG2Ed5uvT-8SRnZa6iuGVNC3YSyD5A/edit?usp=sharing)
### [Forest Atlas Style Guide Spreadsheet](https://docs.google.com/spreadsheets/d/1teIyXzKpwQz1pyjuDJLXteRODLt1-xRNBAYe4kvOH2I/edit?usp=sharing)

Please note that these pre-defined map styles are not intended as hard-and-fast rules that cannot be broken, but rather, basic guidelines. You may wish/need to modify them to best suit your needs.

## How to create a new Forest Atlas
### Preparing the data and .MXD
1. Fork/clone/download this repository.
2. Open ArcMap and reate a new .MXD file, which you'll use to style your data. You'll need a separate MXD file for each map theme.
3. Open the Style Manager, by clicking Customize->Style Manager.
4. Select *Styles*, then *Add Style to List*, and then navigate to, and select, the appropriate .style file from this repository.
5. Right-click on the Data Frame (the main map window), and select *Data Frame Properties*. Select the *General* tab. Ensure that the *Label Engine* is set to *Maplex Label Engine*.

### Styling and labeling the data in ArcMap
1. Open the *Forest Atlas Style Guide* spreadsheet. This document identifies all of the data layers that should appear in each map theme, their classification schemes, and their rendering order. The spreadsheet itself contains detailed directions for use.
2. In ArcMap, add the appropriate layers to the map canvas. Ensure they're arranged in the proper order. Classify the layers according to the *Forest Atlas Style Guide* spreadsheet.
3. Some of the layers include zoom-dependent rendering rules. These are also defined in the *Forest Atlas Style Guide* spreadsheet, and can be implemented in the *Scale Range* section of the *General* tab in the *Layer Properties* pane, which you can access by double-clicking on each layer.
3. Symbolize the data using the pre-configured symbols included in the .style file earlier. The fastest way to do this is to click on the small symbol swatch to the left of each class in the table of contents, and in the Symbol Selector window, click on the appropriate symbol. The descriptive symbol names should correspond to the class names. *Note: if the preloaded symbols do not appear in the Symbol Selector window, the .style file may not have loaded properly. Click on *Style References*, and ensure that the .style file's box is ticked. If the .style file does not  appear in the list, click Add Style to List, navigate to the .style file on your computer, and open it.
4. Once all of the data classes have been symbolized, you must repeat the process for labels. Double-click on each layer in the table of contents, and then click on the *Labels* tab. Select *Label Styles* in the *Pre-definied Label Style* section in the lower-right of the pane. Select the appropriate label style for this layer. In the main labeling window, be sure to tick the *Label features in this layer* box
5. You may wish to confirm that the conditional labeling rules have been applied properly. Consult with the *Forest Atlas Style Guide* spreadsheet, as necessary. 

### Uploading the map to ArcGIS Online
