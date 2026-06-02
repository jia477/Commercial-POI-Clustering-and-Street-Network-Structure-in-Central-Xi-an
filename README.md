# Commercial POI Clustering and Street Network Structure in Central Xi'an

This repository contains the final files for my URBAN5160 Advanced Topics for Urban Analytics project.

## Project overview

This project analyses commercial POI clustering in central Xi'an. The study area is within 5 km of the Bell Tower, and the main spatial unit is a 500 m grid cell.

The project explores whether commercial POI density is associated with distance from the Bell Tower and local street-network structure.

## Main files

* `xian_poi_project.ipynb` — final Jupyter Notebook
* `xian_poi_project.html` — HTML version of the final report
* `data/` — input and processed datasets
* `outputs/` — figures and model result tables

## Data

The project uses:

* Amap commercial POI data
* 500 m grid cells
* Bell Tower point location
* OpenStreetMap road edges and nodes

All spatial analysis uses EPSG:32649.

## Methods

The workflow includes POI cleaning, spatial join, feature engineering, exploratory OLS modelling, and residual checks.

The dependent variable is commercial POI density. The main predictors are distance to the Bell Tower, road density, intersection density, and mean intersection degree.

## Main findings

Commercial POIs are unevenly clustered in central Xi'an. Distance from the Bell Tower is negatively associated with POI density, but distance alone does not explain the full pattern.

Among the tested street-network variables, mean intersection degree gives the strongest simple OLS model. However, residual Moran's I shows that spatial autocorrelation remains, so the OLS result should be treated as exploratory.

## Author

Xun Jia
URBAN5160 Advanced Topics for Urban Analytics
University of Glasgow
