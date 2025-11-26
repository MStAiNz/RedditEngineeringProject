# Reddit Data Pipeline

This project outlines a step-by-step process for extracting, transforming, and loading Reddit data, enabling easy analysis. It uses several popular tools and services from AWS and others.

## How it works:
Extract data from Reddit using Reddit's API to collect posts and comments
Save the extracted raw data into an S3 bucket. Airflow helps schedule and manage this step.
AWS Glue and Athena organize and transform the raw data into a cleaner, more useful format.
The cleaned data is loaded into Redshift, a data warehouse, where you can run queries and get insights.

## Tools Used
Apache Airflow: schedules and controls the pipeline
Celery: helps with task management
PostgreSQL: supports task tracking
Amazon S3: stores raw data
AWS Glue and Athena: clean and prepare data
Amazon Redshift: stores final data for analysis
