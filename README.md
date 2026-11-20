# 2025-AQI-Weather-Data-Delhi-Analysis-using-Python-Pandas-NumPY-Matplotlib-seaborn-Project
Delhi AQI &amp; Weather Analysis 2025  Analysed one year (2025) of hourly Delhi air quality and weather data (52,560 records, 6 stations) using Python, Pandas, NumPy and Matplotlib. Twelve visualisations reveal seasonal dust and winter smog peaks, daily patterns, and how rain, fog and temperature affect AQI and PM2.5. 
Delhi AQI & Weather Analysis 2025
Analysis of one year (1 Jan to 31 Dec 2025) of hourly air quality and weather data from six Delhi stations, using Python, Pandas, NumPy and Matplotlib. The project produces 12 visualisations that show seasonal, daily and weather-driven pollution patterns.
Dataset
File: `AQI.xlsx` (one worksheet, 52,560 rows = 6 stations x 8,760 hours)
Stations: Anand Vihar, Connaught Place, Dwarka, IGI Airport, Okhla Phase III, Rohini
Key columns: `Datetime`, `location`, `AQI`, `PM 2.5`, `PM 10`, `CARBON MONOOXIDE`, `Nitrogen Dioxide concentration`, `Ambient Temperature`, `humidity`, `ATOM PRESSURE`, `WINDSPEED`, `Condition`
The original `AQICategory` column is empty, so the code rebuilds it using the Indian CPCB bands (Good, Satisfactory, Moderate, Poor, Very Poor, Severe).
Project files
File	Description
`Delhi\_AQI\_Analysis.ipynb`	Google Colab notebook (run cell by cell)
`delhi\_aqi\_analysis.py`	Same code as a single Python file
`Delhi\_AQI\_Project\_Documentation.docx`	Full documentation with code, graphs and explanations
`AQI.xlsx`	Input data
How to run (Google Colab)
Open colab.research.google.com.
Choose File > Upload notebook and select `Delhi\_AQI\_Analysis.ipynb`.
Run the first cell and upload `AQI.xlsx` when asked.
Run the remaining cells from top to bottom. Each graph appears under its cell.
No installation is needed. Pandas, NumPy, Matplotlib and openpyxl come pre-installed in Colab.
Graphs produced
Monthly AQI trend (mean vs median)
Share of hours in each AQI category
Average AQI, PM 2.5 and PM 10 by station
Monthly trends of PM 2.5, PM 10, NO2 and CO
Daily PM 2.5 with 7-day average and the 60 ug/m3 limit
Average AQI, PM 2.5 and NO2 by hour of day
Heatmap of PM 2.5 by month and hour
Pollution by day of week
Correlation heatmap (pollutants and weather)
PM 2.5 against temperature, humidity and wind speed
PM 2.5 by weather condition (boxplots)
Top 10 most polluted days
Key findings
No hour in the year was rated Good. About 31.7% of hours were Poor or worse.
263 of 365 days had average PM 2.5 above the 60 ug/m3 daily limit.
There are two pollution seasons: coarse dust (PM 10) drives extreme AQI from March to June, while fine particles (PM 2.5), CO and NO2 peak in December and January.
September is the cleanest month and May the worst (by mean AQI).
PM 2.5 is lowest in the afternoon and highest late at night (around 10 pm).
Rain and drizzle roughly halve typical PM 2.5. Fog hours have the highest PM 2.5 (median about 197).
Data notes
The six stations form two groups with identical AQI and pollutant values (Dwarka, IGI Airport and Okhla Phase III in one; Anand Vihar, Connaught Place and Rohini in the other). Only the weather columns differ, so the pollution data may come from two shared sources rather than six separate monitors.
About 13% of AQI values are above 500 (maximum 2,742), which is beyond the standard AQI scale. The "top 10 days" graph caps hourly AQI at 500 for this reason.
Units for wind speed, pressure, CO and NO2 are not stated in the file.
The results cover one year only. Correlation does not prove cause.
Tech stack
Python 3, Pandas, NumPy, Matplotlib, Google Colab
