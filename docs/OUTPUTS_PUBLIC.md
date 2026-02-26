# Outputs Spec (Sanitized)
This document defines the public structure of CI Monitor outputs (MVP).
It describes what a report contains, not how it is produced.

---

## Output package (MVP)
A weekly run produces the following artifacts:

1) Executive Summary (EN + FR required)
2) Opportunity / Threat Backlog (EN MVP)
3) Change Log
4) Evidence Index
5) Coverage Report
6) Approval Record (gate before export)

Optional by policy later: RU/DE.

---

## 1) Executive Summary (EN + FR)
Purpose: a decision-ready snapshot for busy stakeholders.

Required sections:
- What changed since last run (top 3–7 items)
- Why it matters (impact framing)
- Recommended next actions (1–5 actions)
- Risks / uncertainties (explicit)

Rules:
- Facts must be backed by evidence (internally)
- Inferences must be labeled
- No unsupported "big claims"

---

## 2) Opportunity / Threat Backlog (EN, MVP)
Purpose: convert observations into trackable work.

Each item includes:
- Type: Opportunity / Threat
- Short title
- Description
- Impact: Low / Medium / High
- Confidence: Low / Medium / High
- Suggested action
- Owner (optional)
- Status: New / Open / In progress / Done / Parked
- Evidence reference (internally)

This backlog is designed to plug into product/marketing/strategy workflows.

---

## 3) Change Log
Purpose: a transparent record of detected changes.

Each entry includes:
- Date/time window
- What changed (plain language)
- Where it changed (category-level, not public sources)
- Evidence reference (internally)
- Notes (uncertainty, follow-ups)

---

## 4) Evidence Index
Purpose: prove traceability.

Public description:
- Evidence is stored as snapshots with timestamps and integrity checks.
- Each claim maps to one or more evidence items.

We do not publish operational collection details or source lists in public docs.

---

## 5) Coverage Report
Purpose: honest boundaries.

Includes:
- What we checked (categories)
- What we could not verify (and why)
- What is out of scope
- Confidence notes and known blind spots

Coverage gaps are explicitly shown, not hidden.

---

## 6) Approval Record (Export Gate)
Purpose: governance before anything leaves the system.

Includes:
- Approval status (approved / rejected)
- Reviewer (role label, not necessarily a personal identity)
- Timestamp
- Scope of approval (what is being exported/shared)
- Notes / conditions

By default, there is no automatic external export.

---

## Reporting language policy (public)
- MVP: Executive Summary EN+FR required
- Backlog: EN
- RU/DE: optional later by policy

---

## What is intentionally not described here
This public spec does not include:
- source lists or domains
- collection tactics
- internal configs, limits, or fingerprints
- client-specific logic
