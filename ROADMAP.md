# CocoaGadget Architecture Lab — Roadmap

> **I had a question. So I built a world where I could find out.**

CocoaGadget is a long-running technical laboratory for investigating how
data, infrastructure, and organizations behave when reality stops
cooperating with the design.

The roadmap is organized around four laboratories.

The problems determine the tools.

---

## 01 — Data Forensics

### Question
**What happened?**

Investigate systems from incomplete, conflicting, or uncertain evidence.

Work may involve:

- SQL and data investigation
- data quality and reconciliation
- lineage and dependency discovery
- logs and system evidence
- vendor and third-party dependencies
- decommissioning
- retention and deletion
- IAM and access
- incident reconstruction
- evidence confidence

### Current Investigation

**The Data That Refuses to Die — In Development**

A third-party AI system has supposedly been decommissioned and its
customer data removed.

The assignment:

**Prove it.**

---

## 02 — AI Archaeology

### Question
**What did we inherit?**

A longitudinal experiment involving an organization whose original
technical team is gone while its systems remain.

The work is to discover what exists, reconstruct how it works,
identify dependencies and ownership, determine what can be trusted,
and decide what can safely change.

This environment will evolve over time.

Earlier decisions will not be rewritten.

The world remembers what happened.

---

## 03 — Data Center Reliability

### Question
**How do we keep it operating?**

Build and investigate a simulated data-center environment involving:

- compute
- storage
- networking
- power
- cooling
- workloads
- telemetry
- capacity
- dependencies
- reliability
- recovery

Failures and changing operating conditions will be introduced as the
environment develops.

---

## 04 — Critical Infrastructure

### Question
**How do we protect and modernize systems society cannot afford to lose?**

A longitudinal architecture laboratory exploring systems such as
water, energy, industrial infrastructure, and other environments where
technical failures can produce physical consequences.

Areas may include:

- legacy architecture
- IT/OT dependencies
- data architecture
- resilience
- modernization
- vendor dependencies
- security and IAM
- governance
- cryptographic inventory
- crypto-agility
- post-quantum migration

---

# Investigation Method

The laboratories generally follow:

**Build → Observe → Break → Investigate → Remediate → Retest → Document**

The sequence may change when the evidence requires it.

A successful query is not proof that a conclusion is true.

A successful remediation is not proof that the problem is solved.

System restoration is not necessarily recovery.

---

# Evidence

Findings should distinguish between:

**KNOWN / VERIFIED**

Supported directly by available evidence.

**INFERRED / PROBABLE**

Supported by evidence but not conclusively established.

**UNKNOWN**

Evidence is insufficient.

**CONFLICTING**

Available evidence supports incompatible conclusions.

---

# Independent Handoff Test

Where appropriate, completed work should allow another technically
competent person to:

1. Understand what the system is intended to do.
2. Understand its important dependencies.
3. Reconstruct what happened.
4. Identify unresolved risks or uncertainty.
5. Continue the work without depending on undocumented knowledge.

**Recovery is complete only when the work is finished or the remaining
work is safe to inherit.**

---

# Historical Record

Earlier work will remain visible.

SQL investigations, healthcare data work, automation projects,
incorrect assumptions, failed approaches, corrections, and earlier
architecture decisions are part of the laboratory record.

Future work should not rewrite earlier decisions to make them appear
more sophisticated than they were.

When judgment changes, document why.

---

# Technical Development

Tools are introduced when the problem requires them.

Current and future work may involve:

`SQL` · `Python` · `Databricks` · `Spark` · `Linux` · `Git` ·
`Cloud` · `APIs` · `IAM` · `Containers` · `Observability`

This is not a checklist.

The objective is not to collect tools.

The objective is to develop the ability to understand systems,
investigate their behavior, make defensible decisions, and safely
change them.

---

# Principle

**Service. Stewardship.**

**Trustworthy AI requires trustworthy data.**
