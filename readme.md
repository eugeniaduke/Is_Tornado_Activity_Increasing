# Is Tornado Activity Increasing?

## Description
This project investigates tornado activity in the United States from 2015 to 2025 to identify long‑term trends, seasonal patterns, and potential environmental drivers. By combining NOAA tornado track data with daily weather observations from the National Climatic Data Center, the analysis explores:

- Whether tornado frequency has increased over the past decade
- How temperature relate to tornado occurrence
- Whether the magnitude of thunderstorms has increased over time
- How the temperatures have changed or if they have changed drastically over time

The workflow includes data cleaning, SQL queries, geospatial mapping, and Python‑based visualizations to uncover meaningful insights into severe weather behavior.

## Project Structure

```
Database/  
 |--tornado_tracks.db 

Datasets/  
 |--Clean Files/  
    |--tornado_tracks_combined_cleaned.csv  
    |--weather_detail_cleaned.csv 
 |--Original Files/  
    |--Tornado_tracks_2015_2019.csv   
    |--Tornado_tracks_2020_2025.csv  
    |--Weather_Detail.csv  

Notebooks/ 
    |--data_cleaning_Tornado_tracks.ipynb   
    |--data_cleaning_weather.ipynb  
    |--tornado_tracks.ipynb 

Visuals/ 
    |--Average Magnitude of Thunderstorms Over Time.png  
    |--Average Monthly Temperatures.png
    |--Summer Tornado Count vs Average Temperature.png

README.md  

requirements.txt   
```



## Installation
1. Fork and clone this repository
2. Create a virtual environment
        - to do this run (in GitBash) python -m venv myevn
3. Activate the virtual environment 
        - to do this run (in GitBash) source source myenv/Scripts/activate 
        - you'll know it worked if your prompt changes to show (myenv)
2. Install the required Python packages:  
    pip install -r requirements.txt
3. Open `Tornado_tracks_Database.ipynb` in Jupyter Notebook or JupyterLab.

## Example Output 

![alt text](<Screenshot 2025-12-19 063450.png>)

![alt text](<Screenshot 2025-12-19 084956.png>)

![alt text](<Screenshot 2025-12-19 093844.png>)

## Data Sources

-   Tornado Data   
        -   NOAA https://www.ncei.noaa.gov/stormevents/choosedates.jsp?statefips=21%2CKENTUCKY

-   Weather Data   
        -   National Climatic Data Center https://www.ncdc.noaa.gov/cdo-web/search


## Results
The analysis reveals several key observations:
- Tornado occurrences show year‑to‑year variability, with no clear correlation to temperature.
- The scatterplot of the average magnitude of thunderstorms shows an upstick up strength starting in 2022 and continuing through 2024 with a sharp decline in 2025.  2025 could be anomoly. 
- A heatmap of average monthly temperatures shows a slight upward trend for temperatures in the summer months by a few degrees.  Even though it is only a few degrees that could be a signal that the earth is getting warmer overall. 



## Acknowledgements

I used this website, https://www.geeksforgeeks.org/python/get-the-city-state-and-country-names-from-latitude-and-longitude-using-python/, to convert the latitude and longitude to a zipcode.

AI tools (Co-Pilot specifically) were used to help with the code to convert the latitude and longitude to a zipcode as well as the code used to merge that data back into the original dataframe.

## Author
Eugenia Duke

