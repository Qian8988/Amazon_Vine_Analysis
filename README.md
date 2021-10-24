# Amazon_Vine_Analysis

Module 16 Challenge

## Overview of the analysis:  
This challenge is to analyze Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

I choose [amazon_reviews_us_Books_v1_01] as the datasets and use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, I used PySpark to determine if there is any bias toward favorable reviews from Vine members in the dataset. Then, I wrote a summary of the analysis for Jennifer to submit to the SellBy stakeholders.

## Results: 

### How many Vine reviews and non-Vine reviews were there?

Total Number of Reviews PAID : 4781

Total Number of Reviews UNPAID : 332395


<img width="396" alt="1" src="https://user-images.githubusercontent.com/86527347/138576521-890b02c4-fc55-49da-ba4b-1a120be3c068.png">




### How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

The Number of 5-star Reviews Paid : 1604

<img width="435" alt="2" src="https://user-images.githubusercontent.com/86527347/138576518-ef7c184a-2985-4254-a9fd-fd1cc555c242.png">

The Number of 5-star Reviews Unpaid: 168800

<img width="437" alt="3" src="https://user-images.githubusercontent.com/86527347/138576519-6ef03e46-9067-48d9-8245-5231a8711ec7.png">


### What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

Percent of 5-Star Reviews for PAID : 0.335495

Percent of 5-Star Furniture Reviews from UNPAID : 0.507830

<img width="531" alt="4" src="https://user-images.githubusercontent.com/86527347/138576520-00c9bacc-c020-446c-b476-c45cea4e5c04.png">


## Summary:  

There are 4781 vine reviews and 332395 of non-Vine reviews. 98.58% of the reviews are from non-Vine participants. The percentage of 5-star reviews from vine participants is 33.55% whereas the percentage of 5-star reviews from the non-Vine reviews is 50.78%. So, we cannot say there is any positivity bias for reviews in the Vine program.

As for recommendations, more data needed to be collected and we need to see the spread of  reviews for each star rating and calculate mean, median, and  frequency of the reviews.



