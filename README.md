<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:1E3A8A,50:2563EB,100:0EA5E9&height=190&section=header&text=Tianyi%20Luo&fontSize=52&fontColor=ffffff&fontAlignY=36&desc=Data%20pipelines%20%C2%B7%20ML%20systems%20%C2%B7%20LLM%20applications&descSize=18&descAlignY=58" alt="Tianyi Luo">
</p>

<p align="center">
  Engineer working across data pipelines, ML systems, and LLM applications.<br>
  I like building close to the people who use what I build.
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/tianyi-luo-b483b81ab"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:tianyitokyoosaka@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>
  <img src="https://img.shields.io/badge/San%20Francisco,%20CA-444444?style=for-the-badge" alt="San Francisco, CA">
</p>

## About

<table>
  <tr>
    <td colspan="2" valign="top">
      <h3>Now</h3>
      <b>AI Engineer</b> at an early-stage AI developer-tools startup (stealth), San Francisco.<br>
      I build the import pipelines and API / MCP integrations that bring a team's existing work in from the tools they already use, designed for both people and their AI coding agents:
      <ul>
        <li>MCP tools that let an agent preview an import before applying it, with the agent-facing tool text cut 30% to fit the context budget</li>
        <li>Chunked, resumable import runs with rate-limit backoff; re-running an import changes nothing</li>
        <li>Server-side run approval in PostgreSQL with row-level security, so a run applies only the plan a person approved</li>
        <li>In progress: imports an agent can start on its own over MCP with OAuth</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3>Before</h3>
      <b>Machine Learning Researcher</b>, Manor Lab, UC San Diego<br>
      ETL pipeline that turns 1,300+ raw auditory recordings from 125 mice into 12,187 validated waveforms, with schema checks and leakage-free splits; 1D U-Net autoencoder producing 32-feature embeddings for synapse-count models.
    </td>
    <td width="50%" valign="top">
      <h3>Education</h3>
      <b>M.S. in Data Science</b>, Concentration in Data Engineering<br>
      University of San Francisco
    </td>
  </tr>
</table>

## How I work

<table>
  <tr>
    <td width="33%" valign="top">
      <h3>Bridge between teams</h3>
      I probe the platform API and partner tool catalogs before coding, which catches spec gaps early.
    </td>
    <td width="33%" valign="top">
      <h3>Think from the user's side</h3>
      I present projects at startup meetups and adjust the pitch to the audience. I would rather ask what someone needs than build in isolation.
    </td>
    <td width="33%" valign="top">
      <h3>Read and apply research</h3>
      Currently reading on AI research agents and evaluation. I care about agent behavior that is measurable and reliable, not demos.
    </td>
  </tr>
</table>

## Projects

<table>
  <tr>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/Tianyi-2000/PhysicalAI-sense-the-world">Edge AI Depth Estimation</a></h3>
      ExecuTorch Hackathon, October 2026 (team of three). A Qualcomm-based Arduino VENTUNO Q labels its own training data by pairing camera frames with a time-of-flight sensor, then fits a depth head on frozen DINOv2 features on the board. Exported with ExecuTorch and the XNNPACK delegate: 3.6x faster than PyTorch on the same CPU (870 to 242 ms p50); int8 quantization shrank the model 4x.<br><br>
      <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" alt="PyTorch">
      <img src="https://img.shields.io/badge/ExecuTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" alt="ExecuTorch">
      <img src="https://img.shields.io/badge/DINOv2%20(Hugging%20Face)-FFD21E?style=flat-square&logo=huggingface&logoColor=black" alt="DINOv2 (Hugging Face)">
      <img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white" alt="OpenCV">
      <img src="https://img.shields.io/badge/Arduino-00878F?style=flat-square&logo=arduino&logoColor=white" alt="Arduino">
    </td>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/Tianyi-2000/streaming-fraud-detection">Streaming Fraud Detection</a></h3>
      Kafka pipeline that detects artificial streaming fraud in 45K+ music play events (team of two). My part: the cached MusicBrainz catalog, a seeded event generator with three fraud cohorts, the frozen Pydantic event contract, contract-validated replay into Redpanda, and the Streamlit review dashboard. Two keyed consumer stages with a re-key prove that no single partition key catches both fraud patterns.<br><br>
      <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python">
      <img src="https://img.shields.io/badge/Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white" alt="Kafka">
      <img src="https://img.shields.io/badge/Redpanda-E14226?style=flat-square&logo=redpanda&logoColor=white" alt="Redpanda">
      <img src="https://img.shields.io/badge/Docker%20Compose-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker Compose">
      <img src="https://img.shields.io/badge/Pydantic-E92063?style=flat-square&logo=pydantic&logoColor=white" alt="Pydantic">
      <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white" alt="Streamlit">
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/Tianyi-2000/cinema-atlas">Cinema Atlas</a></h3>
      Film data lakehouse on Databricks. Ingests IMDb, TMDB and Wikidata into an S3 lake; dbt silver models with tests and lineage; incremental daily runs; SCD Type 2 history; entity resolution linking 67K+ people across 10K+ films.<br><br>
      <img src="https://img.shields.io/badge/Databricks-FF3621?style=flat-square&logo=databricks&logoColor=white" alt="Databricks">
      <img src="https://img.shields.io/badge/Delta%20Lake-003366?style=flat-square&logo=delta&logoColor=white" alt="Delta Lake">
      <img src="https://img.shields.io/badge/dbt-FF694B?style=flat-square&logo=dbt&logoColor=white" alt="dbt">
      <img src="https://img.shields.io/badge/PySpark-E25A1C?style=flat-square&logo=apachespark&logoColor=white" alt="PySpark">
      <img src="https://img.shields.io/badge/AWS%20S3%20%7C%20IAM%20%7C%20Glue-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white" alt="AWS">
    </td>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/tkovalcik/openfire">OpenFire</a></h3>
      Wildfire risk ML platform for Southern California (team project). Built the batch pipeline that recomputes 38 features per 1 km cell every 5 days with an all-or-nothing publish contract, and the CI/CD for 5 containerized services.<br><br>
      <img src="https://img.shields.io/badge/GCP%20BigQuery%20%7C%20Cloud%20Run-4285F4?style=flat-square&logo=googlecloud&logoColor=white" alt="GCP">
      <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker">
      <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" alt="GitHub Actions">
      <img src="https://img.shields.io/badge/MLflow-0194E2?style=flat-square&logo=mlflow&logoColor=white" alt="MLflow">
      <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" alt="FastAPI">
      <img src="https://img.shields.io/badge/XGBoost-189FDD?style=flat-square" alt="XGBoost">
    </td>
  </tr>
</table>

## Skills

<table>
  <tr>
    <td width="22%" valign="top"><b>Languages</b></td>
    <td valign="top">
      <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python">
      <img src="https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=mysql&logoColor=white" alt="SQL">
      <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript">
    </td>
  </tr>
  <tr>
    <td width="22%" valign="top"><b>Data</b></td>
    <td valign="top">
      <img src="https://img.shields.io/badge/PySpark-E25A1C?style=flat-square&logo=apachespark&logoColor=white" alt="PySpark">
      <img src="https://img.shields.io/badge/dbt-FF694B?style=flat-square&logo=dbt&logoColor=white" alt="dbt">
      <img src="https://img.shields.io/badge/Databricks-FF3621?style=flat-square&logo=databricks&logoColor=white" alt="Databricks">
      <img src="https://img.shields.io/badge/Delta%20Lake-003366?style=flat-square&logo=delta&logoColor=white" alt="Delta Lake">
      <img src="https://img.shields.io/badge/Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white" alt="Kafka">
      <img src="https://img.shields.io/badge/Airflow-017CEE?style=flat-square&logo=apacheairflow&logoColor=white" alt="Airflow">
      <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL">
      <img src="https://img.shields.io/badge/GraphQL-E10098?style=flat-square&logo=graphql&logoColor=white" alt="GraphQL">
    </td>
  </tr>
  <tr>
    <td width="22%" valign="top"><b>ML and AI</b></td>
    <td valign="top">
      <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" alt="PyTorch">
      <img src="https://img.shields.io/badge/ExecuTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" alt="ExecuTorch">
      <img src="https://img.shields.io/badge/Hugging%20Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black" alt="Hugging Face">
      <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white" alt="scikit-learn">
      <img src="https://img.shields.io/badge/MLflow-0194E2?style=flat-square&logo=mlflow&logoColor=white" alt="MLflow">
      <img src="https://img.shields.io/badge/XGBoost-189FDD?style=flat-square" alt="XGBoost">
      <img src="https://img.shields.io/badge/MCP-000000?style=flat-square&logo=modelcontextprotocol&logoColor=white" alt="MCP">
      <img src="https://img.shields.io/badge/Claude%20Code-D97757?style=flat-square&logo=claude&logoColor=white" alt="Claude Code">
    </td>
  </tr>
  <tr>
    <td width="22%" valign="top"><b>Cloud and tooling</b></td>
    <td valign="top">
      <img src="https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white" alt="AWS">
      <img src="https://img.shields.io/badge/GCP-4285F4?style=flat-square&logo=googlecloud&logoColor=white" alt="GCP">
      <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker">
      <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white" alt="Kubernetes">
      <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" alt="GitHub Actions">
      <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" alt="FastAPI">
      <img src="https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB" alt="React">
    </td>
  </tr>
</table>

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0EA5E9,50:2563EB,100:1E3A8A&height=90&section=footer" alt="">
</p>
