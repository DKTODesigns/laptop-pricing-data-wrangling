# laptop-pricing-data-wrangling
Data wrangling and preprocessing project using pandas: cleaning, transforming, and preparing a laptop pricing dataset for analysis and modeling.
Data Wrangling – Laptop Pricing Dataset
Overview

This project demonstrates end-to-end data wrangling using a laptop pricing dataset. The goal is to clean, transform, and prepare raw data for analysis by handling missing values, correcting data types, standardizing units, and creating new features.

Tools & Libraries
Python
Pandas
NumPy
Matplotlib
Dataset

The dataset contains laptop specifications such as:

Manufacturer
Category
Screen type
CPU details
RAM and storage
Weight
Price
Data Wrangling Steps
1. Data Loading
Loaded dataset from external source using Pandas
Removed unnecessary column (Unnamed: 0)
2. Missing Value Handling
Identified missing values using .isnull()
Replaced missing numerical values with mean:
Weight_kg
Screen_Size_cm
3. Data Type Correction
Converted columns to appropriate formats:
Float: Weight_kg, Screen_Size_cm
Integer: Price
4. Feature Engineering
Created new features:
Weight_pounds (kg → lbs conversion)
Price-binned (Low / Medium / High categories)
5. Normalization
Scaled CPU_frequency between 0 and 1
6. Categorical Encoding
Converted Screen into indicator variables:
Full HD
IPS Panel
Visualization
Created a bar chart to visualize distribution of price categories

See: price_bins.png

Before & After

Before Cleaning
Raw dataset loaded with original structure
before_cleaning.png

After Cleaning
Processed dataset with new features and transformations applied
after_cleaning.png

Key Takeaways
Applied real-world data cleaning techniques
Transformed raw data into analysis-ready format
Practiced feature engineering and normalization
Improved dataset usability for machine learning
Insights
Majority of laptops fall into the Low price category
CPU frequency values vary within a normalized range
Most laptops are relatively lightweight (~under 2.5kg)
Why This Matters

Data preprocessing is a critical step in any data workflow. This project ensures:

No missing values
Consistent data types
Scaled numerical features
Encoded categorical variables

These steps make the dataset ready for modeling and analysis.
