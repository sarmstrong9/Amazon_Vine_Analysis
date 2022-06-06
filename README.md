# Amazon_Vine_Analysis

analyzing Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

In this project, you’ll have access to approximately 50 datasets. Each one contains reviews of a specific product, from clothing apparel to wireless products. You’ll need to pick one of these datasets and use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, you’ll use PySpark, Pandas, or SQL to determine if there is any bias toward favorable reviews from Vine members in your dataset. Then, you’ll write a summary of the analysis for Jennifer to submit to the SellBy stakeholders.

## Deliverable 1: Perform ETL on Amazon Product Reviews
Using your knowledge of the cloud ETL process, you’ll create an AWS RDS database with tables in pgAdmin, pick a dataset from the Amazon Review datasets (Links to an external site.), and extract the dataset into a DataFrame. You'll transform the DataFrame into four separate DataFrames that match the table schema in pgAdmin. Then, you'll upload the transformed data into the appropriate tables and run queries in pgAdmin to confirm that the data has been uploaded.



PySpark Customers Dataframe</br>
![PySpark Customers Dataframe](results/customers_table_df.png)</br>

PySpark Products Dataframe</br>
![PySpark Products Dataframe](results/products_table_df.png)</br>

PySpark Review ID Dataframe</br>
![PySpark Review ID Dataframe](results/review_id_table_df.png)</br>

PySpark Vine Dataframe</br>
![PySpark Vine Dataframe](results/vine_table_df.png)</br>


![RDS Connection](results/rds_connection.png) </br>
PySpark Customers Table</br>
![PySpark Customers Table](results/customers_table.png)</br>
PySpark Products Table</br>
![PySpark Products Table](results/products_table.png)</br>
[PySpark Review ID Table</br>
![PySpark Review ID Table](results/review_id_table_sql.png)</br>
PySpark Vine Table</br>
![PySpark Vine Table](results/vine_table.png)</br>

## Deliverable 2: Determine Bias of Vine Reviews
Using PySpark, you’ll determine if there is any bias towards reviews that were written as part of the Vine program. For this analysis, you'll determine if having a paid Vine review makes a difference in the percentage of 5-star reviews


Overview of the analysis: Explain the purpose of this analysis.

Results: Using bulleted lists and images of DataFrames as support, address the following questions:

How many Vine reviews and non-Vine reviews were there?
7
105,979
How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
0
67580
What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
0%
63.8%

Summary: In your summary, state if there is any positivity bias for reviews in the Vine program. Use the results of your analysis to support your statement. Then, provide one additional analysis that you could do with the dataset to support your statement.