# Absenteeism-at-work

This repository contains a Python script that performs an analysis of absenteeism in a company using a dataset titled "Absenteeism_at_work.xls". The dataset contains various features related to employees' absence, such as ID, Reason for absence, Month of absence, Day of the week, Seasons, Transportation expense, Distance from Residence to Work, Service time, Age, Workload Average/day, and more.

Installation
Before running the script, you need to install the required libraries. Use the following command to install them:

Copy code
pip install xlrd pandas seaborn scikit-learn imbalanced-learn matplotlib
Usage
To use this script, follow these steps:

Clone this repository to your local machine.
Make sure you have Python and the required libraries installed.
Place the "Absenteeism_at_work.xls" dataset in the same directory as the script.
Now, you are ready to run the script. Open a terminal or command prompt and navigate to the script's directory. Then, run the following command:

Copy code
python absenteeism_analysis.py
The script will execute the analysis and display various visualizations and insights related to absenteeism.

Functionality
The script performs the following tasks:

Reads the dataset into a Pandas DataFrame and displays the first five rows.
Retrieves the shape of the dataset and prints information about the data types and missing data.
Computes basic statistics (mean, std, min, max) for each numeric column.
Checks for duplicated rows in the dataset.
Analyzes the "Absenteeism time in hours" column, its distribution, and the target class balance.
Creates a new column "mask" that contains boolean values indicating if the target column is more than 3 hours.
Calculates the number of participants absent for more than three hours and those absent for less than three hours.
Collapses the "Reason for absence" column to reduce dimensionality and enhance explainability.
Explores the dataset based on various features such as "Month of absence," "Day of the week," "Seasons," "Transportation expense," etc.
Calculates the Pearson correlation of the features in the dataset.
Generates visualizations for better insights into the data, including histograms, bar plots, and correlation matrices.
Conclusion
This analysis provides valuable insights into absenteeism patterns in the company and identifies potential factors that may contribute to extended absences. The visualizations and statistical information can help in understanding and addressing absenteeism-related challenges.

# dataset
The dataset used for this task was obtained from the UCI machine learning repository website archive.ics.edu/ml/datasets.php and is titled Absenteeism at work.
The data was created with records of absenteeism from July 2007 to July 2010 at a courier company in Brazil. The data contains 740 observations and 21 features.
