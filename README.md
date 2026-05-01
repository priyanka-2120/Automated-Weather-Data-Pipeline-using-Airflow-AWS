# 🌦️ Automated Weather Data Pipeline using Airflow & AWS

## 📌 Overview
Built an automated data engineering pipeline to collect, process, and store real-time weather data using Apache Airflow and AWS. The pipeline fetches data from an external API, performs transformations, and stores structured data in AWS S3 for further analysis.

## 🎯 Key Features
- Automated data ingestion from weather API  
- Workflow orchestration using Apache Airflow DAGs  
- Data transformation using Python & Pandas  
- Scheduled execution (daily pipeline runs)  
- Scalable storage using AWS S3  

## 🏗️ Architecture
Weather API → Airflow DAG → Data Transformation → AWS S3  

## ⚙️ Tech Stack
- Workflow Orchestration: Apache Airflow  
- Programming: Python  
- Data Processing: Pandas  
- Cloud: AWS S3  
- API: OpenWeatherMap  

## 🔄 Pipeline Workflow
1. API Availability Check using HttpSensor  
2. Data Extraction using SimpleHttpOperator  
3. Data Transformation (temperature conversion, field extraction, timestamp formatting)  
4. Data Loading to AWS S3 in CSV format with timestamp-based naming  

## 📊 Sample Output
- City  
- Temperature (F)  
- Feels Like  
- Humidity  
- Pressure  
- Wind Speed  
- Sunrise & Sunset Time  

## 📅 Scheduling
Runs automatically using Airflow scheduler: @daily  


## 🔐 Configuration
- OpenWeatherMap API key required  
- AWS credentials required (use environment variables or IAM roles)  

## 🚀 Key Outcomes
- Automated end-to-end data pipeline with minimal manual effort  
- Continuous ingestion of real-time weather data  
- Demonstrated workflow orchestration and cloud integration  

## 📌 Future Improvements
- Add real-time streaming using Kafka  
- Implement data validation and logging  
- Integrate data warehouse (Redshift/BigQuery)  
- Add dashboard for visualization  
