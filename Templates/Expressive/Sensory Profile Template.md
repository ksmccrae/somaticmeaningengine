---
tags:
  - Template
  - Layer/Expressive
  - Layer/Sensory
  - Status/Draft
title: Sensory Profile Template
file_class: Template
template_type: Expressive Profile
layer: Expressive Layers
expressive_sub_layer: Sensory
status: Draft
version: 0.1
last_updated: 2026-07-03
---

# Sensory Profile Template

## Purpose

Use this template to define a Sensory Profile.

A Sensory Profile defines perceived qualities associated with an anatomical site, fluid, activation, mirror route, environmental condition, sonic condition, temporal condition, or other upstream context.

It defines what may be perceived. It does not define biological mechanism, pleasure, desire, symbolic meaning, authorial language, corpus truth, or consent.

## YAML Pattern

```yaml
tags:
  - Ontology Node
  - Expressive Layer
  - Sensory Profile
  - Status/Draft
title: <Profile Name>
file_class: Ontology Node
node_type: Sensory Profile
layer: Expressive Layers
expressive_sub_layer: Sensory
status: Draft
version: 0.1
sensory_scope: Local / Regional / Systemic / Environmental / Sonic / Temporal
primary_sensory_anchor: <Canonical Node or Context>
validation_status: Candidate
```

## Required Sections

```text
Purpose
Sensory Classification
Source Context
Referenced Canonical Nodes
Referenced Activation Profiles
Referenced Fluid Entities / Profiles, if any
Referenced Mirror Routes, if any
Sensory Qualities
Intensity / Rhythm / Location
Valence Boundary
Somatic Boundary
Desire Boundary
Symbolic Boundary
Consent Boundary
Relationship Statements
Review Questions
Status
```

## Section Pattern

## Purpose

This node defines perceived sensory qualities associated with `<source context>`.

It may be enabled or contextualized by `<upstream profile>`, but it does not define that upstream process.

It defines sensory perception only. It does not define activation mechanics, anatomy, fluid identity, pleasure, desire, symbolic meaning, authorial language, corpus usage, or consent.

## Sensory Classification

| Field | Value |
|---|---|
| Node Type | Sensory Profile |
| Layer | Expressive Layers |
| Expressive Sublayer | Sensory |
| Sensory Scope | Local / Regional / Systemic / Environmental / Sonic / Temporal |
| Primary Sensory Anchor | `<anchor>` |
| Validation Status | Candidate |

## Source Context

| Source | Role | Notes |
|---|---|---|
| `<Activation Profile>` | May Enable / Contextualize | Does not define sensation directly |
| `<Canonical Node>` | Anatomical Context | Does not define perception by itself |
| `<Fluid Entity / Fluid Profile>` | Optional Perceptual Input | Used only if fluid qualities are perceptually relevant |
| `<Mirror Profile>` | Optional Traversal Context | Does not define sensation mechanically |

## Referenced Canonical Nodes

| Canonical Node | Sensory Role | Notes |
|---|---|---|
| `<Node>` | Primary Sensory Anchor / Context / Adjacent Context | Do not redefine anatomy |

## Referenced Activation Profiles

| Activation Profile | Role | Notes |
|---|---|---|
| `<Activation Profile>` | May Enable / Contextualize | Activation remains upstream |

## Referenced Fluid Entities / Profiles

Use only when fluid perception is relevant.

| Fluid Entity / Profile | Sensory Role | Notes |
|---|---|---|
| `<Fluid Entity or Profile>` | Optional Perceptual Input | Do not redefine fluid identity |

## Referenced Mirror Routes

Use only when mirror traversal may become perceptually salient.

| Mirror Profile | Sensory Role | Notes |
|---|---|---|
| `<Mirror Profile>` | May Contextualize | Mirror remains traversal only |

## Sensory Qualities

| Sensory Quality | Possible Presentation | Notes |
|---|---|---|
| Pressure | Present / Absent / Variable | Perceived quality only |
| Tension | Present / Absent / Variable | Perceived quality only |
| Warmth | Present / Absent / Variable | Perceived quality only |
| Wetness | Present / Absent / Variable | Use only if fluid context exists |
| Movement | Present / Absent / Variable | Perceived movement, not activation mechanics |
| Ache | Present / Absent / Variable | Sensory quality, not emotional meaning |

Add or remove qualities as appropriate.

## Intensity / Rhythm / Location

| Dimension | Possible Range | Notes |
|---|---|---|
| Intensity | Low / Moderate / High / Variable | Does not imply pleasure or distress |
| Rhythm | Steady / Pulsed / Intermittent / Absent / Variable | Does not define activation sequence |
| Location | Localized / Diffuse / Boundary-Aware / Unclear | Does not redefine anatomy |
| Duration | Brief / Sustained / Recurrent / Variable | Does not define temporal structure unless linked to Temporal profile |

## Valence Boundary

```text
Sensation is not pleasure.
Sensation is not discomfort.
Sensation is not desire.
Sensation is not consent.
```

Pleasure, discomfort, neutrality, ambiguity, aversion, or relief may be referenced downstream only if a valence register or profile governs them.

## Somatic Boundary

```text
Sensory Profile
= perceived qualities

Somatic Profile
= whole-body or body-state experience
```

Do not duplicate Somatic Profile content here.

## Desire Boundary

```text
Sensation may be desired, undesired, ignored, resisted, or ambiguous.
Sensation does not define desire by itself.
```

## Symbolic Boundary

```text
Sensation may later be interpreted symbolically.
Sensation does not define symbolic meaning by itself.
```

## Consent Boundary

```text
Sensation is not consent.
Pleasure is not consent.
Desire is not consent.
Arousal is not consent.
Fluid presence is not consent.
Contraction is not consent.
Symbolic meaning is not consent.
```

## Relationship Statements

```text
<Profile Name> IS_SENSORY_PROFILE
<Profile Name> HAS_SENSORY_SCOPE <Scope>
<Profile Name> HAS_PRIMARY_SENSORY_ANCHOR <Anchor>
<Profile Name> MAY_BE_ENABLED_BY <Activation Profile>
<Profile Name> MAY_REFERENCE_ANATOMICAL_SITE <Canonical Node>
<Profile Name> MAY_REFERENCE_FLUID_ENTITY <Fluid Entity>
<Profile Name> MAY_REFERENCE_FLUID_PROFILE <Fluid Profile>
<Profile Name> MAY_REFERENCE_MIRROR_ROUTE <Mirror Profile>
<Profile Name> MAY_DEFINE_SENSORY_QUALITY <Sensory Quality>
<Profile Name> MAY_HAVE_VALENCE Pleasure Register / Discomfort Register / Neutral Valence
<Profile Name> MAY_CONTEXTUALIZE Desire Register
<Profile Name> MAY_BE_INTERPRETED_BY Symbolic Meaning Register
<Profile Name> MAY_BE_USED_BY Authorial Term Register
<Profile Name> MAY_BE_ANNOTATED_IN Corpus Annotation
```

Include only relationships actually used by the profile.

## Review Questions

1. Are all sensory qualities perceptions rather than mechanisms?
2. Does the profile avoid defining pleasure, desire, symbolic meaning, and consent?
3. Are upstream Activation, Fluid, and Mirror records referenced without being redefined?
4. Is the sensory scope accurate?
5. Are candidate-only nodes left as plain text unless they already exist?

## Status

Draft v0.1.

Template for first-generation Sensory Profiles.