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
1. Fork boilerplate repo
2. Set up the project with version control (e.g. Git)
3. Read the README.md file and have a look around the project
4. Get colors, fonts etc from the style-guide.md file
5. Set up your project/file architecture however you want
6. Start coding!

## 7. Resources / Hints & Tips
- (free book) The Analytics Setup Guidebook from Holistics.io: https://www.holistics.io/books/setup-analytics/start-here-introduction/
- (free course) dbt Fundamentals Course from dbt Labs: https://courses.getdbt.com/courses/fundamentals
- (blog series) Three-Part Data Modeling Series from airbyte: 
https://airbyte.com/blog/data-modeling-unsung-hero-data-engineering-introduction
https://airbyte.com/blog/data-modeling-unsung-hero-data-engineering-approaches-and-techniques 
https://airbyte.com/blog/data-modeling-unsung-hero-data-engineering-architecture-pattern-tools 

## 8. Glossary
- **[Airbyte](https://airbyte.io/)**: An open-source data integration platform that extracts and loads data from various sources.
  <details>
  <summary> Learning Resources</summary>

    - **[Airbyte Documentation](https://docs.airbyte.io/)**
    - **[Set up a modern data stack with Docker and Airbyte](https://airbyte.com/tutorials/modern-data-stack-docker)**

    - **[Getting Started with Airbyte Guide](https://docs.airbyte.com/quickstart/getting-started/)**

    - **[Airbyte YouTube Channel](https://www.youtube.com/@AirbyteHQ)**

    - **[Airbyte Community](https://airbyte.io/community)**

    - **[Airbyte on GitHub](https://github.com/airbytehq/airbyte)**
    - **[Data Modelling in Airbyte](https://airbyte.com/blog/data-modeling-unsung-hero-data-engineering-introduction)**

  </details>

- **[Airflow](https://airflow.apache.org/)**: A platform to programmatically author, schedule, and monitor workflows.
  <details>
  <summary> Learning Resources</summary>

    - **[Airflow Documentation](https://airflow.apache.org/docs/stable/index.html)**

    - **[Principles of Airflow on GitHub](https://github.com/apache/airflow/blob/main/README.md)**

    - **[Airflow YouTube Videos](https://www.youtube.com/results?search_query=apache+airflow+)**

    - **[Airflow Community and Mailing lists](https://airflow.apache.org/community/)**

  </details>

- **BI (Business Intelligence)**: A technology-driven process for analyzing data and presenting actionable information to help executives, managers and other corporate end users make informed business decisions.
  <details>
  <summary> Learning Resources</summary>

    - **[Business Intelligence on Wikipedia](https://en.wikipedia.org/wiki/Business_intelligence)**

    - **[Foundations of Business Intelligence on Coursera](https://www.coursera.org/learn/foundations-of-business-intelligence)**

    - **[IBM introduction on Business Intelligence](https://www.linkedin.com/learning/topics/business-intelligence)**

  </details>

- **[BigQuery](https://cloud.google.com/bigquery)**: A web service from Google that is used for handling and analyzing big data.
  <details>
  <summary> Learning Resources</summary>

    - **[BigQuery Official Documentation](https://cloud.google.com/bigquery/docs)**

    - **[BigQuery Quickstart Guides](https://cloud.google.com/bigquery/docs/quickstarts)**

    - **[BigQuery Guided Project on Coursera](https://www.coursera.org/projects/working-with-bigquery)**

  </details>

- **Data Modelling**: The process of creating a data model for an information system by applying certain formal techniques.
  <details>
  <summary> Learning Resources</summary>

    - **[Data Modelling on Airbyte Blog, part 1 - Introduction](https://airbyte.com/blog/data-modeling-unsung-hero-data-engineering-introduction)**

    - **[Data Modelling on Airbyte Blog, part 2 - Approaches and Techniques](https://airbyte.com/blog/data-modeling-unsung-hero-data-engineering-approaches-and-techniques)**

    - **[Data Modelling on Airbyte Blog, part 3 - Architecture Pattern, Tools](https://airbyte.com/blog/data-modeling-unsung-hero-data-engineering-architecture-pattern-tools)**

  </details>

- **Data Stack**: A collection of software tools, platforms, and languages to systematically manage and perform tasks with large sets of data.
  <details>
  <summary> Learning Resources</summary>

    - **[A bit more on Modern Data Stack](https://www.altexsoft.com/blog/modern-data-stack/)**

  </details>

- **Data Warehouse**: A technology that aggregates structured data from one or more sources so that it can be compared and analyzed for greater business intelligence.
  <details>
  <summary> Learning Resources</summary>

    - **[A book on Data Warehouse concepts and Analytics Setup in general](https://www.holistics.io/books/setup-analytics/start-here-introduction/)**

    - **[IBM introduction to Data Warehouse Concept](https://www.ibm.com/topics/data-warehouse)**

    - **[Data Warehouse on Wikipedia](https://en.wikipedia.org/wiki/Data_warehouse)**

      </details>

    - **Database Normalization**: The process of structuring a relational database in accordance with a series of so-called normal forms in order to reduce data redundancy and improve data integrity.
      <details>
      <summary> Learning Resources</summary>

        - **[Database Normalization on Wikipedia](https://en.wikipedia.org/wiki/Database_normalization)**

        - **[Database Normalization on GeeksforGeeks](https://www.geeksforgeeks.org/normal-forms-in-dbms/)**

      </details>

    - **[DBT (Data Build Tool)](https://www.getdbt.com/)**: A tool that allows data analysts and engineers to transform data in their warehouses by simply writing select statements.
      <details>
      <summary> Learning Resources</summary>

        - **[DBT Documentation](https://docs.getdbt.com/docs/introduction)**

        - **[DBT Tutorials](https://www.getdbt.com/dbt-learn/)**
        - **[The tutorial on dbt fundamentals](https://courses.getdbt.com/courses/fundamentals)**

      </details>

    - **[Docker](https://www.docker.com/)**: An open-source platform that automates the deployment, scaling, and management of applications.
      <details>
      <summary> Learning Resources</summary>

        - **[Docker Official Documentation](https://docs.docker.com/get-started/overview/)**

        - **[Docker Get Started Guide](https://docs.docker.com/get-started/)**

        - **[Docker Tutorials](https://www.tutorialspoint.com/docker/index.htm)**

      </details>

    - **[Docker-compose](https://docs.docker.com/compose/)**: A tool for defining and managing multi-container Docker applications.
      <details>
      <summary> Learning Resources</summary>

        - **[Getting Started guide](https://docs.docker.com/compose/gettingstarted/)**

      </details>

    - **ETL (Extract, Transform, Load)**: The process of extracting data from outside sources, transforming it to fit operational needs, then loading it into the end target.
      <details>
      <summary> Learning Resources</summary>

        - **[ETL explaind by AWS](https://aws.amazon.com/what-is/etl/)**

        - **More details at [Wikipedia](https://en.wikipedia.org/wiki/Extract,_transform,_load)**

      </details>

    - **[GCP (Google Cloud Platform)](https://cloud.google.com/)**: A suite of cloud computing services that runs on the same infrastructure that Google uses internally for its end-user products.
      <details>
      <summary> Learning Resources</summary>

        - **[BigQuery and GCP tutorial](https://www.cloudskillsboost.google/quests/68)**

      </details>

    - **[Metabase](https://www.metabase.com/)**: An open-source business intelligence tool that lets you ask questions about your data, and displays answers in formats that make sense, either as a chart, dashboard, or detailed data table.
      <details>
      <summary> Learning Resources</summary>

        - **[Metabase Documentation](https://www.metabase.com/docs/latest/)**

        - **[Metabase Tutorials](https://www.metabase.com/learn/)**

      </details>

    - **[pgAdmin](https://www.pgadmin.org/)**: An open-source, full-featured and web-based PostgreSQL management tool.
      <details>
      <summary> Learning Resources</summary>

        - **[pgAdmin Documentation](https://www.pgadmin.org/docs/)**

      </details>

    - **[Postgres](https://www.postgresql.org/)**: An open-source, object-relational database system that uses and extends the SQL language combined with many features that safely store and scale the most complicated data workloads.
      <details>
      <summary> Learning Resources</summary>

        - **[Postgres Official Documentation](https://www.postgresql.org/docs/)**

        - **[Getting Started with PostgreSQL Tutorial](https://www.postgresqltutorial.com/postgresql-getting-started/)**

      </details>

    - **Star Schema**: A relational database schema for representing multidimensional data.
      <details>
      <summary> Learning Resources</summary>

        - **[Star Schema on Wikipedia](https://en.wikipedia.org/wiki/Star_schema)**

        - **[Star Schema on GeeksforGeeks](https://www.geeksforgeeks.org/star-schema-in-data-warehouse-modeling/)**

      </details>
    - **[Superset](https://superset.apache.org/)**: An open-source data exploration and visualization platform designed to be intuitive and interactive.
      <details>
      <summary> Learning Resources</summary>

        - **[Superset Documentation](https://superset.apache.org/docs/intro)**

        - **[A Superset YouTube Tutorial](https://www.youtube.com/playlist?list=PLz-a3JGXUF8FPvKkm6yDgwAllb3kj2ZS2)**

      </details>