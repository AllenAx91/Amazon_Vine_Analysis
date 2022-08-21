# Amazon_Vine_Analysis ☁️

## 1: Overview

The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review. Using PySpark, Pandas this project attempts to determine if there is any bias toward favorable reviews from Vine members in the dataset for Video Games. The dataset list can be found in this [link](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt).

## 2: Results

### 2.1: Vine reviews 🆚 non-Vine reviews

From the original data set, only rows with helpful votes equal to or greater than 50% of the total were chosen. From this new and cleaned data set, only **94** out of **40565** had Vine reviews. The majority of the population (**40471**) comprises of non-Vine reviews. 

### 2.2: '5 ⭐' Reviews

Interestingly, our analysis shows that **51.1%** of the Vine reviews are 5 stars in comparison to **38.7%** of the non-Vine reviews. 

## 3: Summary

It is clear from our analysis that there is a positivity bias for reviews in the Vine program. 

| ![](https://github.com/AllenAx91/Amazon_Vine_Analysis/blob/main/Images/Vine.png) | 
|:--:| 
| *Split of Vine reviews. Total: 94* |

| ![](https://github.com/AllenAx91/Amazon_Vine_Analysis/blob/main/Images/Non-Vine.png) | 
|:--:| 
| *Split of non-Vine reviews. Total: 40471* |

Consider the above tables and the totals we are already aware of. We can see a trend of bias in reporting positive reviews by Vine members. However, we can validate this hypothesis by expanding the data set. We can first consider all the rows from the original data set (removing the 50% helpful votes criteria). In addition, we can test this hypothesis on other data sets (other products listed in the [link](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt)). 
