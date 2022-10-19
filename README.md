# Cost of Living Analysis
Analysing Cost of Living Index statistically!

## Team
-   Amar Rai
-   Nandhini Nallathambi
-   Siyuan Liang
-   Vivian Nnadozie

## Technologies Used
-   Python
-   Pandas
-   Matplotlib
-   Python-API

## Files Uploaded
-   Data_Exploration_CleanUp.ipynb used for cleaning up the source files and format as required for further analysis.
-   Analysis.ipynb used for further analysis of the data and plot visualisations as required.
-   Input and Output CSV files in the folder "Data".
-   Output Images in the folder "Images".
-   Powerpoint presentations for the Project Scope and Analysis in the "Powerpoint Presentations" folder.

## Introduction
Cost of Living is the cost of maintaining a certain standard of living. 

With the global health crisis and conflicts in Ukraine, the increase in inflation and currency fluctuation are affecting international economic balances and the cost of living for each of us.

In this project we are analysing the Cost of Living Index data with G8 countries and understand where the United Kingdom stands.

We are also analysing how Cost of Living Index is impacted by other indexes like Rent Index, Groceries Index and Restaurant Price Index.

## Data Exploration and Cleaning
We have used the datasets from Kaggle (https://www.kaggle.com/datasets/ankanhore545/cost-of-living-index-2022) and Numbeo (https://www.numbeo.com/cost-of-living/rankings.jsp?title=2022).

Both are simple datasets with columns for Rank, Country / City, Cost of Living Index, Rent Index, Cost of Living Plus Rent Index, Groceries Index, Restaurant Price Index and Local Purchasing Power Index. Numbeo calculates the Cost of Living Index, Rent Index, Cost of Living Plus Rent Index, Groceries Index, Restaurant Price Index and Local Purchasing Power Index based on user inputs and data collected from authoritative sources. See https://www.numbeo.com/cost-of-living/cpi_explained.jsp and https://www.numbeo.com/common/motivation_and_methodology.jsp for the explanation and calculation of indexes by Numbeo.

We cleaned up the data by adding, deleting and splitting up of columns for ease of use. We also filtered out the data based on our requirement to analyse the performance of UK with that of countries with similar economic status. See Data_Exploration_CleanUp.ipynb for details.

![Bar_all_indexes_min_max](https://user-images.githubusercontent.com/111614210/196624808-1c0dfce5-baa2-46d7-8bc0-ddd2902df5a3.png)

This image shows the different indexes available along with the range (min and max values for each of the indexes).

## Why G8 countries for comparison?
The dataset has around 170 countries. The bar graph of Cost of Living Index for all countries is as follows:
![Bar_Cost_of_Living_all_countries](https://user-images.githubusercontent.com/111614210/196630707-9e1711e6-fbf4-4f2a-9ba5-f192137c5322.png)

To make it more realistic we decided to compare the performance of UK with a subset of countries.

![image](https://user-images.githubusercontent.com/111614210/196631418-3f09f1e3-19ff-450f-8394-d391ca58c1ee.png)

The top 10 countries by Cost of Living Index are developing nations and their economic structure is very different from that of UK and so these cannot be compared.

The G8 countries are not strictly the largest in the world nor the highest-income per capita, but they do represent the largest high-income countries. So we decided to use the G8 countries for this analysis.

## UK, in comparison with the other G8 countries
We decided to start our analysis by studying the different cost indexes for the G8 countries in comparison to the UK. We plotted some bar and pie charts for this.

![image](https://user-images.githubusercontent.com/111614210/196809359-323213ea-dbea-4ca7-91a3-1df3ed849ca6.png)
![image](https://user-images.githubusercontent.com/111614210/196809447-468e88da-b81b-476d-b8de-d64e4b830be4.png)
![image](https://user-images.githubusercontent.com/111614210/196809606-5ca1e5a7-c841-43ae-a297-37f4f5c782dd.png)
![image](https://user-images.githubusercontent.com/111614210/196809671-af07c706-6b3e-4530-ae97-868717f73bd7.png)
![image](https://user-images.githubusercontent.com/111614210/196809749-801021b6-0a4d-4caa-a3bb-7e1af4d37cfc.png)

As our pie charts show, Japan has the highest cost of living at 77.03 amongst the G8 and the highest groceries index at 81.31 compared to the UK which holds 69.65 and 56.58 respectively.

The US has the highest rent index at 42.07 compared the UK’s 31.84. 

The UK has the highest restaurant price index at 76.79 and the US has the highest local purchasing power index at 106.34 compared to the UK’s 88.78.

But what stands out is that Russians have the least  indexes compared to the rest.

## The biggest impact on Cost of Living
![image](https://user-images.githubusercontent.com/111614210/196807114-dc412430-8db6-427b-974f-936ddb44c207.png)
![image](https://user-images.githubusercontent.com/111614210/196807308-a1221ed1-ea70-4635-b923-2acbaf446f84.png)
![image](https://user-images.githubusercontent.com/111614210/196807809-df1c8ae5-48d6-4954-8a68-bf700b596ba1.png)

These plots are based on the index values of the G8 countries.

While all the 3 indexes (Rent, Groceries and Restaurant Price) have a strong relationship with the Cost of Living index, the impact of Groceries Index on Cost of Living Index is higher.

![image](https://user-images.githubusercontent.com/111614210/196807942-c163bd1f-e618-4791-8208-60b679493330.png)
![image](https://user-images.githubusercontent.com/111614210/196808107-850f339c-e5da-4b5c-bd24-37565b455cb4.png)
![image](https://user-images.githubusercontent.com/111614210/196808156-d108b700-99ac-43dd-99ee-c59b19e7bed0.png)

These plots are based on the index values of the G8 cities.

These graphs also confirm that all the 3 indexes (Rent, Groceries and Restaurant Price) have a strong relationship with the Cost of Living index but the impact of Groceries Index on Cost of Living Index is higher.

## Local Purchasing Power Index
![image](https://user-images.githubusercontent.com/111614210/196808576-ac91bc0b-923c-4b93-ba51-ee07391eb277.png)
![image](https://user-images.githubusercontent.com/111614210/196808694-66002c43-0935-451c-85ed-993a7c54ebb1.png)

These plots for the relationship between the Cost of Living index and LPP index values show that the relationship is strong when plotted based on country’s index value.

However, when plotted by using the index values of cities, it shows that the relationship is weak.

## Explanatory Data Analysis
### Cost of Living Index
![image](https://user-images.githubusercontent.com/111614210/196802845-ce3ff554-e7e1-49f0-9895-3e6c962760e5.png)

This box plot is based on the Cost of Living Index of the G8 cities.

While the distribution for UK, Canada, Germany and Italy are close to symmetric (normal distribution), that of the US, Japan, France and Russia are positively skewed (skewed right).

In comparison, the cost of living in the cities in UK, US, Canada, Germany and Italy seem to be in the similar range while that of the cities in Germany and France seem to be higher and that of Russia is less.

The outlier here for the UK is that of London which shows that the cost of living in London is way higher than the other major cities.

The cost of living index across the major US cities is widely spread.

### Local Purchasing Power Index
![image](https://user-images.githubusercontent.com/111614210/196801618-928cc990-a742-479f-8e0a-56e9bfba5486.png)

This box plot is based on Local Purchasing Power Index of the G8 cities.

While the distribution for the US, UK, Canada, Germany and Italy are close to symmetric (normal distribution), that of Japan is negatively skewed (skewed left), France and Russia are positively skewed (skewed right).

In comparison, the local purchasing power in the cities in UK and Canada seem to be in the similar range.

The outlier here for the UK is that of Derby which shows that the local purchasing power in Derby is way higher than the other major cities.

The local purchasing power index across the major cities in US and Canada are widely spread.

## Cost of Living Heatmap

![Heatmap_cost_of_living_all_cities](https://user-images.githubusercontent.com/111614210/196636197-91c5c33f-9e43-4676-bccd-380dac249601.png)

## Conclusions

1) The United Kingdom stands 5th in terms of Cost of Living amongst the G8 countries. However in terms of Local Purchasing Power, UK seem to be doing better than most, standing 3rd. Only Germany’s numbers are better with a lower Cost of Living (6th) and higher Local Purchasing Power (2nd).

2) It is interesting that the Local Purchasing Power has a strong correlation with Cost of Living. Ideally, the decrease in the Local Purchasing Power causes serious negative economic consequences leading to the increase in Cost of Living.

3) As expected, all the 3 indexes for Rent, Groceries and Restaurant Price have a strong impact on Cost of Living. Groceries Index has a very high impact on Cost of Living Index.

4) Looking at the box plots for cost of living and local purchasing power, London is the most expensive city within the UK. With the highest local purchasing power Derby would be the best place to live in. The other cities seem to be within the national range for both cost of living and local purchasing power.

## Limitations

1) Numbeo uses user inputs and data from the government websites to calculate the indexes. This may not necessarily give the correct picture.

2) The dataset used is from early 2022 and so may not represent the current status.
