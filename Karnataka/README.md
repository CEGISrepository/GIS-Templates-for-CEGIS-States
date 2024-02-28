# GIS Templates for Karnataka
This repository contains shapefiles at different levels of administration for Karnataka. 

Shapefiles are available for the following levels of administration:  
- State  
- District  
- Sub-District or Taluk  
- Hobli (an administrative division between village and taluk only in KA)
- Village

Combinations of different levels are also available, namely:  
- District-Wise Taluk division
- District-Wise Hobli division
- District-Wise Village
- Taluk-Wise Hobli division within each district
- Taluk-Wise Village division within each district

### The respective column names for the divisions are as follows:

- District name- d_name
- District id- d_id
- Sub district name-  sd_name
- Sub district id- sd_id
- Hobli id- h_id
- Hobli name - h_name
- Village name- v_name
- Village id- v_id

### Date of update and source of the shapefiles
- All shapefiles taken from [Karnataka GIS](https://kgis.ksrsac.in/kgis/downloads.aspx)
- Information was sourced in February 2024. If this repository is being viewed on a later date then kindly cross-check if any administrative re-organization has taken place before using the files.

## Known Issues
- For Hobli level and Village, districts Kalaburgi and Belagavi do not have shapefiles.
- Combination shapefiles with MLA/MP constituencies are not available because their boundaries don't exactly overlap with other admin boundaries (district/sub-district/hobli/village)

