---
tags:
  - Ontology Node
  - Fluid Layer
  - Fluid Profile
  - Female Embodiment
  - Status/Draft
title: Female - Vaginal Canal Fluid Profile
file_class: Ontology Node
node_type: Fluid Profile
layer: Fluid Layer
embodiment_scope: Female
status: Draft
version: 0.4
anatomical_anchor: Female - Vaginal Canal
canonical_layer_reference: Canonical Embodiment
fluid_relevance: Present / Cyclical / Contextual
---

# Female - Vaginal Canal Fluid Profile

## Purpose

This node defines fluid relationships associated with [[Female - Vaginal Canal]].

It links the canonical anatomical anchor to reusable fluid entities without redefining anatomy or the fluid entities themselves.

---

## Anatomical Anchor

| Field | Value |
|---|---|
| Anatomical Anchor | [[Female - Vaginal Canal]] |
| Anchor Layer | Canonical Embodiment |
| Fluid Layer Role | Present / Cyclical / Contextual |

---

## Referenced Fluid Entities

| Fluid Entity | Relationship To Anchor | Notes |
|---|---|---|
| [[Vaginal Fluid]] | Surface Presence / Contains / Conducts | Primary local fluid entity for this anatomical anchor |
| [[Menstrual Fluid]] | Conducts / Receives | Conducted through the vaginal canal during relevant cycle conditions |
| [[Cervical Mucus]] | Receives / Conducts / Adjacent Source | Distinct cervical mucosal fluid that may be received or conducted through the vaginal canal |

---

## Anatomical Sources, Conduits, and Output Sites

| Role | Anatomical Node | Fluid Entity | Notes |
|---|---|---|---|
| Source / Surface | [[Female - Vaginal Mucosa]] | [[Vaginal Fluid]] | Local mucosal surface relationship |
| Conduit | [[Female - Vaginal Canal]] | [[Vaginal Fluid]] | Internal canal relationship |
| Conduit | [[Female - Vaginal Canal]] | [[Menstrual Fluid]] | Reproductive-cycle pathway |
| Conduit / Receives | [[Female - Vaginal Canal]] | [[Cervical Mucus]] | May receive or conduct mucus from cervical sources |
| Adjacent / Source | [[Female - Cervix]] | [[Cervical Mucus]] | Cervical source relationship; source belongs to cervix, not the vaginal canal |
| Output Site | [[Female - Vaginal Opening]] | [[Vaginal Fluid]] | External transition site |
| Output Site | [[Female - Vaginal Opening]] | [[Menstrual Fluid]] | External transition site during relevant conditions |
| Output Site | [[Female - Vaginal Opening]] | [[Cervical Mucus]] | Possible external transition site without redefining source |

---

## Local Fluid Qualities

Local qualities should be inherited primarily from the referenced fluid entities.

This profile may record anatomical-contextual variation such as internal surface presence, discharge, flow path, or cyclical conduction.

---

## Activation Hooks

| Activation Profile | Fluid Entity | Role |
|---|---|---|
| [[Female - Vulvar Lubrication Activation Profile]] | [[Vaginal Fluid]] | Produces / Alters / Exposes |
| [[Female - Menstruation Activation Profile]] | [[Menstrual Fluid]] | Releases / Moves / Exposes |
| Cervical Mucus Cycle Activation Profile | [[Cervical Mucus]] | Alters / Releases / Moves |

Existing Activation Profiles are wikilinked by their canonical node names. Candidate profiles that do not yet exist remain plain text.

---

## Boundary Rules

Do not collapse Vaginal Fluid, Menstrual Fluid, Cervical Mucus, Urine, or paraurethral glandular fluid into one category.

Do not include sensory interpretation, symbolic meaning, emotional interpretation, activation mechanics, authorial language, or corpus examples.

---

## Relationship Statements

```text
Female - Vaginal Canal Fluid Profile DESCRIBES_FLUID_RELATIONSHIPS_OF Female - Vaginal Canal
Female - Vaginal Canal Fluid Profile REFERENCES_FLUID_ENTITY Vaginal Fluid
Female - Vaginal Canal Fluid Profile REFERENCES_FLUID_ENTITY Menstrual Fluid
Female - Vaginal Canal Fluid Profile REFERENCES_FLUID_ENTITY Cervical Mucus
Female - Vaginal Canal Fluid Profile REFERENCES_FLUID_SOURCE Female - Vaginal Mucosa
Female - Vaginal Canal Fluid Profile REFERENCES_FLUID_SOURCE Female - Cervix
Female - Vaginal Canal Fluid Profile REFERENCES_FLUID_CONDUIT Female - Vaginal Canal
Female - Vaginal Canal Fluid Profile REFERENCES_FLUID_OUTPUT_SITE Female - Vaginal Opening
Female - Vaginal Canal Fluid Profile REFERENCES_ACTIVATION_PROFILE Female - Vulvar Lubrication Activation Profile
Female - Vaginal Canal Fluid Profile REFERENCES_ACTIVATION_PROFILE Female - Menstruation Activation Profile
```

---

## Review Questions

1. Should Vaginal Mucosa have a separate fluid profile or remain represented through this profile?
2. Which cycle or hormonal activation profiles are required before baseline?
3. Does the vaginal canal profile correctly treat Cervical Mucus as received or conducted rather than locally produced?

---

## Status

Draft v0.4.

Canonical Activation hook names synchronized with the Activation Layer.
