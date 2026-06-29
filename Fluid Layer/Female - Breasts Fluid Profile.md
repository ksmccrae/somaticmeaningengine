---
tags:
  - Ontology Node
  - Fluid Layer
  - Fluid Profile
  - Female Embodiment
  - Status/Draft
title: Female - Breasts Fluid Profile
file_class: Ontology Node
node_type: Fluid Profile
layer: Fluid Layer
embodiment_scope: Female
status: Draft
version: 0.1
anatomical_anchor: Female - Breasts
canonical_layer_reference: Canonical Embodiment
fluid_relevance: Conditional
---

# Female - Breasts Fluid Profile

## Purpose

This node defines fluid relationships associated with [[Female - Breasts]].

It links to the canonical anatomical node without redefining anatomical structure.

---

## Anatomical Anchor

| Field | Value |
|---|---|
| Anatomical Anchor | [[Female - Breasts]] |
| Anchor Layer | Canonical Embodiment |
| Fluid Layer Role | Conditional / Cyclical / Contextual |

---

## Fluid Relationship Type

| Relationship Type | Description |
|---|---|
| Produces | Breast tissue may be associated with lactation under specific physiological conditions |
| Conducts | Fluid may be conducted through ductal structures when lactation is physiologically active |
| Conditional | Fluid relationship is not continuously present and depends on hormonal, reproductive, postpartum, medical, or induced-lactation contexts |
| Adjacent | Surface moisture belongs to skin or external context rather than breast tissue itself |

---

## Fluid Sources

| Source | Relationship | Notes |
|---|---|---|
| [[Female - Mammary Tissue]] | Produces / Conditional | Tissue associated with lactation-related fluid production |
| [[Female - Nipples]] | Conducts / Output Site | Paired structures associated with output when lactation is active |
| [[Female - Areolae]] | Adjacent | Surrounding paired areolar structures |
| [[Female - Breast Skin]] | Adjacent | Surface tissue; not a primary lactation source |

---

## Fluid Outputs or Presence

| Fluid Presence | Relationship | Notes |
|---|---|---|
| Milk | Conditional / Produces | Lactation-related fluid under specific physiological or medical conditions |
| Surface moisture | Adjacent | Belongs primarily to skin or external context rather than breast fluid production |

---

## Boundary Rules

This profile does not define sensory experience, symbolic meaning, erotic language, activation pathways, propagation routes, authorial usage, or corpus examples.

---

## Relationship Statements

```text
Female - Breasts Fluid Profile DESCRIBES_FLUID_RELATIONSHIPS_OF Female - Breasts
Female - Breasts Fluid Profile REFERENCES_FLUID_SOURCE Female - Mammary Tissue
Female - Breasts Fluid Profile REFERENCES_FLUID_SOURCE Female - Nipples
```

---

## Candidate Downstream Links

| Future Record | Purpose |
|---|---|
| Female - Breasts Activation Profile | Activation behaviour involving lactation, swelling, or vascular change |
| Female - Breasts Sensory Profile | Sensory experience of fullness, tenderness, moisture, or dryness |
| Female - Breasts Symbolic Profile | Symbolic meaning attached to breast fluid imagery |
| Female - Breasts Term Register | Authorial terminology and language constraints |
| Female - Breasts Corpus Annotations | Story, song, essay, or research usage |

---

## Review Questions

1. Should lactation be modelled here, or should it require a dedicated Lactation Profile linked to Mammary Tissue and Nipples?
2. Should Mammary Tissue have its own fluid profile?
3. Should induced lactation and medical lactation contexts be handled in Fluid Layer, Hormonal Layer, or Medical History annotations?

---

## Status

Draft v0.1.

This node validates conditional and low-relevance fluid relationships.
