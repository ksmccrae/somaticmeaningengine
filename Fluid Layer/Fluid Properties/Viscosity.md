---
tags:
  - Ontology Node
  - Fluid Layer
  - Fluid Property
  - Status/Draft
title: Viscosity
canonical_name: Viscosity
file_class: Ontology Node
node_type: Fluid Property
layer: Fluid Layer
status: Draft
version: 0.1
property_class: Physical
measurement_type: Both
sensory_boundary: Sensory-Adjacent
---

# Viscosity

## Purpose

This node defines Viscosity as a reusable fluid property.

It describes a fluid's resistance to flow, without defining the fluid entity, anatomical context, activation process, sensory perception, symbolic meaning, authorial language, or corpus use.

## Property Classification

| Field | Value |
|---|---|
| Node Type | Fluid Property |
| Layer | Fluid Layer |
| Property Class | Physical |
| Measurement Type | Both |
| Sensory Boundary | Sensory-Adjacent |
| Typical Use | Fluid Entity / Fluid Profile |

## Allowed Value Ranges

| Range Term | Use | Notes |
|---|---|---|
| Watery | Low viscosity | Neutral descriptor |
| Thin | Low to moderate viscosity | Neutral descriptor |
| Mucosal | Cohesive or mucus-like viscosity | Neutral descriptor |
| Thick | Higher viscosity | Neutral descriptor |
| Variable | Context-dependent viscosity | Use where fluid state changes |

## Applies To

| Target | Relationship | Notes |
|---|---|---|
| [[Tears]] | HAS_FLUID_PROPERTY | Usually watery / variable |
| [[Vaginal Fluid]] | HAS_FLUID_PROPERTY | Variable / mucosal |
| [[Menstrual Fluid]] | HAS_FLUID_PROPERTY | Variable |
| [[Milk]] | HAS_FLUID_PROPERTY | Variable |
| [[Blood]] | HAS_FLUID_PROPERTY | Moderate / variable |
| [[Sweat]] | HAS_FLUID_PROPERTY | Watery / thin |
| [[Saliva]] | HAS_FLUID_PROPERTY | Thin / mucosal / variable |

## Sensory Boundary

Viscosity as a fluid property is distinct from the sensory experience of thickness, slickness, drag, coating, or texture.

## Relationship Statements

```text
Viscosity IS_FLUID_PROPERTY
Fluid Entity HAS_FLUID_PROPERTY Viscosity
Fluid Profile HAS_LOCAL_FLUID_PROPERTY Viscosity
Viscosity MAY_BE_PERCEIVED_BY Viscosity Sensory Profile
```

## Status

Draft v0.1.
