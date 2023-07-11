# KPMG_-SPROCKET-CENTRAL

<img width="372" alt="Screenshot 2023-07-11 102725" src="https://github.com/Olauryn/KPMG_-SPROCKET-CENTRAL/assets/118401566/ad3efd16-687f-447f-b1f5-9858fb3c9efc">

## BACKGROUND INFORMATION OF THE TASK

**Sprocket Central Pty Ltd** is a medium size bikes & cycling accessories organisation, and has approached KPMG’s Lighthouse & Innovation Team. Sprocket Central Pty Ltd  is keen to learn more about KPMG’s expertise in its Analytics, Information & Modelling team. 

Sprocket Central Pty Ltd wants the team to effectively analyse it's datasets to help them grow its business.

Primarily, Sprocket Central Pty Ltd needs help with its customer and transactions data. The organisation has a large dataset relating to its customers, but their team is unsure how to effectively analyse it to help optimise resource allocation for targeted marketing. Hence, improve performance by focusing on high value customers.

However, in order to support the analysis, it was advised that **“the importance of optimising the quality of a customer's datasets cannot be underestimated. The better the quality of the dataset, the better chance one will be able to use it drive company growth.”**

The client provided KPMG with 3 datasets:

Customer Demographic 

Customer Addresses

Transactions data in the past 3 months

following the advise, **preliminary data exploration was done and ways to improve the quality of Sprocket Central Pty Ltd’s data was identfied.**

In order to achieve the goal the goals of the analysis, I carried out three processes to achieve this; **Data Exploration, Model Development and Results Interpretation**

### TOOLS USED FOR ANALYSIS
Python, Microsoft Excel, Power BI

## DATA EXPLORATION

Sprocket Central Pty Ltd has asked the team to assess the quality of their data; as well as make recommendations on ways to clean the underlying data for better analytical proccess and mitigate current data quality concerns going forward.

The dataset received contained four (4) tables; **Transaction**, **NewCustomerList**, **CustomerDemographic**, **CustomerAddress**. Careful exploratory analysis was done for each of the tables and the following results were obtained. 

### TRANSACTION TABLE
The Transaction table contained a total of 13 columns, and 2000 rows. 

**transaction_id**: This column contained 20000 distinct values and 20000 unique values. Duplicate and null values are not allowed because of the structure of the database. 

**Product_id**: There was no Null values in the column and the column contains 3494 distinct values and 49 unique values.  All positive values. 

**Transaction_date**: This column contained no Null values. 

**Order_online**: This column contains three distinct values; “True”, “False”, “Null”, but this column is ought to contain just two distinct values of True and False. The total number of Null values in this column was “360”. 

**Order_status**: This column contained 2 distinct values “Approved” and “Cancelled”. There was no Null values in this column. 

**Brand**: This column 7 has distinct values and 0 unique and contained 197 Null values. 

**Product_line**: This column contains 5 distinct values of which one of the distinct values is null. The total number of null values was 197. 

**Product_size**: Total number of null values is 197 and has 4 distinct values. 

**List_price**: 

**Standard_cost**: Total number of null values is 197.

**Product_first_sold_date**: Total number of null values is 197.

### CUSTOMER ADDRESS TABLE

The customerAddress table contained a total of 3999 rows and 6 columns. 

**Customer_id**: This column contains 3999 distinct values., no duplicates and Null values. 

**Address**: This column contains 3996 distinct values and 3993 unique values. No null values. 

**Post_code**: This column contains 873 distinct values and 229 unique values with no null values. 

**State**: This column contains 5 distinct values, but this column is supposed to contain 3 distinct values; **NSW, QLD,  VIC**. The other 2 distinct values were New South Wales and Victoria, but this column is contain state names in it’s abbreviated format. Hence the **86 rows containing New South Wales was changed to NSW, the 82 rows containing Victoria was changed to VIC**. 

**Country**: This column contains just one distinct value which is Australia. 

**Property_Valuation**: This column contains a total of 12 distinct positive values, with no null values. 

### CUSTOMER DEMOGRAPHIC TABLE 
The customer demograpic table contained a total of 2841 rows and 12 columns. 

**Customer_id**: This column contains a total of 2841 distinct values with no duplicates and null values. 

**First_name**: This column contains 2396 distinct values and 1997 unique values with no null values. 

**Last_name**: This column contains 2768 distinct values and 2696 unique values with no null values. 

**Gender**: This column contains three distinct values; Male, Female and U with no null values. 

**Past_3_years_bike_related_purchased**: This column contains 100 distinct values with no duplicate. 

**DOB**: This column contains 87 null values and 3913 number of records. 

**Job_title**: This column contains 196 distinct values and 506 null values. 

**Job_industry_category**: This column contains 10 distinct values with no Null values. 

**Wealth_segment**: This column contains 3 distinct values and no Null values. 

**Diseased_indicator**: This column contains 2 distinct values with no null values. 

**Own_car**: This column contains 2 distinct values with no null values. 

**Tenure**: This column contains 23 distinct values with 87 null values. 

### NEW CUSTOMER DEMOGRAPHIC LIST

The new customer demographic table contains 1000 rows and 23 columns. 

**First_name**: This column contains 940 distinct values and 883 unique values with no null values. 

**Last_name**: This column contains 962 distinct values and 951 unique values with 29 null values. 

**Gender**: This column contains 3 distinct values and no null values. 

**Past_3_years_bike_related_purchases**: This column contains 100 distinct values with no duplicate. 

**DOB**: This column contains 959 distinct values and 933 unique values with 17 null values. 

**Job_title**: This column contains 15 distinct values and 14 unique values with 106 null values. 

**Job_industry_category**: This column contains 3 distinct values and 2 unique values with no null values. 

**Wealth_segment**: This column contains 3 distinct values with no null values. 

**Diseased_indicator**: This column contains 1 distinct value with no null values. 

**Owns_car**: This column contains 2 distinct values with no null values. 

**Tenure**: This column contains 23 distinct positive values with no null values

**Address**: This column contains 1000 distinct and unique values with no null values. 

**Postcode**: This column contains 522 distinct values and 281 unique values with no null values. 

**State**: This column contains 3 distinct values with no null values. 

**Country**: This column contains just 1 distinct value named Australia.

**Property_valuation**:  This column contains 12 distinct values with no null values. 

## MODEL DEVELOPMENT 
The following steps were what I used in carrying out the model development; 

**Developed a predictive model** by building a machine learning model to predict customer behavior and identify potential high-value customers.

**Performed feature engineering** by transforming and creating new features to improve model performance.

**Model selection and training** by choosing an appropriate algorithm and train the model using the labeled dataset.


## RESULT INTERPRETATION (DATA VISUALIZATION)

<img width="829" alt="Screenshot 2023-07-11 102129" src="https://github.com/Olauryn/KPMG_-SPROCKET-CENTRAL/assets/118401566/8626d56b-aafd-4495-80d7-dfa71b15feb7">

My findings answers the following questions;

What are the trends in the underlying data?

Which customer segment has the highest customer value?

What I propose should be Sprocket Central Pty Ltd ’s marketing and growth strategy?

What additional external datasets may be useful to obtain greater insights into customer preferences and propensity to purchase the products?

And specifically who Sprocket Central Pty Ltd’s marketing team should be targeting out of the new 1000 customer list as well as the broader market segment to reach out to. 







