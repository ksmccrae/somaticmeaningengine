---
tags:
  - Ontology Node
  - Fluid Layer
  - Fluid Property
  - Status/Draft
title: Coagulation State
canonical_name: Coagulation State
file_class: Ontology Node
node_type: Fluid Property
layer: Fluid Layer
status: Draft
version: 0.1
property_class: Physical
measurement_type: Qualitative
sensory_boundary: Objective Property
---

# Coagulation State

## Purpose

This node defines Coagulation State as a reusable fluid property.

It describes whether blood-containing fluid remains uncoagulated, is undergoing partial coagulation, or presents in a clotted state. It does not define a separate fluid entity, anatomical context, activation process, sensory experience, symbolic meaning, authorial language, or corpus use.

## Canonical Definition

Coagulation State is the physical state of a blood-containing fluid in relation to clot formation.

Within the Somatic Meaning Engine, `Clotted` is the lowest governed traversal level. Clot size, frequency, morphology, and composition are not modelled unless a future demonstrated use case requires them.

## Property Classification

| Field | Value |
|---|---|
| Node Type | Fluid Property |
| Layer | Fluid Layer |
| Property Class | Physical |
| Measurement Type | Qualitative |
| Sensory Boundary | Objective Property |
| Typical Use | Fluid Entity / Fluid Profile |

## Allowed Value Ranges

| Range Term | Use | Notes |
|---|---|---|
| Uncoagulated | Fluid remains liquid without observable clot formation | Neutral descriptor |
| Partially Coagulated | Fluid contains developing or incomplete coagulated material | Neutral descriptor |
| Clotted | Fluid presents observable clot formation | Terminal governed value; do not subdivide by size, frequency, morphology, or composition |

## Applies To

| Target | Relationship | Notes |
|---|---|---|
| [[Blood]] | HAS_FLUID_PROPERTY | May present across the governed coagulation states |
| [[Menstrual Fluid]] | HAS_FLUID_PROPERTY | May present as uncoagulated, partially coagulated, or clotted |

## Sensory Boundary

Coagulation State is an objective physical property. The perceived heaviness, warmth, texture, passage, aversion, attraction, or symbolic interpretation of a clot belongs to downstream Sensory, Somatic, Emotional, Symbolic, Authorial, or Corpus layers.

## Boundary Rules

Do not create `Clot` as a separate Fluid Entity.

Do not model clot size, frequency, morphology, or composition beneath the `Clotted` value without a demonstrated traversal requirement and governance review.

## Relationship Statements

```text
Coagulation State IS_FLUID_PROPERTY
Blood HAS_FLUID_PROPERTY Coagulation State
Menstrual Fluid HAS_FLUID_PROPERTY Coagulation State
Fluid Profile HAS_LOCAL_FLUID_PROPERTY Coagulation State
```

## Status

Draft v0.1.
