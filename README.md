# Amazon_Vine_Analysis
ETL and meta-analysis of Amazon Vine reviews with AWS, postgresql, PySpark, and Google Colab

# Overview
The overarching purpose of this project was to conduct a meta-analysis of Amazon reviews. Specifically it was to analyze reviews produced as part of the Amazon Vine program, where select members of Amazon's reviewer community are compensated to review sample products. The primary goal of this inquiry is to determine if there is any bias towards favorable reviews from the paid Vine members in the available data.

Out of the 50 datasets of product categories available to chose from, I chose to analyze reviews in the Camera category - high-value, technical products requiring experience and knowledge to effectively review. The initial ETL portion of the project was conducted, as proscribed, using AWS, postgresql, and PySpark in Google Colab. The data analysis segment was conducted using PySpark and Google Colab.

# Results
To begin with, I filtered the available reviews to just those with more than 20 votes, and those which were more than 50% "helpful." 
![image](https://user-images.githubusercontent.com/95143562/165007547-2404e994-fd16-471d-a8b1-586399a2e08e.png)
Calculations were made from this filtered dataset. Results were as follows:
![image](https://user-images.githubusercontent.com/95143562/165007586-cdc0c0ed-aa94-43c6-8624-32d366ddf7ab.png)
* Out of a total of 51,123 reviews in the dataset, 50,516 (98.81%) were unpaid and 607 (1.19%) were paid reviews.
![image](https://user-images.githubusercontent.com/95143562/165007630-12b651e7-4bf8-4554-b924-c324952f9470.png)
* Out of a total of 25,473 five-star reviews, 25,300 (99.32%) were unpaid, while only 257 (1.01%) were paid.
![image](https://user-images.githubusercontent.com/95143562/165007725-ee84f4b7-5dc7-449a-ae41-968269cbed7b.png)
* Out of 607 total paid/Vine reviews, 257 (42.3%) were 5-star reviews.
![image](https://user-images.githubusercontent.com/95143562/165007768-c3719911-764f-4582-9b18-6051d954f62b.png)
* Out of 607 total paid/Vine reviews, 257 (42.3%) were 5-star reviews.
![image](https://user-images.githubusercontent.com/95143562/165007829-d6eae4c9-abe7-45e1-aff8-28a3e8c7a3e8.png)
* Out of 50,516 unpaid reviews, 25,300 (50.08%) were 5-star reviews.

# Summary
What these numbers seems to suggest is that there is not strong bias toward five-star reviews from paid Amazon Vine reviewers. If anything, Vine reviews might show a tendency towards being more critical in their reviews. This conclusion could be further examined by looking at the distribution of all star-levels across paid and unpaid reviews. Also, for a more thorough analysis, this same meta-analysis should be conducted across a few different product catagories.
