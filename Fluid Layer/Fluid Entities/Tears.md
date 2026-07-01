---
tags:
  - Ontology Node
  - Fluid Layer
  - Fluid Entity
  - Status/Draft
title: Tears
canonical_name: Tears
file_class: Ontology Node
node_type: Fluid Entity
layer: Fluid Layer
status: Draft
version: 0.2
primary_system: Lacrimal System
embodiment_scope: Cross-Embodiment
fluid_class: Exocrine / Surface
---

# Tears

## Purpose

This node defines Tears as a reusable fluid entity in the Somatic Meaning Engine.

It defines the fluid itself, not a local anatomical relationship, activation process, sensory perception, symbolic meaning, authorial language, or corpus use.

## Canonical Definition

Tears are lacrimal fluid associated with the eye and lacrimal system.

They may be referenced by anatomical fluid profiles involving the eyes, lacrimal glands, tear ducts, eyelids, face, or cheeks.

They may also be referenced by activation profiles involving crying, irritation, reflex tearing, emotional expression, pain response, or environmental exposure.

## Fluid Classification

| Field | Value |
|---|---|
| Node Type | Fluid Entity |
| Layer | Fluid Layer |
| Fluid Class | Exocrine / Surface |
| Primary System | Lacrimal System |
| Embodiment Scope | Cross-Embodiment |
| Typical State | Liquid |
| Cyclical | false |
| Conditional | true |

## Common Anatomical Sources

| Anatomical Source | Relationship | Notes |
|---|---|---|
| Lacrimal glands | Produces | Source structure to be linked when canonical eye anatomy is populated |
| Eye surface | Receives / Surface Presence | Local anatomical profile to be modelled separately |

## Common Anatomical Output or Surface Sites

| Anatomical Site | Relationship | Notes |
|---|---|---|
| Eye | Surface Presence | Local profile required |
| Eyelids | Conducts / Surface Presence | Local profile required |
| Face / Cheeks | Surface Presence | Downstream anatomical anchors required |

## Fluid Properties

| Fluid Property | Range / Description | Notes |
|---|---|---|
| [[Viscosity]] | Thin / watery / variable | Neutral description only |
| [[Colour]] | Clear / variable | Neutral description only |
| [[Opacity]] | Clear / translucent | Neutral description only |
| [[Odour]] | None / mild / variable | Neutral description only |
| [[Taste]] | Saline / variable | Use only where relevant and not authorialized |
| [[Volume]] | Trace / low / moderate / high / variable | Context-dependent |
| [[Flow]] | Surface / stream / variable | Local profile determines anatomical path |
| [[Cyclicity]] | None / contextual | Not cyclical by default |
| [[Surface Presence]] | Trace / surface / stream / transferred / variable | Local profile defines anatomical relation |

## Common Activation Processes

| Activation Process | Relationship | Notes |
|---|---|---|
| Crying Activation Profile | Produces / Releases / Exposes | To be defined in Activation Layer |
| Reflex Tearing Activation Profile | Produces / Releases | To be defined in Activation Layer |

## Expressive Layer Hooks

| Future Record | Purpose |
|---|---|
| Tears Sensory Profile | Perception of wetness, salt, temperature, or surface movement |
| Tears Symbolic Profile | Symbolic associations and meaning |
| Tears Emotional Profile | Emotional context or affective charge |
| Tears Term Register | Authorial language rules |
| Tears Corpus Annotations | Usage across works |

## Boundary Rules

Do not include activation mechanics, sensory interpretation, symbolic meaning, emotional interpretation, authorial language, or corpus examples.

## Relationship Statements

```text
Tears IS_FLUID_ENTITY
Tears HAS_COMMON_SOURCE Lacrimal Glands
Tears HAS_COMMON_OUTPUT_SITE Eye
Tears HAS_FLUID_PROPERTY Viscosity
Tears HAS_FLUID_PROPERTY Colour
Tears HAS_FLUID_PROPERTY Opacity
Tears HAS_FLUID_PROPERTY Odour
Tears HAS_FLUID_PROPERTY Taste
Tears HAS_FLUID_PROPERTY Volume
Tears HAS_FLUID_PROPERTY Flow
Tears HAS_FLUID_PROPERTY Cyclicity
Tears HAS_FLUID_PROPERTY Surface Presence
Tears MAY_BE_PRODUCED_BY Crying Activation Profile
Tears MAY_BE_PRODUCED_BY Reflex Tearing Activation Profile
Tears MAY_BE_REFERENCED_BY Eye Fluid Profile
```

## Review Questions

1. Should Tears be split into basal, reflex, and emotional tear subtypes?
2. Should lacrimal fluid be the canonical entity name, with Tears as alias?
3. Which anatomical eye nodes must exist before Tears can be fully linked?

## Status

Draft v0.2.
