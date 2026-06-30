---
tags:
  - Ontology Node
  - Fluid Layer
  - Fluid Profile
  - Female Embodiment
  - Status/Draft
title: Female - Skene's Glands Fluid Profile
file_class: Ontology Node
node_type: Fluid Profile
layer: Fluid Layer
embodiment_scope: Female
status: Draft
version: 0.2
anatomical_anchor: Female - Skene's Glands
canonical_layer_reference: Canonical Embodiment
fluid_relevance: Present / Contextual
---

# Female - Skene's Glands Fluid Profile

## Purpose

This node defines fluid relationships associated with [[Female - Skene's Glands]].

It links the canonical anatomical anchor to reusable fluid entities without redefining anatomy or the fluid entities themselves.

---

## Anatomical Anchor

| Field | Value |
|---|---|
| Anatomical Anchor | [[Female - Skene's Glands]] |
| Anchor Layer | Canonical Embodiment |
| Fluid Layer Role | Produces / Contextual |

---

## Referenced Fluid Entities

| Fluid Entity | Relationship To Anchor | Notes |
|---|---|---|
| Paraurethral Glandular Fluid | Produces / Conducts / Surface Presence | Candidate fluid entity required before this profile is baseline |
| [[Urine]] | Adjacent | Nearby urinary output; not produced by Skene's glands |

---

## Anatomical Sources, Conduits, and Output Sites

| Role | Anatomical Node | Fluid Entity | Notes |
|---|---|---|---|
| Source | [[Female - Skene's Glands]] | Paraurethral Glandular Fluid | Glandular source relationship |
| Conduit / Output Candidate | [[Female - Vestibular Gland Openings]] | Paraurethral Glandular Fluid | Candidate anatomical relationship needing review |
| Adjacent Site | [[Female - Urethral Opening]] | [[Urine]] | Nearby urinary output anchor, not a source relationship |
| Adjacent Region | [[Female - Vestibule]] | Paraurethral Glandular Fluid | Parent transitional region |

---

## Local Fluid Qualities

Local qualities should be inherited primarily from the referenced fluid entity once it exists.

This profile may record contextual presence near the vestibular or paraurethral region.

---

## Activation Hooks

| Activation Profile | Fluid Entity | Role |
|---|---|---|
| Paraurethral Glandular Activation Profile | Paraurethral Glandular Fluid | Produces / Releases / Exposes |

---

## Boundary Rules

Do not collapse paraurethral glandular fluid with urine, vaginal fluid, or cervical mucus.

Do not include sensory interpretation, symbolic meaning, emotional interpretation, activation mechanics, authorial language, or corpus examples.

---

## Relationship Statements

```text
Female - Skene's Glands Fluid Profile DESCRIBES_FLUID_RELATIONSHIPS_OF Female - Skene's Glands
Female - Skene's Glands Fluid Profile REFERENCES_FLUID_ENTITY Paraurethral Glandular Fluid
Female - Skene's Glands Fluid Profile REFERENCES_FLUID_SOURCE Female - Skene's Glands
Female - Skene's Glands Fluid Profile REFERENCES_FLUID_OUTPUT_SITE Female - Vestibular Gland Openings
```

---

## Review Questions

1. Should Paraurethral Glandular Fluid be created as a fluid entity now?
2. Should gland openings be separated more clearly from the gland structure in canonical anatomy?
3. Should urinary-system boundaries be represented through adjacent links only?

---

## Status

Draft v0.2.
