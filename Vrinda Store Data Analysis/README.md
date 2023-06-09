<img width="917" alt="image" src="https://github.com/jayantjy9/Excel/assets/118092998/40124c0f-9fec-481e-994a-d7b449fd1f5e">


# Vrinda Store Annual Sales Report

This repository contains the Annual Sales Report for a store, presented in an Excel format. The report provides valuable insights derived from thorough data analysis, aiming to enhance the store's sales growth and drive strategic decision-making.



## Data Cleaning Steps

To ensure the accuracy and reliability of the data for analysis, the following cleaning steps were performed:

1. **Changes in Gender**: Inconsistent gender entries such as "M" and "W" were standardized to "Men" and "Women" respectively.

2. **Changes in Quantity**: The quantity entries were standardized, with "one" changed to "1" and "two" changed to "2".

3. **Added "Age Group" Column**: A new column named "Age Group" was added, calculated using the formula:
```
=IF(E2>60,"60+",IF(E2>=50,"50-60",IF(E2>=40,"40-50",IF(E2>=30,"30-40",IF(E2>=18,"18-30","default")))))
```
This formula categorizes the customers into different age groups based on their age.

4. **Added "Month" Column**: A new column named "Month" was added, calculated using the formula:
```
=TEXT(G2,"mmm")
```
This formula extracts the month from the date of sales, providing a clear overview of sales distribution by month.

5. **Added "Weekday" Column**: A new column named "Weekday" was added, calculated using the formula:
```
=TEXT(G2,"ddd")
```
This formula extracts the weekday from the date of sales, allowing us to analyze sales patterns by the day of the week.

6. **Added "Count_of_unique_CustID" Column**: A new column named "Count_of_unique_CustID" was added, calculated using the formula:
```
=COUNTIF(C:C,C2)
```
This formula counts the number of unique Customer IDs, enabling us to identify repeat customers.

7. **Added "Repeat Customer" Column**: A new column named "Repeat Customer" was added, calculated using the formula:
```
=IF(D2=1,"No","Yes")
```
This formula categorizes customers as "No" if they made a single purchase and "Yes" if they made multiple purchases, indicating repeat customers.


## Report Insights


The report reveals several key insights that can guide business strategies:

1. **B2B Business:** B2B accounts for only 1% of business, highlighting the opportunity to explore and expand in this segment.

2. **Repeat Customers:** 15% of customers are loyal, repeat customers, a testament to the exceptional experience offered.

3. **Monthly Sales:** March emerged as the highest-grossing month, indicating a potential seasonal trend for sales.

4. **Weekday Analysis:** "Tuesday" was found to have generated the maximum number of orders and sales on average across the analyzed period.

5. **Channel-wise Sales:** Amazon was the leading sales channel, contributing to 36% of total sales, followed by Myntra (23%) and Flipkart (22%).

6. **Customer Age and Gender:** Women between the ages of 18 and 50 accounted for approximately 56% of total orders, making them a crucial target segment.

7. **Sales by Location:** Bengaluru topped the sales chart, followed by Hyderabad, New Delhi, Chennai, and Mumbai.

8. **Size-based Sales:** Medium and Large sizes had the highest sales figures, representing 17.81% and 16.27% respectively.

## Additional Information:

- The report includes two filters for further analysis: "Category" and "State". These filters allow users to explore data insights at a granular level, specific to each category or state.


## Author

- [@jayant_yadav](https://www.github.com/jayantjy9)

