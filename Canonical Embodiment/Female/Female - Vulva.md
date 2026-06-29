---
tags:
  - Ontology Node
  - Canonical Embodiment
  - Anatomical Site
  - Female Embodiment
  - Status/Draft
aliases:
  - Female Vulva
  - Vulva
title: Female - Vulva
canonical_name: Vulva
file_class: Ontology Node
node_type: Anatomical Site
layer: Canonical Embodiment
embodiment_scope: Female
classification: Composite Anatomical Node
status: Draft
version: 0.1
parent: Female - External Genitalia
paired: false
distributed: false
transitional: true
last_updated: 2026-06-29
---

# Female - Vulva

## Purpose

This node defines the vulva as a canonical anatomical site within Female Embodiment.

It exists to describe anatomical structure, containment relationships, boundaries, and canonical placement in the Somatic Meaning Engine.

This node does not define activation, sensory register, somatic experience, symbolic meaning, authorial usage, terminology rules, or corpus annotation.

---

## Canonical Definition

The vulva is the external genital anatomical region within Female Embodiment.

It includes the external genital structures surrounding the vestibule and forms the primary external genital composite node within the pelvic branch.

The vulva should be distinguished from the vaginal canal, clitoral complex, vestibule, pelvic floor, and perineum, each of which may require its own canonical node.

---

## Ontological Classification

| Field | Value |
|---|---|
| Node Type | Anatomical Site |
| Classification | Composite Anatomical Node |
| Layer | Canonical Embodiment |
| Embodiment Scope | Female |
| Parent | [[Female - External Genitalia]] |
| Region | [[Female - Pelvis]] |
| External / Internal | External |
| Paired | false |
| Distributed | false |
| Transitional | true |

---

## Parent Relationships

```text
Female - Vulva BELONGS_TO Female - External Genitalia
Female - External Genitalia BELONGS_TO Female - Pelvis
Female - Pelvis BELONGS_TO Female Embodiment
```

---

## Child Structures

The vulva contains or organizes the following anatomical child structures:

| Child Structure | Proposed Node | Classification |
|---|---|---|
| Mons Pubis | [[Female - Mons Pubis]] | Atomic Anatomical Node |
| Labia Majora | [[Female - Labia Majora]] | Paired Atomic or Composite Node |
| Labia Minora | [[Female - Labia Minora]] | Paired Atomic or Composite Node |
| Clitoral Complex | [[Female - Clitoral Complex]] | Composite Anatomical Node |
| Vestibule | [[Female - Vestibule]] | Transitional Composite Node |
| Perineal Boundary | [[Female - Perineal Boundary]] | Boundary or Transitional Node |

---

## Containment Relationships

```text
Female - Vulva CONTAINS Female - Mons Pubis
Female - Vulva CONTAINS Female - Labia Majora
Female - Vulva CONTAINS Female - Labia Minora
Female - Vulva CONTAINS Female - Clitoral Complex
Female - Vulva CONTAINS Female - Vestibule
Female - Vulva CONTAINS Female - Perineal Boundary
```

---

## Boundary Notes

| Nearby Structure | Distinction |
|---|---|
| [[Female - Vaginal Canal]] | Internal reproductive passage rather than the external genital composite site |
| [[Female - Vaginal Opening]] | Transitional opening within the vestibule |
| [[Female - Urethral Opening]] | Urinary opening within the vestibule |
| [[Female - Perineum]] | Adjacent external pelvic region |
| [[Female - Pelvic Floor]] | Muscular support structure beneath the pelvic region |
| [[Female - Clitoral Complex]] | Child composite structure within the vulva rather than a synonym for the vulva |

---

## Anatomical Notes

The vulva is a composite external genital site.

It should not be collapsed into the vagina, clitoris, vestibule, pelvic floor, or perineum.

This node functions as an anatomical container for several distinct structures, each of which may require its own canonical anatomical node.

---

## Layer Separation

The following concerns are intentionally excluded from this canonical node and should be modelled in later layers.

| Concern | Target Layer |
|---|---|
| Sensory response | Sensory Layer |
| Somatic experience | Somatic Layer |
| Mirror relationships | Mirror Layer |
| Propagation pathways | Propagation Layer |
| Symbolic meaning | Symbolic Layer |
| Emotional associations | Emotional Layer |
| Fluid behaviour | Fluid Layer |
| Authorial terminology | Authorial Systems or Term Register |
| Corpus usage | Corpus Annotation |

---

## Candidate Downstream Links

These are not canonical anatomical definitions, but likely future linked records.

| Future Record | Purpose |
|---|---|
| Female - Vulva Sensory Profile | Sensory responsiveness and tactile qualities |
| Female - Vulva Somatic Profile | Embodied experience and internal sensation |
| Female - Vulva Mirror Profile | Mirror relationships to clitoral, breast, pelvic, or emotional systems |
| Female - Vulva Propagation Profile | Activation movement into pelvic floor, breath, or internal awareness |
| Female - Vulva Symbolic Profile | Symbolic and ritual associations |
| Female - Vulva Term Register | Allowed, restricted, and banned language |
| Female - Vulva Corpus Annotations | Usage across stories, songs, essays, or research |

---

## Source Migration Notes

This node was derived from the earlier Vulva register file.

The earlier register included canonical anatomy, sensory notes, mirror notes, propagation patterns, symbolic associations, fluid relationships, and terminology governance in one document.

This canonical node intentionally keeps only anatomical placement, structure, containment, and boundary information.

---

## Review Questions

1. Should Labia Majora and Labia Minora be modelled as paired atomic nodes or paired composite nodes?
2. Should Perineal Boundary be a canonical anatomical node or a boundary marker?
3. Should Vestibule be classified primarily as Composite, Transitional, or both?
4. Should this node use `CONTAINS`, `HAS_PART`, or both as controlled relationship verbs?
5. Should anatomical nodes include downstream placeholder links before those downstream records exist?

---

## Status

Draft v0.1.

This node should be used to validate the Anatomical Site Template before additional anatomical nodes are populated.
