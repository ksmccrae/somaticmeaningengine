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
version: 0.4
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

## Scope Decision Rule

```text
Local
= one primary anatomical anchor undergoes the defined state change

Regional
= two or more nearby anatomical nodes actively participate in the same process

Cross-System
= distinct anatomical systems, physiological systems, or separated regions are coordinated
```

Do not count the following as active participation by themselves:

```text
adjacency
boundary context
mirror engagement
downstream candidate reference
possible Propagation handoff
```

Decision sequence:

```text
1. List nodes undergoing or directly contributing to the state change.
2. Remove nodes used only for adjacency, boundary, mirror, or downstream context.
3. One active anchor = Local.
4. Two or more nearby active participants = Regional.
5. Distinct systems or separated regions = Cross-System.
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

## Anatomical Participation Governance

Use:

```text
ACTIVATES_ANATOMICAL_SITE
```

for the primary site undergoing the defined state change.

Use:

```text
INVOLVES_ANATOMICAL_NODE
```

only when another node directly participates in the same process.

Use:

```text
REFERENCES_ADJACENT_ANATOMICAL_SITE
```

when a nearby or boundary object is relevant but does not undergo or directly contribute to the state change.

## Fluid Adjacency Governance

Use:

```text
REFERENCES_ADJACENT_FLUID_ENTITY
```

when a nearby fluid is relevant to distinction or boundary governance but is not involved in the activation.

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

Activation profiles define process only. They must not define anatomy, fluid identity, mirror correspondence, propagation mechanics, sensory perception, affective valence, desire, consent, symbolic interpretation, authorial language, corpus usage, or narrative effect.

## Consent Boundary

```text
Physiological activation is not consent.
Autonomic response is not consent.
Fluid release is not consent.
Muscular contraction is not consent.
Pleasure is not consent.
Desire is not consent.
Symbolic meaning is not consent.
```

## Review Questions

1. Is `activation_type` a single controlled value?
2. Are all components controlled values?
3. Does scope follow direct participation rather than proximity?
4. Are adjacency relationships non-participatory?
5. Are mirror routes engaged rather than redefined?
6. Are downstream systems candidate links only?
7. Is a Propagation handoff required without defining propagation?
8. Does the profile avoid implying consent?

## Validation Basis

This template has been successfully instantiated by three Candidate profiles covering fluid-dependent, glandular, and fluid-independent motor / kinetic activation.

## Status

Validated v0.4.

This template is validated for Activation Profile construction. It is not Baseline.
