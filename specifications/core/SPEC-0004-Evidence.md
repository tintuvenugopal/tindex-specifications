# SPEC-0004 — Evidence

## Status

Approved

---

# Purpose

Evidence provides the justification that increases confidence in an Observation.

While an Observation records what was observed, Evidence explains why that Observation should be trusted.

---

# Definition

Evidence is a canonical object that supports one or more Observations by providing verifiable justification for their accuracy, reliability, or authenticity.

Evidence does not create Observations.

Evidence strengthens confidence in existing Observations.

---

# Characteristics

Every Evidence record:

* References one or more Observations.
* Provides supporting justification.
* May reference one or more external sources.
* May vary in strength or reliability.
* Can support multiple Claims.

---

# Relationships

Entity

↓

Property

↓

Observation

↓

Evidence

↓

Claim

↓

Validation

Evidence depends upon one or more Observations.

Claims depend upon Evidence.

---

# Constraints

* Evidence cannot exist without at least one Observation.
* Evidence never changes the content of an Observation.
* Multiple Evidence records may support the same Observation.
* Evidence may support multiple Claims.

---

# Examples

## Example 1

Observation

Apple FY2024 Revenue = USD 391 Billion

Evidence

Apple Annual Report 2024

Audited Financial Statements

Page 34

---

## Example 2

Observation

CEO changed on 2025-04-01

Evidence

Official stock exchange announcement

Company press release

Regulatory filing

---

# Design Principles

Evidence increases confidence.

It does not guarantee truth.

Evidence is separate from validation because confidence and correctness are different concepts.

---

# Rationale

Separating Evidence from Observation enables Tindex to preserve factual observations independently from the reasons those observations are considered trustworthy.

This separation supports auditing, provenance, multiple supporting sources, and evidence-based reasoning while keeping the canonical model simple and extensible.
