# Hi, I'm Tianyi Luo

Data engineer building cloud data platforms and ML systems end to end — from raw, messy sources to validated tables, trained models, and things people can actually use.

Currently finishing my M.S. in Data Science (Data Engineering concentration) at the University of San Francisco, and working as an ML research intern at UC San Diego's Manor Lab. I care most about the unglamorous parts that make systems trustworthy: data quality, entity resolution, evaluation design, and pipelines that fail loudly instead of silently.

## Projects

### [Cinema Atlas](https://github.com/Tianyi-2000/cinema-atlas) — Film Analytics Data Lakehouse

A medallion lakehouse unifying **10,221 films** from TMDB, IMDb, and Wikidata into one connected analytical platform, with a Next.js app for exploring film relationships, popularity trends, and box-office history.

- End-to-end Bronze → Silver pipeline on Databricks + AWS S3, orchestrated with parallel ingestion branches
- Two-pass entity resolution linking **67,000+ people** across sources (ID joins + fuzzy name matching)
- Data-quality gates: snapshot deduplication, quarantine tables with audit trails, SCD Type 1/2 modeling via MERGE

`Databricks` `Spark` `Delta Lake` `AWS S3` `Unity Catalog` `Next.js`

### [OpenFire](https://github.com/tkovalcik/openfire) — Wildfire Risk Prediction Platform

A production geospatial ML platform (3-person team) predicting wildfire risk across Southern California on a 1 km grid, re-scored every 5 days on a fully scheduled cloud pipeline.

- 38 engineered features per cell in BigQuery; XGBoost with temporal holdouts to prevent spatiotemporal leakage
- Scheduled batch inference on Cloud Run + Cloud Scheduler, with data contracts and row-count invariants
- MLflow experiment tracking, Evidently drift monitoring, Docker + GitHub Actions CI/CD

`BigQuery` `GCP Cloud Run` `XGBoost` `MLflow` `Docker` `GitHub Actions` `FastAPI`

### ABR Synapse Prediction — ML Research, UC San Diego

Research pipeline predicting cochlear synapse counts from auditory brainstem response waveforms — **15,741 recordings** across 162 subjects. Built a two-stage model (classifier feeding regression) with CNN-based waveform features, and leakage-proof evaluation using subject-level splits. *(Lab code private.)*

`Python` `PyTorch` `scikit-learn` `XGBoost`

## Tech

**Languages** — Python, SQL, PySpark, JavaScript, R
**Data engineering** — Spark, Databricks, Delta Lake, Airflow, ETL/ELT, data modeling (star schema, SCD), data quality & validation
**Cloud** — AWS (S3, EC2, EMR), GCP (BigQuery, Cloud Run), Docker, CI/CD, Git
**ML** — PyTorch, scikit-learn, XGBoost, MLflow, Evidently, evaluation design

## Beyond the code

Before data engineering, I studied environmental science — which is how I ended up caring about fog sensors, wildfire risk, and what messy real-world data actually looks like. And Cinema Atlas started as a personal film log: I cared enough about connecting scattered film knowledge that I eventually built a data platform for it.

## Connect

[LinkedIn](https://www.linkedin.com/in/tianyi-luo-b483b81ab/)
