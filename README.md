# Country-Delight-Data-Analysis-Documentation

## INTRODUCTION
 This document contains the step by step process of the data analysis conducted using Country Delight dataset with the aim of solving a business challenge. A little background information on the company Country Delight is a company that started in India in 2015 with the goal of bringing back the basics to milk.The company specializes in delivering natural,fresh and unadulterated milk to the consumers doorstep. The company is posed with a challenge that this analysis aims to solve and i will be sharing my process with you. This analysis and Visualization was completed using Excel,I used Excel because its suitable for the data size.

## DATA DESCRIPTION
The raw dataset contains contains 6 columns and 1,449 rows, it contains country delight orders data from the 14th of september, 2022  to the 13th of march 2023 the columns were named as follows:

1 Year of Created_date: This contains the year part of the order date.

2 Month of created_Month: This cointains the month part of the order date.

3 Week of created_date: This contains the week of the year the order falls.

4 Day of created_date: As the name implies its the day part of the order date.

5 Measure Names: This contains the names of 8 different values namely AOV( Average order value), ASP per unit(Average selling price), sku per Order (stock keeping unit), Qty/order (Average quantity per order), customers(Number of customers per day), Order amount(subtotal of orders per day), Quantity (toal quantity ordered per day),Count of orders (total order per day).

6 Measure Values: This contains values that corresponds with the measure names  

## BUSINESS QUESTION
Country delight is faced with a challenge overall orders per day in a region are increasing but the overall quantity ordered in given region is not. So i will be conducting an exploratory data analysis to solve the problem and provide recommendations.

## DATA QUALITY ASSESSMENT 
Before conducting the EDA the first step was to assess the quality of the dataset to ensure that the dataset is valid, accurate and void of discrepancies. To do this I  started by  loading the dataset in Excel after which i did the following:

1 Check for Duplicate values using Excel built in feature: The dataset does not contain  duplicate values.

2 Check for missing Values by filtering the data set: The data set has no missing value

3 Check for Inconsistency: The data set is consistent and does not cointain outliers.

After this phase i proceeded to the next step  data transformation.

## DATA TRANSFORMATION
After assesing the data quality I transformed the data by creating a new column called date. I created this to combine the date values that was seperated  in 3 different columns into one datevalue containing the day, month and year. To do this  I used the CONCATENATE function in excel to combine the 3 columns using this formula

```=CONCATENATE(D2,"-",B2,"-",A2)```

This formula combined the day which is contained in cell D2 with the month in cell B2 and the year contained in cell A2, then i used the autofill feature to fill other cells. Then I created another column to convert the combined date to an actual date value in Excel with the standard date format in Excel "mm/dd/yy". To do this I used the 'datevaule' function in Excel 

```=DATEVALUE(G2)```

This coverted the G2 cell  which was created using the CONCATENATE function into date, the month written in words was converted into the equivalent numeric value.
[Insert picture]

## DATA ANALYSIS
To begin the data analysis I identified the column relevant to the business question 
