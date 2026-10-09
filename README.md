# AWS Solutions Architect & Data Engineer Portfolio

This repository documents advanced cloud engineering projects that demonstrate proficiency as an AWS Certified Solutions Architect - Associate (SAA-C03). The architectures are inspired by high-volume, production-grade data pipelines, referencing the architectural patterns highlighted in [Linked Images](https://github.com/dominicnyabuto/AWS-SAA/blob/main/1790521312961.jpeg).

The solutions are designed around the official domains of the SAA-C03 exam:

* **Design Secure Architectures**
* **Design Resilient Architectures**
* **Design High-Performing Architectures**
* **Design Cost-Optimized Architectures**

Each implementation strictly adheres to the six pillars of the AWS Well-Architected Framework: Operational Excellence, Security, Reliability, Performance efficiency, Cost optimization, and Sustainability. The projects tackle complex, domain-specific challenges across supply chain, IoT manufacturing, business intelligence, logistics, and data science.

## Folders in the repo:

**Project-1:** [Real-Time Change Data Capture (CDC) for Global Supply Chain](./Project-1)

* **Industry:** Supply Chain & Logistics
* **Focus:** Streaming Analytics, High-Performing Architectures
* **Description:** An event-driven architecture using AWS DMS to capture ongoing operational database changes and stream them into Amazon MSK. AWS Glue streaming ETL deduplicates and processes the records in real-time before storing them in S3 for Athena queries, ensuring a trusted single source of truth for global inventory tracking.

**Project-2:** [Multi-Region IoT Sensor Ingestion for Manufacturing](./Project-2)

* **Industry:** IoT Manufacturing
* **Focus:** Resilient Architectures, Operational Excellence
* **Description:** A highly available, active-active event ingestion pipeline processing millions of sensor events daily. The architecture utilizes Amazon API Gateway, Kinesis Data Streams, and Lambda for micro-batching across two regions. Data is persisted in DynamoDB Global Tables to ensure cross-region read/write consistency and fault tolerance.

**Project-3:** [Schema-Driven Batch Data Lake for Business Intelligence](Project-3)

* **Industry:** Business Intelligence / Data Engineering
* **Focus:** Cost-Optimized Architectures, Reliability
* **Description:** An automated, metadata-driven ingestion framework orchestrated by Amazon MWAA (Apache Airflow). Dynamic DAGs trigger PySpark jobs on AWS Glue that fetch schema rules from DynamoDB, validating and sanitizing raw data before writing optimized Parquet files to a curated S3 bucket for BI reporting in Amazon QuickSight.

**Project-4:** [Automated Fleet Telemetrics & Executive Remediation Workflow](./Project-4)

* **Industry:** Logistics
* **Focus:** Secure Architectures, Operational Excellence
* **Description:** A serverless Step Functions state machine that analyzes telemetrics anomalies and cost drivers. The workflow integrates Lambda for root-cause analysis via Athena, SNS for human-in-the-loop executive approvals, and automated remediation actions, outputting operational health metrics to QuickSight dashboards.

**Project-5:** [Predictive Maintenance ML Pipeline & Feature Store](./Project-5)

* **Industry:** Data Analytics & Science
* **Focus:** Performance Efficiency, Reliability
* **Description:** An end-to-end data pipeline feeding machine learning models using Amazon SageMaker Feature Store. Raw data is ingested via Amazon Kinesis Data Firehose, transformed by AWS Glue, and securely stored in S3, demonstrating the decoupling of data preparation from model training and deployment.

**Project-6:** [Legacy Infrastructure Migration & Cost Analytics Engine](./Project-6)

* **Industry:** Cross-Industry Data Engineering
* **Focus:** Cost Optimization, Security
* **Description:** A comprehensive migration strategy coordinating the retirement of legacy pipelines. The system utilizes AWS Cost Explorer APIs and AWS Budgets to track expenditure, paired with a custom dashboard to analyze cost savings achieved during the transition while maintaining strict IAM security boundaries and data governance.