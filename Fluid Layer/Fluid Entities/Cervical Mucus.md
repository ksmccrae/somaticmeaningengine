---
tags:
  - Ontology Node
  - Fluid Layer
  - Fluid Entity
  - Status/Draft
title: Cervical Mucus
canonical_name: Cervical Mucus
file_class: Ontology Node
node_type: Fluid Entity
layer: Fluid Layer
status: Draft
version: 0.1
primary_system: Reproductive System
embodiment_scope: Anatomy-Dependent
fluid_class: Reproductive / Mucosal
---

# Cervical Mucus

## Purpose

This node defines Cervical Mucus as a reusable fluid entity in the Somatic Meaning Engine.

It defines the fluid itself, not a local anatomical relationship, activation process, sensory perception, symbolic meaning, authorial language, or corpus use.

---

## Canonical Definition

Cervical Mucus is a mucus-like reproductive tract fluid associated with the cervix and cervical canal where relevant anatomy is present.

It may be referenced by anatomical fluid profiles involving the cervix, vaginal canal, vaginal fornix, vaginal opening, or adjacent reproductive tract structures, while remaining distinct from [[Vaginal Fluid]], [[Menstrual Fluid]], [[Urine]], and paraurethral glandular fluid.

---

## Fluid Classification

| Field | Value |
|---|---|
| Node Type | Fluid Entity |
| Layer | Fluid Layer |
| Fluid Class | Reproductive / Mucosal |
| Primary System | Reproductive System |
| Embodiment Scope | Anatomy-Dependent |
| Typical State | Mucosal / Variable |
| Cyclical | true |
| Conditional | true |

---

## Common Anatomical Sources

| Anatomical Source | Relationship | Notes |
|---|---|---|
| [[Female - Cervix]] | Produces / Releases | Existing Female anatomical anchor |
| Cervical Canal | Candidate source / conduit | Candidate anatomical node if needed later |

---

## Common Anatomical Conduits, Output, or Surface Sites

| Anatomical Site | Relationship | Notes |
|---|---|---|
| [[Female - Vaginal Canal]] | Receives / Conducts | Existing anatomical anchor |
| [[Female - Vaginal Fornix]] | Adjacent / Receives | Existing anatomical anchor |
| [[Female - Vaginal Opening]] | Output Site / Surface Presence | Existing anatomical anchor |
| [[Female - Vulva]] | Adjacent / Surface Presence | External presence only, not source |

---

## Fluid Properties

| Property | Typical Range | Notes |
|---|---|---|
| [[Viscosity]] | Mucosal / thin / thick / variable | Neutral property only |
| [[Colour]] | Clear / white / pale / variable | Neutral property only |
| [[Opacity]] | Clear / translucent / opaque / variable | Neutral property only |
| [[Odour]] | None / mild / variable | Neutral property only |
| [[Taste]] | Neutral / acidic / variable | Use only where relevant and not authorialized |
| [[Volume]] | Trace / low / moderate / variable | Context-dependent |
| [[Flow]] | Surface / discharge / variable | Activation profile defines process |
| [[Cyclicity]] | Hormonal / reproductive / variable | Cycle-related property |

---

## Common Activation Processes

| Activation Process | Relationship | Notes |
|---|---|---|
| Cervical Mucus Cycle Activation Profile | Alters / Releases / Moves | To be defined in Activation Layer |
| Cycle Regulation Activation Profile | Alters | To be defined in Activation Layer |

---

## Expressive Layer Hooks

| Future Record | Purpose |
|---|---|
| Cervical Mucus Sensory Profile | Perception of texture, wetness, thickness, or presence |
| Cervical Mucus Symbolic Profile | Symbolic associations and meaning |
| Cervical Mucus Term Register | Authorial language rules |
| Cervical Mucus Corpus Annotations | Usage across works |

---

## Boundary Rules

Do not collapse Cervical Mucus with [[Vaginal Fluid]], [[Menstrual Fluid]], [[Urine]], or Paraurethral Glandular Fluid.

Do not define cycle mechanics, sensory interpretation, symbolic meaning, emotional meaning, authorial language, or corpus examples here.

---

## Relationship Statements

```text
Cervical Mucus IS_FLUID_ENTITY
Cervical Mucus HAS_COMMON_SOURCE Female - Cervix
Cervical Mucus MAY_BE_REFERENCED_BY Female - Vaginal Canal Fluid Profile
Cervical Mucus MAY_BE_ALTERED_BY Cervical Mucus Cycle Activation Profile
```

---

## Review Questions

1. Should Cervical Canal be created as a canonical anatomical conduit before this entity is baseline?
2. Should Cervical Mucus variation be handled primarily through Fluid Properties or Activation profiles?
3. How should this entity be represented for Trans Masculine anatomy where relevant structures are present?

---

## Status

Draft v0.1.
