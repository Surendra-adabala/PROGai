APOD & Iris Dataset Analysis Project
Overview
This project is focused on two main parts:
1.	Astronomy Picture of the Day (APOD) Collection & Analysis
o	The goal is to retrieve and store APOD data (including images and videos) for a specified date range from NASA's API.
o	The data is then processed, including:
	Media type count (images vs videos)
	Identifying the longest explanation for an APOD entry
	Exporting the collected data into CSV format for further analysis.
2.	Iris Dataset Analysis
o	The Iris dataset is loaded, cleaned, and analyzed to study flower species attributes and their relationships.
o	Specific tasks include:
	Data correction for erroneous entries
	Feature engineering (e.g., PetalRatio and SepalRatio)
	Correlation analysis
	Creating a scatter plot with linear regression lines
	Generating a pair plot for comprehensive visualization
 
Requirements
•	Python: Version 3.x
•	Libraries:
o	requests
o	json
o	pandas
o	seaborn
o	matplotlib
o	scikit-learn
o	numpy
o	dateutil
Install required libraries with the following:
bash
Copy code
pip install requests pandas seaborn matplotlib scikit-learn numpy python-dateutil
 
APOD Data Collection
1. ApodFetcher
•	Purpose: Fetches the Astronomy Picture of the Day (APOD) data for a specified date range.
•	Key Functions:
o	get_apod_info(date): Retrieves APOD data for a single date.
o	download_apod_in_range(start_date, end_date): Downloads APOD data for a range of dates and stores it in a JSON file.
2. Process Flow:
•	The data is fetched from NASA's APOD API using the provided API key.
•	The collected data includes:
o	Date, Title, Media Type, Image Link, and Explanation.
 
Iris Dataset Analysis
1. ApodDataProcessor
•	Purpose: Processes and analyzes the collected APOD data.
•	Key Functions:
o	read_apod_data(): Reads the stored APOD data from a JSON file.
o	analyze_apod_media(): Analyzes the number of images and videos, and finds the longest explanation.
o	save_apod_to_csv(): Saves the processed APOD data to a CSV file.
2. Iris Dataset
•	Purpose: Analyzes the Iris dataset.
•	Key Functions:
o	load_and_analyze_iris(): Loads the dataset and provides basic analysis (e.g., column info, flower species count).
o	correct_iris_errors(): Corrects erroneous rows in the dataset.
o	add_features_and_save(): Adds new features like PetalRatio and SepalRatio, then saves the updated dataset.
o	calculate_correlations(): Analyzes correlations between features in the dataset.
o	scatter_with_regression(): Generates a scatter plot of Sepal vs Petal ratios with regression lines.
o	create_pair_plot(): Creates a pair plot of the Iris dataset, visualizing relationships between multiple attributes.

