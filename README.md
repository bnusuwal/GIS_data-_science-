# GIS Climate Data Analysis of Nepal:Climate Trend Analysis of Nepal (1971-2014):

## Overview
This project focuses on analyzing climate trends across Nepal using GIS techniques. The analysis involves processing geospatial data, visualizing seasonal and annual climate variations across districts and physiographic regions, and deriving insights from exploratory data analysis (EDA).Observed The dataset used in this project is sourced from Open Data Nepal. It includes climate trends based on observed data recorded across various weather stations in Nepal from 1971 to 2014.

## Objectives

- Load and process geospatial climate datasets for Nepal.
- Visualize climate trends using interactive maps and seasonal climate plots.
- Perform EDA to uncover patterns in temperature and precipitation variations.
- Provide meaningful insights to understand the impact of climate change in Nepal.

## Setup Instructions

### Prerequisites

Ensure you have the following libraries installed before running the notebook:

```bash
pip install numpy pandas geopandas rasterio folium plotly matplotlib seaborn
```

### Running the Analysis

1. Open `gis_assignment.ipynb` in Jupyter Notebook.
2. Run the cells sequentially to load, process, and visualize the data.
3. Explore the interactive Kepler.gl map and precipitation/temperature trend plots.

## Data Sources and Preprocessing

- **District Climate Data (`district_data.geojson`)**: Contains seasonal and annual climate trends for Nepal’s 75 districts.
- **Physiographic Data (`physiographic_data.geojson`)**: Represents climate trends for different physiographic regions.
- **Shapefile (`district_shapefile.shp`)**: Provides geographical boundaries of Nepal’s districts.

### Preprocessing Steps

1. **Data Loading**: GeoJSON and shapefiles are loaded using GeoPandas.
2. **Filtering**: The dataset is filtered to focus only on Nepal.
3. **Cleaning**: Handles missing values and ensures spatial consistency.
4. **Data Transformation**: Converts relevant climate variables into appropriate numerical formats.

## Visualizations and Analysis

### 1. **Interactive Folium Map of Nepal’s Districts**

- Displays district boundaries using an interactive folium map.
- Includes district labels to facilitate spatial exploration.
- Helps in identifying regional climate variations based on geographic location.

### 2. **Seasonal Precipitation Trends Across Districts**

- Line plot showing seasonal precipitation trends (Winter, Pre-Monsoon, Monsoon, Post-Monsoon) across Nepal’s districts.
- The monsoon season shows the highest rainfall across all regions, while winter has the lowest.
- Certain districts exhibit significant rainfall variations.

### 3. **Seasonal Maximum and Minimum Temperature Trends**

- Separate line plots displaying seasonal maximum and minimum temperature trends.
- Maximum temperatures peak during the monsoon season, while minimum temperatures drop sharply in winter.
- Some districts experience extreme seasonal fluctuations, indicating vulnerability to heatwaves and cold waves.

### 4. **Annual Temperature and Precipitation Trends**

- Line plot visualizing annual maximum and minimum temperature trends over time.
- Displays precipitation trends to identify patterns of increasing or decreasing rainfall over the years.
- A gradual increase in maximum temperatures suggests a warming trend in certain districts.
- Annual precipitation trends indicate potential climate shifts, with some regions experiencing drying patterns over time.

## Exploratory Data Analysis (EDA) Findings

- **Temperature Trends**:
  - Districts show varied seasonal temperature patterns, with monsoon months having the highest temperatures.
  - Winter months exhibit significant temperature drops across most regions.
  - Annual temperature analysis suggests a gradual warming trend in certain districts, particularly in lowland areas.
  - The data highlights increasing trends in both seasonal and annual temperature values, supporting global climate change concerns.
- **Precipitation Patterns**:
  - The monsoon season experiences the highest rainfall, while winter and pre-monsoon months have significantly lower precipitation.
  - Some districts show a decreasing trend in annual precipitation indicating possible climate shifts.
- **Regional Differences**:

  - Some districts experience higher temperature variations due to their topography and climate zones.
  - There are significant differences in climate trends between lowland and highland regions.
  - Districts in the southern plains exhibit higher temperatures, whereas mountainous regions show more extreme variations in seasonal temperatures.
  - Certain areas in the mid-hills show moderate climate stability, making them potentially less vulnerable to climate extremes.

-**Elevation Impact on Climate**:

-Higher elevations show more stable precipitation trends but greater temperature sensitivity.

-Mountainous regions are vulnerable to rising temperatures, accelerating glacier melt and altering water resources.

## Conclusion

This analysis provides a clear visualization of climate trends across Nepal helping in understanding climate change impacts. 
The interactive tools and climate trend plots allow for deeper insights into seasonal and regional variations.
Identifying temperature and precipitation patterns helps assess climate vulnerabilities and potential long-term environmental changes.
Findings from this analysis can be used for climate adaptation strategies, disaster risk management, and sustainable development planning in Nepal.
