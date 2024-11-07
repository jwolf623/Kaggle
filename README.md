US Election Dataset Preprocessing
This script performs data cleaning and preprocessing steps on a U.S. election dataset, preparing the data for further analysis or modeling. It handles missing values, cleans string columns, and provides a summary of the data.

Features of the Script
Load Data:

The dataset is loaded from a CSV file located at /Users/jordanwolfson/Desktop/US_Election_dataset_v1.csv.
Drop Unnecessary Columns:

The script removes the column Unnamed: 0, which is assumed to be an index column without useful information.
Data Cleaning:

String Columns with Percentages: Columns that contain percentage signs (%) are cleaned by removing the % symbol and converting the values into numeric (float) format.
Numeric Formatting: Commas (if present) are removed from numeric strings before conversion.
Handle Missing Data:

Numeric Columns: Missing values in numeric columns are replaced with the column mean.
Categorical Columns: Missing values in categorical columns are replaced with the most frequent value (mode).
Missing Values Summary:

The script calculates and prints a summary of missing values in each column, highlighting which columns still contain missing data after preprocessing.
Optional Encoding of Categorical Variables:

An optional step (currently commented out) for encoding categorical variables (like state) using one-hot encoding (pd.get_dummies) is provided. This step can be uncommented and modified as needed.
How to Use
Ensure that the dataset file US_Election_dataset_v1.csv is located at the specified file path: /Users/jordanwolfson/Desktop/.
Run the script in a Python environment with the pandas library installed.
The script will:
Load the dataset.
Clean and preprocess the data (drop unnecessary columns, clean percentage values, handle missing values).

It also assumes that missing numeric data should be filled with the mean, and missing categorical data should be filled with the most frequent value (mode).
The script can be customized further based on the specific structure and requirements of the dataset.
