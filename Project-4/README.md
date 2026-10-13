**Project-4:** [Automated Fleet Telemetrics & Executive Remediation Workflow](https://www.google.com/search?q=./Project-4)

* **Industry:** Logistics
* **Focus:** Secure Architectures, Operational Excellence
* **Description:** A serverless Step Functions state machine that analyzes telemetrics anomalies and cost drivers. The workflow integrates Lambda for root-cause analysis via Athena, SNS for human-in-the-loop executive approvals, and automated remediation actions, outputting operational health metrics to QuickSight dashboards.


### 4. Fleet Health Monitoring and Automated Operational Remediation

**Industry:** Logistics and fleet operations  
**Business problem:** Fleet managers need to identify vehicles or routes driving excess cost, delays, safety risk, or maintenance issues. Manual review of telematics data is slow, and issues may remain unresolved without a clear ownership and approval process.

**Business goal:** Turn fleet telemetry into timely operational alerts, root-cause analysis, and accountable remediation actions.

**Decision enabled:**  
- Identify vehicles or routes with abnormal cost or performance  
- Determine likely causes of operational anomalies  
- Route high-impact issues to managers for approval  
- Automate low-risk corrective actions  
- Monitor fleet health through executive dashboards  

**Target outcome:**  
- Faster identification of cost and performance issues  
- Reduced manual investigation time  
- Clear accountability for remediation  
- Improved operational visibility for fleet leadership  

**Solution approach:**  
Use an orchestration workflow to analyze anomalous telemetry, investigate contributing factors through SQL-based analytics, notify the appropriate stakeholders, and execute approved remediation steps.

**Planned AWS services:**  
AWS Step Functions, AWS Lambda, Amazon Athena, Amazon S3, Amazon SNS, Amazon QuickSight, Amazon EventBridge, IAM, CloudWatch.

**Well-Architected focus:**  
Security, operational excellence, reliability, and cost optimization.

**Status:** 🚧 In progress
