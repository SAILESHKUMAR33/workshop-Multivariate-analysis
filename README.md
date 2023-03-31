#Workshop-Multivariate-analysis
Aim

To perform Multivariate EDA on the given data set.

##Explanation

Exploratory data analysis is used to understand the messages within a dataset. This technique involves many iterative processes to ensure that the cleaned data is further sorted to better understand the useful meaning.The primary aim with exploratory analysis is to examine the data for distribution, outliers and anomalies to direct specific testing of your hypothesis.
Algorithm

Step1

Import the built libraries required to perform EDA and outlier removal.

Step2

Read the given csv file.

Step3

Convert the file into a dataframe and get information of the data.

Step4

Return the objects containing counts of unique values using (value_counts()).

Step5

Plot the counts in the form of Histogram or Bar Graph.

Step6

Use seaborn the bar graph comparison of data can be viewed.

Step7

Find the pairwise correlation of all columns in the dataframe.corr()

Step8

Save the final data set into the file.

Types of bivariate analyis:

1)Numerical & Numerical(Scatter plot)
2)Numerical & Categorical(Bar plot,Box plot,Dist plot)

Program:

Developed by :saileshkumar A
Registration Number : 212222230126

import pandas as pd
import numpy as py
import seaborn as sns
import matplotlib.pyplot as plt

df=pd.read_csv('FlightInformation (1).csv')sns.scatterplot(df['Duration'],df['Price'],hue=df['Dep_Time'])
df
df.head()
df.info()
df.describe()
df.isnull().sum()
df.dtypes

sns.scatterplot(df['Duration'],df['Price'],hue=df['Dep_Time'])
sns.barplot(x=df['Dep_Time'],y=df['Price'],data=df)
df.corr()

Output:

Data Head

![image](https://user-images.githubusercontent.com/113497410/229035802-9dd6ed5d-7584-4d58-a19e-fd02c0d8b3bc.png)

Data Information

![image](https://user-images.githubusercontent.com/113497410/229035872-d8be3400-bcd7-40f1-b337-2621089c76d5.png)

Numerical & Numerical(Scatter plot)

![image](https://user-images.githubusercontent.com/113497410/229035932-58bb3f64-9012-4829-b591-0eb6a9747fd8.png)

Numerical & Categorical(Bar plot)

![image](https://user-images.githubusercontent.com/113497410/229035995-8c7a5be4-a294-434f-bc29-c8c1da65a4c0.png)

Non-Graphical method(correlation)

![image](https://user-images.githubusercontent.com/113497410/229036057-cdaf1859-cf77-4851-9139-fd2947f2a702.png)

Result:

Thus we have performed Multivariate EDA on the given data set.
