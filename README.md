**Project Title & Overview**
# Ottawa Transit Analytics (Microsoft Fabric)
An end-to-end data engineering solution that ingests bus stop data from the City of Ottawa (ArcGIS REST API) into a Microsoft Fabric Medallion Architecture.

# Architecture Diagram (Text or Image)
Explain the flow you built:
  Bronze: Raw JSON/CSV ingestion using Data Factory Pipelines (handling REST API pagination).
  Silver: Data cleaning and Delta table conversion using Spark Notebooks (PySpark).
  Gold: Semantic modeling and visualization in Power BI.

# Technical Features
Highlight the hard parts you solved:
  Advanced Pagination: Implemented resultRecordOffset logic to bypass the 1,000-row API limit for a 5,800-row dataset.
  Environment Governance: Full ALM (Application Lifecycle Management) using Dev -> Test -> Prod deployment pipelines.
  CI/CD: Workspace integration with GitHub for version control of Notebooks and Semantic Models.

# Setup Instructions
Briefly mention how to deploy:
  Connect the Fabric Workspace to this Repo.
  Configure Deployment Rules for Lakehouse re-mapping.
  Run the Ingestion Pipeline.
