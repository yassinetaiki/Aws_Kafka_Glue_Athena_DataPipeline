## Introduction

Welcome to the Real-Time Analysis project with Apache Kafka! This project leverages Kafka, a distributed streaming platform, along with AWS services to enable real-time data processing and analysis. By utilizing Kafka's scalable and fault-tolerant architecture, 
you can reliably ingest, transform, and analyze data streams in real-time.

## Architecture
The architecture of the project consists of several components, including a Kafka cluster for data streaming, AWS services such as S3, Athena, and Glue for data storage and processing, and EC2 instances for running the necessary scripts and applications. 
The diagram above provides a visual representation of the project's architecture.
![text alternatif](https://github.com/yassinetaiki/Aws_Kafka_Glue_Athena_DataPipeline/blob/master/architecture.png)

## Repository Contents

- `architecture.png`: Architecture diagram of the project.
- `consumer_kafka.ipynb`: Python script to consume data from a Kafka cluster.
- `produce_kafka.ipynb`: Python script to produce data to a Kafka cluster.
- `indexProcessed.csv`: Sample file containing data sources.

## AWS Services Used
- `Amazon S3 (Simple Storage Service)`: Amazon S3 is used for storing the data streams consumed from Kafka. It provides a durable and scalable object storage solution.

- `AWS Glue Crawler`: AWS Glue Crawler is used to automate the process of discovering data and generating associated metadata. The crawler analyzes the data sources, 
such as files in S3, and extracts schemas, tables, partitions, and other structural information about the data. It keeps the metadata up-to-date and detects schema or 
data changes.

- `AWS Glue Catalog`: AWS Glue Catalog acts as a centralized repository for storing the metadata of the discovered data. It stores information such as data schemas, tables, 
partitions, relationships between tables, and more. The Glue Catalog provides a unified and organized view of the data in your AWS environment, making it easier to access
, query, and analyze the data.

- `Amazon Athena`: Amazon Athena is used to query and analyze the data stored in S3 through the Glue Catalog. It allows you to run SQL queries on your data without the need
for managing infrastructure or setting up complex data pipelines.
  
