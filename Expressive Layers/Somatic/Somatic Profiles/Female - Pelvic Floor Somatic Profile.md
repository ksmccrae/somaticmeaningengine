---
tags:
  - Ontology Node
  - Expressive Layer
  - Somatic Profile
  - Female Embodiment
  - Status/Draft
title: Female - Pelvic Floor Somatic Profile
file_class: Ontology Node
node_type: Somatic Profile
layer: Expressive Layers
expressive_sub_layer: Somatic
status: Draft
version: 0.1
somatic_scope: Local / Whole-Body
primary_somatic_anchor: Female - Pelvic Floor
validation_status: Candidate
---

# Female - Pelvic Floor Somatic Profile

## Purpose

This node defines body-state or embodied-orientation experience associated with [[Female - Pelvic Floor]] in contexts where [[Female - Pelvic Floor Contraction Activation Profile]] may enable or contextualize local muscular contraction, support, tension, holding, or release.

It may be informed by Female - Pelvic Floor Sensory Profile, but it does not require that profile to be complete before existing as a Candidate somatic record.

It defines somatic experience only. It does not define pelvic-floor anatomy, activation mechanics, reflex mechanics, localized sensory qualities by themselves, pleasure, desire, symbolic meaning, authorial language, corpus usage, diagnosis, or consent.

## Somatic Classification

| Field | Value |
|---|---|
| Node Type | Somatic Profile |
| Layer | Expressive Layers |
| Expressive Sublayer | Somatic |
| Somatic Scope | Local / Whole-Body |
| Primary Somatic Anchor | [[Female - Pelvic Floor]] |
| Validation Status | Candidate |

## Source Context

| Source | Role | Notes |
|---|---|---|
| [[Female - Pelvic Floor Contraction Activation Profile]] | May Enable / Contextualize | Supported upstream Motor / Kinetic Activation Profile; does not define somatic experience directly |
| [[Female - Pelvic Floor]] | Primary Somatic Anchor | Canonical anatomical context; not redefined here |
| Female - Pelvic Floor Sensory Profile | May Inform | Candidate sensory companion; provides localized perception without defining whole-body state |
| [[Female - Perineum]] | Boundary Context | May contribute to body-state localization or guardedness without becoming the somatic anchor |
| [[Female - Pelvis]] | Structural Context | May contextualize support, grounding, or posture; not a somatic state by itself |

## Referenced Canonical Nodes

| Canonical Node | Somatic Role | Notes |
|---|---|---|
| [[Female - Pelvic Floor]] | Primary Somatic Anchor | Local support structure associated with holding, bracing, release, support, or grounding |
| [[Female - Pelvis]] | Structural Context | Parent structure that may contextualize posture and support without defining somatic state |
| [[Female - Perineum]] | Boundary Context | Boundary region may help orient embodied holding or release without becoming the primary anchor |

## Referenced Activation Profiles

| Activation Profile | Role | Notes |
|---|---|---|
| [[Female - Pelvic Floor Contraction Activation Profile]] | May Enable / Contextualize | Activation owns motor recruitment, contraction, tension, support, and release; this profile owns body-state experience only |

## Referenced Sensory Profiles

| Sensory Profile | Role | Notes |
|---|---|---|
| Female - Pelvic Floor Sensory Profile | May Inform | Candidate sensory pilot; localized qualities such as pressure or tension may inform body-state but do not define it |

## Somatic States

| Somatic State | Possible Presentation | Notes |
|---|---|---|
| Bracing | Present / Absent / Variable | Body-state of guarded support or preparation; not refusal by itself |
| Holding | Present / Absent / Variable | Body-state of maintained tension or containment; not consent or desire |
| Support | Present / Absent / Variable | Embodied sense of being held, lifted, or structurally steadied; not symbolic meaning by itself |
| Release | Present / Absent / Variable | Body-state of letting go or reduction in held tension; not consent |
| Letting Go | Present / Absent / Variable | Experiential orientation toward release; not desire or consent |
| Steadiness | Present / Absent / Variable | Body-state of stability or grounded support; not emotional meaning by itself |
| Collapse | Present / Absent / Variable | Body-state of loss of support or yielding; not diagnosis |
| Grounding | Present / Absent / Variable | Body-state of embodied anchoring; not symbolic meaning by itself |
| Guarding | Present / Absent / Variable | Protective or defensive holding pattern; not refusal or trauma diagnosis by itself |

## Body Orientation / Posture / Holding Pattern

| Dimension | Possible Range | Notes |
|---|---|---|
| Orientation | Approach / Withdrawal / Neutral / Ambiguous / Variable | Does not define desire by itself |
| Posture | Braced / Supported / Collapsed / Settled / Unsettled / Variable | Does not define emotion by itself |
| Holding Pattern | Guarded / Held / Released / Supported / Variable | Does not define consent |
| Duration | Brief / Sustained / Recurrent / Variable | Does not define temporal structure unless linked to a Temporal profile |
| Body Scale | Localized / Whole-Body Echo / Mixed / Variable | Records whether pelvic-floor state remains local or affects wider embodied orientation |

## Valence Boundary

```text
Pelvic-floor somatic state is not pleasure.
Pelvic-floor somatic state is not discomfort.
Pelvic-floor somatic state is not desire.
Pelvic-floor somatic state is not consent.
```

This profile may later reference [[Pleasure Register]] or a future discomfort/neutral-valence register, but it does not define valence itself.

## Sensory Boundary

```text
Female - Pelvic Floor Sensory Profile
= perceived local qualities such as pressure, tension, pulsing, support, and release

Female - Pelvic Floor Somatic Profile
= body-state or embodied orientation such as bracing, holding, steadiness, collapse, guarding, grounding, or letting go
```

Do not duplicate Sensory Profile content here.

## Desire Boundary

```text
Pelvic-floor somatic state may accompany desire, refusal, ambivalence, withdrawal, approach, or indifference.
Pelvic-floor somatic state does not define desire by itself.
```

## Symbolic Boundary

```text
Pelvic-floor somatic state may later be interpreted symbolically.
Pelvic-floor somatic state does not define symbolic meaning by itself.
```

## Consent Boundary

```text
Somatic readiness is not consent.
Opening is not consent.
Relaxation is not consent.
Bracing is not refusal by itself.
Guarding is not refusal by itself.
Release is not consent.
Letting go is not consent.
Pleasure is not consent.
Desire is not consent.
Symbolic meaning is not consent.
```

## Relationship Statements

```text
Female - Pelvic Floor Somatic Profile IS_SOMATIC_PROFILE
Female - Pelvic Floor Somatic Profile HAS_SOMATIC_SCOPE Local / Whole-Body
Female - Pelvic Floor Somatic Profile HAS_PRIMARY_SOMATIC_ANCHOR Female - Pelvic Floor
Female - Pelvic Floor Somatic Profile MAY_BE_ENABLED_BY Female - Pelvic Floor Contraction Activation Profile
Female - Pelvic Floor Somatic Profile MAY_REFERENCE_ANATOMICAL_SITE Female - Pelvic Floor
Female - Pelvic Floor Somatic Profile MAY_REFERENCE_ANATOMICAL_SITE Female - Pelvis
Female - Pelvic Floor Somatic Profile MAY_REFERENCE_ANATOMICAL_SITE Female - Perineum
Female - Pelvic Floor Somatic Profile MAY_REFERENCE_SENSORY_PROFILE Female - Pelvic Floor Sensory Profile
Female - Pelvic Floor Somatic Profile MAY_DEFINE_SOMATIC_STATE Bracing
Female - Pelvic Floor Somatic Profile MAY_DEFINE_SOMATIC_STATE Holding
Female - Pelvic Floor Somatic Profile MAY_DEFINE_SOMATIC_STATE Support
Female - Pelvic Floor Somatic Profile MAY_DEFINE_SOMATIC_STATE Release
Female - Pelvic Floor Somatic Profile MAY_DEFINE_SOMATIC_STATE Letting Go
Female - Pelvic Floor Somatic Profile MAY_DEFINE_SOMATIC_STATE Steadiness
Female - Pelvic Floor Somatic Profile MAY_DEFINE_SOMATIC_STATE Collapse
Female - Pelvic Floor Somatic Profile MAY_DEFINE_SOMATIC_STATE Grounding
Female - Pelvic Floor Somatic Profile MAY_DEFINE_SOMATIC_STATE Guarding
Female - Pelvic Floor Somatic Profile MAY_HAVE_VALENCE Pleasure Register
Female - Pelvic Floor Somatic Profile MAY_CONTEXTUALIZE Desire Register
Female - Pelvic Floor Somatic Profile MAY_BE_INTERPRETED_BY Symbolic Meaning Register
Female - Pelvic Floor Somatic Profile MAY_BE_USED_BY Authorial Term Register
Female - Pelvic Floor Somatic Profile MAY_BE_ANNOTATED_IN Corpus Annotation
```

## Review Questions

1. Are Bracing, Holding, Support, Release, Letting Go, Steadiness, Collapse, Grounding, and Guarding acceptable first-generation Somatic State terms, or should they become governed nodes later?
2. Does Local / Whole-Body scope adequately capture a local pelvic-floor source with possible whole-body echo?
3. Should Guarding remain a neutral somatic state rather than implying refusal, fear, trauma, or diagnosis?
4. Should Letting Go be retained as a somatic state, or treated as authorial phrasing until governed?
5. Should Female - Pelvic Floor Sensory Profile be created or promoted before this profile is advanced?

## Status

Draft v0.1.

First Somatic Profile pilot. Built as a companion to Female - Pelvic Floor Sensory Profile to test the distinction between localized sensory perception and whole-body or body-state experience.