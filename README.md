# Cost of Living Analysis
Analysing Cost of Living Index statistically!

## Technologies Used
-   Python
-   Pandas
-   Matplotlib
-   Python-API

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

