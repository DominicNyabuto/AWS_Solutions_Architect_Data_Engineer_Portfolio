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
* **External Free Tools**: Python Mock Sensor Script
* **Description**: Designed for resilience and operational excellence. A fleet of simulated local factory sensors (Python script) sends telemetry data to an AWS API Gateway. Lambda micro-batches the payloads and writes them to DynamoDB Global Tables, demonstrating cross-region read/write consistency and active-active high availability using strictly free-tier eligible services.
  
**Project-3:** [Schema-Driven Batch Data Lake for Business Intelligence](Project-3)

* **Status**: ⏳ Planned
* **Industry**: Business Intelligence / Data Engineering
* **AWS Services**: EC2 (t2.micro), S3, AWS Glue (Trial/Minimal DPU), Amazon Athena
* **External Free Tools**: Apache Airflow (Self-hosted on EC2), Streamlit Community Cloud
* **Description**:A cost-optimized, metadata-driven ingestion framework. Rather than using expensive managed orchestration, Apache Airflow is hosted on a free-tier EC2 instance to trigger ETL jobs. Raw data lands in S3, is transformed into Parquet using lightweight PySpark/Glue, and is queried via serverless Amazon Athena. A free Streamlit web app is connected to Athena to serve BI dashboards.


**Project-4:** [Automated Fleet Telemetrics & Executive Remediation Workflow](./Project-4)

* **Status**: ⏳ Planned
* **Industry**: Logistics
* **AWS Services**: Step Functions, Lambda, SNS, S3
* **External Free Tools**: GitHub Actions (for CI/CD)
* **Description**:A serverless, human-in-the-loop remediation workflow highlighting secure and automated operations. An AWS Step Functions state machine triggers when anomalous fleet fuel or route data lands in S3. It uses Lambda to evaluate the anomaly and SNS to email stakeholders for an Approve/Reject action before writing the final operational health status back to S3.


**Project-5:** [Predictive Maintenance ML Pipeline & Feature Store](./Project-5)

* **Status**: ⏳ Planned
* **Industry**: Data Analytics & Science
* **AWS Services**: API Gateway, Lambda, S3
* **External Free Tools**: Google Colab (Free GPU/TPU), Scikit-Learn
* **Description**:Showcases the decoupling of data preparation from ML training. Historical machinery data is stored in S3. Model training is offloaded to Google Colab to utilize free compute power. The trained model artifact (.pkl) is then uploaded back to S3, where a Lambda function (exposed via API Gateway) loads it to serve real-time serverless predictions.


**Project-6:** [Legacy Infrastructure Migration & Cost Analytics Engine](./Project-6)

* **Status**: ⏳ Planned
* **Industry**: Cross-Industry Data Engineering
* **AWS Services**: AWS Cost & Usage Reports (CUR), S3, Athena
* **External Free Tools**: Metabase (Open Source / Local Docker)
* **Description**:A financial operations (FinOps) architecture highlighting the Cost Optimization pillar. AWS Cost and Usage Reports are configured to deliver directly to an S3 bucket. Using Athena, the raw billing data is queried and connected to a locally hosted instance of Metabase to visualize cost savings and track the budget boundaries of migrating legacy pipelines to the cloud. 
