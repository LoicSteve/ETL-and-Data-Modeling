# ETL-and-Data-Modeling
Develop a data pipeline

##  Introduction
XXX is a new company in the music industry, offering a subscription-based app for streaming songs. Recently, they have expanded their services to include digital song purchases. With this new retail feature, DeFtunes requires a data pipeline to extract purchase data from their new API and operational database, enrich and model this data, and ultimately deliver the comprehensive data model for the Data Analysis team to review and gain insights. Your task is to develop this pipeline, ensuring the data is accurately processed and ready for in-depth analysis
Here is the diagram with the main requirements for this project:

<img width="990" alt="Screenshot 2024-10-18 at 13 27 54" src="https://github.com/user-attachments/assets/f93814f4-0932-47d5-9477-0b16ca6bdcc3">


1. The pipeline has to follow a medallion architecture with a landing, transform and serving zone.
2. The data generated in the pipeline will be stored in the company's data lake, in this case, an S3 bucket.
3. The silver layer should use Iceberg tables, and the gold layer should be inside Redshift.
4. The pipeline should be reproducible, you will have to implement it using Terraform.
5. The data should be modelled into a star schema in the serving layer, you should use dbt for the modelling part.

Before starting, you will need to import some required libraries and modules for the capstone development.
