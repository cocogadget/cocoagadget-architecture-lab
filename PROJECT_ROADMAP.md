# CocoaGadget Architecture Lab — Project Roadmap

## Purpose

This repository is a longitudinal engineering and architecture laboratory.

# Opening Portfolio Progression

Project 1:
**Engineer & Establish Trust**

Can I turn imperfect source data into a trustworthy data product?

↓

Project 2:
**Investigate & Control**

Something is wrong. Can I determine where the failure originated, how it propagated, and how to prevent recurrence?

↓

Project 3:
**Evaluate & Decide**

Now that I understand the system and its failures, what should the organization do?


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
# Project 1 — Healthcare Patient Access Data Pipeline

## Theme

Engineer & Establish Trust

## Core Question

Can I transform imperfect healthcare operational data into a trustworthy, analysis-ready data product?

## Business Context

Build a healthcare patient-access data pipeline that integrates operational data related to:

* Referrals
* Appointments and scheduling
* Providers and specialties
* Patient access events
* Insurance or authorization activity
* Operational targets and service levels

The project will begin with imperfect source data and progressively create a validated, transformed, and curated data layer that can support reliable downstream analysis.

## Primary Learning Objectives

### Data Engineering

* Ingest operational data from multiple source files or tables
* Develop and strengthen SQL skills
* Perform joins, transformations, and aggregations
* Standardize fields and data types
* Identify and handle missing, duplicate, inconsistent, or invalid records
* Apply business rules during transformation
* Create staged and curated datasets
* Validate record counts and transformation results
* Prepare trusted data for downstream analytical use

### Architecture

* Identify where each source dataset originates
* Document movement from source data to ingestion, staging, transformation, and curated layers
* Create a data-flow representation
* Define relationships and dependencies between datasets
* Begin documenting data lineage

### Data Quality & Controls

* Define validation checks at important pipeline stages
* Detect duplicates, nulls, invalid values, and broken relationships
* Reconcile source and transformed record counts where appropriate
* Determine what must be verified before curated data is released for use
* Document failed quality checks and remediation decisions

### Governance

* Identify ownership of important data elements
* Define important business terms such as "referral completed"
* Document metric and transformation definitions
* Consider access, sensitivity, and appropriate use of healthcare operational data
* Define escalation when data cannot be trusted

### Analytics

* Use the curated data layer to answer selected healthcare access questions
* Evaluate referral throughput, scheduling delays, bottlenecks, and operational performance
* Demonstrate that downstream conclusions are supported by engineered and validated data

### Judgment

* Distinguish source-data problems from transformation problems
* Determine when data is sufficiently trustworthy for downstream use
* Communicate limitations and unresolved quality issues
* Explain technical decisions in business language
* Produce defensible recommendations based on validated data

## Initial Data Flow

**Source Data → Raw/Ingested → Validated/Staged → Transformed → Curated → Analytics**

Each layer should have a clear purpose.

The analytical output is not the primary product.

The primary product is the **trusted data pipeline and curated data layer that make reliable analysis possible.**

## Development Principle

Project 1 should remain achievable and evolve with my technical skills.

The first version may use simple files, SQL, and manual execution.

As my capabilities increase, the project may later incorporate:

* Python
* PySpark
* Automated pipelines
* Databricks
* Lakehouse architecture
* Orchestration
* Monitoring
* Additional governance and security controls

Earlier versions should be preserved where useful to demonstrate technical growth.

### Judgment Goal

**Engineer trust.**


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

## Future Job-Posting-Inspired Engineering Builds

These projects are inspired by real engineering problems described in job postings.

The goal is not to reproduce a company's proprietary systems. Each project will build a small, original system around the underlying engineering problem in order to practice system design, data engineering, reliability, testing, documentation, and technical decision-making.





### Instacart-Inspired Virtual Store / Digital Twin

**Theme:** Physical World → Data → Digital State

Build a simplified virtual representation of a physical retail store and the data pipelines required to keep that representation synchronized with changing real-world conditions.

The project will explore how observations from a physical environment can be ingested, validated, transformed, reconciled, and used to maintain a trustworthy digital representation of current store state.

#### Core Questions

- How should physical store entities such as products, shelves, inventory, and locations be represented as data?
- How does new observational data update the digital state?
- How can discrepancies between expected and observed state be detected?
- What happens when observations are missing, duplicated, delayed, or contradictory?
- How can the system determine whether its current representation can be trusted?

#### Engineering Concepts

- Data modeling
- Batch and/or event ingestion
- Data pipelines
- State management
- Data validation
- Reconciliation
- Data quality
- Observability
- Failure handling
- Documentation and lineage

#### Planned Failure Scenarios

The project will intentionally introduce problems such as:

- Duplicate observations
- Missing observations
- Stale inventory data
- Invalid product identifiers
- Conflicting state updates
- Delayed events
- Schema changes

Failures will be detected, investigated, repaired, validated, and documented.

#### Goal

Demonstrate the ability to build a small data system that translates changing real-world conditions into a reliable digital representation.

---

### Pinterest-Inspired Data Pipeline / Warehouse Authoring System

**Theme:** Raw Data → Reliable Data Products

Build a small data platform that ingests raw data, transforms it into trusted analytical datasets, tests data quality, and makes the resulting data available for downstream analysis.

The project will focus not only on creating a successful pipeline, but also on understanding how the system behaves when something goes wrong.

#### Core Questions

- How does raw data enter the system?
- How should transformations be organized and documented?
- How can data quality be tested automatically?
- How should dependencies between transformations be managed?
- What happens when a pipeline partially fails?
- How can failed processing be safely restarted?
- How can another engineer understand and operate the system?

#### Engineering Concepts

- Data ingestion
- SQL transformations
- Data modeling
- ELT/ETL
- Pipeline orchestration
- Dependency management
- Data quality testing
- Logging and observability
- Failure recovery
- Idempotency
- Documentation and lineage

#### Planned Failure Scenarios

The project will intentionally introduce problems such as:

- Broken joins
- Duplicate records
- Missing values
- Schema drift
- Invalid mappings
- Failed transformations
- Late-arriving data
- Partial pipeline failures

Each failure will be traced from symptom to root cause, repaired, validated, and documented.

#### Independent Handoff Test

The completed system should contain enough documentation, logging, lineage, and operational guidance that another technically competent person can:

1. Understand what the pipeline is intended to do.
2. Determine where a failure occurred.
3. Identify the affected data.
4. Safely repair or restart processing.
5. Validate that the system has recovered.

#### Goal

Demonstrate the ability to build, operate, troubleshoot, and document a maintainable data pipeline rather than simply producing a successful final dataset.







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
