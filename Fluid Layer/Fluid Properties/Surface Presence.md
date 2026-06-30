---
tags:
  - Ontology Node
  - Fluid Layer
  - Fluid Property
  - Status/Draft
title: Surface Presence
canonical_name: Surface Presence
file_class: Ontology Node
node_type: Fluid Property
layer: Fluid Layer
status: Draft
version: 0.1
property_class: Relational
measurement_type: Qualitative
sensory_boundary: Sensory-Adjacent
---

# Surface Presence

## Purpose

This node defines Surface Presence as a reusable fluid property.

It describes the local presence of a fluid on or across an anatomical or environmental surface, without defining the fluid entity, anatomy, activation mechanics, sensory perception, symbolic meaning, authorial language, or corpus use.

## Property Classification

| Field | Value |
|---|---|
| Node Type | Fluid Property |
| Layer | Fluid Layer |
| Property Class | Relational |
| Measurement Type | Qualitative |
| Sensory Boundary | Sensory-Adjacent |
| Typical Use | Fluid Profile |

## Allowed Value Ranges

| Range Term | Use | Notes |
|---|---|---|
| None | No meaningful surface presence | Neutral descriptor |
| Trace | Minimal surface presence | Neutral descriptor |
| Localized | Present in a specific local area | Neutral descriptor |
| Distributed | Spread across a broader surface | Neutral descriptor |
| Accumulated | Gathered or built up on a surface | Neutral descriptor |
| Transferred | Moved from one surface to another | Neutral descriptor |
| Variable | Context-dependent surface presence | Use during draft modelling |

## Applies To

| Target | Relationship | Notes |
|---|---|---|
| [[Female - Vulva Fluid Profile]] | HAS_LOCAL_FLUID_PROPERTY | Local surface presence of referenced fluids |
| [[Female - Breasts Fluid Profile]] | HAS_LOCAL_FLUID_PROPERTY | Surface presence near nipples or breast skin |
| [[Tears]] | HAS_FLUID_PROPERTY | Surface presence may occur on eyes, eyelids, face, or cheeks |
| [[Sweat]] | HAS_FLUID_PROPERTY | Surface presence is central to sweat expression |
| [[Saliva]] | HAS_FLUID_PROPERTY | Transfer or oral surface presence may matter |

## Sensory Boundary

Surface Presence as a fluid property is distinct from the sensory experience of wetness, dampness, slickness, soaking, coating, or contact.

## Surface Moisture Boundary

Surface Presence is a property or relationship state.

Surface Moisture should become a fluid entity only when surface wetness is mixed, nonspecific, accumulated, transferred, or independently reusable.

## Relationship Statements

```text
Surface Presence IS_FLUID_PROPERTY
Fluid Entity HAS_FLUID_PROPERTY Surface Presence
Fluid Profile HAS_LOCAL_FLUID_PROPERTY Surface Presence
Surface Presence MAY_BE_PERCEIVED_BY Surface Presence Sensory Profile
```

## Status

Draft v0.1.
