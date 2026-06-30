---
tags:
  - Ontology Node
  - Fluid Layer
  - Fluid Property
  - Status/Draft
title: Colour
canonical_name: Colour
file_class: Ontology Node
node_type: Fluid Property
layer: Fluid Layer
status: Draft
version: 0.1
property_class: Visual
measurement_type: Qualitative
sensory_boundary: Sensory-Adjacent
---

# Colour

## Purpose

This node defines Colour as a reusable fluid property.

It describes visible hue or colouration of a fluid in neutral terms, without defining the fluid entity, anatomical context, sensory perception, symbolic meaning, authorial language, or corpus use.

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
| Clear | No visible colouration | Neutral descriptor |
| White | White or pale white | Neutral descriptor |
| Yellow | Yellow range | Neutral descriptor |
| Red | Red range | Neutral descriptor |
| Brown | Brown range | Neutral descriptor |
| Dark | Darkened colouration | Requires fluid context |
| Pale | Light colouration | Requires fluid context |
| Variable | Context-dependent colour | Use where physiological variation occurs |

## Applies To

| Target | Relationship | Notes |
|---|---|---|
| [[Tears]] | HAS_FLUID_PROPERTY | Usually clear / variable |
| [[Urine]] | HAS_FLUID_PROPERTY | Yellow / variable |
| [[Menstrual Fluid]] | HAS_FLUID_PROPERTY | Red / brown / variable |
| [[Vaginal Fluid]] | HAS_FLUID_PROPERTY | Clear / white / variable |
| [[Milk]] | HAS_FLUID_PROPERTY | White / pale / variable |
| [[Blood]] | HAS_FLUID_PROPERTY | Red / dark red / variable |
| [[Sweat]] | HAS_FLUID_PROPERTY | Clear / variable |
| [[Saliva]] | HAS_FLUID_PROPERTY | Clear / variable |

## Sensory Boundary

Colour as a fluid property is distinct from visual perception, emotional response, symbolism, or authorial interpretation of colour.

## Relationship Statements

```text
Colour IS_FLUID_PROPERTY
Fluid Entity HAS_FLUID_PROPERTY Colour
Fluid Profile HAS_LOCAL_FLUID_PROPERTY Colour
Colour MAY_BE_PERCEIVED_BY Colour Sensory Profile
Colour MAY_BE_INTERPRETED_BY Symbolic Profile
```

## Status

Draft v0.1.
