---
tags:
  - Ontology Node
  - Fluid Layer
  - Fluid Entity
  - Status/Draft
title: Menstrual Fluid
canonical_name: Menstrual Fluid
file_class: Ontology Node
node_type: Fluid Entity
layer: Fluid Layer
status: Draft
version: 0.2
primary_system: Reproductive System
embodiment_scope: Anatomy-Dependent
fluid_class: Reproductive / Mixed
---

# Menstrual Fluid

## Purpose

This node defines Menstrual Fluid as a reusable fluid entity in the Somatic Meaning Engine.

It defines the fluid itself, not a local anatomical relationship, activation process, sensory perception, symbolic meaning, authorial language, or corpus use.

## Canonical Definition

Menstrual Fluid is a cyclical reproductive fluid associated with menstruation where relevant anatomy and physiology are present.

It may be referenced by anatomical profiles involving uterus, cervix, vaginal canal, vaginal opening, vulva, or external surface adjacency, but it should not be treated as produced by all sites where it becomes visible.

## Fluid Classification

| Field | Value |
|---|---|
| Node Type | Fluid Entity |
| Layer | Fluid Layer |
| Fluid Class | Reproductive / Mixed |
| Primary System | Reproductive System |
| Embodiment Scope | Anatomy-Dependent |
| Typical State | Liquid / Mixed / Variable |
| Cyclical | true |
| Conditional | true |

## Common Anatomical Sources

| Anatomical Source | Relationship | Notes |
|---|---|---|
| Uterus | Source / Origin Site | Existing anatomical anchor in Female Embodiment |
| Cervix | Conducts / Transitional | Existing anatomical anchor in Female Embodiment |
| Vaginal Canal | Conducts / Receives | Existing anatomical anchor in Female Embodiment |

## Common Anatomical Output or Surface Sites

| Anatomical Site | Relationship | Notes |
|---|---|---|
| Vaginal Opening | Output Site | Existing anatomical anchor |
| Vulva | Surface Presence / Adjacent | External presence only, not source |
| Perineum | Adjacent / Surface Presence | Local profile may be needed later |

## Fluid Properties

| Fluid Property | Range / Description | Notes |
|---|---|---|
| [[Viscosity]] | Thin / thick / variable | Neutral description only |
| [[Colour]] | Red / dark red / brown / variable | Neutral description only |
| [[Opacity]] | Translucent / opaque / variable | Neutral description only |
| [[Odour]] | Mild / metallic / variable | Neutral description only |
| [[Taste]] | Metallic / variable | Use only where relevant and not authorialized |
| [[Volume]] | Trace / low / moderate / high / variable | Context-dependent |
| [[Flow]] | Cyclical / discharge / variable | Activation profile defines process |
| [[Cyclicity]] | Reproductive / hormonal / cyclical | Fluid entity is cyclical by default |
| [[Surface Presence]] | Output / surface / adjacent / transferred / variable | Local profile defines anatomical relation |

## Common Activation Processes

| Activation Process | Relationship | Notes |
|---|---|---|
| Menstruation Activation Profile | Releases / Moves / Exposes | To be defined in Activation Layer |
| Cycle Regulation Activation Profile | Alters / Withholds / Releases | To be defined in Activation Layer |

## Expressive Layer Hooks

| Future Record | Purpose |
|---|---|
| Menstrual Fluid Sensory Profile | Perception of wetness, thickness, smell, colour, or flow |
| Menstrual Fluid Symbolic Profile | Symbolic associations and meaning |
| Menstrual Fluid Emotional Profile | Emotional context or affective charge |
| Menstrual Fluid Term Register | Authorial language rules |
| Menstrual Fluid Corpus Annotations | Usage across works |

## Boundary Rules

Do not define menstrual activation mechanics here. Do not define sensory interpretation, symbolic meaning, emotional meaning, authorial language, or corpus examples.

## Relationship Statements

```text
Menstrual Fluid IS_FLUID_ENTITY
Menstrual Fluid HAS_COMMON_SOURCE Uterus
Menstrual Fluid HAS_COMMON_OUTPUT_SITE Vaginal Opening
Menstrual Fluid HAS_FLUID_PROPERTY Viscosity
Menstrual Fluid HAS_FLUID_PROPERTY Colour
Menstrual Fluid HAS_FLUID_PROPERTY Opacity
Menstrual Fluid HAS_FLUID_PROPERTY Odour
Menstrual Fluid HAS_FLUID_PROPERTY Taste
Menstrual Fluid HAS_FLUID_PROPERTY Volume
Menstrual Fluid HAS_FLUID_PROPERTY Flow
Menstrual Fluid HAS_FLUID_PROPERTY Cyclicity
Menstrual Fluid HAS_FLUID_PROPERTY Surface Presence
Menstrual Fluid MAY_BE_PRODUCED_BY Menstruation Activation Profile
Menstrual Fluid MAY_BE_PRODUCED_BY Cycle Regulation Activation Profile
Menstrual Fluid MAY_BE_REFERENCED_BY Female - Vaginal Canal Fluid Profile
Menstrual Fluid MAY_BE_REFERENCED_BY Female - Vulva Fluid Profile
```

## Review Questions

1. Should Menstrual Fluid be modelled as a mixed fluid entity with subcomponents later?
2. How should embodiment scope be represented for Trans Masculine anatomy where relevant structures are present?
3. Which cycle and hormonal activation profiles need to exist before this entity is baseline?

## Status

Draft v0.2.
