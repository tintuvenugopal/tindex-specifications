# SPEC-0002 — Property

## Status

Approved

---

# Purpose

A Property defines a measurable, describable, or identifiable characteristic of an Entity.

Without Properties, Entities have identity but no meaningful structure.

Properties provide the vocabulary through which Entities can be described, observed, compared, and reasoned about.

---

# Definition

A Property is a named characteristic that belongs to an Entity and whose value may be observed, measured, inferred, or assigned.

Properties describe the state or nature of an Entity without defining the Entity itself.

---

# Characteristics

Every Property:

* Has a unique name within its context.
* Belongs to one or more Entity types.
* Has a defined meaning.
* May have one or more values.
* May change over time unless explicitly immutable.
* Can be observed and recorded.

---

# Examples

## Company

Properties include:

* Company Name
* Ticker Symbol
* ISIN
* Market Capitalization
* Revenue
* Net Profit

---

## Person

Properties include:

* Name
* Date of Birth
* Nationality
* Occupation

---

# Relationships

Property supports:

* Observation
* Evidence
* Claim
* Validation

A Property cannot exist independently of an Entity.

An Entity may possess zero or many Properties.

---

# Design Principles

Properties define characteristics.

They do not define behavior.

They do not define relationships.

They do not contain evidence.

They do not make claims.

They simply describe the Entity.

---

# Rationale

Separating Entity and Property creates a stable canonical model that supports extensibility, validation, and consistent reasoning across every component of Tindex.
