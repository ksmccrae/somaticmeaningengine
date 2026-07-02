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
version: 0.2
last_updated: 2026-07-01
---

# Activation Profile Template

## Purpose

This template defines the required structure for Activation Profile nodes in the Somatic Meaning Engine.

An Activation Profile defines a physiological or embodied process, state change, or response coordination event. It may reference canonical anatomy, fluid entities, fluid profiles, mirror profiles, propagation candidates, sensory candidates, pleasure, desire, symbolic meaning, authorial systems, and corpus annotation, but it must not define those layers.

## Architectural Rule

```text
Activation Profile
= governed process node defining how a response or state change occurs
```

Activation profiles define process only.

## Classification Rule

`activation_type` is a single controlled value.

Use `Composite Activation` when one profile coordinates more than one activation component.

`activation_components` is a YAML list of the controlled process families coordinated by the profile.

`activation_scope` describes anatomical or systemic reach only and must not include `Composite`.

```text
activation_type
= overall structural class

activation_components
= component process families

activation_scope
= Local / Regional / Cross-System
```

## File Naming Rule

```text
Embodiment - Activation Name Activation Profile.md
```

Examples:

```text
Female - Vulvar Lubrication Activation Profile.md
Female - Pelvic Floor Contraction Activation Profile.md
Female - Paraurethral Glandular Release Activation Profile.md
Crying Activation Profile.md
Sweating Activation Profile.md
```

## YAML Pattern

```yaml
---
tags:
  - Ontology Node
  - Activation Layer
  - Activation Profile
  - Status/Draft
title: Activation Profile Name
file_class: Ontology Node
node_type: Activation Profile
layer: Activation Layer
status: Draft
version: 0.1
activation_type: Composite Activation
activation_components:
  - Fluid Activation
  - Mirror-Route Activation
activation_scope: Local / Regional / Cross-System
embodiment_scope: Cross-Embodiment / Female / Male / Trans Feminine / Trans Masculine / Anatomy-Dependent
primary_anatomical_anchor: Anatomical Node
validation_status: Candidate
---
```

Controlled activation components:

```text
Tissue-State Activation
Fluid Activation
Mirror-Route Activation
Motor / Kinetic Activation
Autonomic Activation
Hormonal / Cyclical Activation
Reflex Activation
```

A non-composite profile may use one component as both `activation_type` and the sole `activation_components` value.

## Activation Classification

| Field | Value |
|---|---|
| Node Type | Activation Profile |
| Layer | Activation Layer |
| Activation Type | Controlled single value |
| Activation Components | One or more controlled component values |
| Activation Scope | Local / Regional / Cross-System |
| Embodiment Scope | Cross-Embodiment / Female / Male / Trans Feminine / Trans Masculine / Anatomy-Dependent |
| Primary Anatomical Anchor | [[Anatomical Node]] |
| Validation Status | Candidate / Supported / Blocked |

## Trigger or Condition

| Trigger / Condition | Role | Notes |
|---|---|---|
| Condition | Initiates / Modulates / Inhibits / Contextualizes | Neutral process note only |

Do not describe desire, pleasure, consent, symbolic meaning, or narrative effect here.

## Participating Canonical Nodes

| Anatomical Node | Role In Activation | Notes |
|---|---|---|
| [[Anatomical Node]] | Primary Anchor / Participant / Conduit / Output Site / Adjacent Site / Modulator | Neutral process note only |

## Referenced Mirror Routes

| Mirror Profile | Role | Notes |
|---|---|---|
| [[Mirror Profile]] | May Engage / May Weight / May Make Available | Do not redefine mirror correspondence |

## Referenced Fluid Entities

| Fluid Entity | Activation Role | Notes |
|---|---|---|
| [[Fluid Entity]] | Produces / Releases / Moves / Exposes / Withholds / Alters | Do not redefine fluid entity |

## Referenced Fluid Profiles

| Fluid Profile | Role | Notes |
|---|---|---|
| [[Fluid Profile]] | Local Context / Surface Presence / Conduit / Output / Adjacent | Do not redefine fluid profile |

## Fluid Property Alterations

| Fluid Property | Possible Change | Notes |
|---|---|---|
| [[Fluid Property]] | Increase / Decrease / Expose / Withhold / Alter / Contextual | Neutral process note only |

Do not define how the property is perceived.

## Activation Sequence

```text
1. Trigger or condition becomes relevant.
2. Primary anatomical anchor enters activation context.
3. Participating anatomical nodes become involved.
4. Fluid entity or property involvement may change.
5. Mirror route may become available or weighted.
6. Downstream systems may later reference the activation.
```

## Modulators and Inhibitors

| Modulator / Inhibitor | Role | Notes |
|---|---|---|
| Candidate factor | Modulates / Inhibits / Suppresses / Delays / Alters | Neutral process note only |

## Candidate Downstream Links

| Downstream Record | Purpose |
|---|---|
| Sensory Profile | May define perception |
| Pleasure Register | May define sensory valence |
| Desire Register | May define motivational orientation |
| Symbolic Meaning Register | May define interpretation |
| Authorial Term Register | May define language |
| Corpus Annotation | May record usage |

## Boundary Rules

Do not include:

```text
canonical anatomical definitions
fluid entity definitions
fluid property definitions
mirror correspondence definitions
propagation routes beyond local handoff
sensory perception
pleasure or discomfort as valence
desire or motivational orientation
consent state
symbolic meaning
emotional meaning
authorial terminology
corpus examples
narrative effect
```

## Consent Boundary

```text
Arousal is not consent.
Lubrication is not consent.
Pleasure is not consent.
Desire is not consent.
Symbolic meaning is not consent.
```

## Relationship Statements

```text
Activation Profile IS_ACTIVATION_PROFILE
Activation Profile HAS_ACTIVATION_TYPE Activation Type
Activation Profile HAS_ACTIVATION_COMPONENT Activation Component
Activation Profile HAS_ACTIVATION_SCOPE Activation Scope
Activation Profile ACTIVATES_ANATOMICAL_SITE Anatomical Node
Activation Profile INVOLVES_ANATOMICAL_NODE Anatomical Node
Activation Profile INVOLVES_FLUID_ENTITY Fluid Entity
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

## Review Questions

1. Does this profile define process without redefining other layers?
2. Is `activation_type` a single controlled value?
3. Are all `activation_components` controlled values?
4. Does `activation_scope` describe reach rather than composition?
5. Are fluid properties altered rather than interpreted?
6. Are mirror routes engaged rather than redefined?
7. Are downstream systems candidate links only?
8. Does the profile avoid implying consent?
9. Does the process need Propagation Layer handoff?

## Status

Draft v0.2.

This template now separates activation class, component processes, and anatomical/systemic scope. It is not yet validated.
