---
tags:
  - Document/Framework
  - Layer/Activation
  - Status/Draft
title: Activation Layer Framework
file_class: Document
document_type: Framework
layer: Activation Layer
status: Draft
version: 0.2
last_updated: 2026-07-01
---

# Activation Layer Framework

## Purpose

The Activation Layer models governed physiological, embodied, and processual state changes.

Activation records define how responses occur without redefining canonical anatomy, fluid entities, mirror routes, sensory experience, pleasure, desire, symbolic meaning, authorial language, or corpus usage.

## Layer Position

```text
Canonical Embodiment
→ defines what exists

Fluid Layer
→ defines fluid entities, properties, and local anatomical fluid relationships

Mirror Layer
→ defines correspondence routes that may become traversable

Activation Layer
→ defines physiological process, state change, route availability, and process coordination

Propagation Layer
→ defines movement across systems once activation needs cross-system transmission

Sensory Layer
→ defines what is perceived

Pleasure Register
→ defines sensory valence

Desire Register
→ defines motivational or affective orientation

Symbolic Meaning Register
→ defines downstream interpretation

Authorial Systems
→ define language and style

Corpus
→ records specific usage
```

## Core Architectural Rule

```text
Activation Profile
= governed process node defining a physiological or embodied activation event/state-change
```

Activation profiles may coordinate anatomy, fluid, mirror, and downstream candidates, but they define activation only.

## Activation Classification Model

Activation classification uses three distinct fields.

```text
activation_type
= one controlled structural class

activation_components
= one or more controlled process families

activation_scope
= anatomical or systemic reach
```

Use:

```yaml
activation_type: Composite Activation
activation_components:
  - Fluid Activation
  - Mirror-Route Activation
activation_scope: Regional
```

when multiple process families are coordinated.

Do not join multiple controlled values into one slash-separated YAML string.

## Controlled Activation Types and Components

```text
Tissue-State Activation
Fluid Activation
Mirror-Route Activation
Motor / Kinetic Activation
Autonomic Activation
Hormonal / Cyclical Activation
Reflex Activation
Composite Activation
```

`Composite Activation` is a structural type. The other values may function as direct types for simple profiles or as components within a composite profile.

## Activation Scope

```text
Local
= primarily within one anatomical anchor or tightly bounded site

Regional
= coordinates multiple nearby anatomical anchors

Cross-System
= coordinates multiple systems or body regions
```

`Composite` is not an activation scope.

## What Activation Owns

```text
trigger or condition
physiological process
participating anatomical nodes
tissue-state change
fluid entity involvement
fluid property alteration
fluid profile involvement
mirror route availability
process sequence
state transitions
inhibiting or modulating conditions
candidate downstream links
```

## What Activation Does Not Own

```text
canonical anatomical definitions
fluid entity definitions
fluid property definitions
mirror correspondence definitions
propagation routes beyond local process handoff
sensory perception
pleasure or discomfort as valence
desire or motivational orientation
consent state
symbolic meaning
emotional meaning
authorial terminology
corpus truth
narrative effect
```

## Relationship to Canonical Embodiment

Activation profiles reference anatomical participants without redefining them.

## Relationship to Fluid Layer

Activation may define that a process produces, releases, moves, exposes, withholds, or alters a fluid. Fluid identity and local anatomical relationships remain in the Fluid Layer.

## Relationship to Mirror Layer

Activation may make mirror routes available, engaged, weighted, or contextually relevant. It does not create or redefine the mirror route.

## Relationship to Propagation Layer

```text
Activation
= process starts or coordinates state change

Propagation
= response travels, spreads, echoes, radiates, or transfers across systems
```

## Relationship to Downstream Systems

Activation profiles may identify candidate downstream records but must not define them.

```text
Sensory Profile
Pleasure Register
Desire Register
Symbolic Meaning Register
Authorial Term Register
Corpus Annotation
```

## Consent Boundary

```text
Arousal is not consent.
Lubrication is not consent.
Fluid release is not consent.
Autonomic response is not consent.
Pleasure is not consent.
Desire is not consent.
Symbolic meaning is not consent.
```

## Current Validation Set

```text
Female - Vulvar Lubrication Activation Profile
Female - Paraurethral Glandular Release Activation Profile
```

The first profile tests:

```text
vulvar primary anchoring
vaginal fluid involvement
fluid-property alteration
supported vulva-to-clitoral-complex mirror engagement
normalized Composite Activation classification
```

The second profile tests:

```text
Skene's glands as primary source anatomy
Paraurethral Glandular Fluid as a distinct fluid entity
Urine as adjacent but separate fluid
urethral opening as adjacent territory rather than automatic glandular source
candidate Skene's-glands-to-urethral-opening mirror engagement
regional glandular release process
```

## Folder Structure

```text
Activation Layer
├── Activation Layer Framework.md
└── Activation Profiles
    ├── Activation Profiles Index.md
    ├── Female - Vulvar Lubrication Activation Profile.md
    └── Female - Paraurethral Glandular Release Activation Profile.md
```

## Relationship Statements

```text
Activation Profile IS_ACTIVATION_PROFILE
Activation Profile HAS_ACTIVATION_TYPE Activation Type
Activation Profile HAS_ACTIVATION_COMPONENT Activation Component
Activation Profile HAS_ACTIVATION_SCOPE Activation Scope
Activation Profile ACTIVATES_ANATOMICAL_SITE Anatomical Node
Activation Profile INVOLVES_ANATOMICAL_NODE Anatomical Node
Activation Profile REFERENCES_ADJACENT_ANATOMICAL_SITE Anatomical Node
Activation Profile INVOLVES_FLUID_ENTITY Fluid Entity
Activation Profile REFERENCES_ADJACENT_FLUID_ENTITY Fluid Entity
Activation Profile REFERENCES_FLUID_PROFILE Fluid Profile
Activation Profile MAY_ALTER_FLUID_PROPERTY Fluid Property
Activation Profile MAY_ENGAGE_MIRROR_ROUTE Mirror Profile
Activation Profile MAY_HAND_OFF_TO Propagation Profile
Activation Profile MAY_ENABLE Sensory Profile
Activation Profile MAY_ENABLE Pleasure Register
Activation Profile MAY_CONTEXTUALIZE Desire Register
Activation Profile MAY_BE_INTERPRETED_BY Symbolic Meaning Register
Activation Profile MAY_BE_USED_BY Authorial Term Register
Activation Profile MAY_BE_ANNOTATED_IN Corpus Annotation
```

## Governance Notes

```text
activation defines process, not anatomy
activation coordinates fluid involvement, not fluid identity
activation may engage mirror routes, not define mirror correspondence
activation may hand off to propagation, not define propagation
activation may enable sensation, pleasure, desire, or symbolic meaning downstream, not define them
activation never implies consent
adjacent anatomy must not be treated as source anatomy by proximity alone
visible fluid must not be identified solely by location or surface presence
```

## Review Questions

1. Is the type/component/scope model sufficient across multiple activation families?
2. Should Autonomic Activation remain a component of the paraurethral profile or become a modulator?
3. Are adjacent anatomy and adjacent fluid relationship verbs sufficiently governed?
4. Does Female - Vestibular Gland Openings require canonical refinement?
5. Which third activation should test a non-fluid family?
6. Which activation profiles are required before Propagation or Sensory validation?
7. Should consent receive separate governance before corpus stress testing resumes?

## Status

Draft v0.2.

This framework reflects the normalized activation classification model and the first two Candidate validation profiles.
