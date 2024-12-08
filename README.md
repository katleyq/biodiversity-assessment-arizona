# Analyzing environmental impacts of urban expansion in Phoenix, Arizona (2017-2020)

![Construction at controversial dam complex in Amazon Basin](https://images.newscientist.com/wp-content/uploads/2024/10/28160337/SEI_227488001.jpg?width=800)
Source: [Mario Tama / Getty Images](https://www.newscientist.com/article/2453640-the-world-is-falling-far-short-of-its-goal-to-halt-biodiversity-loss/)



**About**:

This purpose of this repository is to analyze the environmental impacts of urban expansion in Phoenix, Arizona from 2017 to 2020. This analysis will look at the biodiversity intactness index dataset developed by Gassert et al 2022 to assess how urban expansion has affected biodiversity in Phoenix. This analysis will generate a time series visualization of how biodiversity has changed in the area of interest.

**Highlights**:

In this analysis, we will accomplish the following:

- Retrieve Biodiversity Intactness Index (BII) data for our area of interest from the Microsoft Planetary Computer Data Catalog
- Compute raster stastistics of BII data
- Create data visualizations of BII data as a static plot and a time-series GIF 

**Data Access**:

1. **Phoenix Subdivision boundaries**: The original boundary data was retrieved from the US Census Bureau's 2020 Tiger / Line Shapefiles dataset. This dataset contains counties and subdivision boundaries from the US Census Bureau. It was subsetted for Phoenix and cleaned using `notebooks/phoenix-shapefile.ipynb`. (Original Source: [2020 Tiger/Line shapefiles](https://www.census.gov/cgi-bin/geo/shapefiles/index.php?year=2020&layergroup=County+Subdivisions))

2. **Biodiversity Intactness Index (BII) Dataset**: This data was retrieved from the Microsoft Planetary Computer Data Catalogue. This dataset contains Biodiversity Intactness Index data from a model developed by Gassert et al in their project titled, "Global 100m Projections of Biodiversity Intactness for the years 2017-2020Global 100m Projections of Biodiversity Intactness for the years 2017-2020". (Original Source:  [Microsoft Planetary Computer Data Catalogue](https://planetarycomputer.microsoft.com/dataset/io-biodiversity))

**Repository Structure**:

This repository has two main notebooks:

- `phoenix-shapefile.ipynb` contains code that creates the Phoenix shapefile used in 
- `bio-div-index-timeseries.ipynb` contains f



```
├── README.md
├── LICENSE
├── .gitignore
├── notebooks
│   ├──bio-div-index-timeseries.ipynb
│   └──phoenix-shapefile.ipynb
└── data
    ├── tl_2020_04_cousub
    │   ├──tl_2020_04_cousub.shx
    │   ├──tl_2020_04_cousub.shp.iso.xml
    │   ├──tl_2020_04_cousub.shp.ea.iso.xml
    │   ├──tl_2020_04_cousub.shp
    │   ├──tl_2020_04_cousub.prj
    │   ├──tl_2020_04_cousub.dbf
    │   └──tl_2020_04_cousub.cpg
    └── phoenix
        ├──phoenix.shx
        ├──phoenix.shp
        ├──phoenix.prj
        ├──phoenix.dbf
        └──phoenix.cpg

```


**References**:

F. Gassert, J. Mazzarello, and S. Hyde, “Global 100m Projections of Biodiversity Intactness for the years 2017-2020 [Technical Whitepaper].” Aug. 2022. Available: https://ai4edatasetspublicassets.blob.core.windows.net/assets/pdfs/io-biodiversity/Biodiversity_Intactness_whitepaper.pdf