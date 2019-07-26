---
title: "What is a warehouse?"
---

A warehouse is a central repository of data that has been collected from one or more sources. This is what commonly comes to mind when thinking about a relational database – structured data that fits neatly into rows and columns.

In Segment, a Warehouse is a special subset of destinations where we load data to them in bulk at a regular interval, inserting and updating events and objects while automatically adjusting their schema to fit the data you’ve sent to Segment.

When selecting and building a data warehouse, there are three questions to consider:

1.  What type of data will be collected?
    
2.  How many data sources will there be?
    
3.  How will the data be used?
    

Relational databases are great when you know and predefine the information collected and how it will be linked. This is usually the type of database used in the world of user analytics. For instance, a users table might be populated with the columns “name”, “email address”, “plan name”, etc.

Examples of data warehouses include Amazon Redshift, Google BigQuery, MySQL, and Postgres.