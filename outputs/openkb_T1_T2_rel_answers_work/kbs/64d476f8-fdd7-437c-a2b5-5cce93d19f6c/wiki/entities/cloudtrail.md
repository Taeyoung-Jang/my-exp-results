---
sources: ["summaries/session-07_2025-04-06.md"]
type: "Product"
description: "AWS CloudTrail records API activity for audit purposes."
---

# AWS CloudTrail

## Overview
AWS CloudTrail is an AWS service that records API calls and account activity across AWS services, providing a comprehensive audit log.

## Role in Compliance Automation
In the session-07_2025-04-06, CloudTrail logs were identified as a core log source for the quarterly audit bundle. The SPL query standardizes extraction of CloudTrail events for compliance purposes, aligning with [[concepts/compliance-automation]] and the [[concepts/audit-bundle]] approach.

## Standardized SPL Extraction
The recommended Splunk SPL (see [[concepts/splunk-spl-standardization]]) pulls events from the `cloudtrail` index, filters by key services (EC2, IAM, S3, CloudFormation), and outputs a stable table of fields such as `_time`, `eventName`, `eventSource`, `awsRegion`, `userIdentity`, `requestParameters`, `responseElements`, `sourceIPAddress`, and `userAgent`.

## Integration with Other Tools
CloudTrail data is typically forwarded to [[entities/splunk]] for centralized analysis and combined with logs from [[entities/cloudwatch]] for application‑level visibility. It complements identity logs from [[entities/okta]] and code change records from [[entities/github]] and [[entities/jira]] in the audit bundle.

## References
- Session summary: [[summaries/session-07_2025-04-06]]
- Related AWS service: [[entities/aws]]