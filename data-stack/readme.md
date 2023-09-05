Hello everyone and I hope you are having a good day!

I try to give you all an insight about our tech stack and choices that you can make for this course.


We want to provide a tech stack for building a datawarehouse with which you are able to implement the project, nevertheless it is you who can choice how to set up youe environment for it. 

- Database:
  
  Speaking of which, you first of all need to have a database for storing your data as the original idea was using Bigquery on GCP, we though it might be troublesome for you to setup the billing with your credit card in order to be able to use it, therefore we came up with an easy solution with Postgres running in docker. But feel free if you would like to set up Bigquery anf dive into cloud engineering if you fancy it and contact Amin Abbasloo for assisting you. Please keep in mind Bigquery sandbox won't allow you streaming so you need to setup billing!

- ETL:
  
  Loading and Extracting: in our stack, Airbyte handles these steps.
  Transforming: DBT is a conventional tool and it is a python library so hopefully you find it straightforward to use. It is worth-mentioning that Airbyte can also import BDT scripts and take care of transformation.
  
- BI:
  
  Superset and Metabase are popular tools for the purpose but I found Metabase memory hungry for a local deployment, therefore our stack has Superset.  
