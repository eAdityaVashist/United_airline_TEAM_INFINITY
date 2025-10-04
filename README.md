# United_airline_TEAM_INFINITY
United Airlines Flight Difficulty Analysis

Project Overview:
This project analyzes United Airlines flight data to compute a Flight Difficulty Score for each flight and classify flights into difficulty categories (Easy, Medium, Difficult). The goal is to identify patterns in flight delays, passenger load, special service requests (SSRs), and other operational factors that influence flight difficulty.

Dataset:
The project uses multiple datasets stored in the Data/ folder:
Airports Data: Contains airport codes and country codes.
Bags Data: Contains baggage information, including transfer and checked bags.
Flights Data: Contains flight schedules, departure and arrival times, ground times, total seats, fleet type, and carrier.
PNR Flight Data: Contains passenger reservation details including total passengers, children, basic economy, strollers, and lap children.
PNR Remarks: Contains special service requests (SSRs) associated with passenger records.

Analysis Steps:
Data Loading & Cleaning: Loaded all datasets, converted date/time columns, and handled missing values.
Feature Engineering: Calculated flight delays, passenger metrics, transfer-to-checked bag ratio, tight ground time flags, SSR counts, and Flight Difficulty Score.
Difficulty Classification: Ranked flights daily by difficulty score and classified top 20% as Difficult, middle 60% as Medium, and bottom 20% as Easy.
Exploratory Data Analysis: Analyzed distribution of difficulty scores, top difficult flights, and top difficult destinations.
Correlation Analysis: Evaluated relationships between Flight Difficulty Score and features like passenger count, delay, tight ground time, SSR count, and bag transfer ratio.

Visualizations: Generated histograms, bar charts, and other plots to visualize flight difficulty distribution, top difficult flights, and difficult destinations.

Key Insights:
Most flights have low difficulty scores, with few highly difficult flights.
Certain destinations consistently have higher average flight difficulty.
Passenger count, tight ground time, transfer-to-checked bag ratio, and SSR counts are strongly correlated with flight difficulty.

Usage:
Open the notebooks sequentially to reproduce the analysis.
Ensure the Data/ folder containing all CSV files is in the same directory as the notebooks.
Libraries required: pandas, numpy, matplotlib, seaborn.
