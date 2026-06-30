---
tags:
  - Ontology Node
  - Fluid Layer
  - Fluid Entity
  - Status/Draft
title: Saliva
canonical_name: Saliva
file_class: Ontology Node
node_type: Fluid Entity
layer: Fluid Layer
status: Draft
version: 0.1
primary_system: Oral / Digestive System
embodiment_scope: Cross-Embodiment
fluid_class: Exocrine / Oral
---

# Saliva

## Purpose

This node defines Saliva as a reusable fluid entity in the Somatic Meaning Engine.

It defines the fluid itself, not a local anatomical relationship, activation process, sensory perception, symbolic meaning, authorial language, or corpus use.

## Canonical Definition

Saliva is oral exocrine fluid associated with salivary glands and the mouth.

It may be referenced by anatomical fluid profiles involving salivary glands, mouth, tongue, lips, teeth, throat, skin contact, or external surface transfer.

## Fluid Classification

| Field | Value |
|---|---|
| Node Type | Fluid Entity |
| Layer | Fluid Layer |
| Fluid Class | Exocrine / Oral |
| Primary System | Oral / Digestive System |
| Embodiment Scope | Cross-Embodiment |
| Typical State | Liquid / Mucosal / Variable |
| Cyclical | false |
| Conditional | true |

## Common Anatomical Sources

| Anatomical Source | Relationship | Notes |
|---|---|---|
| Salivary Glands | Produces | Canonical oral anatomy required |
| Mouth | Contains / Surface Presence | Local anatomical profile required |
| Tongue | Surface Presence | Local anatomical profile required |

## Common Anatomical Output or Surface Sites

| Anatomical Site | Relationship | Notes |
|---|---|---|
| Mouth | Contains / Output Site | Local profile required |
| Lips | Surface Presence / Output Site | Local profile required |
| Skin Surface | Transfer / Surface Presence | Local profile may be required |

## Fluid Qualities

| Quality | Range / Description | Notes |
|---|---|---|
| Viscosity | Thin / mucosal / thick / variable | Neutral description only |
| Colour | Clear / variable | Neutral description only |
| Opacity | Clear / translucent / variable | Neutral description only |
| Odour | None / mild / variable | Neutral description only |
| Taste | Neutral / saline / variable | Use only where relevant and not authorialized |
| Volume | Trace / low / moderate / high / variable | Context-dependent |
| Flow | Oral surface / droplet / transfer / variable | Local profile defines path |
| Cyclicity | None / contextual | Not cyclical by default |

## Common Activation Processes

| Activation Process | Relationship | Notes |
|---|---|---|
| Salivation Activation Profile | Produces / Alters | To be defined in Activation Layer |
| Swallowing Activation Profile | Moves | To be defined in Activation Layer |
| Spitting Activation Profile | Releases / Exposes | To be defined in Activation Layer |

## Expressive Layer Hooks

| Future Record | Purpose |
|---|---|
| Saliva Sensory Profile | Perception of wetness, taste, viscosity, or oral texture |
| Saliva Symbolic Profile | Symbolic associations and meaning |
| Saliva Emotional Profile | Emotional context or affective charge |
| Saliva Term Register | Authorial language rules |
| Saliva Corpus Annotations | Usage across works |

## Boundary Rules

Do not define salivation mechanics here. Do not include sensory interpretation, symbolic meaning, emotional interpretation, authorial language, or corpus examples.

## Relationship Statements

```text
Saliva IS_FLUID_ENTITY
Saliva HAS_COMMON_SOURCE Salivary Glands
Saliva HAS_COMMON_OUTPUT_SITE Mouth
Saliva MAY_BE_PRODUCED_BY Salivation Activation Profile
```

## Review Questions

1. Which oral anatomical anchors are required before Saliva can be baseline?
2. Should external transfer belong to Saliva entity, local fluid profiles, or activation events?
3. Should swallowing and spitting be separate activation profiles?

## Status

Draft v0.1.
