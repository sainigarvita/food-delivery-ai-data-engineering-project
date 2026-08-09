# Zomato AI Data Engineering Platform

An end-to-end **AI-powered data engineering platform** that builds a scalable analytics pipeline for restaurant data using **AWS, Apache Airflow, Snowflake, dbt, and Google Gemini AI**.

The project demonstrates how modern data engineering pipelines can be enhanced with Generative AI capabilities such as **customer review analysis, semantic search, and Retrieval Augmented Generation (RAG)**.

---

## Project Overview

Food delivery platforms generate large volumes of structured and unstructured data such as restaurant details, ratings, and customer reviews.

The goal of this project is to build a production-style data platform that:

- Ingests and processes restaurant data
- Creates analytics-ready data models
- Enables business insights through SQL analytics
- Uses Generative AI to extract insights from customer reviews
- Allows users to interact with restaurant data using natural language

---

# Architecture Overview
<img width="1672" height="941" alt="ChatGPT Image Aug 8, 2026, 02_03_43 PM" src="https://github.com/user-attachments/assets/a2b7d163-1e0e-46fd-bccf-7458b02904cf" />


---

# Technology Stack


## Data Engineering

| Technology | Purpose |
|------------|---------|
| **Python** | Data ingestion, processing, and automation |
| **AWS S3** | Scalable cloud data lake for storing raw and processed data |
| **Apache Airflow** | Orchestrates and schedules data pipeline workflows |
| **Snowflake** | Cloud data warehouse for analytics workloads |
| **dbt** | SQL-based transformations, data modeling, and testing |
| **Docker** | Containerization and consistent development environment |


## Generative AI

| Technology | Purpose |
|------------|---------|
| **Google Gemini API** | Generates AI-powered insights from restaurant reviews |
| **Gemini Embeddings** | Converts text reviews into vector representations |
| **Vector Database** | Stores embeddings and enables similarity search |
| **RAG Architecture** | Retrieves relevant context and generates accurate AI responses |


## Application Layer

| Technology | Purpose |
|------------|---------|
| **Streamlit** | Interactive user interface for AI-powered analytics |
| **SQL** | Data analysis and business insights |

---

# Data Pipeline Workflow


### 1. Data Ingestion

Restaurant datasets are extracted using Python and loaded into AWS S3.

Raw data is stored in the data lake before processing.

---

### 2. Data Processing & Transformation

Apache Airflow manages the pipeline execution.

The workflow performs:

- Data validation
- Cleaning and standardization
- Data preparation for analytics


Processed data is loaded into Snowflake.


---

### 3. Data Warehouse Modeling

Snowflake stores analytics-ready data using dimensional modeling.

This enables efficient analysis of:

- Restaurant performance
- Customer feedback
- Ratings and trends


---

### 4. dbt Transformation Layer

dbt manages SQL transformations inside Snowflake.

Benefits:

- Modular SQL models
- Data quality checks
- Version-controlled transformations
- Maintainable analytics layer


---

# Generative AI Features


## 1. AI Review Analysis

Customer reviews are processed using Gemini API to identify:

- Sentiment
- Common complaints
- Positive feedback
- Customer preferences


Example:

```
Input:
"The food was amazing but delivery was slow"

Output:
Sentiment: Mixed
Positive: Food quality
Negative: Delivery experience

```


---

## 2. Semantic Search with Embeddings

Restaurant reviews are converted into embeddings using Gemini embedding models. Users can search using meaning instead of exact keywords.

Example:

```
"Restaurants with great vegetarian options"

```

The system retrieves restaurants with similar customer experiences.


---

## 3. RAG-Based AI Assistant

The project uses Retrieval Augmented Generation (RAG) to answer questions using restaurant data.


Workflow:

```
User Question

      |
      v

Create Query Embedding

      |
      v

Retrieve Similar Reviews

      |
      v

Gemini LLM

      |
      v

Context-Aware Response

```


Example:

```
Question:
Which restaurants have great food but poor delivery?


Response:
Restaurant A has excellent food ratings but multiple delivery complaints.

```

---


# Key Skills Demonstrated

- Cloud Data Engineering
- ETL/ELT Pipeline Development
- Data Lake & Warehouse Architecture
- Workflow Orchestration
- Dimensional Data Modeling
- SQL Analytics
- Generative AI Integration
- Embeddings & Vector Search
- RAG Application Development


---

## Author

**Garvita Saini**

Data Engineer | Analytics Engineer | Generative AI Enthusiast
