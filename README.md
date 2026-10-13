# AWS Solutions Architect & Data Engineer Portfolio

🚧 WORK IN PROGRESS 🚧
Hello Visitors! This repository is currently under active development. I am building out these projects to demonstrate my hands-on proficiency after passing the AWS SAA-C03 exam. I will be updating the folders below as I complete each architecture. Thank you for your patience!

This repository documents hands-on cloud engineering projects demonstrating proficiency as an AWS Certified Solutions Architect - Associate. The architectures focus heavily on Data Engineering, high-volume data pipelines, and adherence to the AWS Well-Architected Framework. Each project will include architecture diagrams, infrastructure-as-code, data models, cost considerations, security controls, and a written business case.

Infrastructure & Cost Note: To maintain cost efficiency, these projects are built utilizing the AWS Free Tier, my $200 trial credits, and integrated with free, open-source third-party tools (like Streamlit, Google Colab, and local Apache Airflow deployments) to simulate enterprise-grade environments without the enterprise price tag.


The solutions are designed around the official domains of the SAA-C03 exam:

* **Design Secure Architectures**
* **Design Resilient Architectures**
* **Design High-Performing Architectures**
* **Design Cost-Optimized Architectures**

Each project in this repository is designed around:

- **The industry problem being solved**
  - The projects tackle complex, domain-specific challenges across supply chain, IoT manufacturing, business intelligence, logistics, and data scienc
- **The business decision the solution supports**
- **The users and workflows affected**
- **The measurable outcome or KPI**
- **The AWS architecture and Well-Architected trade-offs**
  -  Operational Excellence, Security, Reliability, Performance efficiency, Cost optimization, and Sustainability.
- **Security, governance, reliability, performance, cost, and sustainability**
  
## What this portfolio demonstrates

- **Cloud architecture:** Secure, resilient, high-performing, and cost-aware AWS designs.
- **Data engineering:** Batch, streaming, CDC, data-lake, governance, and data-quality patterns.
- **Analytics and BI:** Turning operational data into decision-ready dashboards and insights.
- **Machine learning enablement:** Feature engineering, model-ready data pipelines, and MLOps foundations.
- **Business alignment:** Every project begins with a problem statement, target user, decision, and success metric.
- **Cost-conscious engineering:** Practical designs using AWS Free Tier, trial credits, and open-source tools where appropriate.

## Folders in the repo:

**Project-1:** [Real-Time Change Data Capture (CDC) for Global Supply Chain](./Project-1)

* **Status**: ⏳ In Progress
* **Industry**: Supply Chain & Logistics
* **AWS Services**: DynamoDB Streams, Lambda, S3, EventBridge
* **External Free Tools**: Python (Boto3)
* **Description:** An event-driven, friendly CDC architecture. Instead of heavy streaming services, this project uses DynamoDB Streams to capture operational database changes. AWS Lambda processes and deduplicates the stream in real-time, pushing structured JSON data into S3 to create a highly available, decoupled single source of truth for inventory state.

**Project-2:** [Multi-Region IoT Sensor Ingestion for Manufacturing](./Project-2)

* **Status**: ⏳ Planned
* **Industry**: IoT Manufacturing
* **AWS Services**: API Gateway, Lambda, DynamoDB Global Tables
* **Focus:** Python Mock Sensor Script
* **External Free Tools**: Python Mock Sensor Script
* **Description**: Designed for resilience and operational excellence. A fleet of simulated local factory sensors (Python script) sends telemetry data to an AWS API Gateway. Lambda micro-batches the payloads and writes them to DynamoDB Global Tables, demonstrating cross-region read/write consistency and active-active high availability using strictly free-tier eligible services.
  
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
