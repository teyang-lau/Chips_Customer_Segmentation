# **Quantium Chips Sales Customer Analytics**

[![made-with-kaggle](https://img.shields.io/badge/Made%20with-Kaggle-lightblue.svg)](https://www.kaggle.com/)
[![made-with-python](https://img.shields.io/badge/Made%20with-Python-blue.svg)](https://www.python.org/)
[![made-with-Markdown](https://img.shields.io/badge/Made%20with-Markdown-1f425f.svg)](http://commonmark.org)
[![Generic badge](https://img.shields.io/badge/STATUS-COMPLETED-<COLOR>.svg)](https://shields.io/)
[![GitHub license](https://img.shields.io/github/license/teyang-lau/Dog_Breeds_Classification_CNN.svg)](https://github.com/teyang-lau/Neural_Style_Transfer/blob/master/LICENSE)

Author: TeYang, Lau <br>
Last Updated: 26 November 2020

<p align="center">
<img src = './Pictures/chips.jpg'>
</p>

<br>

### **Please refer to this [notebook](https://www.kaggle.com/teyang/quantium-data-preparation-and-customer-analytics) for a more detailed analysis of the project.** ###

### If it takes a long time to load, the [html file](https://github.com/teyang-lau/Chips_Customer_Segmentation/blob/Master/Customer_Segmentation.html) can also be downloaded. 

<br>

## Project Goals ##

1. *Explore* customer transaction data and find interesting insights to chips **purchase behavior**
2. *Identify* **customer segments** that contribute to sales
3. *Investigate* which brand and size customers have **affinity** to 

<br>

## **About this dataset** ##

This data is provided courtesy of [Quantium](https://quantium.com/) via [InsideSherpa's Data Analytics Virtual Experience Program](https://www.insidesherpa.com/virtual-internships/prototype/NkaC7knWtjSbi6aYv/Data%20Analytics%20Virtual%20Experience%20Program). It contains customer segment data as well as customer transaction data on chips purchase.

<br>

## **EDA** ##

Retirees, older and younger singles and couples are the majority of the customer pool while customer classes are quite evenly split, with more mainstreams followed by budget customers.



<img src = './Pictures/demographics.png' width='440'> <img src = './Pictures/customer_distribution.png' width='440'>

<br>

There seems to be an increase in sales during December, possibly due to people stocking up for Christmas. There were also dips around August and May. it appears that **175g** is the most popular size of chips.



<img src = './Pictures/salestime.png' width='450'> <img src = './Pictures/salesbysize.png' width='450'>

<br>

It appears that **Kettle** is the brand that has the highest quantities sold, followed by **Smiths**. **French Fries** and **The Natural Chip Co.** came in last and second last respectively. However, this could be due to some people purchasing more of a certain brand than another brand, which means that having the most quantity sold doesn't mean that it will be the ***most popular\*** among customers. Transactions by brand gives a better idea but it could also be that some people buy lots of a brand in a single transaction.



<img src = './Pictures/salesbybrand.png'>

<br>

Looking at words and bigrams in the product names, a word cloud suggests that **salt** and **cheese** have the most quantities sold and **sour cream** is the most popular bigram.

<img src = './Pictures/keywords.png'>

<br>



## Analyses ##

`Sales Per Unique Customer` plot has a higher sales per segment and this is because their are multiple customers who made multiple transactions in the given year. It seems that `Older Families` and `Young Families` pay the most for chips in the given year.

<img src = './Pictures/salesbycustomers.png'>

<br>

`Mainstream Young Singles/Couples` contributed to the most sales (above), have the largest number of customers (bottom right) but tend to purchase lower quantities of chips (bottom left), perhaps this group can be further targeted for more advertisements/recommendations/promotions on certain brands to encourage more purchase and for purchasing slightly more expensive chip brands.

<img src = './Pictures/quantity.png' width='440'> <img src = './Pictures/unique_customers.png' width='440'>


<br>


## Affinity Analysis ##

Using affinity analysis, `Mainstream Young Singles/Couples` tend to buy more `Tyrrells`, `Twisties`, and `Doritos`, and prefer product sizes of `270g` to `380g`. The store can perhaps place more of these products near the shelves that tend to attract younger and mainstream customers.

<img src = './Pictures/affinity.png'>

<br>

## **Conclusion** ##

* EDA showed that **Kettle** and **Smiths** brand of chips brought in the largest revenue as well as quantities sold
* Products with **Salt** and **Sour Cream** tend to sell the most
* `Mainstream Young Singles/Couples` contributed to one of the highest sales due to their large customer pool but tend to purchase lower quantity of chips, so advertistments/recommendations/promotions can be targeted towards this group to **encourage more purchase**
* `Mainstream Retirees` tend to be the same as `Mainstream Young Singles/Couples`, except that they tend to purchase more chips and slightly cheaper chips. The general strategy would be the same except to **promote cheaper brands** to them.
* `Budget Older Families` also contributed to the most sales, and they tend to buy lots of chips, but there are not as much of them in the customer base. Therefore, the strategy would be to attract more of this segment to **increase the pool size**.
* Market basket analysis **did not provide** any meaningful support/relationship among brands from `Mainstream Young Singles/Couples` customer purchase behavior.
* Affinity analysis suggests that `Mainstream Young Singles/Couples` have affinity towards **Tyrrells** brand and **270g** product size

