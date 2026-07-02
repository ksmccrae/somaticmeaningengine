---
tags:
  - Template/Translation
  - Template/Activation Profile
  - Status/Draft
aliases:
  - Activation Profile Template
title: Activation Profile Template
file_class: Template
template_type: Translation
node_type: Activation Profile
layer: Activation Layer
status: Draft
version: 0.3
last_updated: 2026-07-01
---

# Activation Profile Template

## Purpose

This template defines the required structure for Activation Profile nodes. An Activation Profile defines a physiological or embodied process, state change, or response coordination event while referencing, rather than redefining, other ontology layers.

## Classification Rule

```text
activation_type
= one controlled structural class

activation_components
= one or more controlled process families

activation_scope
= Local / Regional / Cross-System
```

Use `Composite Activation` when a profile coordinates multiple activation components.

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
  - Motor / Kinetic Activation
  - Tissue-State Activation
activation_scope: Local
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
Activation Sequence
Modulators and Inhibitors
Candidate Downstream Links
Boundary Rules
Consent Boundary
Relationship Statements
Review Questions
Status
```

## Adjacency Governance

Use adjacency relationships only when a nearby object is relevant to boundary or distinction but is not directly activated or involved.

```text
Activation Profile REFERENCES_ADJACENT_ANATOMICAL_SITE Anatomical Node
Activation Profile REFERENCES_ADJACENT_FLUID_ENTITY Fluid Entity
```

Adjacent anatomy must not be treated as source or participant anatomy by proximity alone.

Adjacent fluid must not be treated as the active fluid by location alone.

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

Activation profiles define process only. They must not define anatomy, fluid identity, mirror correspondence, sensory perception, affective valence, desire, consent, symbolic interpretation, authorial language, corpus usage, or narrative effect.

## Review Questions

1. Is classification normalized?
2. Are all component values controlled?
3. Does scope describe reach rather than composition?
4. Are adjacency relationships necessary and non-participatory?
5. Are downstream systems candidate links only?
6. Is a Propagation handoff required?

## Status

Draft v0.3.
