---
type: "Concept"
sources: ["summaries/session-06_2024-06-15.md"]
description: "Managing a dedicated secondary SIM for long‑term, privacy‑preserving SMS 2FA."
---

# Secondary SIM Management

**Definition**: A set of practices for acquiring, maintaining, and securing a dedicated mobile line used solely for verification texts and SMS‑based two‑factor authentication (2FA).

## Core Practices

1. **Choose a low‑cost, always‑on plan**
   - Select a reputable carrier and a cheap monthly plan that renews automatically. This prevents the line from becoming inactive, which is the main trigger for number recycling.
2. **Secure the carrier account**
   - Set a strong carrier PIN or password.
   - Avoid using easily guessable personal details for support verification questions.
3. **Periodic activation**
   - Power the device on at least once a month to confirm the line is active and to spot unexpected messages.
4. **Document usage**
   - Keep a record of which online services rely on the secondary number for SMS 2FA.
5. **Backup and fallback**
   - Store recovery codes in a password manager.
   - Where possible, add an authenticator app or hardware key as an additional 2FA method.

## Risks & Mitigations

- **Number recycling**: Occurs when a line lapses or remains unused for extended periods. Mitigate by maintaining continuous billing and occasional use.
- **SIM‑swap attacks**: Reduce risk by keeping the number private, securing the carrier account with a PIN, and not advertising the number publicly.
- **Carrier policy changes**: Monitor carrier communications for plan or number‑management policy updates.

## Relationship to Other Concepts

- This management approach supports broader [[concepts/online_privacy]] goals by keeping a real mobile number out of everyday use.
- It is a practical implementation detail for [[concepts/two_factor_authentication]] when SMS is the only available method.

## Source

The practices described here are drawn from the discussion in [[summaries/session-06_2024-06-15]].