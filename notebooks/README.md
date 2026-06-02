# Notebooks

This folder separates the original research workflow into smaller notebooks that follow the project pipeline.

| Notebook | Purpose |
|---|---|
| `00_environment_setup.ipynb` | Install packages, mount storage, and initialize Kafka/Spark environment. |
| `01_general_creators_youtube_api_collection.ipynb` | Collect seed channels, video IDs, and video metadata for the general creator sample. |
| `02_general_creators_kafka_pyspark_etl.ipynb` | Process raw YouTube records through Kafka/PySpark and construct creator-month features. |
| `03_general_creators_did_event_study.ipynb` | Run DID, fixed effects, count models, and event-study diagnostics for general creators. |
| `04_professional_creators_data_collection_and_panel.ipynb` | Collect and aggregate data for the top professional creator sample. |
| `05_professional_creators_did_analysis.ipynb` | Run DID and event-study analysis for professional creators. |
| `99_appendix_validation_and_r_handoff.ipynb` | Additional validation checks and R handoff code from the original workflow. |

Note: API keys were removed from the public notebooks. Replace `YOUR_YOUTUBE_API_KEY` with a local key stored securely before running the data collection notebooks.
