---
tags:
  - Template/Translation
  - Template/Activation Profile
  - Status/Validated
aliases:
  - Activation Profile Template
title: Activation Profile Template
file_class: Template
template_type: Translation
node_type: Activation Profile
layer: Activation Layer
status: Validated
version: 0.6
last_updated: 2026-07-02
---

# Activation Profile Template

## Purpose

This template defines the required structure for Activation Profile nodes.

## Classification Rule

```text
activation_type
= one controlled structural class

activation_components
= one or more controlled process families

activation_scope
= Local / Regional / Cross-System
```

Controlled components:

```text
Tissue-State Activation
Fluid Activation
Mirror-Route Activation
Motor / Kinetic Activation
Autonomic Activation
Hormonal / Cyclical Activation
Reflex Activation
```

Use `Composite Activation` when multiple components are coordinated.

## Scope Rule

```text
Local
= one active anatomical anchor

Regional
= two or more nearby anatomical nodes directly participate

Cross-System
= distinct systems or separated regions are coordinated
```

Do not count adjacency, output context, mirror context, downstream references, or possible Propagation handoff as active participation.

## Hormonal / Cyclical Profile Rule

A profile using `Hormonal / Cyclical Activation` should include:

```text
cycle or phase context
phase entry or onset
active tissue or fluid change where applicable
phase completion or cessation
recurrence potential
```

Use neutral `hormonal or cyclical context` language when detailed hormone nodes do not exist.

Do not invent Hormone Entities, endocrine pathways, receptor mechanisms, laboratory values, or diagnoses.

Hormonal influence alone does not determine scope.

## Cycle Regulation versus Active Phase

Choose one primary responsibility:

```text
Cycle Regulation
= timing, recurrence, phase progression, suppression, delay, or transition across a cycle

Active Phase
= the bounded physiological process occurring within one phase
```

A cycle-regulation profile should not absorb all phase-specific anatomy, fluid, motor, or sensory processes.

An active-phase profile should not claim ownership of the entire cycle.

Describe regulatory-to-phase dependency in prose until a repeated graph pattern justifies a dedicated relationship verb.

## YAML Pattern

```yaml
---
title: Activation Profile Name
file_class: Ontology Node
node_type: Activation Profile
layer: Activation Layer
status: Draft
version: 0.1
activation_type: Composite Activation
activation_components:
  - Hormonal / Cyclical Activation
  - Tissue-State Activation
activation_scope: Regional
embodiment_scope: Anatomy-Dependent
primary_anatomical_anchor: Anatomical Node
validation_status: Candidate
---
```

## Required Sections

```text
Purpose
Activation Classification
Trigger or Condition
Participating Canonical Nodes
Referenced Mirror Routes
Referenced Fluid Entities, where applicable
Referenced Fluid Profiles, where applicable
Fluid Property Alterations, where applicable
Temporal or Phase Sequence, where cyclical
Activation Sequence
Modulators and Inhibitors
Candidate Downstream Links
Boundary Rules
Consent Boundary
Relationship Statements
Review Questions
Status
```

## Participation Governance

```text
ACTIVATES_ANATOMICAL_SITE
= primary site undergoing change

INVOLVES_ANATOMICAL_NODE
= another direct participant

REFERENCES_ADJACENT_ANATOMICAL_SITE
= nearby, boundary, or output context only

INVOLVES_FLUID_ENTITY
= fluid directly participating

REFERENCES_ADJACENT_FLUID_ENTITY
= nearby fluid used for distinction only
```

Use the adjacency relationship for output territory until a dedicated output relationship is proven reusable.

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

## Boundary Rules

Activation profiles define process only. They must not define anatomy, fluid identity, hormone entities, endocrine mechanisms, mirror correspondence, propagation mechanics, sensory perception, affective interpretation, consent, authorial language, corpus usage, or narrative effect.

## Consent Boundary

```text
Physiological activation is not consent.
Hormonal state is not consent.
Cyclical state is not consent.
Fluid release is not consent.
Pleasure is not consent.
Desire is not consent.
Symbolic meaning is not consent.
```

## Review Questions

1. Is classification normalized?
2. Does scope follow direct participation?
3. Is the profile regulatory or active-phase, rather than both without separation?
4. Are cyclical phases distinguished from endocrine mechanisms?
5. Are hormone nodes referenced only if they exist?
6. Are fluid entities involved without being redefined?
7. Is Propagation limited to handoff?
8. Are downstream systems candidate-only?
9. Does the profile avoid implying consent?

## Status

Validated v0.6.

This version separates cycle regulation from active-phase execution and clarifies output-context handling.
