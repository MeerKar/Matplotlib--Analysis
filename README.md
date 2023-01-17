# Matplotlib--Analysis

# Background

You've just joined Pymaceuticals, Inc., a new pharmaceutical company that specializes in anti-cancer medications. Recently, it began screening for potential treatments for squamous cell carcinoma (SCC), a commonly occurring form of skin cancer.

As a senior data analyst at the company, you've been given access to the complete data from their most recent animal study. In this study, 249 mice who were identified with SCC tumors received treatment with a range of drug regimens. Over the course of 45 days, tumor development was observed and measured. The purpose of this study was to compare the performance of Pymaceuticals’ drug of interest, Capomulin, against the other treatment regimens.

The executive team has tasked you with generating all of the tables and figures needed for the technical report of the clinical study. They have also asked you for a top-level summary of the study results.


 This assignment is broken down into the following tasks:

1. Prepare the data.

2. Generate summary statistics.

3. Create bar charts and pie charts.

4. Calculate quartiles, find outliers, and create a box plot.

5. Create a line plot and a scatter plot.

6. Calculate correlation and regression.

7. Submit your final analysis.

For these analysis both datasets imported, merged and the aggregate data displayed into s single dataframe.This project is conducted in Jupyter Noebook and the link is as follows.

http://localhost:8889/notebooks/Pymaceuticals/pymaceuticals_starter.ipynb

# 1. Prepare the data

  With the provided dependencies data imports, and then merge the mouse_metadata and study_results DataFrames into a single DataFrame.

 The number of unique mice IDs in the data, and  any mouse ID with duplicate time pointshas been displayed and checked. Then the data associated with that mouse ID has been displayed, and then created a new DataFrame where this data is removed. 
 And this cleaned DataFrame is uesd for the remaining steps.

 The updated first 20 number of unique mice IDs are ,
 
 
<img width="786" alt="image" src="https://user-images.githubusercontent.com/116701851/212794017-58fef9ed-7b01-4cef-bc3a-36677eac1257.png">


With this cleaned  DataFrame the number of mice found was 248.

# 2. Generate summary statistics.

In this feild,

 A DataFrame is created with summary statistics. 
And the summary statistics  includes:
A row for each drug regimen. These regimen names  contains  the index column.
A column for each of the following statistics: mean, median, variance, standard deviation, and SEM of the tumor volume.

And the values are

<img width="490" alt="image" src="https://user-images.githubusercontent.com/116701851/212795188-a4b87b93-3873-4b21-bc1d-ef06ffd872c0.png">


# 3. Create bar charts and pie charts.

Generate two bar charts. Both charts should be identical and show the total number of time points for all mice tested for each drug regimen throughout the study.

Create the first bar chart with the Pandas DataFrame.plot() method.

Create the second bar chart with Matplotlib's pyplot methods.

Generate two pie charts. Both charts should be identical and show the distribution of female versus male mice in the study.

Create the first pie chart with the Pandas DataFrame.plot() method.

Create the second pie chart with Matplotlib's pyplot methods.









