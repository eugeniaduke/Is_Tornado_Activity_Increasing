# Is Tornado Activity Increasing?

## Description

This project analyzes tornado activity in the United States between 2015 and 2025 to identify long‑term trends and seasonal patterns. By combining tornado track data with daily weather observations, it examines whether tornado frequency has increased over the past decade and explores how temperature variations may influence tornado occurrence and intensity. The workflow includes data cleaning, SQL‑based analysis, and visualizations in Python to uncover meaningful insights into the relationship between severe weather and atmospheric conditions.

## Project Structure

'''

Database/
  |--tornado_tracks.db
Datasets/
  Clean Files/
    |--tornado_tracks_combined_cleaned.csv 
    |--weather_detail_cleaned.csv 
  Original Files/
    |--Tornado_tracks_2015_2019.csv
    |--Tornado_tracks_2020_2025.csv
    |--Weather_Detail.csv
Notebooks/
  |--data_cleaning_Tornado_tracks.ipynb
  |--data_cleaning_weather.ipynb
  |--tornado_tracks.ipynb
readme.md
'''



## Installation
1. Fork and clone this repository
2. Install the required Python packages:  
    pip install -r requirements.txt
3. Open `Tornado_tracks_Database.ipynb` in Jupyter Notebook or JupyterLab.

## Example Output 

## Data Sources

-   Tornado Data   
        -   NOAA https://www.ncei.noaa.gov/stormevents/choosedates.jsp?statefips=21%2CKENTUCKY

-   Weather Data
        -   National Climatic Data Center https://www.ncdc.noaa.gov/cdo-web/search


## Results
The analysis shows trends in tornado occurrences geographical distribution. Initially the data was visualized using static maps, but an interactive heatmap was later implemented for better insights.  While the bar graph used showed an increase in tornado occurrences, the heatmap provided a clearer geographical distribution.  The analysis is inclusive at this time because it's unknown if the increase in tornado activity is due to better tracking or an actual increase in occurrences.

## Acknowledgements

I used this website, https://www.geeksforgeeks.org/python/get-the-city-state-and-country-names-from-latitude-and-longitude-using-python/, to convert the latitude and longitude to a zipcode.

## Author
Eugenia Duke

