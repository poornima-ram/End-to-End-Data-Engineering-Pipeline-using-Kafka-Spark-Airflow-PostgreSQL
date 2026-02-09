# End-to-End Data Engineering Pipeline using Kafka, Spark, Airflow & PostgreSQL

## 📌 Overview
This project demonstrates the design and implementation of an end-to-end data engineering pipeline that ingests real-time data from an external API, processes it using Apache Spark, orchestrates workflows with Apache Airflow, and stores the transformed data in PostgreSQL.  

The entire system is containerized using Docker and Docker Compose, making it easy to deploy, run, and reproduce locally.

---

## 🎯 Problem Statement
Real-time data generated from APIs often needs to be ingested, processed, and stored reliably for analytical and downstream use cases.  
This project showcases how to build a scalable and fault-tolerant data pipeline using modern data engineering tools and best practices.

---

## 🏗 Architecture Overview
The pipeline consists of the following layers:

- **Ingestion Layer**: Kafka is used to stream real-time data from an external API.
- **Processing Layer**: Apache Spark consumes messages from Kafka, applies transformations, and prepares data for storage.
- **Orchestration Layer**: Apache Airflow schedules and orchestrates ingestion and processing tasks.
- **Storage Layer**: PostgreSQL stores the processed data for analytical querying.
- **Infrastructure**: Docker and Docker Compose are used to containerize and manage all services.

> The architecture diagram provides a high-level view of data flow across the system.

---

## 🔄 Data Flow
1. Data is fetched from an external API and published to a Kafka topic  
2. Apache Spark consumes data from Kafka and performs necessary transformations  
3. Transformed data is written into PostgreSQL tables  
4. Apache Airflow orchestrates the workflow, ensuring task dependencies and scheduling  
5. Docker Compose manages all services for local execution  

---

## 🧰 Technologies Used
- **Python**
- **Apache Kafka**
- **Apache Spark**
- **Apache Airflow**
- **PostgreSQL**
- **Docker & Docker Compose**

---

## ⚙️ How to Run the Project

### Prerequisites
- Docker
- Docker Compose

### Steps
1. Clone the repository:
   ```bash
   git clone <your-repo-url>
   cd <your-repo-name>
