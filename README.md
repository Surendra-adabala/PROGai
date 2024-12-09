# NASA APOD Data Analysis

This project is designed to solve four key problems based on the given assignment requirements. It integrates API data fetching, JSON data manipulation, matrix operations using NumPy, and analytical exploration of the Iris dataset with feature engineering.

---

## Project Description

The project resolves the following challenges:

1. **Fetching Data from NASA APOD API**: 
   - Retrieve data from the NASA Astronomy Picture of the Day (APOD) website using API keys. 
   - API keys are securely managed using the `dotenv` module.

2. **JSON Data Manipulation**: 
   - Read data fetched from the API in JSON format.
   - Perform manipulations and transformations as per the requirements.

3. **Matrix Operations with NumPy**: 
   - Create a 2D NumPy array based on predefined conditions.
   - Apply filtering techniques to extract a final processed array.

4. **Iris Dataset Analysis**: 
   - Conduct analytical observations on the Iris dataset.
   - Generate new features using feature engineering and analyze the results.

---

## Project Installation

Follow the steps below to set up the project environment:

1. Clone the repository:
   ```bash
   git clone https://github.com/Surendra-adabala/PROGai.git


NASA-APOD-Data-Analysis/
├── requirements.txt    # Python dependencies
├── README.md           # Project documentation
├── src/                # Source code
│   ├── CA_1.py         # Script combining all four problems
│   └── static_files/   # Static files directory
│       ├── apod_data.json  # JSON output file (generated dynamically)
│       └── apod_summary.csv # CSV output file (generated dynamically)

