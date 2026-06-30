---
tags:
  - Ontology Node
  - Fluid Layer
  - Fluid Entity
  - Status/Draft
title: Vaginal Fluid
canonical_name: Vaginal Fluid
file_class: Ontology Node
node_type: Fluid Entity
layer: Fluid Layer
status: Draft
version: 0.1
primary_system: Reproductive System
embodiment_scope: Anatomy-Dependent
fluid_class: Reproductive / Mucosal
---

# Vaginal Fluid

## Purpose

This node defines Vaginal Fluid as a reusable fluid entity in the Somatic Meaning Engine.

It defines the fluid itself, not a local anatomical relationship, activation process, sensory perception, symbolic meaning, authorial language, or corpus use.

## Canonical Definition

Vaginal Fluid is a mucosal and reproductive-tract fluid associated with the vaginal canal and related internal genital structures where relevant anatomy is present.

It may be referenced by anatomical fluid profiles involving vaginal mucosa, vaginal canal, vaginal opening, vestibule, or vulva, while keeping source, conduit, output, and adjacent relationships separate.

## Fluid Classification

| Field | Value |
|---|---|
| Node Type | Fluid Entity |
| Layer | Fluid Layer |
| Fluid Class | Reproductive / Mucosal |
| Primary System | Reproductive System |
| Embodiment Scope | Anatomy-Dependent |
| Typical State | Liquid / Mucosal / Variable |
| Cyclical | conditional |
| Conditional | true |

## Common Anatomical Sources

| Anatomical Source | Relationship | Notes |
|---|---|---|
| Vaginal Mucosa | Surface Moisture / Source-Adjacent | Existing anatomical anchor in Female Embodiment |
| Vaginal Canal | Receives / Contains / Surface Presence | Existing anatomical anchor in Female Embodiment |
| Cervix | Adjacent / Contributes | Cervical mucus should remain a separate fluid entity |

## Common Anatomical Output or Surface Sites

| Anatomical Site | Relationship | Notes |
|---|---|---|
| Vaginal Opening | Output Site / Surface Presence | Existing anatomical anchor |
| Vestibule | Adjacent / Surface Presence | Existing anatomical anchor |
| Vulva | Adjacent / Surface Presence | External presence only, not primary source |

## Fluid Qualities

| Quality | Range / Description | Notes |
|---|---|---|
| Viscosity | Thin / mucosal / thick / variable | Neutral description only |
| Colour | Clear / white / pale / variable | Neutral description only |
| Opacity | Clear / translucent / opaque / variable | Neutral description only |
| Odour | None / mild / variable | Neutral description only |
| Taste | Saline / acidic / variable | Use only where relevant and not authorialized |
| Volume | Trace / low / moderate / high / variable | Context-dependent |
| Flow | Surface / discharge / variable | Local profile defines path |
| Cyclicity | Contextual / hormonal / reproductive / variable | Not always cyclical in the same way as menstrual fluid |

## Common Activation Processes

| Activation Process | Relationship | Notes |
|---|---|---|
| Vaginal Lubrication Activation Profile | Produces / Alters / Exposes | To be defined in Activation Layer |
| Cycle-Related Moisture Activation Profile | Alters | To be defined in Activation Layer |

## Expressive Layer Hooks

| Future Record | Purpose |
|---|---|
| Vaginal Fluid Sensory Profile | Perception of wetness, texture, smell, taste, or flow |
| Vaginal Fluid Symbolic Profile | Symbolic associations and meaning |
| Vaginal Fluid Term Register | Authorial language rules |
| Vaginal Fluid Corpus Annotations | Usage across works |

## Boundary Rules

Do not collapse Vaginal Fluid with Cervical Mucus, Menstrual Fluid, Urine, or Paraurethral Glandular Fluid. Do not include activation mechanics, sensory interpretation, symbolic meaning, authorial language, or corpus examples.

## Relationship Statements

```text
Vaginal Fluid IS_FLUID_ENTITY
Vaginal Fluid HAS_COMMON_SOURCE Vaginal Mucosa
Vaginal Fluid HAS_COMMON_OUTPUT_SITE Vaginal Opening
Vaginal Fluid MAY_BE_PRODUCED_BY Vaginal Lubrication Activation Profile
```

## Review Questions

1. Should Vaginal Fluid and Cervical Mucus remain separate fluid entities?
2. Should fluid variation by hormonal state be handled here or in activation / hormonal profiles?
3. Which anatomical anchors are required before this entity can be baseline?

## Status

Draft v0.1.
