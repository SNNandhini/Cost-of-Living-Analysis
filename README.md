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

![G8 Cost of Living Index](https://user-images.githubusercontent.com/111614210/196632411-efbe5dcb-7510-48f2-a655-dfa0a4d21a6e.png)  ![G8 Local Purchasing Power Index](https://user-images.githubusercontent.com/111614210/196632502-306619bc-0918-4237-9d3a-feb7e4833871.png)   ![G8 Rent Index](https://user-images.githubusercontent.com/111614210/196632853-1d0dc64a-472b-463d-a7db-56de327e9b25.png)   ![G8 Groceries Index](https://user-images.githubusercontent.com/111614210/196632905-70aa8416-9aae-446a-b053-3663cd31053c.png)   ![G8 Restaurant Price Index](https://user-images.githubusercontent.com/111614210/196632963-3b77abb2-95ea-4a1d-aa8b-a5c85da00e0b.png)

As our pie charts show, Japan has the highest cost of living at 77.03 amongst the G8 and the highest groceries index at 81.31 compared to the UK which holds 69.65 and 56.58 respectively.

The US has the highest rent index at 42.07 compared the UK’s 31.84. 

The UK has the highest restaurant price index at 76.79 and the US has the highest local purchasing power index at 106.34 compared to the UK’s 88.78.

But what stands out is that Russians have the least  indexes compared to the rest.

## The biggest impact on Cost of Living
![G8 Cost of Living Index vs Rent Index](https://user-images.githubusercontent.com/111614210/196634153-98457bb0-d5f6-4001-b4ed-3372c5181e98.png)
![G8 Cost of Living Index vs Groceries Index](https://user-images.githubusercontent.com/111614210/196634225-bae48727-7214-4ee9-b0cd-f921d7e72d62.png)
![G8 Cost of Living Index vs Restaurant Price Index](https://user-images.githubusercontent.com/111614210/196634288-52405ba6-be2e-4bc3-85a2-4fa4865dbf79.png)

These plots are based on the index values of the G8 countries.

While all the 3 indexes (Rent, Groceries and Restaurant Price) have a strong relationship with the Cost of Living index, the impact of Groceries Index on Cost of Living Index is higher.

![G8_CitiesCost of Living Index_vs_Rent Index](https://user-images.githubusercontent.com/111614210/196634611-af814a52-d9fb-4f68-b132-31f2020a32f1.png)
![G8_CitiesCost of Living Index_vs_Groceries Index](https://user-images.githubusercontent.com/111614210/196634643-4bd1f341-947d-4f43-a530-7296d5bc49a8.png)
![G8_CitiesCost of Living Index_vs_Restaurant Price Index](https://user-images.githubusercontent.com/111614210/196634716-60794467-b4dc-49de-9bcf-9b886672d623.png)

These plots are based on the index values of the G8 cities.

These graphs also confirm that all the 3 indexes (Rent, Groceries and Restaurant Price) have a strong relationship with the Cost of Living index but the impact of Groceries Index on Cost of Living Index is higher.











