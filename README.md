# Amazon Vine Analysis

## Overview 

This repo uses Pyspark via Google Colab to analyze reviews on Amazon for pet supplies. 

First I used Amazon Web Services to create and export tables to PgAdmin sql. I then ran further analysis on the Vine Table. I wanted to see if there was a favorable bias for Amazon Vine review, which are reviews that companies can pay for. Amazon Vine members to write.

Before running the analysis, I first filtered the dataset for reviews with 20 or more votes and where the percentage of helpful review was greater or equal to 50%. 


## Results


![Screen Shot 2021-08-07 at 4 55 50 PM](https://user-images.githubusercontent.com/80648379/128653028-cfebcc0d-ba86-4967-9fcc-a9f33d85cef3.png)



* Out of the 38,010 reviews, only 170 were Vine reviews and the other 37,840 were not, which means only 0.45% of the reviews were part of the Vine program. 
* Of the 170 Vine reviews, only 65 of them were 5-star reviews and 20612 of the non-vine reviews were 5-Star reviews.
* 38.2% of the Vine reviews were 5-star reviews and 54.5% of the regular reviews were 5-star reviews 

## Summary 
From the results above, there does not appear to be a favorable bias for Vine reviews. In fact, the percentage of 5-star reviews for Vine reviews was less than the percentage of 5-star reviews for non-Vine reviews. To run further analysis to see if there was a bias, I would run a similar analysis looking at the number of 4-star reviews as well, because we do not know what those other 105 Vine ratings are. If the percentage of 4 and 5 star reviews was greater for Vine vs. Non-Vine reviews, then there would be a bias for favorable reviews. Since there are not many Vine reviews for Pet Supplies, it would also be helpful to run this analysis on other categories as well to get a better picture of Vine vs. non-Vine reviews. 
