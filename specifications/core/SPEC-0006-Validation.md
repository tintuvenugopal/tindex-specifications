# SPEC-0006 — Validation

## Status

Approved

---

# Purpose

Validation evaluates the credibility and correctness of a Claim based on the available Observations and supporting Evidence.

Validation completes the reasoning process by recording whether a Claim is accepted, rejected, revised, or remains inconclusive.

---

# Definition

A Validation is a canonical object that records the outcome of evaluating one or more Claims using available Observations, supporting Evidence, and a defined validation method.

Validation represents an assessment.

It does not create Observations, Evidence, or Claims.

It evaluates them.

---

# Characteristics

Every Validation:

* References one or more Claims.
* Is performed using a defined validation method.
* Produces a recorded outcome.
* May include supporting rationale.
* Is itself subject to future review if new information becomes available.

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

Validation depends upon one or more Claims.

Claims depend upon Observations and Evidence.

---

# Constraints

* A Validation cannot exist without at least one Claim.
* Validation never changes the historical Observation.
* Validation records an evaluation, not a fact.
* Multiple independent Validations may exist for the same Claim.

---

# Examples

## Example 1

Claim

Apple is among the world's largest technology companies by revenue.

Validation

Accepted

Method

Comparison with audited financial statements and industry rankings.

---

## Example 2

Claim

Company revenue declined during FY2024.

Validation

Rejected

Reason

Supporting Observations demonstrate revenue increased compared to FY2023.

---

# Design Principles

Validation evaluates reasoning.

It does not create reasoning.

Validation remains open to revision when new Observations or Evidence become available.

---

# Rationale

Separating Validation from Claim preserves a clear distinction between making an assertion and evaluating that assertion.

This enables transparent review, explainable AI, institutional learning, and continuous improvement while maintaining a stable canonical object model.
