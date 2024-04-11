# QGISAU Sharing Resources
This repository contains styles, scripts, models, and other QGIS resources for Australian QGIS operations.

# Collections
## QLD
- QPWS

# Add a new collection
Do some checks first:  
> - Resources should come from the custodian themselves or with express permission to add them to this repository.  
> - Files that have been created by another software need to be checked that they are legally allowed to be uploaded here.

Under the collection folder, create a folder for your theme and load in all the required files. There is no requirement to load for the QGIS Resource Sharing Plugin.

## Optional - To load into QGIS Resource Sharing Plugin
*The following method is for loading up to the QGIS Resource Sharing Plugin that currently has some bug.*

This method is to undertake all the fiddly work on your machine. You can undertake it directly on repo. 
1. On your machine, download this [zip file](collections/collectionN.zip)
2. Rename your folder with a short name with no spaces and in lowercase  
   | Accepted | Not Accepted |
   | --- | --- |
   | thisstyle | This style |
   | this_style | this style|   
3. Populate `addendum_for_metadata-ini.txt` to add in your collection metadata. See [here](https://qgis-contribution.github.io/QGIS-ResourceSharing/authoring/creating-metadata.html) for instructions and structure.  
   - The actual name for the style that will appear in the plugin occurs after `name=` and not in the `[]`.  
     e.g. If your style is to be known as 'This Style'in the plugin, this is what you would put in after `name=`  
   - The  `[]` is for the folder name (see point 2 above).          
4. Move your files into the appropirate folder as per the guide below:  
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
5. In this repo, edit the `metadata.ini` and populate it from the `addendum_for_metadata-ini.txt`.
  - Check you have used the same name as your collection folder for the heading between `[]`  (this is the one with lowercase).
  - Copy this name up under the general heading, seperated with a comma.
       See [here](https://qgis-contribution.github.io/QGIS-ResourceSharing/authoring/creating-metadata.html) for instructions and structure.
6. Click on the `collections` folder and select upload file 
7. Copy over your folder and hit Commit
8. In QGIS, test it by loading up (or reloading if it is already loaded) the repository in the QGIS Resource sharing plugin. Once loaded, go to Intall and see if it is there and will load. If you experience any issues, put it in the repo's Issues.

# Load into QGIS
Install these resources:
Use the ["Resources Sharing"](http://www.akbargumbira.com/qgis_resources_sharing/) plugin to add this collection:\
Settings -> Add repository...:\
--- Name: Australian QGIS Styles\
--- URL: https://github.com/qgisau/QGISAU-Resources.git

Last updated: 5th April 2024
