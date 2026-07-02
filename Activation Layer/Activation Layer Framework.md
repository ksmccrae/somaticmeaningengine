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
version: 0.6
last_updated: 2026-07-02
---

# Activation Layer Framework

## Purpose

The Activation Layer models governed physiological, embodied, and processual state changes without redefining other ontology layers.

## Classification Model

```text
activation_type
= one controlled structural class

activation_components
= one or more controlled process families

activation_scope
= Local / Regional / Cross-System
```

Controlled values:

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

`Composite Activation` is structural. Other values may be direct types or components.

## Scope Decision Rule

```text
Local
= one active anatomical anchor

Regional
= two or more nearby anatomical nodes directly participate

Cross-System
= distinct systems or separated regions are coordinated
```

Adjacency, output context, mirror engagement, downstream references, and possible Propagation handoff do not increase scope by themselves.

## Hormonal / Cyclical Activation Governance

Hormonal / Cyclical Activation models recurring, phase-dependent, or hormonally influenced process coordination.

It may define:

```text
cycle or phase context
recurrence
phase transition
hormonally influenced timing
cyclical tissue-state change
cyclical fluid release or withholding
anatomical coordination across a recurring process
```

It must not define:

```text
missing Hormone Entities
endocrine anatomy
hormone production pathways
receptor mechanisms
laboratory values
clinical diagnosis
sensory or emotional meaning
```

Neutral language such as `hormonal or cyclical context` is permitted when detailed endocrine nodes are not yet modelled.

Hormonal influence does not by itself establish Cross-System scope.

## Cyclical Regulation versus Active Phase

Hormonal / Cyclical profiles must distinguish between regulation of a recurring cycle and execution of one active phase.

```text
Cycle Regulation Activation Profile
= coordinates recurrence, phase progression, timing, suppression, delay, or transition across a cycle

Active Phase Activation Profile
= defines the physiological process occurring during one bounded phase of that cycle
```

A cycle-regulation profile must not absorb every phase-specific tissue, fluid, or motor process.

An active-phase profile must not become the owner of the entire cycle.

A regulatory profile may contextualize or enable an active-phase profile in prose. A formal Activation-to-Activation relationship verb should not be added until repeated use establishes a stable need.

## Temporal Governance

Cyclical profiles should distinguish:

```text
cycle context
phase entry
active state change
movement or release where applicable
phase completion or cessation
recurrence potential
```

Temporal sequence belongs to Activation. Cross-system transmission belongs to Propagation.

## Layer Boundaries

Activation owns triggers, process sequence, participating anatomy, state change, fluid involvement where applicable, modulators, and downstream candidates.

Activation does not own canonical anatomy, fluid identity, mirror correspondence, propagation mechanics, sensation, pleasure, desire, consent, symbolic meaning, authorial language, or corpus truth.

## Relationship Governance

```text
ACTIVATES_ANATOMICAL_SITE
= primary site undergoing change

INVOLVES_ANATOMICAL_NODE
= another node directly participating

REFERENCES_ADJACENT_ANATOMICAL_SITE
= nearby, boundary, or output context only

INVOLVES_FLUID_ENTITY
= fluid directly participating

REFERENCES_ADJACENT_FLUID_ENTITY
= fluid used for distinction only
```

Output territory may use `REFERENCES_ADJACENT_ANATOMICAL_SITE` until repeated use justifies a dedicated output relationship.

## Propagation Boundary

```text
Activation
= process begins or coordinates change

Propagation
= response travels or transfers beyond the activation process
```

A candidate handoff may be recorded without defining spread mechanics.

## Consent Boundary

```text
Physiological activation is not consent.
Hormonal state is not consent.
Menstruation is not consent.
Fluid release is not consent.
Autonomic response is not consent.
Muscular contraction is not consent.
Pleasure is not consent.
Desire is not consent.
Symbolic meaning is not consent.
```

## Validation Set

```text
Female - Vulvar Lubrication Activation Profile
Female - Paraurethral Glandular Release Activation Profile
Female - Pelvic Floor Contraction Activation Profile
Female - Menstruation Activation Profile
Female - Menstrual Cycle Regulation Activation Profile
```

The fourth profile tests active-phase Hormonal / Cyclical execution with Menstrual Fluid involvement.

The fifth profile tests cycle-level regulation without requiring Fluid Activation.

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

## Status

Validated v0.6.

This version separates cycle regulation from active-phase execution and clarifies output-context handling.
