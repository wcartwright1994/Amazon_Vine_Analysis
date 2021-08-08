# Amazon_Vine_Analysis

## Overview of the Analysis

The purpose of this analysis is to determine if reviewers in the Amazon Vine program (paid reviewers) have more favorable reviews towards products than unpaid reviewers. This analysis will be completed on sports products.

## Results

Before performing the analysis, the dataset was cleaned to remove reviews that received less than 20 votes and for helpful reviews. Helpful reviews are defined as reviews with greater than or equal to 50 percent of the total votes being flagged as helpful.

Based on the data as of 8/7/2021:
  * there were 334 total paid reviews and 61,614 total unpaid reviews
  * there were 139 total 5-star paid reviews and 32,665 total 5-star unpaid reviews
  * 42 percent of paid reviews were rated 5 stars
  * 53 percent of unpaid reviews were rated 5 stars

![calc_support](https://user-images.githubusercontent.com/82549092/128620127-81bed6fb-9a1d-4b84-a168-a8a5cd095bd5.PNG)

## Summary

Based on the clean dataset, there does not appear to be positivity bias for reviews from the Vine program. As seen in the results section, there is approximately a 10 bps difference in paid versus unpaid 5 star reviews, with the unpaid reviewers having the higher count. 

Additional analysis that can be performed include:
 * Analyzing the differences in paid versus unpaid average review instead of only looking into 5-star reviews
 * Including reviews that were considered "unhelpful" and excluded from this analysis, especially for the paid reviews
 * Update the code to loop through the different product categories to look for categories with positivity bias
