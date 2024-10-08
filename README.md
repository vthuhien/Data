## About This Data
Ask a home buyer to describe their dream house, and they probably will begin with the height of the basement ceiling or the proximity to an east-west railroad. 
But this dataset proves that much more influences price negotiations than the number of bedrooms or a white-picket fence.

With 79 explanatory variables describing (almost) every aspect of residential homes in Ames, Iowa, this data challenges you to predict the price of each home.

Data that we download from Kaggle: https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data <br/>

Here is the [Dataset](https://drive.google.com/drive/folders/1JZd7pHYeC-Idl23-w7VEsZS_1xPse9Nq?usp=drive_link) that we're going to analyze.

## Data Overview
### 1. The tip here : we use the heatmap to find the correlation coefficient
![image](https://github.com/user-attachments/assets/12d7f3bf-46a0-4e5b-a41e-1e9ac34add15)


Seeing this chart, we draw conclusion. We have 10 variables, including: 'OverallQual', 'GrLivArea', 'GarageCars','GarageArea', '1stFlrSF','FullBath', 'TotRmsAbvGrd', 'YearBuilt', 'YearRemodAdd', that have a positive correlation relationship with 'SalePrice'. Let's analyze evidently.

### 2. Similarly, we also use the combined chart
![image](https://github.com/user-attachments/assets/fd0db0de-5b6d-4fc6-925a-8c7a8a80ab09)
![image](https://github.com/user-attachments/assets/e504fbf7-a54d-4727-967e-f20240081fb2)
![image](https://github.com/user-attachments/assets/ec2df3b1-3f99-4b3a-9064-3367db065493)

According to the combined chart, the 'SalePrice' almost ranges from 1 thousand to more than 2 thousand. 
Besides, we realize that the 'SalePrice' relies on conditions about the property, such as: overall material, living area, garage area with car capacity, number of rooms and construction year.

## Variable Relationships 
### 1. Relationship with numeric variates
![image](https://github.com/user-attachments/assets/a7a0507f-9207-4a57-a24d-dbd883c9cda3)


Through the chart, we can see a positive correlation between 'GrLivArea' and 'SalePrice' that is 0.7086. It suggests that the sale price will increase in proportion to the living area.</br>
We see 2 points that have a large living area, but they didn't sell at a high price. These are the outliers that need to be resolved.

![image](https://github.com/user-attachments/assets/bb6a8902-9834-48b5-9f07-e33c8e711501)

The chart indicates that the property will be sold at a high price if it has four to ten rooms. This illustrates how difficult it will be to sell a propety with either few rooms or too many rooms.

### 2. Relationship with categorical variates.
![image](https://github.com/user-attachments/assets/3dfa422d-99d1-403a-9bad-196a4eef8782)

The primary takeaway from the chart is that a property with a lot of positive evaluations will be sold for a high price. With the property's evaluations being 9 or 10, the price ranges from nearly 2 thousand to more 6 thousand but it has some outlier prices.

![image](https://github.com/user-attachments/assets/5c79f8ec-aa60-42d0-86a2-415b573b830d)

As we can see, the mean sale price with condition material is nearly 2 thousand. It will have high prices and some outlier prices if the house has good, average, or typical material.

## Summary

After we compare the 'SalePrice' with some variates, we can indicate that :
 * Both relationships are positive, which means that one variate increases, the other also increases. In the case 'GrLivArea', we see the value of correlation coefficient is 0.708, so it returns that the slope of linear relationships is quite high and clear.
 * The other variates also seem to be related with 'SalePrice'. The relationship is showed clearly by the box plot. This suggest that how the sale price increase with overall quality.
 * We just compared some variates that we thought, because this data also has a lot of variates that needed to be analyzed.

