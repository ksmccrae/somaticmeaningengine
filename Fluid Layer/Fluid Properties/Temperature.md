---
tags:
  - Ontology Node
  - Fluid Layer
  - Fluid Property
  - Status/Draft
title: Temperature
canonical_name: Temperature
file_class: Ontology Node
node_type: Fluid Property
layer: Fluid Layer
status: Draft
version: 0.1
property_class: Thermal
measurement_type: Both
sensory_boundary: Sensory-Adjacent
---

# Temperature

## Purpose

This node defines Temperature as a reusable fluid property.

It describes thermal condition of a fluid in neutral terms, without defining sensory experience, symbolic meaning, authorial language, or corpus use.

## Property Classification

| Field | Value |
|---|---|
| Node Type | Fluid Property |
| Layer | Fluid Layer |
| Property Class | Thermal |
| Measurement Type | Both |
| Sensory Boundary | Sensory-Adjacent |
| Typical Use | Fluid Profile / Fluid Entity |

## Allowed Value Ranges

| Range Term | Use | Notes |
|---|---|---|
| Cool | Lower relative temperature | Context-dependent descriptor |
| Neutral | No notable thermal emphasis | Neutral descriptor |
| Warm | Higher relative temperature | Context-dependent descriptor |
| Body-temperature | Approximate body-context temperature | Neutral descriptor |
| Variable | Context-dependent temperature | Use where local context changes |

## Applies To

| Target | Relationship | Notes |
|---|---|---|
| [[Tears]] | HAS_FLUID_PROPERTY | Local profile may foreground temperature |
| [[Urine]] | HAS_FLUID_PROPERTY | Local profile may foreground temperature |
| [[Milk]] | HAS_FLUID_PROPERTY | Local profile may foreground temperature |
| [[Blood]] | HAS_FLUID_PROPERTY | Local profile may foreground temperature |
| [[Sweat]] | HAS_FLUID_PROPERTY | Surface cooling context may matter |
| [[Saliva]] | HAS_FLUID_PROPERTY | Local oral context may matter |

## Sensory Boundary

Temperature as a fluid property is distinct from the sensory experience of warmth, coolness, shock, comfort, discomfort, or intimacy.

## Relationship Statements

```text
Temperature IS_FLUID_PROPERTY
Fluid Entity HAS_FLUID_PROPERTY Temperature
Fluid Profile HAS_LOCAL_FLUID_PROPERTY Temperature
Temperature MAY_BE_PERCEIVED_BY Temperature Sensory Profile
```

## Status

Draft v0.1.
