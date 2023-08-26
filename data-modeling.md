# Data Warehouse - Dimensional Modeling of Orders Data with dbt

## 1. Approach
To enable the analytics team to continue finding insights in what books their customers are ordering, we will build an ETL pipeline that extracts their data from Postgres, stages them in BigQuery, and transforms data into a set of dimensional tables. The orders data was modeled using a star schema, with `order_lines` as a central fact table and `books`, `authors`, `customers` and `time` as dimension tables optimized for queries on order analysis. The resulting database supports optimized fast queries about customers, the books they buy, and the time periods when they visit the ecommerce site.

## 2. Schema for Orders Data

Please see a description of the sample bookstore dataset we are using [here](https://www.databasestar.com/sample-bookstore-database/). The webpage gives you descriptions of the tables and the database diagram. This dataset mimics the normalized data models you will encounter in production. 


## 3. Target Star Schema

You will transform the data into a star schema with one fact table and several dimensions enriching the dataset. You can read more about fact tables [here](https://www.holistics.io/blog/the-three-types-of-fact-tables/)

### Fact Table
1. **order_lines** - records in database associated with individual book orders <br>
*order_id*, *order_date*, *customer_id*, *price*, *book_id*, *author_id* 

### Dimension Tables
2. **customers** - customers of the website <br>
*user_id*, *first_name*, *last_name*, *email*, *country*
4. **books** - books sold <br>
*book_id*, *title*, *author_id*, *year*, *publisher*, *num_pages*
5. **authors** - authors of the books <br>
*author_id*, *name*
6. **time** - timestamps of records in orders table broken down into specific units <br>
*order_date*, *hour*, *day*, *week*, *month*, *year*, *weekday*
