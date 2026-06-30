---
tags:
  - Ontology Node
  - Fluid Layer
  - Fluid Property
  - Status/Draft
title: Volume
canonical_name: Volume
file_class: Ontology Node
node_type: Fluid Property
layer: Fluid Layer
status: Draft
version: 0.1
property_class: Physical / Quantitative
measurement_type: Both
sensory_boundary: Objective Property
---

# Volume

## Purpose

This node defines Volume as a reusable fluid property.

It describes amount or quantity of fluid in neutral terms, without defining activation mechanics, sensory perception, symbolic meaning, authorial language, or corpus use.

## Property Classification

| Field | Value |
|---|---|
| Node Type | Fluid Property |
| Layer | Fluid Layer |
| Property Class | Physical / Quantitative |
| Measurement Type | Both |
| Sensory Boundary | Objective Property |
| Typical Use | Fluid Entity / Fluid Profile |

## Allowed Value Ranges

| Range Term | Use | Notes |
|---|---|---|
| Trace | Minimal amount | Neutral descriptor |
| Low | Small amount | Neutral descriptor |
| Moderate | Mid-range amount | Neutral descriptor |
| High | Large amount | Neutral descriptor |
| Variable | Context-dependent amount | Use where activation or physiology changes quantity |

## Applies To

| Target | Relationship | Notes |
|---|---|---|
| [[Tears]] | HAS_FLUID_PROPERTY | Trace to high / variable |
| [[Urine]] | HAS_FLUID_PROPERTY | Variable |
| [[Menstrual Fluid]] | HAS_FLUID_PROPERTY | Variable / cyclical |
| [[Vaginal Fluid]] | HAS_FLUID_PROPERTY | Variable |
| [[Milk]] | HAS_FLUID_PROPERTY | Conditional / variable |
| [[Blood]] | HAS_FLUID_PROPERTY | Trace to high / context-dependent |
| [[Sweat]] | HAS_FLUID_PROPERTY | Trace to high / variable |
| [[Saliva]] | HAS_FLUID_PROPERTY | Variable |

## Sensory Boundary

Volume may influence perception, but it is not itself the sensory experience of abundance, scarcity, soaking, flooding, fullness, or dryness.

## Relationship Statements

```text
Volume IS_FLUID_PROPERTY
Fluid Entity HAS_FLUID_PROPERTY Volume
Fluid Profile HAS_LOCAL_FLUID_PROPERTY Volume
Volume MAY_BE_PERCEIVED_BY Volume Sensory Profile
```

## Status

Draft v0.1.
