# CastelDazur CI Monitor (Sanitized Overview)

**CastelDazur Systems** builds local-first AI systems on your hardware.  
This repo is the public, sanitized build log for our first product: CI Monitor.

---

## What it does
CI Monitor is a weekly workflow that produces competitive intelligence only when claims are backed by evidence.

Core idea:
- Evidence snapshot (proof)
- Change tracking (what changed since last run)
- Coverage report (what we could NOT verify)
- Approval gate (review before export)

---

## Why it exists
Most CI outputs fail for one of these reasons:
1) They are not reproducible
2) They mix facts with assumptions without labeling
3) They hide what they didn't cover

CI Monitor is built to fix that:
- If we cannot prove it, we don't claim it
- If we cannot cover it, we say it explicitly

---

## Who it's for
Teams that track competitors on a cadence (weekly / bi-weekly), such as:
- marketing & growth teams
- e-commerce operators
- consulting and strategy teams

Typical focus:
- positioning changes
- product/pricing updates
- messaging shifts
- new landing pages / offers
- major announcements

---

## Outputs (MVP)
Public promise (structure only):
- Executive Summary: EN + FR (required)
- Opportunity/Threat Backlog: EN (MVP)
- Evidence Index (proof list)
- Change Log (diff highlights)
- Coverage Report (honest limits)
- Approval Gate before export/download

Optional later by policy: RU/DE.

---

## Local-first by default
We default to running on local infrastructure:
- predictable performance baseline
- sensitive workflows remain on-prem
- cloud is opt-in, never mandatory

*(This public repo does not include operational configs.)*

---

## Non-goals & boundaries
We explicitly do not build:
- CAPTCHA bypass workflows
- methods to ignore robots restrictions
- stealth scraping or covert collection
- public docs that disclose sources, client lists, or private configs

---

## Build-in-public rhythm
We publish sanitized weekly notes:
- docs/updates/ — narrative weekly updates
- Issues labeled weekly-log — short status + decisions

If you want a private pilot on your infrastructure, open an issue:
**"Pilot request — CI Monitor"**
