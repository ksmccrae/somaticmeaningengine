---
tags:
  - Ontology Node
  - Fluid Layer
  - Fluid Property
  - Status/Draft
title: Flow
canonical_name: Flow
file_class: Ontology Node
node_type: Fluid Property
layer: Fluid Layer
status: Draft
version: 0.1
property_class: Relational / Physical
measurement_type: Qualitative
sensory_boundary: Sensory-Adjacent
---

# Flow

## Purpose

This node defines Flow as a reusable fluid property.

It describes movement pattern or movement state of a fluid in neutral terms, without defining activation mechanics, anatomy, sensory perception, symbolic meaning, authorial language, or corpus use.

## Property Classification

| Field | Value |
|---|---|
| Node Type | Fluid Property |
| Layer | Fluid Layer |
| Property Class | Relational / Physical |
| Measurement Type | Qualitative |
| Sensory Boundary | Sensory-Adjacent |
| Typical Use | Fluid Profile / Activation Boundary |

## Allowed Value Ranges

| Range Term | Use | Notes |
|---|---|---|
| Static | Present without notable movement | Neutral descriptor |
| Surface | Moving or distributed across a surface | Neutral descriptor |
| Droplet | Discrete drop pattern | Neutral descriptor |
| Stream | Directed continuous movement | Neutral descriptor |
| Discharge | Outward movement from a site | Neutral descriptor |
| Cyclical | Patterned by cycle or timing | Neutral descriptor |
| Variable | Context-dependent flow | Use where activation changes movement |

## Applies To

| Target | Relationship | Notes |
|---|---|---|
| [[Tears]] | HAS_FLUID_PROPERTY | Surface / stream / variable |
| [[Urine]] | HAS_FLUID_PROPERTY | Stream / release / variable |
| [[Menstrual Fluid]] | HAS_FLUID_PROPERTY | Discharge / cyclical / variable |
| [[Vaginal Fluid]] | HAS_FLUID_PROPERTY | Surface / discharge / variable |
| [[Milk]] | HAS_FLUID_PROPERTY | Droplet / stream / release / variable |
| [[Blood]] | HAS_FLUID_PROPERTY | Circulation / surface flow / variable |
| [[Sweat]] | HAS_FLUID_PROPERTY | Surface / bead / stream / variable |
| [[Saliva]] | HAS_FLUID_PROPERTY | Oral surface / droplet / transfer / variable |

## Sensory Boundary

Flow as a fluid property is distinct from the sensory experience of movement, dripping, spreading, soaking, pressure, release, or loss of control.

## Relationship Statements

```text
Flow IS_FLUID_PROPERTY
Fluid Entity HAS_FLUID_PROPERTY Flow
Fluid Profile HAS_LOCAL_FLUID_PROPERTY Flow
Flow MAY_BE_ALTERED_BY Activation Profile
Flow MAY_BE_PERCEIVED_BY Flow Sensory Profile
```

## Status

Draft v0.1.
