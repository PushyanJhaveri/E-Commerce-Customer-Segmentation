# E-Commerce-Customer-Segmentation
Ecommerce Data Analysis with Python

This repository contains a comprehensive Python script for analyzing an ecommerce dataset. The script covers data retrieval, preprocessing, feature engineering, and exploratory data analysis (EDA). It utilizes popular libraries such as pandas, numpy, and matplotlib.

**Introduction**

This code focuses on analyzing an ecommerce dataset to derive insights through data cleaning, transformation, and visualization. The script performs the following tasks:

Loads the dataset and explores its structure.
Cleans the data by handling missing values, duplicates, and outliers.
Encodes categorical variables and transforms data types.
Engineers new features from existing data.
Visualizes data distributions and correlations.

**Dataset**

The dataset (ecommerce_data.csv) contains transaction records, including:

Invoice numbers
Product descriptions
Quantities sold
Unit prices
Customer IDs
Transaction dates
Countries

Make sure the dataset is in the same directory as the script or provide the correct path.

**Requirements**

The following Python libraries are required:

pandas
numpy
matplotlib
Install Dependencies
Copy code
pip install pandas numpy matplotlib
Code Breakdown

**1. Data Retrieval**

Load the dataset with the appropriate encoding (ISO-8859-1).
Explore the dataset using head(), info(), describe(), and functions to check for missing and duplicate values.

**2. Data Preprocessing**

Drop rows with missing CustomerID.
Fill missing Description values with "Unknown".
Remove duplicate rows.
Filter out rows with negative values in Quantity and UnitPrice.
Remove extreme outliers in Quantity and UnitPrice.
Convert InvoiceDate to datetime format.

**3. Encoding Categorical Variables**

Encode the Country column using one-hot encoding.
Convert InvoiceNo and StockCode to string type.

**4. Feature Engineering**

Extract Year, Month, Day, and Hour from InvoiceDate.
Create a new feature TotalAmount as Quantity × UnitPrice.

**5. Exploratory Data Analysis (EDA)**

Distribution of Total Transaction Amount: Visualize the distribution of total amounts.

Number of Transactions by Country: Plot the number of transactions for each country.

Correlation Matrix: Analyze correlations between Quantity, UnitPrice, and TotalAmount.

Running the Code

Clone the repository:
bash

Copy code
git clone https://github.com/yourusername/ecommerce-data-analysis.git
Navigate to the project directory:
bash
Copy code
cd ecommerce-data-analysis

Run the script:

Copy code
python ecommerce_analysis.py
Ensure the ecommerce_data.csv file is in the same directory or provide the correct path.

Results

Data Cleaning: Missing values, duplicates, and outliers are handled.
Feature Engineering: New features like Year, Month, Day, Hour, and TotalAmount are created.

Visualizations:

Distribution of transaction amounts.
Number of transactions by country.
Correlation matrix heatmap.
