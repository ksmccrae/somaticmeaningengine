---
tags:
  - Ontology Node
  - Fluid Layer
  - Fluid Property
  - Status/Draft
title: Opacity
canonical_name: Opacity
file_class: Ontology Node
node_type: Fluid Property
layer: Fluid Layer
status: Draft
version: 0.1
property_class: Visual
measurement_type: Qualitative
sensory_boundary: Sensory-Adjacent
---

# Opacity

## Purpose

This node defines Opacity as a reusable fluid property.

It describes how much light passes through a fluid, without defining the fluid entity, anatomy, activation, sensory perception, symbolic meaning, authorial language, or corpus use.

## Property Classification

| Field | Value |
|---|---|
| Node Type | Fluid Property |
| Layer | Fluid Layer |
| Property Class | Visual |
| Measurement Type | Qualitative |
| Sensory Boundary | Sensory-Adjacent |
| Typical Use | Fluid Entity / Fluid Profile |

## Allowed Value Ranges

| Range Term | Use | Notes |
|---|---|---|
| Clear | Transparent or nearly transparent | Neutral descriptor |
| Translucent | Partly light-permeable | Neutral descriptor |
| Cloudy | Reduced clarity | Neutral descriptor |
| Opaque | Not visibly transparent | Neutral descriptor |
| Variable | Context-dependent opacity | Use where fluid composition changes |

## Applies To

| Target | Relationship | Notes |
|---|---|---|
| [[Tears]] | HAS_FLUID_PROPERTY | Usually clear / translucent |
| [[Urine]] | HAS_FLUID_PROPERTY | Clear / cloudy / variable |
| [[Vaginal Fluid]] | HAS_FLUID_PROPERTY | Clear / translucent / opaque / variable |
| [[Milk]] | HAS_FLUID_PROPERTY | Opaque / variable |
| [[Blood]] | HAS_FLUID_PROPERTY | Opaque |
| [[Saliva]] | HAS_FLUID_PROPERTY | Clear / translucent / variable |

## Sensory Boundary

Opacity as a fluid property is distinct from visual perception, attention, disgust, desire, alarm, symbolism, or authorial emphasis.

## Relationship Statements

```text
Opacity IS_FLUID_PROPERTY
Fluid Entity HAS_FLUID_PROPERTY Opacity
Fluid Profile HAS_LOCAL_FLUID_PROPERTY Opacity
Opacity MAY_BE_PERCEIVED_BY Opacity Sensory Profile
```

## Status

Draft v0.1.
