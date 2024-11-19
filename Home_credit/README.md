CÁI NÀY MÌNH CODE QUÊN KHÔGN COMMIT NÊN NÓ MẤT ĐOẠN CODE DƯỚI CAY VĐ NAO MÌNH CODE LẠI HA 🙂
## About Data
https://www.kaggle.com/competitions/home-credit-default-risk/data </br>
Many people struggle to get loans due to insufficient or non-existent credit histories. And, unfortunately, this population is often taken advantage of by untrustworthy lenders.

Home Credit Group

Home Credit strives to broaden financial inclusion for the unbanked population by providing a positive and safe borrowing experience. In order to make sure this underserved population has a positive loan experience, Home Credit makes use of a variety of alternative data--including telco and transactional information--to predict their clients' repayment abilities.

While Home Credit is currently using various statistical and machine learning methods to make these predictions, they're challenging Kagglers to help them unlock the full potential of their data. Doing so will ensure that clients capable of repayment are not rejected and that loans are given with a principal, maturity, and repayment calendar that will empower their clients to be successful.

* I coded directly in Github. The data files are too large so I can't put them into the Git space. So, the raw data is [here](https://drive.google.com/drive/folders/1BMby6ZnQbWOBw-LVZIwXhdHSXgHiLzVw?usp=drive_link)

## Correlate relationship between `TARGET` and the other variables
### 1. `Target` distribution 
![image](https://github.com/user-attachments/assets/12e6a101-4680-469b-ab4c-151dbe78cd76)
From this chart, we draw the conclusion that almost all the clients paid the loans in time but still have some customers in value of 1 who have trouble with making payment or late time. The customers with value of 1 just account for 10 percents of all transactions. Since we get into deeper with machine learning models, we can weight the classes by their representations in the data to reflect this imbalance

### 2. Relationships between variables
![image](https://github.com/user-attachments/assets/58c69313-fc2f-4c37-af4c-43fb4ae6006f)
As we see, the value of the other variables is too small to have a correlation relationship with the `target` variable. This chart shows almost all variables only have values from 0.01 to 0.07, and the others have negative values. In this case, we only see 28 variables relates to the variable needs to be analyzed. </br>

## Visualization 
  In this, we will analyze them one by one, starting at `DAYS_BIRTH`, continuing on `REGION_RATING_CLIENT_W_CITY`, ending at `REGION_RATING_CLIEN`
### a. `DAYS_BIRTH`
![image](https://github.com/user-attachments/assets/86fedf29-58ae-4572-9f17-6aaa584405f6)
![image](https://github.com/user-attachments/assets/49e65ac6-fe22-4f60-b427-8866ce643bcc) </br>
As we see, In line of `target = 0`, which means the customers who repaid the loans in time have an even distribution density across age groups. However, in line of `target = 1`, which means the client with payment difficulties that is highest in range from the age of 25 to 40 and eases towards 50 to 70. Then, we can point out that older customers are more likely to pay loans well than young customers. With younger customers, they tend to have difficulty in debt repayment because they have many problems to solve but are not yet stable in their jobs, so it forms weak finances.

![image](https://github.com/user-attachments/assets/5220913a-3c3f-4831-8168-4f3477d19eba)</br>
The chart return the results that show the percentage of clients who repaid loans late over each age groups. The column from the age of 20 to 25 has about more 12% the number of people have difficulty in paying debt. But, the density starts decreasing towards the right and it only has 4% in last column. Through this chart, we see an inverse correlation between date of birth and debt repayment ability. So, we are more certain about our judgment.  

### b. `REGION_RATING_CLIENT_W_CITY` : Our rating of the region where client lives with taking city into account (1,2,3) `REGION_RATING_CLIENT` : Our rating of the region where client lives (1,2,3)
![image](https://github.com/user-attachments/assets/02a7a296-e962-4ff7-9ecb-f38d377be0c4)




