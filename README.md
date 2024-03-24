# Data Pipeline - User Data

## Description

This project creates an end-to-end data pipeline from ingestion to processing and finally to storage. It uses docker to containerize the project for ease of deployment and scalability.

## Tech Stack

The project is designed with the following components:

- **Data Source**: Used the `randomuser.me` API to generate mock user data for our pipeline.
- **Apache Airflow**: Used to control the pipeline and store fetched data in a PostgreSQL database.
- **Apache Kafka and Zookeeper**: Used for streaming data from PostgreSQL to the processing engine.
- **Apache Spark**: Processes data with its driver and worker nodes.
- **Cassandra**: Stored the processed data

## Getting Started

After cloning the repo, run the following command to start up the services.

    
    docker compose up
    
