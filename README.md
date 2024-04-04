# QGISAU Sharing Resources
This repository contains styles, scripts, models, and other QGIS resources for Australian QGIS operations that you can share through the QGIS Resources Sharing.

# Collections
## QLD
- QPWS


## Install
Use the ["Resources Sharing"](http://www.akbargumbira.com/qgis_resources_sharing/) plugin to add this collection:\
Settings -> Add repository...:\
--- Name: Australian QGIS Styles\
--- URL: https://github.com/qgisau/QGISAU-Resources.git

## Add a new collection
1. In `metadata.ini` add in your collection metadata. See [here](https://qgis-contribution.github.io/QGIS-ResourceSharing/authoring/creating-metadata.html) for instructions and structure.
   - Use the same name as the collection folder
   - Add in the name under the general heading. Seperate from others with a comma.
     
2. Under the `collections` folder, create a new folder with the name of your collection  
3. Add in the relevant folders in the structure as per this structure  
   └── collections  
    ├── [Collection1 register id] (the id string used in "collections" in metadata.ini)  
    │   ├── checklists (optional, containing checklist definition JSON files)  
    │   ├── expressions (optional, containing JSON files with QGIS Expressions)  
    │   ├── image (optional, containing all kinds of image files)  
    │   ├── models (optional, containing Processing models)  
    │   ├── preview (encouraged, containing previews for the collection, referenced in metadata.ini)  
    │   ├── processing (optional, containing Python Processing scripts)  
    │   ├── rscripts (optional, containing R scripts)  
    │   ├── style (optional, containing QML files - QGIS Layer style)  
    │   ├── svg (optional, containing SVG files)  
    │   ├── symbol (optional, containing symbol definition XML files)  
    │   └── license file (encouraged)  

Last updated: 4th April 2024
