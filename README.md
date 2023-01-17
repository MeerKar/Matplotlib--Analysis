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

7. Final analysis.

For these analysis both datasets imported, merged and the aggregate data displayed into s single dataframe.This project is conducted in Jupyter Noebook and the link is as follows.

http://localhost:8889/notebooks/Pymaceuticals/pymaceuticals_starter.ipynb

# 1. Prepare the data

  With the provided dependencies data imports, and then merge the mouse_metadata and study_results DataFrames into a single DataFrame.

 The number of unique mice IDs in the data, and  any mouse ID with duplicate time points has been displayed and checked. Then the data associated with that mouse ID has been displayed, and then created a new DataFrame where this data is removed. 
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

A two bar charts has been generated. Both charts were identical and showed the total number of time points for all mice tested for each drug regimen throughout the study. The first bar chart with the Pandas DataFrame.plot() method and the second bar chart with Matplotlib's pyplot methods.It is as shown below.

<img width="736" alt="image" src="https://user-images.githubusercontent.com/116701851/212795862-ec0b6307-a75d-4352-9a04-fc6d0b9f7d9b.png">

<img width="288" alt="image" src="https://user-images.githubusercontent.com/116701851/212795980-10f89285-800d-42d6-a0f7-5002a6243bb4.png">


<img width="735" alt="image" src="https://user-images.githubusercontent.com/116701851/212796104-b2fc7013-d041-4b75-b355-b734ecd64c78.png">


Similarly generated two pie charts which identical and showed the distribution of female versus male mice in the study.
Like the bar chart \ the first pie chart with the Pandas DataFrame.plot() method and the second pie chart with Matplotlib's pyplot methods. 

Inorder to get the pie plot showing the distribution of female versus male mice using Pandas
  First used Group by gender and got the number to plot

<img width="305" alt="image" src="https://user-images.githubusercontent.com/116701851/212818954-1f958179-806e-4139-80b5-9fd8a8a6b7fc.png">


<img width="686" alt="image" src="https://user-images.githubusercontent.com/116701851/212819041-15707650-77d9-40b6-a812-970bfae96e54.png">

Pie chart with pyplot method.

<img width="732" alt="image" src="https://user-images.githubusercontent.com/116701851/212819162-cf0232c2-7fac-44de-af1b-dd22f4a79643.png">


# 4. Calculate quartiles, find outliers, and create a box plot.

The final tumor volume of each mouse across four of the most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin. 
The quartiles and IQR, to determine if there are any potential outliers across all four treatment regimens also  been calculated:

Capomulin Final Tumor Volume:

<img width="722" alt="image" src="https://user-images.githubusercontent.com/116701851/212820345-50fca071-5851-4ddc-a70d-fe1c46379f1c.png">

Capomulin Quartiles , IQR and values above and below outliers:

<img width="550" alt="image" src="https://user-images.githubusercontent.com/116701851/212821614-e702f2de-b7f3-4012-b000-951dca6b240c.png">

Ramicane  Final Tumor Volume:
<img width="735" alt="image" src="https://user-images.githubusercontent.com/116701851/212822283-258d302e-8a4a-4382-a707-946850048fd6.png">


Ramicane Quartiles , IQR and values above and below outliers:

<img width="546" alt="image" src="https://user-images.githubusercontent.com/116701851/212822336-4b8062f2-e679-44c9-a1d4-4095c9b7b3e0.png">

Infubinol Final Tumor Volume:

<img width="714" alt="image" src="https://user-images.githubusercontent.com/116701851/212822587-41f08fac-af8d-4d05-adeb-9508f5a69de2.png">

Infubinol Quartiles , IQR and values above and below outliers:

<img width="571" alt="image" src="https://user-images.githubusercontent.com/116701851/212822775-356db8c1-06a9-40ed-8601-9d6b90577cf5.png">

Ceftamin Final Tumor Volume:

<img width="751" alt="image" src="https://user-images.githubusercontent.com/116701851/212822966-0b471932-3b7b-4cbc-bc82-5f499c2922db.png">

Ceftamin Quartiles , IQR and values above and below outliers:

<img width="545" alt="image" src="https://user-images.githubusercontent.com/116701851/212823024-72016a9e-0d5c-4c4c-9c04-f0aced789217.png">

A box plot is generated to shows the distrubution of the tumor volume for each treatment group.

<img width="721" alt="image" src="https://user-images.githubusercontent.com/116701851/212824074-033b0c5c-4fa6-4da4-b3d2-5a0a127fdfbb.png">


# 5. Create a line plot and a scatter plot.

A line plot is generated to find the  tumor volume vs. time point for a mouse ID 'b742' with Capomulin

<img width="776" alt="image" src="https://user-images.githubusercontent.com/116701851/212825824-c4afc25b-289a-4ab1-a83c-065b5ca345a6.png">


A scatter plot is generated to find the average tumor volume vs. mouse weight for the Capomulin regimen

<img width="739" alt="image" src="https://user-images.githubusercontent.com/116701851/212826056-bbd561ac-9724-4efd-ab6e-7fe0a875a0f0.png">



# 6. Calculate correlation and regression.

The correlation coefficient and linear regression model is found as

<img width="405" alt="image" src="https://user-images.githubusercontent.com/116701851/212826446-bbaae128-7ed72fd10a5aebd.png">

<img width="466" alt="image" src="https://user-images.githubusercontent.com/116701851/212826674-46ec34a4-96eb-44f4-abb7-0dbedde1d853.png">

A linear plot is created as follows,

<img width="728" alt="image" src="https://user-images.githubusercontent.com/116701851/212826921-178ffce5-b97c-42d7-94ac-84413abfdd86.png">

#  7. Final analysis.

 The final analysis prove that from the selected treatements Capomulin and Ramicane reduces the size of tumors better. In order to get these results it is seen from the bar graph that Capomulin Drug has the maximun mice number(230) and Zoniferol has the minimun mice number(182).After cleaning the duplicates ,the total mice was shown as 248 and the total female mice is 124 and the male is 125.There is a strong corelation value of 0.84, shows when the mouse weight increase the average tumor volume also icrease.The R-squared value(0.70) shows the 70%  of the variation in response variable around its mean.





