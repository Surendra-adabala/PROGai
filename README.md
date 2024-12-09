# APOD & Iris Dataset Analysis Project

## Overview

This project is focused on two main parts:

### 1. Astronomy Picture of the Day (APOD) Collection & Analysis
- The goal is to retrieve and store APOD data (including images and videos) for a specified date range from NASA's API.
- The data is then processed, including:
  - Media type count (images vs videos)
  - Identifying the longest explanation for an APOD entry
  - Exporting the collected data into CSV format for further analysis.

### 2. Iris Dataset Analysis
- The Iris dataset is loaded, cleaned, and analyzed to study flower species attributes and their relationships.
- Specific tasks include:
  - Data correction for erroneous entries
  - Feature engineering (e.g., PetalRatio and SepalRatio)
  - Correlation analysis
  - Creating a scatter plot with linear regression lines
  - Generating a pair plot for comprehensive visualization

---

## Requirements

- **Python**: Version 3.x
- **Libraries**:
  - `requests`
  - `json`
  - `pandas`
  - `seaborn`
  - `matplotlib`
  - `scikit-learn`
  - `numpy`
  - `dateutil`

### Install required libraries with the following:
pip install requests pandas seaborn matplotlib scikit-learn numpy python-dateutil
```
APOD Data Collection

ApodFetcher
Purpose: Fetches the Astronomy Picture of the Day (APOD) data for a specified date range.
Key Functions:
get_apod_info(date): Retrieves APOD data for a single date.
download_apod_in_range(start_date, end_date): Downloads APOD data for a range of dates and stores it in a JSON file.
Process Flow:
The data is fetched from NASA's APOD API using the provided API key.
The collected data includes:
Date, Title, Media Type, Image Link, and Explanation.
Iris Dataset Analysis

ApodDataProcessor
Purpose: Processes and analyzes the collected APOD data.
Key Functions:
read_apod_data(): Reads the stored APOD data from a JSON file.
analyze_apod_media(): Analyzes the number of images and videos, and finds the longest explanation.
save_apod_to_csv(): Saves the processed APOD data to a CSV file.
Iris Dataset
Purpose: Analyzes the Iris dataset.
Key Functions:
load_and_analyze_iris(): Loads the dataset and provides basic analysis (e.g., column info, flower species count).
correct_iris_errors(): Corrects erroneous rows in the dataset.
add_features_and_save(): Adds new features like PetalRatio and SepalRatio, then saves the updated dataset.
calculate_correlations(): Analyzes correlations between features in the dataset.
scatter_with_regression(): Generates a scatter plot of Sepal vs Petal ratios with regression lines.
create_pair_plot(): Creates a pair plot of the Iris dataset, visualizing relationships between multiple attributes.
```
