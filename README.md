# Sunflower Yield Analysis and Vegetation Index Project

## Overview

This project focuses on the analysis of agricultural yield data for sunflowers using spatial interpolation techniques. The first goal is to create accurate yield maps and understand spatial patterns in crop productivity. As a secondary objective, the project explores the potential correlation between yield data and vegetation indices derived from satellite imagery.


## Project Components

1. **Exploratory Data Analysis (EDA_cleaning.ipynb)**
   - Initial data exploration and cleaning
   - Visualization of yield data
   - Preparation of data for further analysis

2. **Yield Mapping (Yield_mapping.ipynb)**
   - Data preprocessing phase
   - Creation of interpolated yield maps
   - Variogram analysis

3. **Vegetation Index Analysis (Vegetation_index.ipynb)**
   - Calculation of vegetation indices (e.g., NDVI, GCVI) from satellite imagery
   - Correlation of vegetation indices with yield data

## Usage

To use this project:

1. Clone the repository to your local machine.
2. Ensure you have the required dependencies installed (see `requirements.txt`) in a virtual environment.
3. Run the notebooks in the following order:
   - `EDA_cleaning.ipynb`
   - `Yield_mapping.ipynb`
   - `Vegetation_index.ipynb`

4. Make sure to update the file paths in each notebook to match your local directory structure.

## Data Requirements

- Yield data in GeoPackage format is provided in the `Data`folder (`resa_girasole_2022.gpkg`).
- Sentinel-2 satellite imagery (accessed via Google Earth Engine).

In order to access Google Earth Engine, you need an account in Google Cloud Console and have/create a dedicated Project with Google Earth Engine API enabled. Visit (https://earthengine.google.com) for further information. Once you have the account set up, run the following commands in the Terminal:

```
earthengine authenticate
```

This will authenticate your Google Earth Engine account and allow you to access the API. Remember that whenever you want to use Google Earth Engine, you need to initialise the session with the following command:

```
import ee
ee.Initialize(project='YOUR_PROJECT_ID')
```


