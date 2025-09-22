Explanation of the Code
1.	Imports: The script begins by importing necessary libraries: pandas for data manipulation, csv for writing CSV files, math for mathematical operations, pathlib for handling file paths, and os for interacting with the operating system.
2.	Variable Initialization:
o	column_year is set to 2012, which is the starting year for data aggregation.
o	transform and data dictionaries are initialized to store aggregated results.
3.	Reading CSV Files:
o	A loop iterates over the years 2013 to 2016 (indicated by the range 3 to 7).
o	For each year, it reads the corresponding CSV file into a DataFrame using pd.read_csv().
4.	Data Aggregation:
o	For each row in the DataFrame, the script initializes quarterly totals for each state.
o	It checks for missing values using math.isnan() and sums the values for each quarter (Q1 to Q4).
o	The results are stored in the data dictionary, with each state as a key.
5.	Writing to CSV:
o	The script checks if a directory named "data" exists; if not, it creates one.
o	It then writes the aggregated data into a new CSV file named "Formula_Fed-Totals.csv".
