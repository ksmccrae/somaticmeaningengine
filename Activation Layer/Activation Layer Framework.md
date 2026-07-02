---
tags:
  - Document/Framework
  - Layer/Activation
  - Status/Validated
title: Activation Layer Framework
file_class: Document
document_type: Framework
layer: Activation Layer
status: Validated
version: 0.4
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
= governed process node defining a physiological or embodied activation event or state change
```

Activation profiles may coordinate anatomy, fluid, mirror, motor, autonomic, and downstream candidates, but they define activation only.

## Activation Classification Model

```text
activation_type
= one controlled structural class

activation_components
= one or more controlled process families

activation_scope
= Local / Regional / Cross-System
```

Use `Composite Activation` when multiple process families are coordinated.

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

`Composite Activation` is structural. The other values may be direct types for simple profiles or components of a composite profile.

## Activation Scope Decision Rule

Scope is determined by active participation, not by proximity, adjacency, mirror linkage, or downstream possibility.

```text
Local
= one primary anatomical anchor undergoes the defined state change
= nearby anatomy may be referenced as context, adjacency, or mirror territory
= adjacency alone does not make the activation Regional
= mirror engagement alone does not make the activation Regional

Regional
= two or more nearby anatomical nodes actively participate in the same activation process
= each participating node has a defined process role rather than contextual relevance only

Cross-System
= the activation coordinates distinct anatomical systems, physiological systems, or separated body regions
= cross-system movement itself should hand off to Propagation where appropriate
```

Decision sequence:

```text
1. Identify every node undergoing or directly contributing to the state change.
2. Exclude nodes used only for adjacency, boundary context, mirror traversal, or downstream reference.
3. One active anchor = Local.
4. Two or more nearby active participants = Regional.
5. Distinct systems or separated regions = Cross-System.
```

`Composite` is not an activation scope.

## What Activation Owns

```text
trigger or condition
physiological process
participating anatomical nodes
tissue-state change
motor or kinetic change
fluid entity involvement where applicable
fluid property alteration where applicable
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
propagation routes beyond handoff
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

Activation references anatomical participants without redefining them.

`INVOLVES_ANATOMICAL_NODE` is reserved for a node that directly participates in the activation process.

`REFERENCES_ADJACENT_ANATOMICAL_SITE` is used when a nearby or boundary node is relevant but does not undergo or directly contribute to the defined state change.

## Relationship to Fluid Layer

Activation may coordinate fluid processes where relevant. Non-fluid activation profiles must not be forced to include Fluid Layer content.

## Relationship to Mirror Layer

Activation may make mirror routes available, engaged, weighted, or contextually relevant without redefining them.

Mirror engagement does not establish activation scope.

## Relationship to Propagation Layer

```text
Activation
= process starts or coordinates state change

Propagation
= response travels, spreads, echoes, radiates, or transfers across systems
```

A candidate handoff may be recorded before a Propagation Profile exists, but Activation must not define spread mechanics.

## Relationship to Downstream Systems

Activation may identify candidate Sensory, Pleasure, Desire, Meaning, Authorial, and Corpus records without defining them.

## Consent Boundary

```text
Arousal is not consent.
Lubrication is not consent.
Fluid release is not consent.
Autonomic response is not consent.
Muscular contraction is not consent.
Reflexive contraction is not consent.
Pleasure is not consent.
Desire is not consent.
Symbolic meaning is not consent.
```

## Current Validation Set

```text
Female - Vulvar Lubrication Activation Profile
Female - Paraurethral Glandular Release Activation Profile
Female - Pelvic Floor Contraction Activation Profile
```

The first profile tests fluid-dependent tissue-state activation and a Supported mirror route.

The second profile tests glandular release, fluid identity separation, adjacent anatomy, and a Candidate mirror route.

The third profile tests Motor / Kinetic Activation, tissue-state change, a fluid-independent local process, Candidate mirror engagement, boundary context, and possible Propagation handoff.

## Folder Structure

```text
Activation Layer
├── README.md
├── Activation Layer Framework.md
└── Activation Profiles
    ├── Activation Profiles Index.md
    ├── Female - Vulvar Lubrication Activation Profile.md
    ├── Female - Paraurethral Glandular Release Activation Profile.md
    └── Female - Pelvic Floor Contraction Activation Profile.md
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
activation may enable downstream systems, not define them
activation never implies consent
scope follows active participation, not proximity
adjacent anatomy must not be treated as source or participant anatomy by proximity alone
visible fluid must not be identified solely by location or surface presence
non-fluid profiles should remain fluid-independent unless fluid participation is required
```

## Validation Basis

This framework has been tested against three Candidate profiles covering:

```text
fluid-dependent activation
fluid-identity boundary activation
fluid-independent motor / kinetic activation
Supported and Candidate mirror routes
adjacent anatomy and adjacent fluid governance
candidate Propagation handoff
```

## Remaining Questions

1. When should Reflex Activation become a component rather than a trigger or modulator?
2. Which profile should test Hormonal / Cyclical Activation?
3. Which profile should first test Cross-System scope?
4. What criteria should promote a Candidate Activation Profile to Supported?

## Status

Validated v0.4.

This framework is validated as the governing architecture for Activation Profiles. It is not Baseline.
