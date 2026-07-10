---
tags:
  - Template
  - Layer/Expressive
  - Layer/Emotional
  - Status/Draft
title: Emotional-Motivational Profile Template
file_class: Template
template_type: Expressive Profile
layer: Expressive Layers
expressive_sub_layer: Emotional / Motivational
status: Draft
version: 0.1
last_updated: 2026-07-09
---

# Emotional-Motivational Profile Template

## Purpose

Use this template to define an Emotional / Motivational Profile.

An Emotional / Motivational Profile defines affective or motivational orientation associated with an embodied route. It may describe wanting, non-wanting, ambivalence, aversion, curiosity, indifference, suppression, redirection, longing, or other governed orientations.

It does not define anatomy, activation mechanics, fluid identity, sensation, somatic body-state, sensory valence, symbolic meaning, authorial language, corpus truth, or consent.

## YAML Pattern

```yaml
tags:
  - Ontology Node
  - Expressive Layer
  - Emotional Profile
  - Status/Draft
title: <Profile Name>
file_class: Ontology Node
node_type: Emotional / Motivational Profile
layer: Expressive Layers
expressive_sub_layer: Emotional / Motivational
status: Draft
version: 0.1
motivational_scope: Local / Regional / Whole-Body / Relational / Situational
primary_motivational_context: <Profile, Site, or Situation>
validation_status: Candidate
```

## Required Sections

```text
Purpose
Emotional / Motivational Classification
Source Context
Referenced Sensory Profiles
Referenced Somatic Profiles
Referenced Valence Registers
Affective / Motivational Orientations
Orientation Dimensions
Activation Boundary
Sensory Boundary
Somatic Boundary
Valence Boundary
Symbolic Boundary
Consent Boundary
Relationship Statements
Review Questions
Status
```

## Core Distinctions

```text
Activation
= physiological process or state change

Sensation
= what is perceived

Somatic state
= how experience is held or organized in the body

Valence
= how perception or body-state is appraised

Emotional / Motivational orientation
= wanting, non-wanting, ambivalence, aversion, curiosity, indifference, suppression, redirection, longing, or related orientation

Symbolic meaning
= interpretation or significance

Consent
= separately governed decision and communication
```

## Candidate Orientation Pattern

| Orientation | Possible Presentation | Notes |
|---|---|---|
| Wanting | Present / Absent / Variable | Not consent |
| Non-Wanting | Present / Absent / Variable | Must not be treated as permission |
| Ambivalence | Present / Absent / Variable | Mixed or unresolved orientation; not consent |
| Aversion | Present / Absent / Variable | Motivational movement away; not diagnosis |
| Curiosity | Present / Absent / Variable | Interest without commitment or consent |
| Indifference | Present / Absent / Variable | Absence of motivational investment; not consent |
| Suppression | Present / Absent / Variable | Orientation withheld or inhibited; not authorial language |
| Redirection | Present / Absent / Variable | Orientation moved toward another object, action, or meaning |

Orientation terms are controlled candidate values unless governed nodes are created later. Do not wikilink them unless the target node exists.

## Relationship Pattern

```text
<Profile Name> IS_EMOTIONAL_MOTIVATIONAL_PROFILE
<Profile Name> HAS_MOTIVATIONAL_SCOPE <Scope>
<Profile Name> HAS_PRIMARY_MOTIVATIONAL_CONTEXT <Context>
<Profile Name> MAY_BE_CONTEXTUALIZED_BY <Activation Profile>
<Profile Name> MAY_REFERENCE_SENSORY_PROFILE <Sensory Profile>
<Profile Name> MAY_REFERENCE_SOMATIC_PROFILE <Somatic Profile>
<Profile Name> MAY_REFERENCE_VALENCE_REGISTER Sensory Valence Register
<Profile Name> MAY_REFERENCE_DESIRE_REGISTER Desire Register
<Profile Name> MAY_DEFINE_MOTIVATIONAL_ORIENTATION <Orientation>
<Profile Name> MAY_BE_INTERPRETED_BY Symbolic Meaning Register
<Profile Name> MAY_BE_USED_BY Authorial Term Register
<Profile Name> MAY_BE_ANNOTATED_IN Corpus Annotation
```

Include only relationships actually used.

## Consent Boundary

```text
Arousal is not consent.
Sensation is not consent.
Somatic state is not consent.
Pleasure is not consent.
Wanting is not consent.
Curiosity is not consent.
Ambivalence is not consent.
Indifference is not consent.
Non-wanting must not be treated as permission.
Aversion must not be ignored or overridden.
Desire is not consent.
Symbolic meaning is not consent.
```

## Review Questions

1. Are all orientations affective or motivational rather than sensory, somatic, symbolic, or authorial?
2. Does the profile distinguish bodily approach/withdrawal from motivational wanting/non-wanting?
3. Are valence and desire referenced without being collapsed together?
4. Does the profile avoid inferring consent from any orientation?
5. Are candidate values left as plain text unless governed nodes exist?

## Status

Draft v0.1.

Initial reusable template for Emotional / Motivational Profiles.