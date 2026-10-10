---
type: "Concept"
sources: ["summaries/session-39_2025-02-15.md"]
description: "Identifies app permission requests that signal potential privacy or security risks."
---

# Permission Red Flags

**Definition**: Permission red flags are requests for device or data access that do not align with an app's stated functionality, indicating potential privacy or security concerns.

---

## Overview
Permission red flags serve as quick visual cues during the **pre‑install checklist** to help users decide whether an app merits further consideration. They complement other **app trust signals** such as developer reputation, recent updates, and authentic reviews.

---

## Common Red‑Flag Permissions
| Permission | Why it can be a red flag | Typical legitimate use |
|------------|--------------------------|-----------------------|
| **Location** | Requested by apps that have no spatial component (e.g., note‑taking, reading apps). | Maps, delivery, ride‑hailing, weather.
| **Contacts** | Unnecessary for most utilities; may be used for data harvesting. | Messaging, social networking, caller ID.
| **Photos/Media** | Requested by apps that do not involve image capture or editing. | Photo editors, social media, scanning apps.
| **Microphone** | Rarely needed outside communication or recording apps. | Calls, voice assistants, audio recorders.
| **SMS/Call logs** | Often abused for verification bypass or advertising. | Messaging, two‑factor authentication.

---

## Contextual Relevance
A permission is only a red flag when its purpose cannot be justified by the app’s primary function. Users should **deny** such requests initially and only grant them if a clear, contextual need arises during use.

---

## Role in the Pre‑Install Checklist
During the rapid mental script described in [[concepts/pre_install_checklist]], users should:
1. Scan the app description and screenshots for implied permission needs.
2. Flag any listed permissions that seem unrelated.
3. Use these flags as part of the overall **risk flag system** to decide whether to install.

---

## Connection to App Trust Signals
Permission red flags are a subset of broader trust signals. Even if an app scores well on developer reputation and update recency, a mismatch between requested permissions and functionality can outweigh those positives.

---

## Example from [[summaries/session-39_2025-02-15]]
In the conversation, the assistant highlights that a **notes app asking for location** is an immediate dealbreaker, while a **maps or delivery app** requesting location is acceptable. This illustrates how contextual relevance determines whether a permission becomes a red flag.

---

## Practical Tips
- **Deny first**: Install the app, then reject all permission prompts until you encounter a feature that justifies a request.
- **Re‑evaluate**: If an app repeatedly pushes for unrelated permissions, consider uninstalling.
- **Document**: Keep a mental note of red‑flag permissions encountered to refine your future pre‑install assessments.
