---
type: "Concept"
sources: ["summaries/session-34_2024-07-20.md", "summaries/session-07_2022-07-20.md"]
description: "OKRs designed with clear attribution and evidence to survive performance reviews."
---

# Review‑Proof OKRs

**Definition**: Review‑proof OKRs are objectives and key results written so that the owner’s individual contribution is unmistakable, and the evidence needed for a performance review is captured continuously.

---

## Why They Matter
- Aligns with an **IC track ambition** by emphasizing personal technical impact rather than team‑wide outcomes that could be attributed to others.
- Supports **technical‑leadership‑without‑management** by framing leadership actions (design, architecture, automation) as owned deliverables.
- Provides a concrete narrative for managers and reviewers, reducing ambiguity about who drove the results.

---

## Core Principles (derived from [[summaries/session-07_2022-07-20]])
1. **Ownership‑focused verbs** – Use “lead”, “drive”, “design”, “implement”, or “author” to highlight personal agency.
2. **Measurable, individual‑controlled metrics** – Choose KR metrics that you can directly influence (e.g., latency reductions you engineered, incidents you mitigated, cost savings from changes you authored).
3. **Pre‑planned evidence** – Define the artefacts you will collect up‑front (dashboards, incident reports, design‑doc approvals, adoption stats).
4. **Attribution safeguard** – Phrase KRs so that even if other teams contribute, the KR still reads “as a result of my leadership on …”.

---

## Evidence Checklist
| Evidence Type | Where to Store | Example Source |
|---------------|----------------|----------------|
| Latency / throughput dashboards | Shared Grafana folder | Before/after charts for the workflow improvement |
| Incident statistics | SRE ticketing system export | Monthly incident‑volume reduction report |
| Design doc links | Confluence or repo README | ADR with approval comments |
| Adoption metrics | GitHub PR labels or internal surveys | Number of teams using the new standard |
| Ownership log | Personal markdown file or wiki page | Chronological notes of shipped components |

---

## Sample Review‑Proof OKR (Distributed‑Systems)
**Objective:** Strengthen the reliability and performance of the core distributed workflow while increasing my technical ownership.

**Key Results**
- Lead latency improvements that achieve a **25 % reduction in p99 latency** (tracked via Grafana).
- Drive reliability work that cuts workflow‑related incidents by **30 %** (incident reports).
- Author and ship **two design proposals** that are adopted by the team (design‑doc approvals).
- Publish onboarding documentation making me the **primary point of contact** (doc link and usage metrics).

---

## Sample Review‑Proof OKR (Platform Engineering)
**Objective:** Increase platform reliability and efficiency through a high‑impact infrastructure initiative.

**Key Results**
- Cut recurring platform incidents by **20‑25 %** (incident dashboard).
- Implement an **auto‑recovery mechanism** that resolves a major failure class autonomously (deployment logs).
- Reduce compute/storage cost by **10‑15 %** while meeting SLA (cost‑explorer snapshots).
- Define new SLOs and achieve **>99.9 % availability** for two consecutive quarters (SLO reports).

---

## Linking to Entities
- The distributed‑systems example directly relates to the [[entities/distributed-systems]] domain.
- The platform‑engineering example is scoped to [[entities/platform-engineering]].

---

## Further Reading
- [[concepts/ic-track-ambition]] – How to frame ambition without management.
- [[concepts/technical-leadership-without-management]] – Ways to demonstrate leadership through technical ownership.
- [[summaries/session-07_2022-07-20]] – Original conversation that introduced the concept.


See also: [[summaries/session-34_2024-07-20]]