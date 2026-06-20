# SPEC-0001 — Entity

**Status:** Draft

**Version:** 0.1

**Owner:** Tindex

---

# Purpose

Define the canonical concept of an Entity within Tindex.

Every observation, property, evidence item, claim, and validation must ultimately reference one or more entities.

---

# Definition

An **Entity** is any uniquely identifiable thing that Tindex can reason about.

An Entity may represent:

* Company
* Person
* Financial Instrument
* Index
* Sector
* Country
* Economic Indicator
* Event
* Organization
* Regulation
* Document
* Dataset

An Entity is independent of observations.

Entities exist whether or not observations currently exist.

---

# Requirements

An Entity SHALL:

* have exactly one canonical identifier
* have one canonical name
* belong to one canonical type
* remain stable across observations
* support aliases
* support relationships with other entities

---

# Rules

* Every observation MUST reference at least one Entity.
* Every claim MUST ultimately resolve to one or more Entities.
* Entity identity is immutable.
* Entity names may change.
* Aliases do not create new Entities.

---

# Constraints

An Entity SHALL NOT contain observations.

An Entity SHALL NOT contain evidence.

An Entity SHALL NOT contain claims.

Those belong to their respective canonical objects.

---

# Examples

## Valid

Entity

Company

Name

Tata Consultancy Services Ltd.

---

Entity

Economic Indicator

Name

Consumer Price Index

---

## Invalid

Revenue = ₹100 Cr

Reason:

Revenue is an Observation, not an Entity.

---

# References

Future specifications:

* SPEC-0002 Property
* SPEC-0003 Observation

---

# Revision History

| Version | Description   |
| ------- | ------------- |
| 0.1     | Initial draft |
