# CocoaGadget Architecture Lab — Project Roadmap

## Purpose

This repository is a longitudinal engineering and architecture laboratory.

The portfolio is designed to develop and demonstrate technical judgment across:

- Data and analytics
- Data engineering
- Cloud
- Security and IAM
- Architecture
- Technology risk and controls
- AI systems
- Governance
- Resilience
- Documentation and decision-making

Projects are not intended to demonstrate isolated tools.

They are designed to show increasing ability to understand systems, identify problems, investigate failures, evaluate tradeoffs, and make defensible technical and business decisions.

---

# Project 1 — Healthcare Access Data & Operations Analysis

## Theme
Analyze & Establish Trust

## Core Question

Can I produce a trustworthy business conclusion from imperfect operational data?

## Business Context

Analyze healthcare access and referral operations to understand:

- Referral throughput
- Scheduling delays
- Operational bottlenecks
- Specialty/provider variation
- Patient access performance
- Whether operational targets are being met

## Primary Learning Objectives

### Data
- Explore and clean operational data
- Develop SQL skills
- Perform joins and aggregations
- Identify missing, duplicate, inconsistent, or questionable records
- Understand how data quality affects conclusions

### Architecture
- Identify where the data originates
- Document how information reaches the analytical layer
- Create a simple data-flow representation

### Controls
- Define basic validation checks
- Determine what should be verified before metrics are trusted
- Document reconciliation or quality checks

### Governance
- Identify ownership of important data and metric definitions
- Define terms such as "referral completed"
- Consider escalation when data cannot be trusted

### Judgment
- Distinguish what the evidence supports from what it does not support
- Communicate limitations
- Produce defensible management recommendations

## Development Principle

Project 1 should remain achievable.

It establishes the baseline for what correct joins, reasonable metrics, validation, clean-ish data, and defensible conclusions look like.

### Judgment Goal

**Trust carefully.**

---

# Project 2 — Data Architecture Failure Investigation

## Theme
Investigate & Control

## Core Question

Can I diagnose a failure propagating through a data architecture?

## Scenario

A data system begins producing suspicious or incorrect results.

The failure may involve intentionally introduced problems such as:

- Duplicates
- Missing values
- Schema drift
- Broken joins
- Invalid mappings
- Stale data
- Pipeline failures
- Incorrect transformations
- Dependency failures

The objective is not merely to clean the final dataset.

The objective is to trace the failure through the system.

## Investigation Method

Document:

1. Symptom
2. Investigation
3. Root cause
4. Downstream impact
5. Control or guardrail
6. Fix
7. Validation

## Architecture Questions

- Where did the failure originate?
- How did it propagate?
- Which downstream systems or metrics were affected?
- Why was the problem not detected earlier?
- What control should have detected or prevented it?
- How can recurrence be monitored?

## Judgment Goal

**Distrust intelligently.**

---

# Project 3 — Failing AI Implementation Evaluation

## Theme
Evaluate & Decide

## Core Question

Can I determine whether a failing technology implementation should continue?

## Scenario

An organization has invested in an AI solution that is not producing the expected results.

Management must decide whether to:

- Continue
- Remediate
- Redesign
- Restrict
- Replace
- Decommission

## Investigation Areas

Evaluate:

- Original business objective
- Expected benefits
- Actual performance
- Data quality
- Model/system performance
- Integration architecture
- Workflow fit
- User adoption
- Security
- IAM/access
- Controls
- Governance
- Vendor dependency
- Cost
- Operational risk
- Regulatory/compliance considerations

## Decision Questions

- Is the technology itself failing?
- Is the underlying data inadequate?
- Is the integration poorly designed?
- Is the workflow inappropriate?
- Are controls insufficient?
- Is the vendor failing to meet requirements?
- Was the original business case flawed?
- Can the system be remediated?
- At what cost and risk?
- Is continued investment justified?

## Judgment Goal

**Decide under uncertainty.**

---

# Opening Portfolio Progression

Project 1:
**Analyze & Establish Trust**

Can I trust this?

↓

Project 2:
**Investigate & Control**

Something is wrong. Can I determine why?

↓

Project 3:
**Evaluate & Decide**

Now that I understand the problem, what should the organization do?

---

# Longitudinal Critical-Infrastructure Architecture Laboratory

## Purpose

This project is intentionally designed to evolve over multiple years.

Unlike the shorter portfolio projects, it does not have a traditional final state.

The system will age as my technical knowledge and the technology environment change.

## Lifecycle

Design → Build → Operate → Observe → Reassess → Accumulate Technical Debt → Investigate → Modernize → Migrate → Decommission

## Areas That May Evolve Over Time

- Data architecture
- Cloud infrastructure
- Networking
- IAM
- Cybersecurity
- AI components
- Data lineage and dependencies
- Vendor dependencies
- Legacy/orphaned technology
- Technical debt
- Observability
- Resilience and availability
- Governance
- Technology risk
- Cryptographic inventory
- Crypto-agility
- Post-quantum cryptography migration

## Historical Record

Earlier designs will NOT be rewritten to make them appear more sophisticated than they originally were.

The repository should preserve:

- Original architecture
- Original assumptions
- Architecture Decision Records (ADRs)
- Mistakes
- Failed approaches
- Contemporary reasoning
- Documentation
- Changes in technical judgment
- Later critiques of earlier decisions

The purpose is to demonstrate maturation over time.

---

# Portfolio Principle

These projects are not primarily demonstrations of tools.

Tools will change.

The portfolio is intended to demonstrate increasingly sophisticated:

**Technical judgment.**

The progression is:

**Trust carefully → Distrust intelligently → Decide under uncertainty → Architect for change.**
