# Analyzing environmental impacts of urban expansion in Phoenix, Arizona (2017-2020)

![Construction at controversial dam complex in Amazon Basin](https://images.newscientist.com/wp-content/uploads/2024/10/28160337/SEI_227488001.jpg?width=800)
Source: [Mario Tama / Getty Images](https://www.newscientist.com/article/2453640-the-world-is-falling-far-short-of-its-goal-to-halt-biodiversity-loss/)



**About**:

This purpose of this repository is to analyze the environmental impacts of urban expansion in Phoenix, Arizona from 2017 to 2020. This analysis will look at the biodiversity intactness index dataset developed by Gassert, Mazzarello, & Hyde (2022) to assess how urban expansion has affected biodiversity in Phoenix. This analysis will generate a time series visualization of how biodiversity has changed in the area of interest.

**Highlights**:

In this analysis, we will accomplish the following:

- Retrieve Biodiversity Intactness Index (BII) data for our area of interest from the Microsoft Planetary Computer Data Catalog
- Compute raster stastistics of BII data
- Create data visualizations of BII data as a static plot and a time-series GIF 


**Repository Structure**:

This repository contains the following structure:

```
├── notebooks
│   ├──bio-div-index-timeseries.ipynb # contains analysis of BII data
│   └──phoenix-shapefile.ipynb # contains code that creates Phoenix shapefile, output is stored in data folder
├── .gitignore
├── LICENSE
├── README.md

```

**Data Description**:

1. **Phoenix Subdivision boundaries**: The original boundary data was retrieved from the US Census Bureau's 2020 Tiger / Line Shapefiles dataset. This dataset contains counties and subdivision boundaries from the US Census Bureau. It was subsetted for Phoenix and cleaned using `notebooks/phoenix-shapefile.ipynb`. (Original Source: [2020 Tiger/Line shapefiles](https://www.census.gov/cgi-bin/geo/shapefiles/index.php?year=2020&layergroup=County+Subdivisions))

2. **Biodiversity Intactness Index (BII) Dataset**: This data was retrieved from the Microsoft Planetary Computer Data Catalogue. This dataset contains Biodiversity Intactness Index data from a model developed by Gassert, Mazzarello, & Hyde (2022). (Original Source:  [Microsoft Planetary Computer Data Catalogue](https://planetarycomputer.microsoft.com/dataset/io-biodiversity))

**Data Access**

To access the data used in this repository, you can download the data folder from this link: https://drive.google.com/drive/folders/10OI35VwtgBZTdSjY6668Joyu5mRAEB6_?usp=sharing

Once you download the data, you can add it to your local copy of the repository to run the notebooks.

**Data Folder Structure**:


```
├── data
│   ├── phoenix # contains Phoenix spatial data from phoenix-shapefile.ipynb output
│   │   ├── phoenix.shx
│   │   ├── phoenix.shp
│   │   ├── phoenix.prj
│   │   ├── phoenix.dbf
│   │   └── phoenix.cpg
│   ├── tl_2020_04_cousub # contains all county boundary spatial data used in phoenix-shapefile.ipynb
│   │   ├── tl_2020_04_cousub.shp
│   │   ├── tl_2020_04_cousub.shx
│   │   ├── tl_2020_04_cousub.prj
│   │   ├── tl_2020_04_cousub.dbf
│   │   ├── tl_2020_04_cousub.cpg
│   │   ├── tl_2020_04_cousub.shp.iso.xml
│   │   └── tl_2020_04_cousub.shp.ea.iso.xml

```

**References**:

Gassert, F., Mazzarello, J., & Hyde, S. (2022, August). Global 100m projections of biodiversity intactness for the years 2017-2020 [Technical whitepaper]. Retrieved from https://ai4edatasetspublicassets.blob.core.windows.net/assets/pdfs/io-biodiversity/Biodiversity_Intactness_whitepaper.pdf

Microsoft Planetary Computer. (n.d.). Biodiversity intactness index [Data set]. Retrieved December 5, 2024, from https://planetarycomputer.microsoft.com/dataset/io-biodiversity

U.S. Census Bureau. (2020). County subdivisions shapefiles [Data set]. Retrieved from https://www.census.gov/cgi-bin/geo/shapefiles/index.php?year=2020&layergroup=County+Subdivisions

**Acnknowledgements**

This repository was created as an assignment for [EDS 220: Working with Environmental Datasets](https://meds-eds-220.github.io/MEDS-eds-220-course/) at the [UCSB Bren School of Environmental Science & Management](https://bren.ucsb.edu/). This course is led by Dr. Carmen Galaz-Garcia and Annie Adams. 