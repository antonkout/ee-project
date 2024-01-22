# Earth Engine Gas Emissions Analysis
This project involves retrieving and analyzing gas emissions data from Sentinel-5P (TROPOMI) using Google Earth Engine. The analysis focuses on parameters such as CO, SO2, and NO2 over a specified region and time period.

**Author: Antonios Koutroumpas**
**Contact: antonkout@gmail.com**

## Requirements
- Python 3
- Earth Engine Python API
- Shapely
- GeoJSON
- Pandas
- Matplotlib
- Seaborn

## Setup
1. **Authentication:** Before running the script, make sure to authenticate Earth Engine by running ee.Authenticate().
2. **Initialization:** Initialize the Earth Engine library using ee.Initialize() with your specific project information.
3. **GeoJSON File:** Specify the path to your GeoJSON file containing the region of interest.
4. **Gas Parameters:** Customize the list of gas parameters (ls variable) for analysis.
5. **Date Range:** Set the initial and final dates of interest (i_date and f_date variables).
6. **Point of Interest:** Define the urban area of interest using an Earth Engine point geometry.
7. **Scale:** Set the scale for data retrieval.

## Running the Analysis
The script performs the following steps:

- Retrieves gas emissions data for specified parameters and region.
- Converts Earth Engine array data to a Pandas DataFrame.
- Performs inner joins based on datetime.
- Plots the air quality over time.
- Displays the correlation matrix for gas parameters.

## Usage
Run the script and observe the generated plots and correlation matrix to gain insights into gas emissions trends over the specified region.
