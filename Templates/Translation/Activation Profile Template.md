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
version: 0.1
last_updated: 2026-07-01
---

# Activation Profile Template

## Purpose

This template defines the required structure for Activation Profile nodes in the Somatic Meaning Engine.

An Activation Profile defines a physiological or embodied process, state change, or response coordination event.

It may reference canonical anatomy, fluid entities, fluid profiles, mirror profiles, propagation candidates, sensory candidates, pleasure, desire, symbolic meaning, authorial systems, and corpus annotation, but it must not define those layers.

---

## Architectural Rule

```text
Activation Profile
= governed process node defining how a response or state change occurs
```

Activation profiles define process only.

---

## File Naming Rule

Activation profile nodes should use the pattern:

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

Use embodiment-specific names when the activation depends on embodiment-specific anatomy.

Use cross-embodiment names when the process is not embodiment-specific.

---

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
activation_type: Tissue-State Activation / Fluid Activation / Mirror-Route Activation / Motor / Kinetic Activation / Autonomic Activation / Hormonal / Cyclical Activation / Reflex Activation / Composite Activation
activation_scope: Local / Regional / Cross-System / Composite
embodiment_scope: Cross-Embodiment / Female / Male / Trans Feminine / Trans Masculine / Anatomy-Dependent
primary_anatomical_anchor: Anatomical Node
validation_status: Candidate
---
```

---

# Activation Profile Name

## Purpose

Define the activation process in neutral physiological or embodied-process language.

Do not define sensation, pleasure, desire, symbolic meaning, authorial language, or corpus usage.

---

## Activation Classification

| Field | Value |
|---|---|
| Node Type | Activation Profile |
| Layer | Activation Layer |
| Activation Type | Tissue-State Activation / Fluid Activation / Mirror-Route Activation / Motor / Kinetic Activation / Autonomic Activation / Hormonal / Cyclical Activation / Reflex Activation / Composite Activation |
| Activation Scope | Local / Regional / Cross-System / Composite |
| Embodiment Scope | Cross-Embodiment / Female / Male / Trans Feminine / Trans Masculine / Anatomy-Dependent |
| Primary Anatomical Anchor | [[Anatomical Node]] |
| Validation Status | Candidate / Supported / Blocked |

---

## Trigger or Condition

Describe the trigger, condition, or context in neutral process language.

| Trigger / Condition | Role | Notes |
|---|---|---|
| Condition | Initiates / Modulates / Inhibits / Contextualizes | Neutral process note only |

Do not describe desire, pleasure, consent, symbolic meaning, or narrative effect here.

---

## Participating Canonical Nodes

List anatomical participants without redefining them.

| Anatomical Node | Role In Activation | Notes |
|---|---|---|
| [[Anatomical Node]] | Primary Anchor / Participant / Conduit / Output Site / Adjacent Site / Modulator | Neutral process note only |

---

## Referenced Mirror Routes

List mirror routes that may become available, engaged, or weighted by this activation.

| Mirror Profile | Role | Notes |
|---|---|---|
| [[Mirror Profile]] | May Engage / May Weight / May Make Available | Do not redefine mirror correspondence |

---

## Referenced Fluid Entities

List fluid entities involved in the activation process.

| Fluid Entity | Activation Role | Notes |
|---|---|---|
| [[Fluid Entity]] | Produces / Releases / Moves / Exposes / Withholds / Alters | Do not redefine fluid entity |

---

## Referenced Fluid Profiles

List local fluid profiles involved in the activation process.

| Fluid Profile | Role | Notes |
|---|---|---|
| [[Fluid Profile]] | Local Context / Surface Presence / Conduit / Output / Adjacent | Do not redefine fluid profile |

---

## Fluid Property Alterations

List fluid properties that may change during activation.

| Fluid Property | Possible Change | Notes |
|---|---|---|
| [[Fluid Property]] | Increase / Decrease / Expose / Withhold / Alter / Contextual | Neutral process note only |

Do not define how the property is perceived. Perception belongs to the Sensory Layer.

---

## Activation Sequence

Define the process sequence neutrally.

```text
1. Trigger or condition becomes relevant.
2. Primary anatomical anchor enters activation context.
3. Participating anatomical nodes become involved.
4. Fluid entity or property involvement may change.
5. Mirror route may become available or weighted.
6. Downstream sensory, pleasure, desire, meaning, authorial, or corpus systems may later reference the activation.
```

Use the sequence only for process order, not narrative pacing or felt intensity.

---

## Modulators and Inhibitors

List factors that may modulate, inhibit, suppress, delay, or alter activation.

| Modulator / Inhibitor | Role | Notes |
|---|---|---|
| Candidate factor | Modulates / Inhibits / Suppresses / Delays / Alters | Neutral process note only |

Do not define emotional meaning or consent state here.

---

## Candidate Downstream Links

List downstream records that may later interpret, perceive, language, or annotate the activation.

| Downstream Record | Purpose |
|---|---|
| Sensory Profile | May define perception |
| Pleasure Register | May define sensory valence |
| Desire Register | May define motivational orientation |
| Symbolic Meaning Register | May define interpretation |
| Authorial Term Register | May define language |
| Corpus Annotation | May record usage |

These are candidate links only.

---

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

---

## Consent Boundary

Activation must never imply consent.

```text
Arousal is not consent.
Lubrication is not consent.
Pleasure is not consent.
Desire is not consent.
Symbolic meaning is not consent.
```

Consent requires separate governance if modelled later.

---

## Relationship Statements

Use controlled relationship language.

```text
Activation Profile IS_ACTIVATION_PROFILE
Activation Profile HAS_ACTIVATION_TYPE Activation Type
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

---

## Review Questions

1. Does this profile define process without redefining anatomy, fluids, mirrors, sensation, pleasure, desire, meaning, authorial language, or corpus usage?
2. Are fluid entities referenced rather than defined?
3. Are fluid properties altered rather than interpreted?
4. Are mirror routes engaged or made available rather than redefined?
5. Are downstream systems candidate links only?
6. Does the profile avoid implying consent?
7. Is the activation scope accurate?
8. Does the process need Propagation Layer handoff, or is it local/regional only?

---

## Status

Draft v0.1.

This template is not yet validated.
