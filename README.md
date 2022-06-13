# Amazon Vine Analysis

## Overview
Amazon Vine is a program where sellers pay a small fee and provide products to Amazon users who are then required to publish reviews. Using pyspark, relational databases, and Amazon Web Services (AWS), we will look the effectiveness of the program in the Digital Video Games category.

## Results
Before we conducted analysis on the data, the raw data was filtered to only show products with20 or mote votes and the percentage of helpful votes is 50% or greater. 

![filtering](https://user-images.githubusercontent.com/57120024/173459279-fa115085-7d55-4cc6-a90d-d59868948f0f.PNG)

After the data was filtered it was split into two dataframes, one with reviews from the vine program, the other with regular reviews(non-vine). An empty dataframe was returned for the first dataframe, there were no reviews from the Vine program in the Digital Video Games Category.

![vine_df](https://user-images.githubusercontent.com/57120024/173459291-03724d1f-39a2-45dc-9c77-db12f3883367.PNG)

![nonvine_df](https://user-images.githubusercontent.com/57120024/173459303-067ecb28-3db5-422b-bef7-e3dc29d05132.PNG)

The count of reviews (total, vine, and nonvine), count of 5-star reviews (total, vine, and nonvine), and percentage of 5-star vine and nonvine reviews can be seen below.

![review totals](https://user-images.githubusercontent.com/57120024/173459497-47441684-7152-46d9-834e-f29945b80ce5.PNG)


## Summary
In the video games category, there were no Vine reviews in our cleaned data so it is not known the effect of the program on the category but can be assumed that it is not worth it for sellers. To get a better understanding of reviews we could conduct analysis on the text of the reviews using Natural Language Processing. This will give us better insight on the review than the star rating system because each user's value of the star is different.
