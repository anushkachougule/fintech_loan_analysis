# Scalable Data Pipeline for Fintech Analytics

## Overview  
This project builds a scalable, production-style ETL pipeline to process and analyze lending and customer behavior data in the fintech industry. The system ingests raw data, performs automated validations, and serves clean, analytics-ready data to Tableau dashboards for decision-making.

It is built entirely on AWS services, follows modular design principles, and includes automated quality checks using Great Expectations.

## Objectives  
- Design a scalable ETL architecture using AWS services
- Automate data validation and transformation workflows
- Enable real-time dashboarding and analytics for fintech KPIs
- Support future integration of predictive models and external data

## Dataset  
The project uses the **BigQuery Fintech Dataset** from Kaggle, which includes customer demographics, loan details, lending trends, and regional borrowing data.  

[Kaggle Dataset](https://www.kaggle.com/datasets/mustafakeser4/bigquery-fintech-dataset?select=loan.csv)  

## Tools & Technologies  
- **AWS S3, AWS Glue, AWS RDS (PostgreSQL)** for data storage, ETL processing, and analytics.  
- **Python (Pandas, SQLAlchemy, Boto3)** for data manipulation and AWS interactions.  
- **Great Expectations** for data validation and quality checks.  
- **Tableau** for interactive data visualization.

## Architecture
- Data Ingestion: Raw CSVs uploaded to S3
- ETL Processing: AWS Glue job transforms and loads data into RDS
- Validation Layer: Great Expectations suite integrated into the pipeline to enforce schema, null checks, and range constraints
- Analytics & Reporting: Tableau connected to RDS for real-time dashboards
- Monitoring: CloudWatch used to track Glue job performance and logs

## Key Features
- Modular ETL job with separation of ingestion, transformation, and validation
- Reusable transformation scripts with SQLAlchemy for database interactions
- Dynamic Glue jobs triggered via Lambda based on S3 events
- Fully automated data pipeline for daily refresh cycles
- Integration of Tableau for live querying and interactive filtering

## Analytics Use Cases
- Loan approval volume and trends by region and customer type
- Loan purpose analysis (debt consolidation, business loans, etc.)
- Customer segmentation by risk level, interest rate, and payment behavior
- Drill-down visualizations by state, loan grade, and demographics

## Key Insights  
- **Loan Approval & Regional Trends**: California, Texas, and New York lead in loan amounts.  
- **Loan Purpose Analysis**: Small business loans, debt consolidation, and home improvement are the top categories.  
- **Customer Segmentation**: Risk analysis based on loan grades, interest rates, and installment amounts.  
- **Interactive Dashboard**: Allows filtering by loan type, purpose, and region for deeper insights.  

## Future Enhancements  
- Automate real-time data processing for continuous insights.  
- Integrate external data sources such as credit scores and economic indicators.  
- Develop predictive models for loan defaults and customer segmentation.  

## Team  
- **Anushka Chougule**  
- **Atharva Panvalkar**  
- **Harshitha Ramachandra**  
- **Sagar Das**  

[GitHub Repository](https://github.com/sagar8080/data-prep-for-fintech-loan-analytics)  

---
