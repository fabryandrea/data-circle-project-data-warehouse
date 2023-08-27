---
layout: post
title: Data Warehouse
subtitle: Replicate, transform, and analyze data about book sales and orders
categories: Data-Circle
tags: [data-circle] 
---



## 1. Introduction
- What is the project content about? 
You will replicate, transform, and analyze data about book sales and orders.
- What is the problem we are solving with the project?
Data warehouses are the backbone of company analytics. This project will familiarize you with the design and architecture of data warehouses. If you are interested in a data analyst, analytics engineer, or data engineer role, this project will give you an introduction to how these roles interact with data in production.

## 2. Project Brief 
- How is the student going to work on the project?
You will collaborate with others delivering different parts of the same project.
- What is the major challenge of the project?
You will implement a data pipeline and a star schema data model, then use it for dashboards.


## 3. Learning Objective
List the components / frameworks which the student is going to use / learn. Example below:

- [x] concepts: data warehouses, Extract-Transform-Load, data modeling
- [x] BigQuery - massively parallel processing (MPP) data warehouse
- [x] airbyte - ETL tool
- [x] dbt - transformation tool
- [x] Metabase - BI tool


## 4. Minimum Acceptance Criteria
What are the minimum criteria which the project should meet to be considered "done"? 
- [ ] Users are able to query data from Metabase
- [ ] Users are able to view a dashboard about book sales/orders

## 5. Optional Challenges
Add a few extra challenges for the more ambitious students. 
* Create additional fact table: `orders` that summarizes all order line items and adds shipping costs. Users can analyze sales and shipping.
* Create additional dimensional tables: `publishers` and `languages`. Users can analyze sales per publisher and languages.
* Create additional fact tables: `order_fulfillment`. Users can analyze orders by status.

## 6. Technical Setup
How can the student get started with the project? Example: 
1. Fork the repo.
2. Setup [Bigquery](https://cloud.google.com/bigquery) or [Postgres](https://hub.docker.com/_/postgres). Postgres can be used via docker, or the free variant [podman](https://podman.io/).
3. Pick a dataset, options: [kaggle](https://www.kaggle.com/) where we recommend ecommerce datasets,or [bookstore dataset](https://www.databasestar.com/sample-bookstore-database/).
4. Perform data analysis, as mentioned in Optional Challenges.
5. Try to ingest the data using Airbyte or try using pandas,polars,Apache Spark (Databricks) to ingest data.

## 7. Resources / Hints & Tips
- (free book) The Analytics Setup Guidebook from Holistics.io: https://www.holistics.io/books/setup-analytics/start-here-introduction/
- (free course) dbt Fundamentals Course from dbt Labs: https://courses.getdbt.com/courses/fundamentals
- (blog series) Three-Part Data Modeling Series from airbyte: 
https://airbyte.com/blog/data-modeling-unsung-hero-data-engineering-introduction
https://airbyte.com/blog/data-modeling-unsung-hero-data-engineering-approaches-and-techniques 
https://airbyte.com/blog/data-modeling-unsung-hero-data-engineering-architecture-pattern-tools 
