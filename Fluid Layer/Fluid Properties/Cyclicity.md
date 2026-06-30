---
tags:
  - Ontology Node
  - Fluid Layer
  - Fluid Property
  - Status/Draft
title: Cyclicity
canonical_name: Cyclicity
file_class: Ontology Node
node_type: Fluid Property
layer: Fluid Layer
status: Draft
version: 0.1
property_class: Temporal
measurement_type: Qualitative
sensory_boundary: Objective Property
---

# Cyclicity

## Purpose

This node defines Cyclicity as a reusable fluid property.

It describes whether a fluid's presence, quantity, composition, or flow varies according to cycle, timing, hormonal pattern, reproductive state, environmental rhythm, or other periodic conditions.

It does not define the activation process, sensory perception, symbolic meaning, authorial language, or corpus use.

## Property Classification

| Field | Value |
|---|---|
| Node Type | Fluid Property |
| Layer | Fluid Layer |
| Property Class | Temporal |
| Measurement Type | Qualitative |
| Sensory Boundary | Objective Property |
| Typical Use | Fluid Entity / Fluid Profile / Activation Boundary |

## Allowed Value Ranges

| Range Term | Use | Notes |
|---|---|---|
| None | No cycle-relevant variation | Neutral descriptor |
| Contextual | Depends on specific physiological context | Neutral descriptor |
| Hormonal | Varies with hormonal conditions | Neutral descriptor |
| Reproductive | Varies with reproductive-cycle conditions | Neutral descriptor |
| Environmental | Varies with environmental rhythm | Neutral descriptor |
| Variable | Multiple or unresolved timing patterns | Use during draft modelling |

## Applies To

| Target | Relationship | Notes |
|---|---|---|
| [[Menstrual Fluid]] | HAS_FLUID_PROPERTY | Reproductive / hormonal / cyclical |
| [[Vaginal Fluid]] | HAS_FLUID_PROPERTY | Contextual / hormonal / variable |
| [[Milk]] | HAS_FLUID_PROPERTY | Hormonal / postpartum / contextual |
| [[Sweat]] | HAS_FLUID_PROPERTY | Contextual / environmental |
| [[Tears]] | HAS_FLUID_PROPERTY | Usually contextual rather than cyclical |

## Sensory Boundary

Cyclicity may influence experience but is not itself the sensory experience of recurrence, anticipation, dread, relief, ritual, or timing.

## Relationship Statements

```text
Cyclicity IS_FLUID_PROPERTY
Fluid Entity HAS_FLUID_PROPERTY Cyclicity
Fluid Profile HAS_LOCAL_FLUID_PROPERTY Cyclicity
Cyclicity MAY_BE_ALTERED_BY Activation Profile
```

## Status

Draft v0.1.
