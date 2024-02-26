# GIS Templates for CEGIS States
This repository contains shapefiles at different levels of administration for all the CEGIS States. 

Shapefiles are available for the following states:  
- Telangana 
- Karnataka  
- Tamil Nadu  
- Bodoland Territorial Region
- Delhi
- Uttar Pradesh

Shapefiles are available for different administrative levels, generally:
- Districts
- Sub-Districts
- Gram Panchayats/Villages
  
### Note
- To use the GIS templates efficiently, it is recommended to run a check on your csv data to check the spellings of the column names, specifically division names. 
- The Administration levels have different names in different states or might have added levels of administration. Kindly refer to the README.md and spelling repository for the particular state for the same.
- If .shp file is being used, please make sure all the other supporting files are in the same folder as the .shp file. Similarly upload the supporting files in the same directory on Colab while running the Python code.
- While loading your data for visualization, please make sure that the column names align with the shapefiles column names. If not, kindly make the changes to the column names. Every state folder contains "Spellings Repository- State_Division.csv" which can be referred for all these spellings.
- Further details like last updated shapefiles, sources and discrepancies will be available in README.md files in respective state folders. 

## Usage Instructions for different platforms

### QGIS Choropleth
- Create a project 
- Add new data source : Data source manager-> Vector -> Browse Vector Dataset(select your shapefile here) -> Click on Add(just keep adding, options can be overlooked)
- Add new data source: Data source manager-> Delimited Text -> Browse for the csv file-> Check file format as CSV (again, options can be overlooked)-> Click on Add
- Double click on shapefile in layers -> select Joins from sidebar -> hit the small plus button at the bottom left
- Select district/Sub-district fields from both drop downs, apply and click on ok. 
- Right click on your shapefile from layers and open attribute table to check if the field got added. 
- Right click on your shapefile to go to properties and then Symbology tab on the left sidebar.
- Go to symbology, and select “Graduated” from the drop-down menu on the top.
- Select the type of classification that you want from the dropdown present at the bottom.
- Click on Classify and edit the colour ramp from the given option as needed.


### Tableau Choropleth
- Create a book
- Add data source 1: shapefile
- Add data source 2: csv file containing parameter to plot
- Drag csv file from sidebar to top empty space
- Remove conflicts by equating the fields (eg. “d_name” = *name from your csv* and so on)
- Open Sheet1 on the bottom
- Double click geometry on the sidebar -> Map should show up
- Drag d_name or district name parameter from csv into the detail field, and the label field if wanted
- Drag the field you want to plot as colour into colour tab

### Google Colab Python Choropleth
- Open google colab notebook
- Paste/Upload shapefile and other supporting files (.dbf, .shx, .cpg etc) and the csv file containing the data on the files tab in Colab session found on the left sidebar usually. 
- Copy path of files by right clicking on the file and clicking on "Copy as path".
- Paste the paths wherever indicated for shapefile and csv each.
- Go to Runtime-> Run all
- Dependencies: python, plotly, matplotlib, geopandas, numpy (will be installed in the code itself)


## Known Issues
The known issues for the in the shapefiles data will be found updated in the README.md for the state specific shapefiles. 
