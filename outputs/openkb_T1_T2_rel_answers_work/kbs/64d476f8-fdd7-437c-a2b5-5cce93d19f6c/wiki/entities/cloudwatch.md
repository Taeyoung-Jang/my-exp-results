---
sources: ["summaries/session-07_2025-04-06.md"]
type: "Product"
description: "AWS CloudWatch is a monitoring service for logs and metrics in AWS."
---

# AWS CloudWatch (product)

AWS CloudWatch is Amazon's monitoring and observability service that collects, aggregates, and stores logs, metrics, and events from AWS resources and applications.

## Role in the Session 7 Audit Guidance
- Listed as a **high‑value log source** for the quarterly audit bundle in the [[summaries/session-07_2025-04-06]] summary.
- Recommended to export **application log groups** for the audit period using a consistent time range (quarter + 7‑day buffer).
- Export format suggested: ZIP archive named `App_Logs_QX_YYYY.zip` containing `logStream`, `timestamp`, and `message` fields.
- The export is part of the overall **audit‑bundle** approach, which aims to centralize evidence in a single location.

## Integration with Other Tools
- Works alongside [[entities/cloudtrail]] (which captures API activity) to provide a complete view of infrastructure events.
- Logs are typically forwarded to [[entities/splunk]] for indexing and later queried with standardized SPL statements (see [[concepts/splunk-spl-standardization]]).
- Together with [[entities/aws]] services, CloudWatch helps implement [[concepts/compliance-automation]] by automatically capturing operational evidence without extra manual steps.

## Suggested SPL for Export (from the session guidance)
```spl
index=cloudwatch earliest=START latest=END source="/aws/lambda/..." 
| table _time logStream timestamp message
```
*This SPL follows the standardization patterns described in [[concepts/splunk-spl-standardization]].*

## Related Entities
- [[entities/aws]] – the broader cloud platform hosting CloudWatch.
- [[entities/cloudtrail]] – complementary service for API‑level audit logs.

---
*This entity page consolidates the key facts about AWS CloudWatch as presented in the session‑07 audit guidance.*