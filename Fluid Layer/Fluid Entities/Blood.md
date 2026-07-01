---
tags:
  - Ontology Node
  - Fluid Layer
  - Fluid Entity
  - Status/Draft
title: Blood
canonical_name: Blood
file_class: Ontology Node
node_type: Fluid Entity
layer: Fluid Layer
status: Draft
version: 0.2
primary_system: Circulatory System
embodiment_scope: Cross-Embodiment
fluid_class: Circulatory
---

# Blood

## Purpose

This node defines Blood as a reusable fluid entity in the Somatic Meaning Engine.

It defines the fluid itself, not a local anatomical relationship, activation process, sensory perception, symbolic meaning, authorial language, or corpus use.

## Canonical Definition

Blood is circulatory fluid associated with the cardiovascular system.

It may be referenced by anatomical fluid profiles involving blood vessels, capillaries, tissue injury, mucosal surfaces, menstrual pathways, wounds, or surface exposure, while keeping circulatory source, local exposure, and reproductive-cycle contexts distinct.

## Fluid Classification

| Field | Value |
|---|---|
| Node Type | Fluid Entity |
| Layer | Fluid Layer |
| Fluid Class | Circulatory |
| Primary System | Circulatory System |
| Embodiment Scope | Cross-Embodiment |
| Typical State | Liquid |
| Cyclical | conditional |
| Conditional | true |

## Common Anatomical Sources

| Anatomical Source | Relationship | Notes |
|---|---|---|
| Heart | Circulates | Canonical circulatory anatomy required |
| Blood Vessels | Conducts | Canonical vascular anatomy required |
| Capillaries | Conducts / Exposes | Local tissue profiles may reference this |

## Common Anatomical Output or Surface Sites

| Anatomical Site | Relationship | Notes |
|---|---|---|
| Skin Surface | Surface Presence | Usually via injury or rupture |
| Mucosal Surface | Surface Presence | Local anatomical profile required |
| Vaginal Opening | Output Site / Contextual | Relevant to menstrual fluid distinction |

## Fluid Properties

| Fluid Property | Range / Description | Notes |
|---|---|---|
| [[Viscosity]] | Moderate / variable | Neutral description only |
| [[Colour]] | Red / dark red / brownish / variable | Neutral description only |
| [[Opacity]] | Opaque | Neutral description only |
| [[Odour]] | Metallic / variable | Neutral description only |
| [[Taste]] | Metallic / saline / variable | Use only where relevant and not authorialized |
| [[Volume]] | Trace / low / moderate / high / variable | Context-dependent |
| [[Flow]] | Internal circulation / surface flow / discharge / variable | Activation or injury profile defines process |
| [[Cyclicity]] | None / contextual / reproductive-cycle related | Menstrual fluid should remain a distinct entity |
| [[Surface Presence]] | Internal / exposed / surface / transferred / variable | Local profile defines anatomical relation |

## Common Activation Processes

| Activation Process | Relationship | Notes |
|---|---|---|
| Bleeding Activation Profile | Releases / Exposes | To be defined in Activation Layer |
| Bruising Activation Profile | Alters / Exposes Internally | To be defined in Activation Layer |
| Circulation Activation Profile | Moves | To be defined in Activation Layer |

## Expressive Layer Hooks

| Future Record | Purpose |
|---|---|
| Blood Sensory Profile | Perception of wetness, temperature, smell, taste, or visual presence |
| Blood Symbolic Profile | Symbolic associations and meaning |
| Blood Emotional Profile | Emotional context or affective charge |
| Blood Term Register | Authorial language rules |
| Blood Corpus Annotations | Usage across works |

## Boundary Rules

Do not collapse Blood with Menstrual Fluid. Do not define activation mechanics, sensory interpretation, symbolic meaning, emotional interpretation, authorial language, or corpus examples.

## Relationship Statements

```text
Blood IS_FLUID_ENTITY
Blood HAS_COMMON_SOURCE Blood Vessels
Blood HAS_COMMON_OUTPUT_SITE Skin Surface
Blood HAS_FLUID_PROPERTY Viscosity
Blood HAS_FLUID_PROPERTY Colour
Blood HAS_FLUID_PROPERTY Opacity
Blood HAS_FLUID_PROPERTY Odour
Blood HAS_FLUID_PROPERTY Taste
Blood HAS_FLUID_PROPERTY Volume
Blood HAS_FLUID_PROPERTY Flow
Blood HAS_FLUID_PROPERTY Cyclicity
Blood HAS_FLUID_PROPERTY Surface Presence
Blood MAY_BE_PRODUCED_BY Bleeding Activation Profile
Blood MAY_BE_PRODUCED_BY Bruising Activation Profile
Blood MAY_BE_PRODUCED_BY Circulation Activation Profile
Blood MAY_BE_REFERENCED_BY Tissue Injury Fluid Profile
```

## Review Questions

1. Should Blood remain one fluid entity with menstrual fluid as separate mixed entity?
2. Should capillary exposure be modelled through local tissue profiles or activation events?
3. Which vascular anatomical anchors are needed before baseline?

## Status

Draft v0.2.
