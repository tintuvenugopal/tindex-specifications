# SPEC-0003 — Observation

## Status

Approved

---

# Purpose

An Observation records that an Entity possessed a particular Property with a particular value at a specific point or period in time.

Observations transform abstract Properties into concrete facts that can be reasoned about.

Without Observations, Entities and Properties define only what *can* exist.

Observations record what *was actually observed*.

---

# Definition

An Observation is the canonical record that an Entity exhibited a specific Property with a specific value within a defined temporal context.

Observations represent knowledge acquired from reality.

They do not by themselves establish truth or trustworthiness.

Those concerns belong to Evidence and Validation.

---

# Characteristics

Every Observation:

* References exactly one Entity.
* References exactly one Property.
* Records one observed value.
* Occurs at a specific point or period in time.
* May later be supported by one or more Evidence records.
* May later support one or more Claims.

---

# Examples

## Example 1

Entity

Company: Apple

Property

Revenue

Observation

Revenue = USD 391 Billion

Reporting Period

FY2024

---

## Example 2

Entity

Person

Property

Age

Observation

Age = 42

Observed On

2026-01-01

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

Observation depends upon both Entity and Property.

Evidence depends upon Observation.

---

# Design Principles

Observations record facts.

They do not explain facts.

They do not justify facts.

They do not validate facts.

They simply record what was observed.

---

# Rationale

Separating Observation from Property allows Tindex to support historical change, multiple observations over time, AI extraction, human verification, and evidence-based reasoning while preserving a stable canonical object model.
