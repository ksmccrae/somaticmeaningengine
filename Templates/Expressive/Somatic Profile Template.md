---
tags:
  - Template
  - Layer/Expressive
  - Layer/Somatic
  - Status/Draft
title: Somatic Profile Template
file_class: Template
template_type: Expressive Profile
layer: Expressive Layers
expressive_sub_layer: Somatic
status: Draft
version: 0.1
last_updated: 2026-07-03
---

# Somatic Profile Template

## Purpose

Use this template to define a Somatic Profile.

A Somatic Profile defines whole-body, posture-level, body-state, or embodied-orientation experience associated with activation, sensation, environment, rhythm, temporal condition, emotional context, or narrative condition.

It defines body-state experience only. It does not define biological mechanism, localized sensory quality by itself, pleasure, desire, symbolic meaning, authorial language, corpus truth, diagnosis, or consent.

## YAML Pattern

```yaml
tags:
  - Ontology Node
  - Expressive Layer
  - Somatic Profile
  - Status/Draft
title: <Profile Name>
file_class: Ontology Node
node_type: Somatic Profile
layer: Expressive Layers
expressive_sub_layer: Somatic
status: Draft
version: 0.1
somatic_scope: Local / Regional / Whole-Body / Relational / Environmental / Temporal
primary_somatic_anchor: <Anatomical Node, Activation Profile, or Body-State Context>
validation_status: Candidate
```

## Required Sections

```text
Purpose
Somatic Classification
Source Context
Referenced Canonical Nodes
Referenced Activation Profiles
Referenced Sensory Profiles
Somatic States
Body Orientation / Posture / Holding Pattern
Valence Boundary
Sensory Boundary
Desire Boundary
Symbolic Boundary
Consent Boundary
Relationship Statements
Review Questions
Status
```

## Section Pattern

## Purpose

This node defines body-state or embodied-orientation experience associated with `<source context>`.

It may be enabled or contextualized by `<upstream profile>`, but it does not define that upstream process.

It defines somatic experience only. It does not define activation mechanics, anatomy, fluid identity, localized sensory qualities by themselves, pleasure, desire, symbolic meaning, authorial language, corpus usage, diagnosis, or consent.

## Somatic Classification

| Field | Value |
|---|---|
| Node Type | Somatic Profile |
| Layer | Expressive Layers |
| Expressive Sublayer | Somatic |
| Somatic Scope | Local / Regional / Whole-Body / Relational / Environmental / Temporal |
| Primary Somatic Anchor | `<anchor>` |
| Validation Status | Candidate |

## Source Context

| Source | Role | Notes |
|---|---|---|
| `<Activation Profile>` | May Enable / Contextualize | Does not define somatic state directly |
| `<Sensory Profile>` | May Inform | Provides perceived qualities without becoming body-state |
| `<Canonical Node>` | Anatomical Context | Does not define experience by itself |
| `<Environmental / Temporal / Emotional Context>` | Optional Context | Use only if governed or clearly candidate |

## Referenced Canonical Nodes

| Canonical Node | Somatic Role | Notes |
|---|---|---|
| `<Node>` | Anchor / Context / Boundary | Do not redefine anatomy |

## Referenced Activation Profiles

| Activation Profile | Role | Notes |
|---|---|---|
| `<Activation Profile>` | May Enable / Contextualize | Activation remains upstream |

## Referenced Sensory Profiles

Use only when a sensory profile already exists or is clearly candidate.

| Sensory Profile | Role | Notes |
|---|---|---|
| `<Sensory Profile>` | May Inform | Sensory perception does not define whole-body state by itself |

## Somatic States

| Somatic State | Possible Presentation | Notes |
|---|---|---|
| Bracing | Present / Absent / Variable | Body-state only |
| Holding | Present / Absent / Variable | Body-state only |
| Opening | Present / Absent / Variable | Not consent |
| Tightening | Present / Absent / Variable | Not desire or refusal by itself |
| Release | Present / Absent / Variable | Not consent |
| Collapse | Present / Absent / Variable | Not diagnosis |
| Grounding | Present / Absent / Variable | Not symbolic meaning by itself |

Add or remove states as appropriate.

## Body Orientation / Posture / Holding Pattern

| Dimension | Possible Range | Notes |
|---|---|---|
| Orientation | Approach / Withdrawal / Neutral / Ambivalent / Variable | Does not define desire by itself |
| Posture | Braced / Open / Folded / Settled / Unsettled / Variable | Does not define emotion by itself |
| Holding Pattern | Guarded / Supported / Collapsed / Released / Variable | Does not define consent |
| Duration | Brief / Sustained / Recurrent / Variable | Does not define temporal structure unless linked to Temporal profile |

## Valence Boundary

```text
Somatic state is not pleasure.
Somatic state is not discomfort.
Somatic state is not desire.
Somatic state is not consent.
```

Pleasure, discomfort, neutrality, ambiguity, aversion, or relief may be referenced downstream only if a valence register or profile governs them.

## Sensory Boundary

```text
Sensory Profile
= localized or modality-specific perceived qualities

Somatic Profile
= whole-body, posture-level, body-state, or embodied orientation
```

Do not duplicate Sensory Profile content here.

## Desire Boundary

```text
A body-state may accompany desire, refusal, ambivalence, or withdrawal.
A body-state does not define desire by itself.
```

## Symbolic Boundary

```text
Somatic state may later be interpreted symbolically.
Somatic state does not define symbolic meaning by itself.
```

## Consent Boundary

```text
Somatic readiness is not consent.
Opening is not consent.
Relaxation is not consent.
Bracing is not refusal by itself.
Release is not consent.
Pleasure is not consent.
Desire is not consent.
Symbolic meaning is not consent.
```

## Relationship Statements

```text
<Profile Name> IS_SOMATIC_PROFILE
<Profile Name> HAS_SOMATIC_SCOPE <Scope>
<Profile Name> HAS_PRIMARY_SOMATIC_ANCHOR <Anchor>
<Profile Name> MAY_BE_ENABLED_BY <Activation Profile>
<Profile Name> MAY_REFERENCE_ANATOMICAL_SITE <Canonical Node>
<Profile Name> MAY_REFERENCE_SENSORY_PROFILE <Sensory Profile>
<Profile Name> MAY_DEFINE_SOMATIC_STATE <Somatic State>
<Profile Name> MAY_HAVE_VALENCE Pleasure Register / Discomfort Register / Neutral Valence
<Profile Name> MAY_CONTEXTUALIZE Desire Register
<Profile Name> MAY_BE_INTERPRETED_BY Symbolic Meaning Register
<Profile Name> MAY_BE_USED_BY Authorial Term Register
<Profile Name> MAY_BE_ANNOTATED_IN Corpus Annotation
```

Include only relationships actually used by the profile.

## Review Questions

1. Are all somatic states body-state or embodied-orientation experiences rather than localized sensory qualities?
2. Does the profile avoid defining pleasure, desire, symbolic meaning, diagnosis, and consent?
3. Are upstream Activation and Sensory records referenced without being redefined?
4. Is the somatic scope accurate?
5. Are candidate-only nodes left as plain text unless they already exist?

## Status

Draft v0.1.

Template for first-generation Somatic Profiles.