---
tags:
  - Ontology Node
  - Fluid Layer
  - Fluid Entity
  - Status/Draft
title: Urine
canonical_name: Urine
file_class: Ontology Node
node_type: Fluid Entity
layer: Fluid Layer
status: Draft
version: 0.1
primary_system: Urinary System
embodiment_scope: Cross-Embodiment
fluid_class: Urinary
---

# Urine

## Purpose

This node defines Urine as a reusable fluid entity in the Somatic Meaning Engine.

It defines the fluid itself, not a local anatomical relationship, activation process, sensory perception, symbolic meaning, authorial language, or corpus use.

## Canonical Definition

Urine is urinary fluid associated with the urinary system.

It should be linked to anatomical profiles involving the kidneys, ureters, bladder, urethra, and urethral opening when those canonical anatomical nodes exist.

It may appear adjacent to external genital anatomical profiles, but those adjacent sites should not be treated as urinary sources.

## Fluid Classification

| Field | Value |
|---|---|
| Node Type | Fluid Entity |
| Layer | Fluid Layer |
| Fluid Class | Urinary |
| Primary System | Urinary System |
| Embodiment Scope | Cross-Embodiment |
| Typical State | Liquid |
| Cyclical | false |
| Conditional | true |

## Common Anatomical Sources

| Anatomical Source | Relationship | Notes |
|---|---|---|
| Kidneys | Produces | Canonical urinary anatomy required |
| Bladder | Stores | Canonical urinary anatomy required |
| Urethra | Conducts | Canonical urinary anatomy required |

## Common Anatomical Output or Surface Sites

| Anatomical Site | Relationship | Notes |
|---|---|---|
| Urethral Opening | Output Site | Existing or candidate anatomical anchor |
| Vestibule | Adjacent | Relevant in Female Embodiment but not a source |
| Vulva | Adjacent | External adjacency only, not source or conduit |

## Fluid Qualities

| Quality | Range / Description | Notes |
|---|---|---|
| Viscosity | Thin / watery | Neutral description only |
| Colour | Pale yellow / yellow / amber / variable | Physiological variation possible |
| Opacity | Clear / translucent / cloudy / variable | Neutral description only |
| Odour | Mild / strong / variable | Neutral description only |
| Taste | Saline / bitter / variable | Use only where relevant and not authorialized |
| Volume | Low / moderate / high / variable | Context-dependent |
| Flow | Stream / release / variable | Activation profile defines release mechanics |
| Cyclicity | None / contextual | Not cyclical by default |

## Common Activation Processes

| Activation Process | Relationship | Notes |
|---|---|---|
| Urination Activation Profile | Releases / Moves / Exposes | To be defined in Activation Layer |
| Bladder Control Activation Profile | Withholds / Releases | To be defined in Activation Layer |

## Expressive Layer Hooks

| Future Record | Purpose |
|---|---|
| Urine Sensory Profile | Perception of warmth, smell, flow, wetness, or contact |
| Urine Symbolic Profile | Symbolic associations and meaning |
| Urine Term Register | Authorial language rules |
| Urine Corpus Annotations | Usage across works |

## Boundary Rules

Do not assign urine production to external genital structures. Do not include activation mechanics, sensory interpretation, symbolic meaning, authorial language, or corpus examples.

## Relationship Statements

```text
Urine IS_FLUID_ENTITY
Urine HAS_COMMON_SOURCE Bladder
Urine HAS_COMMON_OUTPUT_SITE Urethral Opening
Urine MAY_BE_PRODUCED_BY Urination Activation Profile
```

## Review Questions

1. Which urinary anatomical anchors need to be created before urine profiles can be validated?
2. Should Urine remain cross-embodiment with embodiment-specific output profiles?
3. Should hydration and medical variation belong in Fluid Layer, Medical History, or Environmental Layer?

## Status

Draft v0.1.
