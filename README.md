# Amazon_Vine_Analysis

## Overview of the analysis: Explain the purpose of this analysis.

The following analysis uses Amazon reviews written by members of the paid Amazon Vine program. This program is a service that allows manufacturers and publishers to receive reviews for their products. The goal of the analysis is to determine if there's any bias toward favorable reviews from Vine members in the selected dataset. 
The dataset used for this analysis was the "BEauty dataset". For The analysis used PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. 

## Results: Using bulleted lists and images of DataFrames as support, address the following questions:

- ##Total number of reviews##
- - Vine reviews: 647

- - Non-vine reviews: 74113

- ##Total number of 5 star reviews##
- - Vine reviews: 229
- - Non-vine reviews: 43217

- ##Percentage of 5 star reviews##
- - Vine reviews: 35.39%
- - Non-vine reviews: 58.31%

##Visual Summary of Vine Reviews##

![Paid Reviews Summary](https://user-images.githubusercontent.com/88411140/144507001-e6979eda-b5e8-4392-b54d-aef43bfaa053.png)

##Visual Summary of Un-Vine Reviews##

![Unpaid Reviews Summary](https://user-images.githubusercontent.com/88411140/144507016-126c0967-b346-4c0c-8cf1-1b0f86778c82.png)



## Summary: In your summary, state if there is any positivity bias for reviews in the Vine program. Use the results of your analysis to support your statement. Then, provide one additional analysis that you could do with the dataset to support your statement.

35.39% of the reviews in the Vine program were 5 stars reviews whereas the percentage in the non-Vine reviews is around 58.31%. This implies that there's no positivity bias for reviews in the Vine program. 
Since beauty products have a wide range of sub categories. Perhaps we could categorize the products that the Vine program reviewed and run an analysis with similar products. The reason why I suggest this is because I noticed that the Vine program reviewed products like electronic face scrubs, while non Vine reviews were more towards baby products, and feet exfoliants. 
