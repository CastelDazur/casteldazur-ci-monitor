# Public Policy (Sanitized)
This document defines what CastelDazur CI Monitor does, does not do, and how we communicate results publicly.

It is intentionally high-level and does not expose operational details.

---

## 1) Evidence-first rule
**No proof → no claim.**

Every factual statement in a report must map to evidence (e.g., a snapshot) or be explicitly labeled as:
- Inference (reasoned conclusion based on evidence)
- Assumption (not verified; treated cautiously)
- Unknown (coverage gap)

---

## 2) Coverage honesty
We do not pretend to have full visibility.

Every run must include a Coverage Report describing:
- what was checked
- what could not be checked (and why)
- what is out of scope

Coverage gaps are not hidden. They are part of the output.

---

## 3) Approval gate before export
We treat CI outputs as governance artifacts.

Exports / downloads / external sharing require an approval gate:
- human review
- explicit sign-off
- clear responsibility for what leaves the system

No "auto-export by default".

---

## 4) Local-first by default
Default mode is on-prem / local-first:
- minimal data movement
- predictable performance baseline
- better control of sensitive workflows

Cloud usage is opt-in only and never required for the core workflow.

---

## 5) Hard boundaries (we refuse)
We do not build or publish workflows that include:
- CAPTCHA bypass or evasion
- ignoring robots restrictions
- covert or stealth collection designed to avoid detection
- credential harvesting, session hijacking, or any form of unauthorized access
- "gray zone" automation that violates platform rules

If a source is not accessible in a compliant way, it becomes a coverage gap, not a target.

---

## 6) Privacy & confidentiality in public materials
Public build logs and docs are sanitized:
- no client names
- no source lists / domains / URLs
- no internal rate limits, allowlists, fingerprints, or configs
- no secrets, tokens, keys, or environment details
- no screenshots that reveal sensitive metadata

If it's not safe to publish, it stays private.

---

## 7) Communication standards
When we communicate results, we prioritize clarity over persuasion:
- separate facts from interpretation
- show evidence references (internally) and describe evidence categories (publicly)
- keep claims proportional to coverage

The goal is decision support, not "winning an argument".

---

## 8) What this repo represents
This public repository is a build-in-public surface:
- principles and boundaries
- report structure promises
- weekly sanitized progress notes

Operational implementation details remain private.
