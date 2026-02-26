# Security Overview (Sanitized)
This document summarizes the security posture and threat-model principles for CastelDazur CI Monitor.
It is intentionally high-level and does not disclose implementation tactics, configs, or sensitive operational details.

---

## 1) Security goals
We protect:
- Confidentiality: client data, internal notes, and any non-public artifacts
- Integrity: evidence artifacts must be tamper-evident
- Availability: the weekly workflow should run reliably and fail safely

---

## 2) What we consider sensitive
Never published in public logs/docs:
- source lists, domains, URLs, identifiers
- client names, datasets, credentials, tokens, keys
- operational limits, allowlists, fingerprints, environment details
- any screenshots that leak metadata (tabs, bookmarks, file paths, account IDs)

Public materials are sanitized by default.

---

## 3) Threat model (high level)
We design against:
- Data leakage (accidental or intentional)
- Unauthorized access (accounts, repos, machines)
- Evidence tampering (modifying artifacts after capture)
- Supply-chain risks (dependencies, scripts, CI/CD exposure)
- Social engineering (phishing, impersonation, credential theft)
- Misuse risk (turning the system into "scraping / evasion tooling")

---

## 4) Security posture principles
### Separation of concerns
- Public repo: sanitized principles, structure, weekly logs
- Private repo / private storage: full specs, internal docs, configs

### Least privilege
- Access is granted only to the minimum scope needed
- Secrets never appear in code, commits, screenshots, or tickets

### Fail-safe defaults
- If a step cannot run safely/compliantly, it becomes a coverage gap
- No automatic export by default (approval gate required)

---

## 5) Integrity & auditability (conceptual)
We treat evidence as governance artifacts:
- artifacts are time-stamped
- integrity checks are used to detect tampering
- changes are tracked with an explicit change log

Public docs describe the concept, not the mechanism.

---

## 6) Handling incidents (high level)
If we suspect leakage or unauthorized access:
1) Contain: revoke access, rotate secrets, disable affected integrations
2) Assess: identify scope and impacted artifacts
3) Remediate: patch, rotate, re-issue, and harden controls
4) Document: record what happened and what changed
5) Prevent: add guardrails to avoid recurrence

---

## 7) Responsible disclosure
If you believe you found a vulnerability:
- Please report privately (do not open a public issue with details)
- Include: what you found, impact, and reproduction steps (if safe)

We will acknowledge and respond, prioritizing user safety and confidentiality.

---

## 8) What this document does NOT include
To protect users and prevent misuse, we do not publish:
- exploitation steps
- bypass or evasion techniques
- hardening "recipes" tied to specific stacks
- operational runbook details
