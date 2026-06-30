---
tags:
  - Template/Translation
  - Template/Fluid Property
  - Status/Draft
aliases:
  - Fluid Property Template
  - Fluid Properties Template
title: Fluid Property Template
file_class: Template
template_type: Translation
node_type: Fluid Property
layer: Fluid Layer
status: Draft
version: 0.1
last_updated: 2026-06-30
---

# Fluid Property Template

## Purpose

This template defines reusable fluid property nodes in the Somatic Meaning Engine.

A fluid property defines an observable, measurable, or physiologically grounded quality that may be associated with one or more fluid entities or local fluid profiles.

Fluid properties do not define fluid entities, anatomical sites, activation mechanics, sensory experience, symbolic meaning, authorial usage, or corpus instances.

---

## Architectural Rule

Fluid modelling uses three linked structures:

```text
Fluid Property
= reusable quality or attribute

Fluid Entity
= what the fluid is

Fluid Profile
= how a fluid entity relates to a specific anatomical anchor
```

Fluid properties prevent duplicated property tables across fluid entities and profiles.

---

## File Naming Rule

Fluid property nodes should use clear property names.

Examples:

```text
Viscosity.md
Density.md
Colour.md
Opacity.md
Odour.md
Taste.md
Temperature.md
Volume.md
Flow.md
Cyclicity.md
Surface Presence.md
```

---

## YAML Pattern

```yaml
---
tags:
  - Ontology Node
  - Fluid Layer
  - Fluid Property
  - Status/Draft
title: Fluid Property Name
canonical_name: Fluid Property Name
file_class: Ontology Node
node_type: Fluid Property
layer: Fluid Layer
status: Draft
version: 0.1
property_class: Physical / Chemical / Visual / Olfactory / Gustatory / Thermal / Temporal / Relational
measurement_type: Qualitative / Quantitative / Both
sensory_boundary: Objective Property / Sensory-Adjacent
---
```

---

# Fluid Property Name

## Purpose

This node defines `[Fluid Property Name]` as a reusable fluid property.

It defines the property itself, not the fluid entity that possesses it, the anatomy where it appears, or the sensory experience of perceiving it.

---

## Canonical Definition

Define the property in neutral language.

The definition should answer:

- What quality does this property describe?
- Is it physical, chemical, visual, olfactory, gustatory, thermal, temporal, or relational?
- Can it be described qualitatively, quantitatively, or both?
- Which downstream layers may perceive or interpret it?

---

## Property Classification

| Field | Value |
|---|---|
| Node Type | Fluid Property |
| Layer | Fluid Layer |
| Property Class | Physical / Chemical / Visual / Olfactory / Gustatory / Thermal / Temporal / Relational |
| Measurement Type | Qualitative / Quantitative / Both |
| Sensory Boundary | Objective Property / Sensory-Adjacent |
| Typical Use | Fluid Entity / Fluid Profile / Both |

---

## Allowed Value Ranges

List governed descriptive ranges for the property.

| Range Term | Use | Notes |
|---|---|---|
| Example value | Neutral descriptor | Do not authorialize |

---

## Applies To

List candidate fluid entities or profiles that may reference this property.

| Target | Relationship | Notes |
|---|---|---|
| [[Fluid Entity]] | HAS_FLUID_PROPERTY | Reusable property assignment |
| [[Fluid Profile]] | HAS_LOCAL_FLUID_PROPERTY | Local anatomical variation |

---

## Sensory Boundary

Fluid properties may be sensory-adjacent but are not sensory profiles.

Example:

```text
Odour
= observable fluid property

Odour Sensory Profile
= how odour is perceived, tolerated, desired, rejected, remembered, or interpreted
```

---

## Boundary Rules

Do not include:

- definitions of fluid entities
- anatomical placement
- activation mechanics
- sensory pleasure or discomfort
- emotional interpretation
- symbolic meaning
- authorial language
- corpus examples

---

## Relationship Statements

Use controlled relationship language.

```text
Fluid Property IS_FLUID_PROPERTY
Fluid Entity HAS_FLUID_PROPERTY Fluid Property
Fluid Profile HAS_LOCAL_FLUID_PROPERTY Fluid Property
Fluid Property MAY_BE_PERCEIVED_BY Sensory Profile
Fluid Property MAY_BE_INTERPRETED_BY Symbolic Profile
```

---

## Review Questions

1. Is this property objective, sensory-adjacent, or both?
2. Should this property be qualitative, quantitative, or both?
3. Does this property belong on the fluid entity, the local fluid profile, or both?
4. Does this property require governed value ranges?
5. Does this property risk crossing into sensory or symbolic interpretation?

---

## Status

Draft v0.1.

This template should be validated before fluid property nodes are populated broadly.
