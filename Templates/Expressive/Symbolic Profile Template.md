---
tags:
  - Template
  - Layer/Expressive
  - Layer/Symbolic
  - Status/Draft
title: Symbolic Profile Template
file_class: Template
template_type: Expressive Profile
layer: Expressive Layers
expressive_sub_layer: Symbolic
status: Draft
version: 0.1
last_updated: 2026-07-09
---

# Symbolic Profile Template

## Purpose

Use this template to define a Symbolic Profile.

A Symbolic Profile defines reusable interpretations or significance attached downstream from embodied, sensory, somatic, emotional, fluid, environmental, temporal, sonic, or liturgical material.

It does not define anatomy, activation mechanics, fluid identity, sensation, somatic body-state, valence, desire, authorial wording, corpus truth, or consent.

## YAML Pattern

```yaml
tags:
  - Ontology Node
  - Expressive Layer
  - Symbolic Profile
  - Status/Draft
title: <Profile Name>
file_class: Ontology Node
node_type: Symbolic Profile
layer: Expressive Layers
expressive_sub_layer: Symbolic
status: Draft
version: 0.1
symbolic_scope: Local / Regional / Relational / Situational / Cross-Layer
primary_symbolic_context: <Profile, Site, Event, or Pattern>
validation_status: Candidate
```

## Required Sections

```text
Purpose
Symbolic Classification
Source Context
Referenced Embodied and Expressive Records
Symbolic Interpretations
Interpretive Dimensions
Biological Boundary
Sensory / Somatic Boundary
Valence / Desire Boundary
Authorial Boundary
Corpus Boundary
Consent Boundary
Relationship Statements
Review Questions
Status
```

## Core Distinctions

```text
Biology
= what exists or occurs

Sensation
= what is perceived

Somatic state
= how experience is held or organized in the body

Valence
= how experience is appraised

Desire
= motivational or affective orientation

Symbolic meaning
= reusable interpretation or significance attached downstream

Authorial expression
= how symbolic meaning is communicated

Corpus annotation
= where a symbolic interpretation is used in a specific work
```

## Candidate Interpretation Pattern

| Symbolic Interpretation | Possible Use | Notes |
|---|---|---|
| Boundary | Separation, edge, protection, contact, or distinction | Does not redefine anatomy |
| Threshold | Transition, crossing, entry, exit, or change | Does not imply permission or consent |
| Exposure | Visibility, uncovering, or vulnerability | Not a biological state |
| Containment | Holding, enclosure, protection, or restraint | Not somatic state by itself |
| Vulnerability | Interpretive significance of openness or exposure | Not consent |
| Sovereignty | Self-possession, authority, or ownership | Must not infer control from anatomy |
| Release | Letting go, transition, or loosening | Not fluid release or consent by itself |
| Return | Repetition, restoration, recurrence, or re-entry | Not temporal mechanism by itself |

Symbolic terms are controlled candidate values unless governed nodes are created later. Do not wikilink them unless the target node exists.

## Relationship Pattern

```text
<Profile Name> IS_SYMBOLIC_PROFILE
<Profile Name> HAS_SYMBOLIC_SCOPE <Scope>
<Profile Name> HAS_PRIMARY_SYMBOLIC_CONTEXT <Context>
<Profile Name> MAY_INTERPRET_ANATOMICAL_SITE <Canonical Node>
<Profile Name> MAY_INTERPRET_ACTIVATION_PROFILE <Activation Profile>
<Profile Name> MAY_INTERPRET_FLUID_ENTITY <Fluid Entity>
<Profile Name> MAY_INTERPRET_SENSORY_PROFILE <Sensory Profile>
<Profile Name> MAY_INTERPRET_SOMATIC_PROFILE <Somatic Profile>
<Profile Name> MAY_INTERPRET_EMOTIONAL_PROFILE <Emotional / Motivational Profile>
<Profile Name> MAY_DEFINE_SYMBOLIC_INTERPRETATION <Interpretation>
<Profile Name> MAY_REFERENCE_SYMBOLIC_REGISTER Symbolic Meaning Register
<Profile Name> MAY_BE_USED_BY Authorial Term Register
<Profile Name> MAY_BE_ANNOTATED_IN Corpus Annotation
```

Include only relationships actually used.

## Consent Boundary

```text
Symbolic openness is not consent.
A threshold does not imply permission.
Exposure does not imply invitation.
Vulnerability does not imply consent.
Wetness does not imply consent.
Pleasure does not imply consent.
Desire does not imply consent.
Sovereignty must not be overwritten by symbolic readings of anatomy or physiology.
```

## Review Questions

1. Are all entries interpretations rather than biology, sensation, body-state, valence, or desire?
2. Does the profile avoid turning authorial motifs into canonical symbolic truth?
3. Are interpretations reusable without being mandatory for every instance?
4. Does the profile preserve consent and sovereignty boundaries?
5. Are candidate values left as plain text unless governed nodes exist?

## Status

Draft v0.1.

Initial reusable template for Symbolic Profiles.