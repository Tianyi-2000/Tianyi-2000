# Tianyi Luo

Data engineer building batch and real-time pipelines with built-in data quality.

- Software Engineer (Data Integrations) at an early-stage AI developer-tools startup (stealth), San Francisco
- M.S. in Data Science, Concentration in Data Engineering, University of San Francisco (Aug 2026)
- Previously Machine Learning Researcher at Manor Lab, UC San Diego
- Open to Data Engineer and AI Engineer roles

## Projects

**[Cinema Atlas](https://github.com/Tianyi-2000/cinema-atlas)**: film data lakehouse on Databricks. Ingests IMDb, TMDB and Wikidata into an S3 lake, dbt silver models with tests and lineage, incremental daily runs, SCD Type 2 history, entity resolution linking 67K+ people across 10K+ films.
Tech: Databricks (Workflows, Unity Catalog), Delta Lake, dbt, PySpark, AWS (S3, IAM, Glue)

**[Streaming Fraud Detection](https://github.com/Tianyi-2000/streaming-fraud-detection)**: real-time Kafka pipeline that flags bot accounts and coordinated play bursts in 45K+ music streaming events. Versioned data contract on every event, checkpointed offsets and deduplication, load-tested at 100K+ events/s.
Tech: Python, Kafka (Redpanda, Kafka Connect), Docker Compose, Pydantic, ArangoDB

**[OpenFire](https://github.com/tkovalcik/openfire)**: wildfire risk ML platform for Southern California (team project). Built the batch pipeline that recomputes 38 features per 1 km cell every 5 days with an all-or-nothing publish contract, and the CI/CD for 5 containerized services.
Tech: GCP (BigQuery, Cloud Run, Cloud Scheduler), Docker, GitHub Actions, MLflow, FastAPI, XGBoost

**ABR Synapse Prediction** (Manor Lab, UC San Diego; lab code is private): ETL pipeline that turns 1,300+ raw auditory recordings from 125 mice into 12,187 validated waveforms, with schema checks and leakage-free train/test splits; 1D U-Net autoencoder producing 32-feature embeddings for downstream models.
Tech: Python, pandas, PyTorch, scikit-learn

## Skills

Python, SQL, PySpark, dbt, Databricks, Delta Lake, Kafka, Airflow, Docker, Kubernetes, AWS (S3, IAM, Glue), GCP (BigQuery, Cloud Run), GitHub Actions, MLflow, FastAPI

## Contact

tianyitokyoosaka@gmail.com | [LinkedIn](https://www.linkedin.com/in/tianyi-luo-b483b81ab)
