# GIS Templates for Telangana
This repository contains shapefiles at different levels of administration for Telangana. 

Shapefiles are available for the following levels of administration:  
- State  
- District  
- Sub-District or Mandal 
- Parliamentary Constituencies (PC)
- Assembly Constituencies (AC)

Combinations of different levels are also available, namely:  
- District-Wise Mandal division
- PC-Wise Mandal division

### The respective column names for the divisions are as follows:

- District name - d_name
- District id - d_id
- Sub-district name -  sd_name
- Sub-district id - sd_id
- Parliamentary Constituency Name - pc_name
- Assembly Constituency ID - ac_id
- Assembly Constituency Name - ac_name

## Date of update and source of the shapefiles
- District and Mandal Shapefiles were obtained from [Telangana Open Data Portal](https://data.telangana.gov.in/)
- PC Boundaries file was obtained from a Github [repository](https://github.com/datameet/maps) and then worked on by us internally
- Information was sourced in February 2024. If this repository is being viewed on a later date then kindly cross-check if any administrative re-organization has taken place before using the files

## Known Issues
- As of February 2024, no up to date village-level shapefiles were found for Telangana state
- All available shapefiles with PC boundaries are not drawn properly, so we had to overlay the shapefile with the mandal shapefile and estimate which mandals belonged in what PC
  - Another effect of this issue was that the Hyderabad and Secunderabad constituencies were more poor than other PCs, and had to be combined to get a more accurate shapefile
  - No combination files with Assembly Constituencies (AC)
    - They have the same problem as the PC files and we are planning to map mandals to Assembly Constituencies in the same way we did for PCs

