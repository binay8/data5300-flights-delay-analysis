# United Airlines Departure Delays

## Project Overview
This report investigates departure delays for United Airlines flights departing from 3 New York airports: John F. Kennedy (JFK), LaGuardia Airport (LGA), and Newark Liberty (EWR) by examining how weather and time of day/year may impact departure delays.  

- **Domain:** Travel, Airlines
- **Key Techniques:** Exploratory Data Analysis, Permutation Testing

---
## Project Structure

```
├── code/                 # Rmd and knitted html files
├── data/                 # Processed data
├── reports/              # Generated reports and visualizations
├── .gitignore            # Files and directory to be omitted in github
├── LICENSE               # MIT License
├── README.md             # Project documentation
└── requirements.txt      # Dependencies
 
```


## Data

The analysis used the nycflights13 dataset. This dataset contains information about flights departing from the three airports in New York airports. 
The source dataset has information about airlines, scheduled departure time, actual departure time, and delays. 
Additionally, this analysis also used hourly weather data for each airport using the weather dataset. 

## Analysis
The analysis is organized into three Rmd files:
1. Data Preparation:
The data preparation process involved importing, investigating, cleaning, and merging the nycflights13 and weather dataset. 
[Data Preparation Link](https://github.com/binay8/data5300-flights-delay-analysis/blob/main/code/flight_delays_analysis_data_prep.Rmd)

2. Exploratory Data Analysis (EDA):
Exploratory data analysis was conducted using descriptive statistics and data visualizations to investigate relationship between departure delays and the potential factors.
[Exploratory Data Analysis Link](https://github.com/binay8/data5300-flights-delay-analysis/blob/main/code/flight_delays_eda_binay.Rmd)

3. Statistical Analysis:
We explored patterns in departure delays based on various factors like time of day (hour), time of year (month), as well as weather related factors like wind speed, temperature, precipitation and visibility. We then conducted statistical testing to further examine departure delays. 
The statistical testing involved repeated shuffling of labels and comparing difference with observed difference in our original dataset. 
[Statistical Analysis Link](https://github.com/binay8/data5300-flights-delay-analysis/blob/main/code/flight_delays_statistical_analysis_binay.Rmd)

## Results
Time of day, precipitation and temperature had the most notable difference in departure delays. 
Flights departing in the Evening hours experienced an average delay of around 18 minutes longer than flights departing in the morning hours. 
Flights departing during precipitation or wet conditions had 17.7% higher rate of delayed departures compared to flights departing during dry conditions. 
Finally, flights departing during hot conditions had 12.93% higher rate of delays compared to flights leaving during moderate temperature. 

## Authors

- Binay Raut - [@binay8](https://github.com/binay8)

## License
This project is licensed under the MIT License.
See the [LICENSE](LICENSE) file for details.

## Acknowledgements

- R packages and datasets used include nycflights13, tidyverse, dplyr, ggplot, knitr.

