---
tags:
  - Ontology Node
  - Fluid Layer
  - Fluid Property
  - Status/Draft
title: Density
canonical_name: Density
file_class: Ontology Node
node_type: Fluid Property
layer: Fluid Layer
status: Draft
version: 0.1
property_class: Physical
measurement_type: Both
sensory_boundary: Objective Property
---

# Density

## Purpose

This node defines Density as a reusable fluid property.

It describes relative mass, heaviness, or concentration of a fluid at the property level, without defining a fluid entity, anatomical context, activation process, sensory perception, symbolic meaning, authorial language, or corpus use.

## Property Classification

| Field | Value |
|---|---|
| Node Type | Fluid Property |
| Layer | Fluid Layer |
| Property Class | Physical |
| Measurement Type | Both |
| Sensory Boundary | Objective Property |
| Typical Use | Fluid Entity / Fluid Profile |

## Allowed Value Ranges

| Range Term | Use | Notes |
|---|---|---|
| Low | Low relative density | Use cautiously |
| Moderate | Mid-range relative density | Neutral descriptor |
| High | High relative density | Use cautiously |
| Variable | Context-dependent density | Use where composition changes |

## Applies To

| Target | Relationship | Notes |
|---|---|---|
| [[Urine]] | HAS_FLUID_PROPERTY | May vary with physiological context |
| [[Menstrual Fluid]] | HAS_FLUID_PROPERTY | Mixed composition may vary |
| [[Blood]] | HAS_FLUID_PROPERTY | Neutral physical property |
| [[Milk]] | HAS_FLUID_PROPERTY | May vary by lactation context |

## Sensory Boundary

Density may influence perception but is not itself the sensory experience of heaviness, thickness, weight, or richness.

## Relationship Statements

```text
Density IS_FLUID_PROPERTY
Fluid Entity HAS_FLUID_PROPERTY Density
Fluid Profile HAS_LOCAL_FLUID_PROPERTY Density
Density MAY_BE_PERCEIVED_BY Density Sensory Profile
```

## Status

Draft v0.1.
