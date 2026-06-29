---
tags:
  - Ontology Node
  - Canonical Embodiment
  - Anatomical Site
  - Female Embodiment
  - Status/Draft
title: Female - Breasts
canonical_name: Breasts
file_class: Ontology Node
node_type: Anatomical Site
layer: Canonical Embodiment
embodiment_scope: Female
classification: Paired Composite Anatomical Node
status: Draft
version: 0.2
parent: Female - Thorax
paired: true
laterality: null
distributed: false
transitional: false
---

# Female - Breasts

## Purpose

This node defines the breasts as canonical anatomical sites within Female Embodiment.

## Canonical Definition

Female - Breasts are paired thoracic anatomical structures associated with the chest region.

This node represents the paired structure as a plural paired node. Left and right breast nodes should only be created when laterality becomes ontologically necessary for surgical history, scar mapping, asymmetry, corpus annotation, or side-specific activation records.

## Parent Relationships

```text
Female - Breasts BELONGS_TO Female - Thorax
Female - Thorax BELONGS_TO Female Embodiment
```

## Child Structures

| Child Structure | Proposed Node | Classification |
|---|---|---|
| Nipple | [[Female - Nipple]] | Paired Atomic Node |
| Areola | [[Female - Areola]] | Paired Atomic Node |
| Mammary Tissue | [[Female - Mammary Tissue]] | Distributed or Composite Node |
| Breast Skin | [[Female - Breast Skin]] | Surface Node |
| Breast Fat Pad | [[Female - Breast Fat Pad]] | Composite or Tissue Node |
| Breast Fascia | [[Female - Breast Fascia]] | Connective Tissue Node |
| Breast Lymphatics | [[Female - Breast Lymphatics]] | Lymphatic Structure Node |

## Layer Separation

Activation, sensory, somatic, mirror, symbolic, fluid, terminology, and corpus details belong to downstream layers.

## Resolved Governance Notes

- Female - Breasts remains plural because it represents a paired anatomical structure.
- Left and right breast nodes are not created by default.
- Laterality is represented as a property unless side-specific modelling becomes necessary.

## Review Questions

1. Should any child structures be moved primarily under Skin and Surface, Musculoskeletal Support, or Circulatory and Lymphatic Systems, with cross-links back to Breasts?

## Status

Draft v0.2.
