---
sources: ["summaries/session-07_2025-04-06.md"]
type: "Product"
description: "Amazon Web Services, a cloud computing platform used for hosting and logging."
---

# Amazon Web Services (AWS)

Amazon Web Services (AWS) is a comprehensive cloud computing platform that provides on‑demand infrastructure, storage, and services. In the context of the **session‑07_2025‑04‑06** compliance discussion, AWS serves as the core cloud environment whose logs are harvested for audit readiness.

## Key facts from the session
- **Log sources**: The audit‑bundle template extracts **AWS CloudTrail** events and **AWS CloudWatch** application logs as part of the quarterly evidence package.
- **CloudTrail** captures identity‑related actions, service‑level API calls, and configuration changes; the SPL query for CloudTrail is defined in the one‑page hand‑off.
- **CloudWatch** provides the high‑value application log streams (service restarts, error messages, drift detections) that are bundled alongside other logs.
- AWS logs are streamed into **Splunk**, enabling the standardized SPL queries used for consistent export.
- The typical compliance stack referenced in the session is **AWS + GitHub + Jira + Okta + Splunk**, illustrating how AWS integrates with other tools for [[concepts/compliance-automation]].

## Related concepts and entities
- [[concepts/audit-bundle]] – the structured export package that includes AWS CloudTrail and CloudWatch data.
- [[concepts/compliance-automation]] – the overall approach of embedding evidence collection into existing AWS workflows.
- [[entities/cloudtrail]] – AWS service that records API activity.
- [[entities/cloudwatch]] – AWS service for monitoring and log aggregation.
- [[entities/splunk]] – the SIEM where AWS logs are indexed and queried.
- [[summaries/session-07_2025-04-06]] – source summary that outlines the AWS‑related audit recommendations.
