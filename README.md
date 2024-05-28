Real-Time Data Streaming Pipeline (From Toronto to Niagara)

Overview

This project demonstrates an end-to-end real-time data streaming pipeline for a smart city application. The pipeline covers data ingestion, processing, and storage, utilizing various tools and technologies to handle large-scale data efficiently. 

Architecture

1. Data Ingestion
IoT Devices: Sensors and devices deployed throughout the city collect real-time data (traffic flow, air quality, weather conditions).
Data Streams: The data from IoT devices are streamed continuously to Apache Kafka.
2. Data Collection and Management
Apache Kafka: Acts as the messaging queue to handle the high throughput of data streams from multiple IoT devices.
Apache Zookeeper: Manages and coordinates the Kafka brokers.
3. Data Processing
Apache Spark (Structured Streaming): Consumes data from Kafka for real-time processing and transformation.
Docker: Containerizes Spark jobs to ensure consistency and scalability.
4. Data Storage
AWS Cloud: Utilizes various AWS services for scalable and efficient data storage.
AWS Glue: ETL service to catalog and prepare data for analysis.
AWS Athena: Interactive query service to analyze data directly from S3 using SQL.
AWS IAM: Manages access and permissions securely.
AWS Redshift: Data warehousing solution for storing processed data, enabling complex queries and reporting.

