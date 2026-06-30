---
tags:
  - Ontology Node
  - Fluid Layer
  - Fluid Profile
  - Female Embodiment
  - Status/Draft
title: Female - Vulva Fluid Profile
file_class: Ontology Node
node_type: Fluid Profile
layer: Fluid Layer
embodiment_scope: Female
status: Draft
version: 0.2
anatomical_anchor: Female - Vulva
canonical_layer_reference: Canonical Embodiment
fluid_relevance: Adjacent / Surface Presence
---

# Female - Vulva Fluid Profile

## Purpose

This node defines fluid relationships associated with [[Female - Vulva]].

It links the canonical anatomical anchor to reusable fluid entities without redefining anatomy or the fluid entities themselves.

---

## Anatomical Anchor

| Field | Value |
|---|---|
| Anatomical Anchor | [[Female - Vulva]] |
| Anchor Layer | Canonical Embodiment |
| Fluid Layer Role | Adjacent / Surface Presence |

---

## Referenced Fluid Entities

| Fluid Entity | Relationship To Anchor | Notes |
|---|---|---|
| [[Vaginal Fluid]] | Adjacent / Surface Presence | May become externally present near the vulval surface but belongs primarily to vaginal canal or vaginal opening profiles |
| [[Menstrual Fluid]] | Adjacent / Surface Presence | May become externally present during relevant cycle conditions but is not produced by the vulva |
| [[Urine]] | Adjacent | Associated with nearby urethral output, not vulval production |
| Paraurethral Glandular Fluid | Adjacent | Candidate fluid entity needed for Skene's gland modelling |
| Surface Moisture | Surface Presence | Candidate pending decision: entity, quality, or relationship type |

---

## Anatomical Sources, Conduits, and Output Sites

| Role | Anatomical Node | Fluid Entity | Notes |
|---|---|---|---|
| Adjacent Site | [[Female - Vulva]] | [[Vaginal Fluid]] | External surface presence only |
| Adjacent Site | [[Female - Vulva]] | [[Menstrual Fluid]] | External surface presence only |
| Adjacent Site | [[Female - Vulva]] | [[Urine]] | Nearby urinary output, not source |
| Output Site | [[Female - Vaginal Opening]] | [[Vaginal Fluid]] | Primary output anchor for vaginal canal fluids |
| Output Site | [[Female - Vaginal Opening]] | [[Menstrual Fluid]] | Primary visible output anchor for menstrual fluid |
| Output Site | [[Female - Urethral Opening]] | [[Urine]] | Urinary output anchor |
| Source / Adjacent | [[Female - Skene's Glands]] | Paraurethral Glandular Fluid | Candidate entity and profile required |

---

## Local Fluid Qualities

Local qualities should be inherited primarily from the referenced fluid entities.

This profile may record only local surface-presence patterns, such as trace, surface, adjacent, or externally present.

---

## Activation Hooks

| Activation Profile | Fluid Entity | Role |
|---|---|---|
| Menstruation Activation Profile | [[Menstrual Fluid]] | Releases / Moves / Exposes |
| Urination Activation Profile | [[Urine]] | Releases / Moves / Exposes |
| Vaginal Lubrication Activation Profile | [[Vaginal Fluid]] | Produces / Alters / Exposes |

---

## Boundary Rules

Do not assign urinary, menstrual, vaginal, or glandular fluid production to the vulva as a whole.

Do not include sensory interpretation, symbolic meaning, emotional interpretation, activation mechanics, authorial language, or corpus examples.

---

## Relationship Statements

```text
Female - Vulva Fluid Profile DESCRIBES_FLUID_RELATIONSHIPS_OF Female - Vulva
Female - Vulva Fluid Profile REFERENCES_FLUID_ENTITY Vaginal Fluid
Female - Vulva Fluid Profile REFERENCES_FLUID_ENTITY Menstrual Fluid
Female - Vulva Fluid Profile REFERENCES_FLUID_ENTITY Urine
Female - Vulva Fluid Profile REFERENCES_FLUID_OUTPUT_SITE Female - Vaginal Opening
Female - Vulva Fluid Profile REFERENCES_FLUID_OUTPUT_SITE Female - Urethral Opening
```

---

## Review Questions

1. Should Surface Moisture be a fluid entity, local quality, or relationship type?
2. Should Paraurethral Glandular Fluid be created before this profile is validated?
3. Should this profile remain mostly adjacent rather than direct?

---

## Status

Draft v0.2.
