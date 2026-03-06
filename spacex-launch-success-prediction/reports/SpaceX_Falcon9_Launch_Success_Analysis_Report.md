# SpaceX Falcon 9 Launch Success Analysis

## 1. Introduction

SpaceX has revolutionized the aerospace industry by developing reusable rocket technology. The Falcon 9 rocket, in particular, has significantly reduced launch costs through successful first-stage booster landings.

This project analyzes historical Falcon 9 launch data to understand the factors that influence launch success and booster landing outcomes. The analysis integrates data from the SpaceX API and web-scraped launch records, followed by exploratory data analysis, geospatial visualization, machine learning modeling, and dashboard development.

The goal is to identify patterns in launch operations and build predictive models that estimate the probability of successful booster landings.

---

## 2. Data Sources

The project uses two main data sources:

### SpaceX API
Historical launch data was collected using the official SpaceX API. The API provides detailed information about past launches including rocket information, payload data, launch sites, and core booster details.

### Web Scraped Launch Records
Additional launch data was obtained by scraping the Falcon 9 launch records from Wikipedia using Python’s Requests and BeautifulSoup libraries. This dataset includes:

- Flight Number
- Launch Site
- Payload Information
- Orbit Type
- Launch Outcome
- Booster Landing Result

---

## 3. Data Preparation

The raw datasets required extensive preprocessing before analysis. The following steps were performed:

- JSON data normalization using Pandas
- Feature selection to retain relevant columns
- Filtering Falcon 9 launches
- Handling missing values
- Feature engineering using additional API calls
- Data type conversion
- Dataset merging and restructuring

Additional features such as booster version, launch site location, payload mass, orbit type, and landing outcomes were extracted to enrich the dataset.

---

## 4. Exploratory Data Analysis

Exploratory Data Analysis (EDA) was performed to identify patterns and relationships within the dataset.

Key analyses included:

- Launch success rates by launch site
- Payload mass distribution
- Launch success trends over time
- Orbit type distribution
- Booster landing success frequency

Correlation analysis was also conducted to determine relationships between features and landing outcomes.

---

## 5. Geospatial Analysis

Geospatial analysis was performed using the Folium library to visualize launch site locations.

Interactive maps were created showing:

- Launch site coordinates
- Successful and failed launches
- Spatial relationships between launch sites and nearby infrastructure

Distances between launch sites and geographic features such as coastlines, highways, railways, and cities were calculated to better understand launch site selection.

Clustering techniques were also applied to group launch sites based on geographic proximity.

---

## 6. Machine Learning Modeling

Machine learning models were trained to predict whether the Falcon 9 first-stage booster would land successfully.

The models evaluated include:

- Logistic Regression
- Support Vector Machines
- Decision Trees
- K-Nearest Neighbors

These models use launch characteristics such as payload mass, orbit type, launch site, and booster reuse information as input features.

---

## 7. Model Evaluation

Model performance was evaluated using classification metrics including:

- Accuracy score
- Confusion matrix
- Model comparison

The results demonstrate how machine learning can be used to predict launch success based on operational parameters.

---

## 8. Interactive Dashboard

An interactive dashboard was developed using Plotly Dash to visualize launch records.

The dashboard allows users to:

- Filter launches by site
- Analyze launch success rates
- Explore payload mass relationships
- Visualize mission outcomes interactively

This dashboard provides an accessible interface for exploring SpaceX launch data.

---

## 9. Conclusion

This project demonstrates an end-to-end data science workflow using real-world aerospace data.

By combining API data collection, web scraping, geospatial mapping, exploratory analysis, and machine learning modeling, the project provides insights into the factors that influence Falcon 9 launch success and booster landings.

The results highlight the potential of data-driven analysis for understanding complex engineering systems and operational performance.