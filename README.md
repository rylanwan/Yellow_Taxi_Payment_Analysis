# Yellow Taxi Credit Card Payment Analysis #
***
## Probelm & Motivation : ## 
Cashless payments have become popular recently. Payment methods such as credit cards and Apple Pay usually offer benefits and awards to their users. Those benefits include cash back, discounts, and point awards. However, not everyone has the access to using credit cards. Some of them don't know the advantages of using credit cards, and some of them don't know how to apply one. The familirity of cahsless payments can in fact cause financial gaps among societies/people.

## Research Objectives : ##
1. Identify the areas which have similar credit card payment rates/trends 
2. Identify the common features which affect credit card payment rates

## Data and Methodology : ##
Data: 
- NYC Taxi & Limousine Comission - Yellow Taxi Trip records from Jan. 2017 to Dec. 2018
- 2017 American Community Survey for demographical data

Data Preprocessing:
- Aggregate total number of trips taken across each taxi zone for each month
- Calculate percentage of trips paid using credit cards out of the total trips made using Yellow Taxi for each month in each zone

Analysis:
Using K-mean Clustering, Complete-linke Clustering, and Gaussian Mixture Model Clustering to identify unusal areas and common features

## Result: ##
### 1. K-mean Clustering with 4 clusters has best interpretability. 

<img src="https://github.com/rylanwan/Yellow_Taxi_Payment_Analysis/blob/master/Kmean.png" alt="alt text" width="600" height="600">

 - Cluster 0 covers midtown and downtown Manhattan, as well as downtown Brooklyn. Thoes areas have the highest credit card usage rate.
 - Cluster 2 has the second highest rate of credit card usage. It includes areas including upper Manhattan, Long Island, Astoria, and central Queens.
 - Cluster 1 has the third highest rate of credit card usage.It includes some remote areas in Queens, and Morrisania in Bronx.
 - Cluster 3 only have 4 areas according to the map. Most of them are non-redisdential areas like cemetery and parks. They are apprently outliers.
 
### 2. K-mean Clustering Analysis
- Investigate the differences within 3 clusters based on:
  - Trip count
  - Median Household income
  - Male population
  - Median age
  - Educational degree level
  - Number of liquors vendors (bars, resturants...)
 
#### Observation: There are positive correlations between the usage of credit cards and the number of trip count, median household income, educational degree level, and the number of liquor vendors.
