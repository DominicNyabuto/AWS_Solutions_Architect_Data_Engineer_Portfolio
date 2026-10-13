**Project-2:** [Multi-Region IoT Sensor Ingestion for Manufacturing](https://www.google.com/search?q=./Project-2)

* **Industry:** IoT Manufacturing
* **Focus:** Resilient Architectures, Operational Excellence
* **Description:** A highly available, active-active event ingestion pipeline processing millions of sensor events daily. The architecture utilizes Amazon API Gateway, Kinesis Data Streams, and Lambda for micro-batching across two regions. Data is persisted in DynamoDB Global Tables to ensure cross-region read/write consistency and fault tolerance.


## 2. Resilient IoT Monitoring for Manufacturing Operations

**Industry:** IoT and manufacturing  
**Business problem:** Manufacturing equipment generates large volumes of sensor data, but operations teams often lack a reliable way to ingest, retain, and analyze it across plants and regions. Delayed or lost telemetry can delay the detection of abnormal machine behavior.

**Business goal:** Enable plant engineers and reliability teams to monitor equipment health across regions with minimal data loss and rapid recovery from regional disruption.

**Decision enabled:**  
- Detect abnormal sensor readings early  
- Trigger maintenance or inspection workflows before failure escalates  
- Compare equipment performance across sites  
- Maintain operational visibility during regional outages  

**Target outcome:**  
- High availability for critical telemetry ingestion  
- Reduced risk of lost sensor events  
- Faster operational response to abnormal equipment behavior  
- Cross-region resilience for mission-critical IoT workloads  

**Solution approach:**  
Build an active-active ingestion layer that accepts high-volume sensor events, buffers and processes them through streaming infrastructure, and persists data using a multi-region database design.

**Planned AWS services:**  
Amazon API Gateway, Amazon Kinesis Data Streams, AWS Lambda, Amazon DynamoDB Global Tables, Amazon S3, IAM, Amazon CloudWatch, AWS CloudFormation or Terraform.

**Well-Architected focus:**  
Reliability, operational excellence, performance efficiency, and security.

**Status:** 🚧 In progress
