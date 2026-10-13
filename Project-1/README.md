**Project-1:** [Real-Time Change Data Capture (CDC) for Global Supply Chain](https://www.google.com/search?q=./Project-1)

* **Industry:** Supply Chain & Logistics
* **Focus:** Streaming Analytics, High-Performing Architectures
* **Description:** An event-driven architecture using AWS DMS to capture ongoing operational database changes and stream them into Amazon MSK. AWS Glue streaming ETL deduplicates and processes the records in real-time before storing them in S3 for Athena queries, ensuring a trusted single source of truth for global inventory tracking.



## 1. Real-Time Inventory Visibility for Global Supply Chains

**Industry:** Supply chain and logistics  
**Business problem:** Global supply-chain teams often discover inventory mismatches too late. Delayed updates between warehouses, ERP systems, and planning tools can cause stockouts, excess inventory, missed shipments, and hours of manual reconciliation.

**Business goal:** Give operations and planning teams a near-real-time, trustworthy view of inventory movement across locations.

**Decision enabled:**  
- Identify inventory discrepancies before they disrupt fulfillment  
- Prioritize corrective action for high-value or time-sensitive stock  
- Reduce dependency on manual spreadsheet reconciliation  
- Improve replenishment and allocation decisions  

**Target outcome:**  
- Faster detection of inventory inconsistencies  
- Reduced manual reconciliation effort  
- Improved inventory accuracy and fulfillment reliability  
- A single trusted source of inventory truth for downstream analytics  

**Solution approach:**  
Capture operational database changes as they occur, stream them through an event-driven pipeline, apply deduplication and data-quality rules, and make the curated data available for both operational queries and BI analysis.

**Planned AWS services:**  
AWS DMS, Amazon MSK, AWS Glue Streaming ETL, Amazon S3, AWS Glue Data Catalog, Amazon Athena, Amazon QuickSight, IAM, CloudWatch.

**Well-Architected focus:**  
Performance efficiency, operational excellence, reliability, and data governance.

**Status:** 🚧 In progress
