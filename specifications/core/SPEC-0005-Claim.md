# SPEC-0005 — Claim

## Status

Approved

---

# Purpose

A Claim is an assertion derived from one or more Observations and supported by Evidence.

Claims transform observed facts into conclusions that can be evaluated, challenged, and validated.

---

# Definition

A Claim is a canonical object that expresses a conclusion, interpretation, or assertion based upon one or more Observations whose credibility is supported by one or more Evidence records.

Claims are not observations.

Claims are reasoned statements built upon observations.

---

# Characteristics

Every Claim:

* References one or more Observations.
* Is supported by one or more Evidence records.
* Represents an assertion or conclusion.
* May later be validated or rejected.
* May change as new observations or evidence become available.

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

Claims depend upon Observations.

Evidence strengthens Claims by supporting the underlying Observations.

Validation evaluates Claims.

---

# Constraints

* A Claim cannot exist without at least one Observation.
* A Claim should reference supporting Evidence.
* Multiple Claims may reference the same Observation.
* Claims may later be confirmed, revised, or rejected through Validation.

---

# Examples

## Example 1

Observation

Apple FY2024 Revenue = USD 391 Billion

Claim

Apple is among the world's largest technology companies by revenue.

---

## Example 2

Observation

Quarterly revenue has increased for eight consecutive quarters.

Claim

The company's revenue growth trend is positive.

---

# Design Principles

Claims represent reasoning.

They are not direct observations.

They remain open to revision as new observations and evidence become available.

---

# Rationale

Separating Claims from Observations enables Tindex to distinguish between recorded facts and reasoned conclusions.

This distinction supports explainable AI, evidence-based reasoning, human review, and transparent decision-making.
