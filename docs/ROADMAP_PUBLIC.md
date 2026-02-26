# Roadmap (Public, Milestone-Based, Sanitized)

This roadmap is intentionally milestone-based (not date-based).
Reason: some milestones depend on hardware assembly and supply constraints.

We will publish progress weekly via docs/updates/ and issues labeled weekly-log.

---

## Guiding principles
- No proof → no claim
- Coverage honesty (Coverage Report is mandatory)
- Approval gate before export
- Local-first by default (cloud opt-in)

---

## Milestone 1 — Public foundation (Vitrine)
Goal: make the public repo understandable and trustworthy without exposing secrets.

Scope:
- [ ] Public docs set (overview, policy, outputs, security, glossary, FAQ)
- [ ] Weekly update structure docs/updates/)
- [ ] Issue templates + labels for build logs

Success criteria:
- A newcomer can understand what CI Monitor is, what it outputs, and what it refuses to do in <10 minutes.

---

## Milestone 2 — Report skeleton + governance (No-hardware required)
Goal: define stable report structure and governance rules before implementation.

Scope:
- [ ] Report templates (Executive Summary EN+FR, Backlog, Change Log, Coverage Report)
- [ ] Approval gate flow definition (what "approved" means)
- [ ] "Sanitized demo pack" structure (no real sources)

Success criteria:
- We can produce a fully formatted report package from synthetic / mock inputs.

---

## Milestone 3 — Evidence & change-tracking concept demo (Sanitized)
Goal: demonstrate the concept of evidence indexing and change tracking safely.

Scope:
- [ ] Example Evidence Index (synthetic identifiers, no domains/URLs)
- [ ] Example Change Log (synthetic "diff" events)
- [ ] Example Coverage Report (explicit unknowns)

Success criteria:
- Public demo shows traceability and honesty without revealing operational collection details.

---

## Milestone 4 — Hardware baseline (Dependent milestone)
Goal: validate predictable runtimes and performance assumptions.

Status:
- This milestone depends on hardware assembly and is subject to delivery/availability.

Scope (high level):
- [ ] Assemble local-first baseline
- [ ] Run safe benchmarks (sanitized; no sensitive inputs)
- [ ] Publish a performance note (high-level metrics only)

Success criteria:
- We can run an end-to-end demo workflow with stable throughput on local hardware.

---

## Milestone 5 — Private pilot readiness (By request)
Goal: be ready for a private pilot on client infrastructure.

Scope:
- [ ] Private deployment checklist
- [ ] Governance checklist (approval + audit expectations)
- [ ] Support boundaries & operating model (sanitized public summary)

Success criteria:
- A pilot can run on client hardware with clear rules, responsibilities, and safe defaults.

---

## What we will NOT accelerate for speed
To protect users and prevent misuse, we will not publish:
- source lists/domains/URLs
- operational configs, rate limits, allowlists/fingerprints
- bypass/evasion tactics (CAPTCHA/robots)
- any client-specific details

---

## How to request a pilot
Open a GitHub issue titled:
**"Pilot request — CI Monitor"**

Keep details high-level in public; specifics can be handled privately.
