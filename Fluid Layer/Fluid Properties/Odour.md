---
tags:
  - Ontology Node
  - Fluid Layer
  - Fluid Property
  - Status/Draft
title: Odour
canonical_name: Odour
file_class: Ontology Node
node_type: Fluid Property
layer: Fluid Layer
status: Draft
version: 0.1
property_class: Olfactory
measurement_type: Qualitative
sensory_boundary: Sensory-Adjacent
---

# Odour

## Purpose

This node defines Odour as a reusable fluid property.

It describes the presence, absence, or intensity of smell associated with a fluid in neutral terms, without defining sensory perception, emotional response, symbolic meaning, authorial language, or corpus use.

## Property Classification

| Field | Value |
|---|---|
| Node Type | Fluid Property |
| Layer | Fluid Layer |
| Property Class | Olfactory |
| Measurement Type | Qualitative |
| Sensory Boundary | Sensory-Adjacent |
| Typical Use | Fluid Entity / Fluid Profile |

## Allowed Value Ranges

| Range Term | Use | Notes |
|---|---|---|
| None | No notable odour | Neutral descriptor |
| Mild | Low-intensity odour | Neutral descriptor |
| Strong | High-intensity odour | Neutral descriptor |
| Metallic | Metallic odour quality | Use only where appropriate |
| Saline | Saline odour quality | Use only where appropriate |
| Variable | Context-dependent odour | Use where physiological variation occurs |

## Applies To

| Target | Relationship | Notes |
|---|---|---|
| [[Urine]] | HAS_FLUID_PROPERTY | Variable |
| [[Menstrual Fluid]] | HAS_FLUID_PROPERTY | Mild / metallic / variable |
| [[Vaginal Fluid]] | HAS_FLUID_PROPERTY | None / mild / variable |
| [[Blood]] | HAS_FLUID_PROPERTY | Metallic / variable |
| [[Sweat]] | HAS_FLUID_PROPERTY | None / mild / strong / variable |
| [[Saliva]] | HAS_FLUID_PROPERTY | None / mild / variable |

## Sensory Boundary

Odour as a fluid property is distinct from smelling, tolerance, disgust, comfort, arousal, memory, symbolic meaning, or authorial framing.

## Relationship Statements

```text
Odour IS_FLUID_PROPERTY
Fluid Entity HAS_FLUID_PROPERTY Odour
Fluid Profile HAS_LOCAL_FLUID_PROPERTY Odour
Odour MAY_BE_PERCEIVED_BY Odour Sensory Profile
```

## Status

Draft v0.1.
