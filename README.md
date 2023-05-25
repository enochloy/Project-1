# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 1: Exploring climate data of Singapore

### Problem Statement

Weather in Singapore may be rainy, windy or sunny. For a picnic essential business, the demand for their goods and services, and customer experience may be greatly influenced by the weather. This project aims to analyze monthly weather patterns over the year and locations to provide valuable insights and recommendations for optimizing picnic planning and operations based on weather conditions. This can help guide the development of tailored marketing campaigns, optimize inventory levels, adjust pricing strategies to maximize sales, and enhance customer experience.

---

### Datasets

From data.gov.sg:
* [`rainfall-monthly-number-of-rain-days.csv`](../data/'rainfall-monthly-number-of-rain-days.csv'): Monthly number of rain days from 1982 to 2022. A day is considered to have “rained” if the total rainfall for that day is 0.2mm or more.
* [`rainfall-monthly-total.csv`](../data/'rainfall-monthly-total.csv'): Monthly total rain recorded in mm(millimeters) from 1982 to 2022.
* [`relative-humidity-monthly-mean.csv`](../data/'relative-humidity-monthly-mean.csv'): Monthly mean relative humidity from 1982 to 2022.
* [`sunshine-duration-monthly-mean-daily-duration.csv`](../data/'sunshine-duration-monthly-mean-daily-duration.csv'): The monthly mean sunshine hours in a day from 1982 to 2022.
* [`surface-air-temperature-monthly-mean.csv`](../data/'surface-air-temperature-monthly-mean.csv'): The monthly mean air temperature recorded from 1982 to 2022.

From Kaggle (https://www.kaggle.com/datasets/cyanaspect/singapore-weather):
* [`amk.csv`](../data/'amk.csv'): Daily meteorological data collected from Ang Mo Kio from 2014 to 2020.
* [`changi.csv`](../data/'changi.csv'): Daily meteorological data collected from Changi from 2014 to 2020.
* [`tuassouth.csv`](../data/'tuassouth.csv'): Daily meteorological data collected from Tuas South from 2014 to 2020.

---

### Data Dictionary

|Feature|Type|Dataset|Description|
|---|---|---|---|
|**year**|*integer*|weather|Year| 
|**month**|*integer*|weather|Month| 
|**no_of_rainy_days**|*integer*|weather|The number of rain days (rain day defined as 0.2mm or more) in a month| 
|**total_rainfall**|*float*|weather|The total monthly rainfall|
|**mean_sunshine_hrs**|*float*|weather|The monthly mean sunshine hours in a day| 
|**mean_temp**|*float*|weather|The monthly mean air temperature| 
|**mean_rh**|*float*|weather|The monthly mean relative humidity| 
|**station**|*string*|stations|Station where the data was recorded| 
|**date**|*datetime*|stations|Date|
|**year**|*integer*|stations|Year| 
|**month**|*integer*|stations|Month| 
|**day**|*integer*|stations|Day|
|**weekday**|*integer*|stations|Weekday (0-6 for Monday-Sunday)|
|**daily_total_rainfall**|*float*|stations|Daily rainfall total (mm)|
|**mean_temp**|*float*|stations|Daily mean Temperature (°C)| 
|**mean_wind_speed**|*float*|stations|Daily mean Wind Speed (km/h)| 
|**rained**|*integer*|stations|1 or 0 for rain day (>=0.2mm) or non-rainy day respectively| 

---

### Conclusion

1. February has the ideal conditions for a picnic.
- Lowest rainfall, number of rainy days, relative humidity
- Highest mean sunshine hours, wind speeds
2. Highest rainfall in November and December.
3. Rainfall variation by weekdays exist.
- Highest chance of rain on Wednesdays
- Heaviest rains on Fridays
- Second lowest chance of rain and second lightest rain on Thursdays
4. Changi offers higher chance of favorable weather conditions
- Higher wind speed and lower rainfall

---

### Recommendations

1. Promote February as the ideal month for picnics
2. Align inventory and product offerings with seasonal variations
3. Focus kite-flying promotions/sales in the East during certain months
4. Thursdays may be the best weekday for picnics