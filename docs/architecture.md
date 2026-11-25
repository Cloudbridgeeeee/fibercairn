# Proposed AWS architecture

| Service | Role |
|---|---|
| S3 and Lambda | Ticket and report exports, customer names removed as they arrive |
| CloudWatch | Import runs, model jobs and alerts monitored |
| SageMaker AI | Incident classes and outage trend models |
| Bedrock | Report summaries that cite tickets and work orders |

One AWS account per customer, encrypted at rest and in transit. The public demo calls none of these services.
