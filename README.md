# Amazon_Vine_Analysis
![](Images/stars.PNG)

## Analysis Overview
![](Resources/Images/MechaCar_mpg.PNG)
<br>
We are tasked with analyzing Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.
<br>
For this project we will be analyzing reviews from the outdoor product category. We will use PySpark to perform the ETL process and to determine if there is any bias toward favorable reviews from vine members in our dataset.  

## Analysis Results
### Paid Vine Rating Summary
Table:<br>
![](Images/paid.PNG)<br>
Summary:<br>
![](Images/paid_summary.PNG)<br>
- There were a total of 107 paid vine reviews.
- 56 of the vine reviews were given 5-stars.
- 52.34% of paid reviews were 5-stars.
<br>

### Unpaid Vine Rating Summary
Table:<br>
![](Images/unpaid.PNG)<br>
Summary:<br>
![](Images/unpaid_summary.PNG)<br>
- There were a total of 39768 unpaid reviews.
- 20990 of the unpaid reviews were given 5-stars.
- 52.78% of unpaid reviews were 5-stars.
<br>

## Analysis Summary
Based on our analysis results there is no evidence of positivity bias for the reviews in the Vine program, in fact vine reviewers proportionately gave slighly less 5-star reviews than the unpaid reviewers. 

To get a more complete picture of potential positivity bias we could do the following:
- From our vine_unpaid_df we should filter out reviews on products that do not have at least one Vine rating, this would help make the populations more alike. 
- Using R perform a statistical summary of the two populations. 
<br>
