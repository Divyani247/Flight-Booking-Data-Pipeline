#  Flight Booking Data Pipeline with Airflow & CI/CD  

## 📌 Project Overview  
This project demonstrates an **end-to-end Data Engineering pipeline** for processing and analyzing Flight Booking data.  
The pipeline leverages **Google Cloud Platform (GCP)**, **Apache Airflow**, **PySpark**, and **BigQuery**, while CI/CD is implemented using **GitHub Actions**.  

The goal of this project is to showcase:  
- Building a **data pipeline** to process flight booking data.  
- Automating deployment using **CI/CD pipelines**.  
- Orchestrating workflows with **Airflow**.  
- Storing and analyzing processed data in **BigQuery**.  


## 🛠️ Tech Stack  
- **Version Control** → Git, GitHub  
- **CI/CD** → GitHub Actions  
- **Data Storage** → Google Cloud Storage (GCS)  
- **Data Processing** → PySpark on Dataproc Serverless  
- **Workflow Orchestration** → Apache Airflow (Cloud Composer)  
- **Data Warehouse** → BigQuery  


## 🚀 Project Architecture  

1. **GitHub Repo** → Source code, DAGs, and configs stored in GitHub.  
2. **GitHub Actions** → Automates deployment (push DAGs/configs to Composer).  
3. **GCS** → Raw + processed data stored in buckets.  
4. **PySpark on Dataproc Serverless** → Data transformation & processing.  
5. **Airflow DAGs** → Orchestrate the pipeline steps (ingestion → processing → loading).  
6. **BigQuery** → Stores the final processed data for analysis.  


## ⚙️ Workflow Steps  

1. **Data Ingestion**  
   - Raw flight booking data uploaded to **GCS**.  

2. **Data Processing (PySpark on Dataproc)**  
   - Cleans & transforms raw data.  
   - Writes output back to GCS.  

3. **Airflow Orchestration (Cloud Composer)**  
   - DAGs trigger ingestion → processing → load sequence.  

4. **Data Load into BigQuery**  
   - Final processed data loaded into BigQuery tables.  

5. **CI/CD Pipeline**  
   - On every Git push:  
     - GitHub Actions validates & deploys DAGs to Cloud Composer.  
     - Syncs variables/configs to GCS.  


##  Demo Screenshots  
<img width="1919" height="888" alt="Screenshot 2025-09-18 193657" src="https://github.com/user-attachments/assets/d3600d1d-5c5b-4297-b131-dd779beb4633" />
<img width="1881" height="719" alt="Screenshot_1 (70)" src="https://github.com/user-attachments/assets/57feec20-1e19-4a7b-9044-f74e9965533c" />

##  Future Enhancements  
- Create **Power BI dashboards** using BigQuery.  
- Add **unit tests** for DAGs and PySpark scripts

## Acknowledgments  
- **Google Cloud Platform (GCP)** for infrastructure.  
- **Apache Airflow & PySpark** for orchestration & processing.  
- **GitHub Actions** for automation.

## REF
- https://growdataskills.com/



  

