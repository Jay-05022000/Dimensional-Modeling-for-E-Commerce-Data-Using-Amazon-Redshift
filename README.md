# Dimensional Modeling for E-Commerce Data Using Amazon Redshift

Aim:

The purpose of this project is to perform dimensional modeling for the popular ‘Instacart Market Basket Analysis’ dataset available on Kaggle. This approach simplifies complex data structures, enhances data retrieval speed, and supports efficient analysis by organizing data into fact and dimension tables, facilitating better decision-making and insights through easier data navigation and interpretation.


Dataset:

You can find the dataset used for this project here: https://www.kaggle.com/c/instacart-market-basket-analysis


Technical Stack:

1) AWS S3: To store the dataset in its raw format (CSV files).
2) AWS Redshift: Data Warehouse to perform dimensional modeling.
3) SQL: To query data in Redshift.


Workflow:

1) Set up an S3 bucket to store the dataset as CSV files.
2) Establish a database within the Redshift data warehouse.
3) Define tables in the Redshift database based on the CSV files and load the data into these tables using the Redshift GUI or Query Editor.
4) Create and populate fact and dimension tables according to the star schema design.
5) Use SQL queries on the fact and dimension tables to extract meaningful insights from the data.


Star Schema for Dimensional Modeling:

![E-R Diagram](https://github.com/user-attachments/assets/c096d4d1-0ffc-417b-b579-1dcfff6a651e)


Generated Insights:

After performing dimensional modeling, the following questions were answered using SQL queries on the created tables:

1) What is the total number of products ordered per department?
2) Which are the top 5 aisles with the highest number of reordered products?
3) What is the average number of products added to the cart per order by day of the week?
4) Who are the top 10 users with the highest number of unique products ordered?


Conclusion:

This project demonstrates the power of dimensional modeling in simplifying complex datasets and enhancing data analysis capabilities. By organizing the Instacart dataset into a star schema, we can efficiently query and gain insights into consumer behavior and product trends, ultimately supporting better business decisions.


How to Run:

1) Clone this repository.
2) Set up an AWS S3 bucket and upload the dataset CSV files.
3) Create a Redshift cluster and establish a database.
4) Use the provided SQL scripts to create tables and load data into Redshift.
5) Execute the example queries to explore the insights generated from the data.
