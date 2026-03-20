# Data-Wrangling
. Aim
To study various data preprocessing techniques and implement the handling of missing values using specific Python functions and operations.

2. Objectives
Understand the necessity of cleaning and preparing raw data for analysis.

Identify common data discrepancies such as missing values, incorrect formats, and duplicate records.

Learn and apply Python functions to detect, count, and resolve missing data points.
+1

3. Theory
Data preprocessing is the foundational step of cleaning raw data before it is utilized for data analysis or machine learning. Real-world datasets are rarely perfect and often contain missing values, inconsistent formats, or duplicate records. Properly handling these issues is critical as it directly improves the quality of the data and the accuracy of the final analysis.
+2

Missing values commonly appear in datasets as:


NaN (Not a Number) or NULL.


Blank cells.


Special symbols such as "?", "-", or "NA".

4. Data Preprocessing Functions
The following table summarizes the primary functions used to inspect and identify the state of a dataset:

Category	Function	Description
Inspection	

head() 

Displays the first few records of the dataset.


tail() 

Displays the last few records of the dataset.


info() 

Shows rows, columns, data types, and missing value counts.


dtypes 

Specifically checks the data type of each column.

Identification	

isnull() 

Returns True for every missing value found.
+1


isnull().sum() 

Provides a total count of missing values per column.
+1


notnull() 

Returns True for valid (non-missing) values.
+1


unique() 

Displays the unique values within a column.


nunique() 

Counts the number of unique values.

5. Methods to Handle Missing Values
Once identified, missing data can be managed using the following strategies:

A. Removal (Deletion)

dropna(): Removes any rows that contain missing data points.


dropna(axis=1): Removes entire columns that contain missing values.

B. Imputation (Filling)

fillna(): Replaces missing values with a specified value.

Mean/Median/Mode:


mean(): Best for numerical data.


median(): Preferred for numerical data containing outliers.


mode(): Used for categorical data.

Directional Fills:


ffill: Replaces the missing value with the previous valid value.


bfill: Replaces the missing value with the next valid value.

6. Additional Operations

replace(): Used to convert custom symbols (like "?" or "-") into standard NaN values.
+1


drop_duplicates(): Removes repeated records to ensure data uniqueness.
+1

7. Conclusion
Through this study, various data preprocessing and missing value handling operations were successfully implemented using Python. These techniques ensure that a dataset is cleaned and optimized for accurate analysis.
