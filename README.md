Food Delivery Efficiency Analysis — R Shiny

An interactive R Shiny dashboard designed to analyze food delivery performance and identify factors associated with delivery delays.

Project Overview

This project provides an interactive dashboard for exploring food delivery data through data cleaning, visualization, K-Means clustering, and Apriori association rule mining.

Users can upload a CSV dataset, clean and transform the data, explore multiple visualizations, perform K-Means clustering, and discover association rules related to late deliveries.

Key Features

* CSV data upload and cleaning
* Missing-value handling and data type conversion
* Outlier detection and removal
* Feature engineering, including Delivery Speed, Late Delivery classification, Speed Category, and Order ID generation
* 12 data visualizations
* K-Means clustering with configurable cluster numbers
* 3D cluster visualization using Plotly
* Cluster centers and cluster distribution analysis
* Apriori association rule mining
* Identification of rules associated with late deliveries
* Download cleaned data, clustered data, and association rules as CSV files
* Interactive tables using DataTables

Technologies & Libraries

* R
* Shiny
* shinydashboard
* readr
* dplyr
* ggplot2
* plotly
* arules
* DT

Data Analysis Techniques

Data Cleaning

The application prepares the uploaded dataset by handling missing values, converting data types, removing extreme delivery-time outliers, and creating additional analytical features.

Data Visualization

The dashboard provides 12 visualizations covering delivery time, vehicle performance, distance, preparation time, weather, time of day, traffic levels, and relationships between delivery variables.

K-Means Clustering

The application uses K-Means clustering to group delivery orders based on selected numerical variables such as distance, delivery time, and speed.

The results include cluster centers, cluster distributions, clustered data, and a 3D visualization.

Apriori Association Rules

The Apriori algorithm is used to discover relationships between categorical delivery attributes such as weather, traffic level, time of day, vehicle type, speed category, and late-delivery status.

The dashboard allows users to adjust minimum support and confidence thresholds and examine rules associated with late deliveries.

Dashboard Screenshots

Data Cleaning

Data Visualization

K-Means Clustering

Association Rules

Project Structure

Food-Delivery-Efficiency-Analysis/
│
├── app.R
├── dataset.csv
├── association rules.png
├── clustering.png
├── data cleaning.png
├── data visualization.png
├── .gitignore
└── README.md

How to Run

1. Install R and RStudio.
2. Install the required packages:

install.packages(c(
  "shiny",
  "shinydashboard",
  "readr",
  "dplyr",
  "ggplot2",
  "plotly",
  "arules",
  "DT"
))

3. Open app.R in RStudio.
4. Run the Shiny application.
5. Upload the provided CSV dataset through the dashboard.
6. Clean the data and explore the available analyses.

Project Purpose

This project demonstrates the use of R for interactive data analysis, data visualization, unsupervised machine learning, and association rule mining through a practical food delivery scenario.
