---
tags:
  - Ontology Node
  - Fluid Layer
  - Fluid Entity
  - Status/Draft
title: Milk
canonical_name: Milk
file_class: Ontology Node
node_type: Fluid Entity
layer: Fluid Layer
status: Draft
version: 0.2
primary_system: Mammary / Lactation System
embodiment_scope: Conditional / Anatomy-Dependent
fluid_class: Exocrine / Reproductive-Adjacent
---

# Milk

## Purpose

This node defines Milk as a reusable fluid entity in the Somatic Meaning Engine.

It defines the fluid itself, not a local anatomical relationship, activation process, sensory perception, symbolic meaning, authorial language, or corpus use.

## Canonical Definition

Milk is lactation-related fluid associated with mammary tissue and nipple output pathways under specific physiological, hormonal, postpartum, medical, or induced-lactation conditions.

It may be referenced by anatomical profiles involving breasts, mammary tissue, nipples, ducts, and related chest or breast anatomy where relevant.

## Fluid Classification

| Field | Value |
|---|---|
| Node Type | Fluid Entity |
| Layer | Fluid Layer |
| Fluid Class | Exocrine / Reproductive-Adjacent |
| Primary System | Mammary / Lactation System |
| Embodiment Scope | Conditional / Anatomy-Dependent |
| Typical State | Liquid / Variable |
| Cyclical | conditional |
| Conditional | true |

## Common Anatomical Sources

| Anatomical Source | Relationship | Notes |
|---|---|---|
| Mammary Tissue | Produces / Conditional | Existing Female anatomical anchor |
| Breasts | Contains / Organizes | Local profile required |
| Nipples | Output Site / Conducts | Existing Female paired anatomical anchor |

## Common Anatomical Output or Surface Sites

| Anatomical Site | Relationship | Notes |
|---|---|---|
| Nipples | Output Site | Output under lactation conditions |
| Breast Skin | Adjacent / Surface Presence | Surface presence only |

## Fluid Properties

| Fluid Property | Range / Description | Notes |
|---|---|---|
| [[Viscosity]] | Thin / creamy / variable | Neutral description only |
| [[Colour]] | White / pale / yellowish / variable | Neutral description only |
| [[Opacity]] | Opaque / variable | Neutral description only |
| [[Odour]] | Mild / variable | Neutral description only |
| [[Taste]] | Sweet / variable | Use only where relevant and not authorialized |
| [[Volume]] | Trace / low / moderate / high / variable | Context-dependent |
| [[Flow]] | Drop / stream / release / variable | Activation profile defines process |
| [[Cyclicity]] | Hormonal / postpartum / contextual | Conditional rather than universal |
| [[Surface Presence]] | Trace / local / surface / transferred / variable | Local profile defines anatomical relation |

## Common Activation Processes

| Activation Process | Relationship | Notes |
|---|---|---|
| Lactation Activation Profile | Produces / Releases / Alters | To be defined in Activation Layer |
| Letdown Activation Profile | Releases / Moves | To be defined in Activation Layer |

## Expressive Layer Hooks

| Future Record | Purpose |
|---|---|
| Milk Sensory Profile | Perception of temperature, taste, smell, wetness, or flow |
| Milk Symbolic Profile | Symbolic associations and meaning |
| Milk Emotional Profile | Emotional context or affective charge |
| Milk Term Register | Authorial language rules |
| Milk Corpus Annotations | Usage across works |

## Boundary Rules

Do not define lactation mechanics here. Do not include sensory interpretation, symbolic meaning, emotional interpretation, authorial language, or corpus examples.

## Relationship Statements

```text
Milk IS_FLUID_ENTITY
Milk HAS_COMMON_SOURCE Mammary Tissue
Milk HAS_COMMON_OUTPUT_SITE Nipples
Milk HAS_FLUID_PROPERTY Viscosity
Milk HAS_FLUID_PROPERTY Colour
Milk HAS_FLUID_PROPERTY Opacity
Milk HAS_FLUID_PROPERTY Odour
Milk HAS_FLUID_PROPERTY Taste
Milk HAS_FLUID_PROPERTY Volume
Milk HAS_FLUID_PROPERTY Flow
Milk HAS_FLUID_PROPERTY Cyclicity
Milk HAS_FLUID_PROPERTY Surface Presence
Milk MAY_BE_PRODUCED_BY Lactation Activation Profile
Milk MAY_BE_PRODUCED_BY Letdown Activation Profile
Milk MAY_BE_REFERENCED_BY Female - Breasts Fluid Profile
```

## Review Questions

1. Should Milk be named Lactation Fluid canonically, with Milk as common alias?
2. Which embodiment-specific breast or chest configurations require separate fluid profiles?
3. Should induced lactation be handled through Activation, Hormonal, or Medical History layers?

## Status

Draft v0.2.
