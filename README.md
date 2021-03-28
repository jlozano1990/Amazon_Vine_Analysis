# Amazon_Vine_Analysis
## Purpose
The purpose of this project was to analyze Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

I chose to look at Digital Video Game reviews. I used PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Afterwards I used PySpark to determine if there was any bias toward favorable reviews from Vine members in the dataset.

## Results
**Q:** How many Vine reviews and non-Vine reviews were there?

**A:** There were 0 Vine reviews and 1563 non-Vine Reviews.

![Vine Y Review Count](https://github.com/jlozano1990/Amazon_Vine_Analysis/blob/main/Images/vine_reviews_Y_count.PNG)

![Vine N Review Count](https://github.com/jlozano1990/Amazon_Vine_Analysis/blob/main/Images/vine_reviews_N_count.PNG)


**Q:** How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

**A:** Being that there were no Vine reviews, none were 5 stars. Of the non-Vine reviews, 582 were 5 star reviews.

![Five star review N vine count](https://github.com/jlozano1990/Amazon_Vine_Analysis/blob/main/Images/five_star_review_N_count.PNG)


**Q:** What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

**A:** 0% of vine reviews were 5 stars since there were none. Of the non-Vine reviews, 37.25% of the reviews were 5 stars.

![Percentage of five star reviews N Vine Count](https://github.com/jlozano1990/Amazon_Vine_Analysis/blob/main/Images/percentage_5_star_N_vine.PNG)

## Summary 
In my analysis, I cannot say there was a positivity bias for reviews in the Vine program. The vine program did not have any reviews in the Digital Video Game dataset. I can only assume that the Vine program does not give out digital video games for reviews. Using a different dataset would obviously have shown different results, but with the dataset I used, there was not enough information to show a positive or negative bias for reviews coming from the Vine Program.
