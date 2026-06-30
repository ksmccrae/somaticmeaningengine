---
tags:
  - Ontology Node
  - Fluid Layer
  - Fluid Property
  - Status/Draft
title: Taste
canonical_name: Taste
file_class: Ontology Node
node_type: Fluid Property
layer: Fluid Layer
status: Draft
version: 0.1
property_class: Gustatory
measurement_type: Qualitative
sensory_boundary: Sensory-Adjacent
---

# Taste

## Purpose

This node defines Taste as a reusable fluid property.

It describes potential gustatory quality in neutral terms, without defining sensory experience, desire, aversion, symbolic meaning, authorial language, or corpus use.

## Property Classification

| Field | Value |
|---|---|
| Node Type | Fluid Property |
| Layer | Fluid Layer |
| Property Class | Gustatory |
| Measurement Type | Qualitative |
| Sensory Boundary | Sensory-Adjacent |
| Typical Use | Fluid Entity / Fluid Profile |

## Allowed Value Ranges

| Range Term | Use | Notes |
|---|---|---|
| Neutral | No dominant taste | Neutral descriptor |
| Saline | Salt-like taste quality | Neutral descriptor |
| Metallic | Metallic taste quality | Neutral descriptor |
| Sweet | Sweet taste quality | Neutral descriptor |
| Bitter | Bitter taste quality | Neutral descriptor |
| Acidic | Acidic taste quality | Neutral descriptor |
| Variable | Context-dependent taste | Use where physiological variation occurs |

## Applies To

| Target | Relationship | Notes |
|---|---|---|
| [[Tears]] | HAS_FLUID_PROPERTY | Saline / variable |
| [[Urine]] | HAS_FLUID_PROPERTY | Variable; use cautiously |
| [[Menstrual Fluid]] | HAS_FLUID_PROPERTY | Metallic / variable |
| [[Vaginal Fluid]] | HAS_FLUID_PROPERTY | Saline / acidic / variable |
| [[Milk]] | HAS_FLUID_PROPERTY | Sweet / variable |
| [[Blood]] | HAS_FLUID_PROPERTY | Metallic / saline / variable |
| [[Sweat]] | HAS_FLUID_PROPERTY | Saline / variable |
| [[Saliva]] | HAS_FLUID_PROPERTY | Neutral / saline / variable |

## Sensory Boundary

Taste as a fluid property is distinct from tasting, desire, aversion, disgust, memory, symbolic meaning, or authorial framing.

## Relationship Statements

```text
Taste IS_FLUID_PROPERTY
Fluid Entity HAS_FLUID_PROPERTY Taste
Fluid Profile HAS_LOCAL_FLUID_PROPERTY Taste
Taste MAY_BE_PERCEIVED_BY Taste Sensory Profile
```

## Status

Draft v0.1.
