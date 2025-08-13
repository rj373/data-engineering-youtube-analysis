## **Project: YouTube Trending Video Analytics Platform**

### **Overview**

This project demonstrates the design and implementation of a robust, end-to-end data pipeline on AWS to process, analyze, and visualize YouTube video data. The core objective is to create a scalable and secure analytics platform that transforms raw, semi-structured data into a clean, query-ready format. This system provides a foundation for deriving business insights from video categories and key trending metrics, enabling data-driven decisions on content strategy.

### **Project Goals & Technical Approach**

The project was executed with the following key objectives:

* **Automated Data Ingestion:** Developed a mechanism to automatically ingest raw YouTube trending data from various sources (e.g., CSV and JSON files) into a centralized repository.
* **Scalable ETL Pipeline:** Engineered a serverless Extract, Transform, Load (ETL) system using **AWS Glue** and **AWS Lambda**. This pipeline is designed to transform raw, inconsistent data into a structured, optimized format, ensuring efficiency and data quality.
* **Centralized Data Lake:** Established a tiered data lake architecture using **Amazon S3** to manage data from multiple sources. This repository provides a flexible and cost-effective solution for storing data in its raw, cleansed, and final reporting states.
* **Cloud-Native Architecture:** Leveraged the scalability and cost-efficiency of the AWS cloud to handle large volumes of data. The architecture is built on a serverless paradigm, minimizing operational overhead and ensuring the system scales dynamically with data growth.
* **Business Intelligence & Reporting:** Created an interactive dashboard using **Amazon QuickSight** to provide key stakeholders with a clear view of video trends, popular categories, and engagement metrics. This reporting layer directly addresses the business questions that the project was designed to solve.

### **AWS Services Utilized**

The following services form the backbone of this project's architecture:

* **Amazon S3:** Implemented a multi-zone data lake for scalable, secure, and durable object storage.
* **AWS IAM:** Configured fine-grained access control and security policies to manage access to AWS resources, ensuring a secure and compliant environment.
* **AWS Glue:** Used as a serverless data integration and cataloging service to orchestrate the ETL workflow and prepare data for analysis.
* **AWS Lambda:** Deployed serverless Python functions to perform automated data transformations, specifically converting raw JSON data into an optimized Parquet format.
* **Amazon Athena:** Utilized this interactive query service to perform ad-hoc analysis directly on the data lake, enabling quick data validation and exploration.
* **Amazon QuickSight:** Connected to the processed data to build and deploy a dynamic, machine learning-powered business intelligence dashboard.

### **Dataset**

The project utilizes a rich dataset from Kaggle, containing statistics on daily trending YouTube videos across several months and regions. The data, stored in both CSV and JSON formats, includes:
* Video metadata (title, channel title, publication time)
* Engagement metrics (views, likes, dislikes, comment count)
* Categorical data (`category_id` in JSON files)
* Video-specific details (tags, description)

### **Architecture**
<img width="1742" height="926" alt="AWS ARCHITECTURE" src="https://github.com/user-attachments/assets/c412f460-d93f-4039-b8a9-e3c06b5a50bd" />

