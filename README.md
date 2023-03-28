# Ex03-Univariate-Analysis

## Aim

To read the given data and perform the univariate analysis with different types of plots.

## Explanation

Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.

## Algorithm

### Step1
Read the given data.

### Step2
Get the information about the data.

### Step3
Remove the null values from the data.

### Step4
Mention the datatypes from the data.

### Step5
Count the values from the data.

### Step6
Do plots like boxplots,countplot,distribution plot,histogram plot.
## Program
```
Developed by : Manikandan P
Registration Number : 212221040099

import pandas as pd
import numpy as np
import seaborn as sns
df=pd.read_csv("SuperStore.csv")
df
df.head()
df.info()
df.describe()
df.isnull().sum()
df.dtypes
df['Sales'].value_counts()
sns.boxplot(x="Sales", data=df)
sns.countplot(x="Postal Code", data=df)
sns.distplot(df["Sales"])
sns.histplot(x="Sales", data=df)
```
## OUTPUT

### DATA
![Data](https://user-images.githubusercontent.com/119160414/228262317-1976afa3-5b61-4c86-93fc-767a93b7b180.png)

### DATA HEAD
![Data head](https://user-images.githubusercontent.com/119160414/228262609-778288ad-0eba-4a53-8f6d-19bc0617c487.png)

### DATA INFORMATION
![Info](https://user-images.githubusercontent.com/119160414/228262805-b8ea80d7-9007-4cae-a843-aa629762b8ab.png)

### DATA DESCRIBE
![Describe](https://user-images.githubusercontent.com/119160414/228262909-721b417e-32cc-4358-8c6d-7511a3cf2cd5.png)

### DATA NULL VALUES
![Null value](https://user-images.githubusercontent.com/119160414/228263003-c298e5fa-a952-4d80-bfb2-dab80cbd5317.png)

### DATA DATA TYPES
![Data type](https://user-images.githubusercontent.com/119160414/228263170-88fb383f-1e88-4fa8-b6a0-f3cd8cac8a3d.png)

### DATA VALUE COUNT
![Value count](https://user-images.githubusercontent.com/119160414/228263352-280dd097-45ad-45c9-bc21-2d9ca6f95981.png)

### BOXPLOT
![Box plot](https://user-images.githubusercontent.com/119160414/228263486-d1fa1547-ac7d-4857-879f-eb7e635f465c.png)

### COUNTPLOT
![Count plot](https://user-images.githubusercontent.com/119160414/228263673-af7fc244-e890-49db-a6ff-381694630f76.png)

### DISTRIBUTION PLOT
![Distribution plot](https://user-images.githubusercontent.com/119160414/228263899-7c7635bd-ea6c-4233-b107-520c323f5567.png)

### HISTOGRAM PLOT
![Histogram plot](https://user-images.githubusercontent.com/119160414/228263994-2c720ac4-871c-4b8d-88c5-d8f6afa8e0a4.png)

## RESULT
Thus we have read the given data and performed the univariate analysis with different types of plots.






