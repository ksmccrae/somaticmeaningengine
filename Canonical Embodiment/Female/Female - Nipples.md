---
tags:
  - Ontology Node
  - Canonical Embodiment
  - Anatomical Site
  - Female Embodiment
  - Status/Draft
title: Female - Nipples
canonical_name: Nipples
file_class: Ontology Node
node_type: Anatomical Site
layer: Canonical Embodiment
embodiment_scope: Female
classification: Paired Atomic Anatomical Node
status: Draft
version: 0.2
parent: Female - Breasts
paired: true
laterality: null
distributed: false
transitional: false
---

# Female - Nipples

## Purpose

This node defines the nipples as canonical anatomical sites within Female Embodiment.

## Canonical Definition

Female - Nipples are paired anatomical structures associated with the breast region.

This node represents the paired structure as a plural paired node. Left and right nipple nodes should only be created when laterality becomes ontologically meaningful, such as asymmetry, injury, surgery, scarring, reconstruction, relocation, side-specific activation, sensory difference, image annotation, or corpus-specific annotation.

## Parent Relationships

```text
Female - Nipples BELONGS_TO Female - Breasts
Female - Breasts BELONGS_TO Female - Thorax
```

## Child Structures

This node has no child structures at the current modelling resolution.

## Boundary Notes

| Nearby Structure | Distinction |
|---|---|
| [[Female - Areolae]] | Surrounding paired areolar structures rather than the nipples themselves |
| [[Female - Breast Skin]] | Broader surface tissue of the breast |

## Layer Separation

Activation, sensory, somatic, mirror, symbolic, fluid, terminology, and corpus details belong to downstream layers.

## Resolved Governance Notes

- Female - Nipples remains plural because it represents a paired anatomical structure.
- Left and right nipple nodes are not created by default.
- Laterality is represented as a property unless side-specific modelling becomes necessary.

## Review Questions

1. Should Female - Nipples remain paired atomic at v1?

## Status

Draft v0.2.
