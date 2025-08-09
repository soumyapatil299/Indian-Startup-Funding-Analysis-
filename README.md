# Indian-Startup-Funding-Analysis-

## Overview
This project involves data cleaning and preparation for a dataset on Indian startup funding rounds. The Jupyter Notebook (`Project.ipynb`) loads a CSV file containing startup funding details, performs data cleaning operations (handling missing values, data type conversions, string normalization), and prepares the data for further analysis or visualization.

The dataset includes information such as:
- Startup names
- Funding dates
- Industry verticals and sub-verticals
- City/Location
- Investors
- Investment types
- Funding amounts (in USD)


- **Source**: The notebook loads data from `/content/startup_funding.csv` (likely sourced from public datasets like those on Kaggle or Tracxn, covering Indian startups from around 2015-2020 based on sample dates).
- **Columns**:
  - Sr No
  - Date dd/mm/yyyy
  - Startup Name
  - Industry Vertical
  - SubVertical
  - City Location
  - Investors Name
  - InvestmentnType
  - Amount in USD
  - Remarks (dropped during cleaning)
- **Size**: 3044 entries.
- **Notes**: The dataset has some inconsistencies (e.g., invalid dates, missing values, malformed strings like URLs in startup names), which are handled in the notebook.

If you don't have the CSV, you can download similar datasets from sources like:
- Kaggle: Search for "Indian Startup Funding Dataset".
- Ensure the CSV matches the structure used in the notebook.

## Requirements
- Python 3.x
- Libraries (installed via pip):
  - pandas
  - numpy
  - matplotlib
  - seaborn

Install dependencies:
```
pip install pandas numpy matplotlib seaborn
```

## Usage
1. Clone or download the repository.
2. Place the `startup_funding.csv` file in the project directory (or update the file path in the notebook).
3. Open the Jupyter Notebook:
   ```
   jupyter notebook Project.ipynb
   ```
4. Run the cells sequentially to load, clean, and inspect the data.
5. The notebook outputs:
   - Dataframe head and info.
   - Cleaned dataframe ready for analysis.

## Notebook Structure
- **Import Libraries**: Loads pandas, numpy, matplotlib, seaborn.
- **Load Data**: Reads the CSV into a pandas DataFrame.
- **Data Cleaning**:
  - Drop unnecessary columns (e.g., 'Remarks').
  - Handle missing values by filling with 'unknown'.
  - Clean and convert 'Amount in USD' to numeric.
  - Convert dates to datetime format.
  - Normalize strings (lowercase, strip whitespace, remove special characters).
- **Output**: Displays cleaned DataFrame info and head.

