# SmartFit PRO - Smart Fitness Tracker Dashboard

An interactive fitness analytics dashboard built with **R Shiny**. Upload your tracker data as a CSV and get instant charts, KPIs, trend analysis and personalised recommendations.

**Live demo:** https://YOUR-ACCOUNT.shinyapps.io/smart-fitness-tracker/
(Upload `data/sample_fitness_data_90days.csv` to try it.)

## Features
- CSV upload with validation (required columns, type checks, missing values)
- KPI cards: total steps, average calories, total distance, average sleep
- Interactive Plotly charts: steps trend, distance, calories vs steps, sleep distribution
- Activity analysis: Low / Moderate / High classification, weekly totals, 7-day moving average, weekday heatmap
- Sleep analysis: quality breakdown (Poor / Fair / Good / Excessive) and metrics
- Searchable data table with CSV / Excel / PDF export
- Insights page: peak and lowest days, correlations, trend and rule-based recommendations

## Tech stack
R, Shiny, bslib, Plotly, dplyr, DT, zoo

## CSV format
`date, steps, calories, distance, sleep_hours`

## Run locally
    install.packages(c("shiny","bslib","plotly","dplyr","DT","ggplot2","zoo","lubridate"))
    shiny::runApp()

## Project structure
    app.R           main app (UI + server)
    R/              config, utils, data_processing, plots
    modules/        one Shiny module per page
    data/           sample datasets
    www/            custom CSS and JavaScript

## Future improvements
Wearable API integration, goal tracking, ML-based predictions, user accounts and a database.