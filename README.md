# Spatial and Temporal Population Analysis in West Virginia (1900–2006)

This repository contains Python Jupyter notebook code and geospatial data for analyzing the spatial distribution and temporal evolution of resident population in West Virginia counties between 1900 and 2006. The project applies exploratory data analysis, statistical visualization, and spatial statistics techniques to identify demographic patterns and spatial autocorrelation.

Python Jupyter notebooks are used to structure the workflow, isolate computationally intensive tasks, and clearly separate data preprocessing, visualization, and spatial analysis.

## Overview

The project implements:

* **Data Preprocessing and Validation** — loading geospatial datasets, inspecting data structure, rearranging columns, checking data types, and verifying missing values.
* **Exploratory Data Analysis (EDA)** — descriptive statistics, boxplots, histograms, skewness, kurtosis, and dispersion measures to analyze population distributions.
* **Temporal Population Analysis** — comparison of county-level population between 1900 and 2006, including growth trends, population ranges, and total population evolution using polynomial interpolation.
* **Geographic Visualization** — choropleth maps representing population ranges, spatial distribution, and population differences across counties.
* **Global Spatial Autocorrelation** — computation of Global Moran’s I statistic with Monte Carlo permutation testing to evaluate spatial dependence.
* **Local Spatial Autocorrelation (LISA)** — Local Moran’s I analysis to identify spatial clusters (hot spots, cold spots) and spatial outliers.

## Files

* `population_analysis_wv.ipynb` — main Jupyter notebook containing data preprocessing, visualization, and spatial statistical analysis
* `counties_detailed.shp` — main shapefile containing county geometries and attributes
* `counties_detailed.shx` — shape index file
* `counties_detailed.dbf` — attribute table with demographic and population data
* `counties_detailed.prj` — coordinate reference system definition
* `counties_detailed.cpg` — character encoding information
* `counties_detailed.sbn` — spatial index file
* `counties_detailed.sbx` — spatial index file
* `counties_detailed.shp.xml` — metadata file describing the shapefile contents

## Requirements

### Core Software

* Python 3.13.15 

### Mandatory Python Packages

* numpy
* pandas
* geopandas
* matplotlib
* seaborn
* libpysal
* esda
* splot

## Outputs

* Descriptive statistics and population summaries per county
* Boxplots and histograms for population comparison across years
* Choropleth maps of population levels and population change
* Global Moran’s I statistic and Monte Carlo p-values
* Local Moran’s I cluster and significance maps
