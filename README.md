# Amazon_Vine_Analysis
## Purpose
The purpose of this project was to analyze Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

I chose to look at reviews for watches. I used PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Afterwards I used PySpark to determine if there was any bias toward favorable reviews from Vine members in the dataset.

## Results
**Q:** How many Vine reviews and non-Vine reviews were there?

**A:** There were 43 Vine reviews and 7750 non-Vine Reviews totaling 7793 reviews.

![Total Review Count](https://github.com/jlozano1990/Amazon_Vine_Analysis/blob/main/Images/total_review_count.PNG)

**Q:** How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

**A:** Of the vine reviews, 14 were five-star reviews. Of the non-Vine reviews, 4027 were 5 star reviews.

![Five star review Y vine count](https://github.com/jlozano1990/Amazon_Vine_Analysis/blob/main/Images/five_star_review_Vine_Y_count.PNG)

![Five star review N vine count](https://github.com/jlozano1990/Amazon_Vine_Analysis/blob/main/Images/five_star_review_Vine_Y_count.PNG)


**Q:** What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

**A:** 32.56% of vine reviews were 5 stars. Of the non-Vine reviews, 51.96% of the reviews were 5 stars.

![Percentage of five star reviews Y Vine Count](https://github.com/jlozano1990/Amazon_Vine_Analysis/blob/main/Images/percentage_5_star_Y_vine.PNG)

![Percentage of five star reviews N Vine Count](https://github.com/jlozano1990/Amazon_Vine_Analysis/blob/main/Images/percentage_5_star_N_vine.PNG)

## Summary 
In my analysis I found that there does not seem to be a positivity bias for reviews in the Vine program. The vine program had a lower percentage of positive reviews than reviews from people who did not participate in the Vine program. Another analysis we could with this dataset would be looking at the difference between 1 star reviews from those in the Vine program as opposed to those not participating in the Vine program. We could look to see if people participating in the Vine program might be more critical of products or not.
