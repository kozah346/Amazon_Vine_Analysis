# Amazon_Vine_Analysis

## Overview
The following analysis is done to analyze Amazon reviews written by members of the paid Amazon Vine program. This program is a service that allows manufacturers and publishers to receive reviews for their products. 

This project is focused on a dataset containing reviews of clothing apparel. PySpark is used to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. PySpark, Pandas or SQL are used to determine if there is any bias toward favorable reviews from Vine members. However, this project will mainly use PySpark in this part of the project. 

## Results

After a careful and thorough analysis, the following is noted:
 
  * There are 33 paid reviews and 45388 unpaid reviews that are obtained as shown below:
       <img width="1280" alt="Total Paid Reviews" src="https://user-images.githubusercontent.com/101376325/178165858-a0c9abd5-1b68-43b6-99ad-3a7062b3ae5e.png">

       <img width="753" alt="Total Unpaid Reviews" src="https://user-images.githubusercontent.com/101376325/178165871-0169a840-6c24-458f-bf37-d10461609112.png">

  * From the 33 paid reviews, 15 had a five-star review on the product while 23733 of the 45388 unpaid reviews had a five-star rating as illustrated below:
        <img width="899" alt="Paid 5 star reviews" src="https://user-images.githubusercontent.com/101376325/178165992-ab570f16-8f83-4ecb-ae0a-44b01933e98a.png">
        <img width="919" alt="Unpaid 5 star reviews" src="https://user-images.githubusercontent.com/101376325/178166037-6cf5a2b1-d833-4f56-817c-96829cec67d0.png">

  * The paid 5 star reviews had a percentage of 45.45% of the total paid review products while unpaid 5 star reviews had a percentage of 52.29% of the total unpaid review products calculated as follows:
         <img width="692" alt="%age paid 5 star reviews" src="https://user-images.githubusercontent.com/101376325/178166227-7fe27f48-1e2b-41bf-b120-24844769609f.png">
        <img width="720" alt="%age unpaid 5 star reviews" src="https://user-images.githubusercontent.com/101376325/178166231-06f762f6-5d39-4edf-a7c9-db8ba2dacaf1.png"> 


## Summary

From the above analysis, it is seen that paid reviews were more strict in their ratings as they had 45.45% of the products with 5 star ratings as compared to unpaid reviews which had 52.29% which is around 7% more. Therefore, it is safe to conclude that there is no positivity bias for reviews in the vine program as seen from the clothing apparel dataset.

A good recommendation to support the above conclusion can be running the same analysis on a different kind of merchandise such as video games, kitchen appliances, mobile electronics and many more to see the general trend.