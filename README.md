# Exploring patterns of environmental justice in historic redlined neighborhoods

### Environmental Data Science 223, HW #2

![Map of Los Angeles county with the HOLC neighborhoods highlighted](images/map.png)


## Description 

This course assignment aims to explore patterns of environmental injustice by combining census data with the historic redlining neighborhoods of Los Angeles County. The goal is to practice manipulating vector and raster data to build multi-layer accessible maps in R using `tmap`.  

## Analysis Highlights 
- **Data Import and Manipulation**: Used the `sf` package to read in geospatial data. Cleaned and filtered data using `dplyr` functions, including removing NAs and selecting relevant geographic regions.
- **Coordinate Reference System (CRS) Alignment**: Applied `st_transform()` to match the CRS of different spatial datasets, ensuring correct spatial analysis when overlaying maps or performing spatial joins.
- **Spatial Data Analysis**: Performed a spatial join using `st_join()` to identify overlapping census block groups and HOLC grades. This helped determine the percentage of census blocks within each HOLC grade, reflecting the legacy of redlining in Los Angeles.
- **Visualization and Mapping**: Created detailed maps and visualizations using the `tmap` and `ggplot` packages to display historical redlining patterns and current environmental justice conditions. Bar graphs and density plots were used to explore relationships between HOLC grades and environmental indicators, such as air quality and life expectancy, with customized colors and titles for clarity.

## Repository Structure

The contents of this project are found in the rendered [redlining-la-spatial.qmd file](https://github.com/eds223-fall-2024-org/hw2-jordancsibley/blob/main/HW2.qmd). The data folder is not included on this repo, however, below is the structure used to execute this project. 

```
EDS223-HW2
│   README.md
│   redlining-la-spatial.qmd
|   HW2.html
│   EDS223-HW2.Rproj    
│
└───data
     └───ejscreen
     └───gbif-birds-LA
     └───mapping-inequality
  

```

## Data Access 

All relevant data to this project are available for download [here](https://drive.google.com/file/d/14CauXFZkVh_6z2Euq0m1Sq1kHQ31fiMk/view?usp=drive_link).

Additional information regarding the data: 

-  United States Environmental Protection Agency’s EJScreen: Environmental Justice Screening and Mapping Tool [website](https://www.epa.gov/ejscreen/purposes-and-uses-ejscreen)
- HOLC Redlining - Digital Scholarship Lab Mapping Inequality project [data information](https://dsl.richmond.edu/panorama/redlining/data)
- Bird Observations - The Global Biodiversity Information Facility [website](https://www.gbif.org/)

## Author 

Jordan Sibley 

Master of Environmental Data Science student at the Bren School of Environmental Science & Management

jcsibley@bren.ucsb.edu

jordan.c.sibley@gmail.com 

## Acknowledgements

Dr. Ruth Oliver created this assignment for the course: Environmental Data Science 223 Geospatial Analysis & Remote Sensing at the Bren School of Environmental Science & Management at the University of California, Santa Barbara. The assignment description is found [here](https://eds-223-geospatial.github.io/assignments/HW2.html)

## References 

1.  [HOLC grade designations for Los Angeles](https://dsl.richmond.edu/panorama/redlining/data/CA-LosAngeles)

Nelson, R. K., Winling, L, et al. (2023). Mapping Inequality: Redlining in New Deal America. Digital Scholarship Lab. https://dsl.richmond.edu/panorama/redlining.

2.  [EJScreen: Environmental Justice Screen and Mapping Tool](https://www.epa.gov/ejscreen)

United States Environmental Protection Agency. 2024 version. EJScreen. Retrieved: \[October, 15, 2024, from url www.epa.gov/ejscreen\]

3.  [Bird Observations](https://www.gbif.org/)

The Global Biodiversity Information Facility. Accessed via https://drive.google.com/file/d/14CauXFZkVh_6z2Euq0m1Sq1kHQ31fiMk/view?usp=sharing \[15 October 2024\]

4.  Ellis-Soto, D., Chapman, M., & Locke, D. H. (2023). Historical redlining is associated with increasing geographical disparities in bird biodiversity sampling in the United States. Nature Human Behaviour, 1-9.
