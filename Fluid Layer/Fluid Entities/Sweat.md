---
tags:
  - Ontology Node
  - Fluid Layer
  - Fluid Entity
  - Status/Draft
title: Sweat
canonical_name: Sweat
file_class: Ontology Node
node_type: Fluid Entity
layer: Fluid Layer
status: Draft
version: 0.1
primary_system: Integumentary System
embodiment_scope: Cross-Embodiment
fluid_class: Exocrine / Surface
---

# Sweat

## Purpose

This node defines Sweat as a reusable fluid entity in the Somatic Meaning Engine.

It defines the fluid itself, not a local anatomical relationship, activation process, sensory perception, symbolic meaning, authorial language, or corpus use.

## Canonical Definition

Sweat is exocrine surface fluid associated with sweat glands and the skin.

It may be referenced by anatomical fluid profiles involving skin surfaces, palms, armpits, face, back, groin, scalp, or other surface regions where sweating occurs.

## Fluid Classification

| Field | Value |
|---|---|
| Node Type | Fluid Entity |
| Layer | Fluid Layer |
| Fluid Class | Exocrine / Surface |
| Primary System | Integumentary System |
| Embodiment Scope | Cross-Embodiment |
| Typical State | Liquid |
| Cyclical | false |
| Conditional | true |

## Common Anatomical Sources

| Anatomical Source | Relationship | Notes |
|---|---|---|
| Sweat Glands | Produces | Canonical integumentary anatomy required |
| Skin | Surface Presence | Local anatomical profile required |

## Common Anatomical Output or Surface Sites

| Anatomical Site | Relationship | Notes |
|---|---|---|
| Skin Surface | Surface Presence | General output surface |
| Palms | Surface Presence | Local profile may be required |
| Face | Surface Presence | Local profile may be required |
| Axillary Region | Surface Presence | Local profile may be required |

## Fluid Qualities

| Quality | Range / Description | Notes |
|---|---|---|
| Viscosity | Thin / watery / variable | Neutral description only |
| Colour | Clear / variable | Neutral description only |
| Opacity | Clear / translucent | Neutral description only |
| Odour | None / mild / strong / variable | Neutral description only |
| Taste | Saline / variable | Use only where relevant and not authorialized |
| Volume | Trace / low / moderate / high / variable | Context-dependent |
| Flow | Surface / bead / film / stream / variable | Local profile defines surface pattern |
| Cyclicity | None / contextual | Not cyclical by default |

## Common Activation Processes

| Activation Process | Relationship | Notes |
|---|---|---|
| Sweating Activation Profile | Produces / Releases / Exposes | To be defined in Activation Layer |
| Heat Response Activation Profile | Produces / Alters | To be defined in Activation Layer |
| Stress Response Activation Profile | Produces / Alters | To be defined in Activation Layer |

## Expressive Layer Hooks

| Future Record | Purpose |
|---|---|
| Sweat Sensory Profile | Perception of wetness, salt, odour, temperature, or surface movement |
| Sweat Symbolic Profile | Symbolic associations and meaning |
| Sweat Emotional Profile | Emotional context or affective charge |
| Sweat Term Register | Authorial language rules |
| Sweat Corpus Annotations | Usage across works |

## Boundary Rules

Do not define sweating mechanics here. Do not include sensory interpretation, symbolic meaning, emotional interpretation, authorial language, or corpus examples.

## Relationship Statements

```text
Sweat IS_FLUID_ENTITY
Sweat HAS_COMMON_SOURCE Sweat Glands
Sweat HAS_COMMON_OUTPUT_SITE Skin Surface
Sweat MAY_BE_PRODUCED_BY Sweating Activation Profile
```

## Review Questions

1. Should Sweat be split into thermoregulatory and stress-related subtypes?
2. Should surface accumulation patterns belong here or in local anatomical fluid profiles?
3. Which skin and surface anatomical anchors are required before baseline?

## Status

Draft v0.1.
