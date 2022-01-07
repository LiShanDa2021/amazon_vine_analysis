### Amazon Vine Review Analysis:
# Investigation of Possible Bias

## Overview
Our client, Sellby, is interested in enrolling in the Amazon Vine program -- a program in which select customers are paid to review the products they purchase --, but they want to know if it is worth the cost. That is, they want to know if Vine reviews are comparatively biased toward favorability. To find out for the client, I did some big data* analysis on a dataset of Amazon reviews containing both standard reviews and vine reviews. I then broke the data set down into vine reviews and standard reviews to determine which were more favorable. The results are as follows.

*OK, I used a 1% sample of the big data. The big data was taking too long to load.

## Results

For my analysis, I determined the following, 

the total number of reviews (of those with 50% or more helpful votes)

![total reviews](https://github.com/LiShanDa2021/amazon_vine_analysis/blob/main/total_helpful_reviews.png?raw=true)

the number of 5-star reviews

![total five star reviews](https://github.com/LiShanDa2021/amazon_vine_analysis/blob/main/total_helpful_5_star.png?raw=true)

the percentage of 5-star reviews for vine reviews and. . .
the percentage of 5-star reviews

![percent five star vine and standard](https://github.com/LiShanDa2021/amazon_vine_analysis/blob/main/percent_5star_vine_novine.png?raw=true)

From the above, it appears that Vine reviews are not more likely to be favorable. A slightly lower percentage of Vine reviews were 5-star reviews. However, before I could advise my client against enrolling in the Vine program, I would need to do further analysis. I decided to create summary statistics for the star-ratings columns of the vine reviews and the standard reviews. The results are below.

Vine reviews.

![vine_summary](https://github.com/LiShanDa2021/amazon_vine_analysis/blob/main/yes_vine_summary.png?raw=true)

Standard reviews
![standard_summary](https://github.com/LiShanDa2021/amazon_vine_analysis/blob/main/no_vine_summary.png?raw=true)

## Summary

From the summary statistics, we can see that although a lower-percentage of Vine reviews were 5-star reviews, the mean Vine rating was higher than the mean standard rating indicating that Vine reviews are in fact biased toward favorability. It seems as though Vine reviewers, though less likely to reward 5-star reviews, were reluctant to give negative reviews -- as the differences in first quartiles in the summary statistics suggest. For further analysis, vine reviews and non-vine reviews of the same product should be compared. It may also be useful to incorporate unhelpful reviews since they might be more negative which would affect the comparative percentage of 5-star vine reviews. In any case, it looks like it may be worth enrolling in Vine after all.

