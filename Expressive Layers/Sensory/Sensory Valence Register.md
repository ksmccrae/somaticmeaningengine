---
tags:
  - Document/Register
  - Layer/Expressive
  - Layer/Sensory
  - Register/Valence
  - Status/Draft
title: Sensory Valence Register
file_class: Document
document_type: Register
layer: Expressive Layers
expressive_sub_layer: Sensory
status: Draft
version: 0.1
last_updated: 2026-07-03
---

# Sensory Valence Register

## Purpose

This register governs sensory valence within the Somatic Meaning Engine.

Sensory valence describes how a perceived sensation may be appraised, received, tolerated, resisted, wanted, unwanted, relieving, distressing, neutral, mixed, or ambiguous.

Valence is downstream from sensation. It is not sensation itself, not activation, not fluid identity, not mirror traversal, not desire, not symbolic meaning, not authorial language, not corpus truth, and not consent.

## Architectural Placement

```text
Activation Layer
→ defines physiological process or state change

Sensory Profile
→ defines perceived sensation

Sensory Valence Register
→ defines appraisal or received quality of perceived sensation

Pleasure Register
→ defines positive, wanted, relieving, satisfying, or intensifying valence

Desire Register
→ defines motivational or affective orientation

Symbolic Meaning Register
→ defines interpretation or significance

Authorial Systems
→ define language and style

Corpus
→ records situated usage
```

## Core Distinction

```text
Sensation
= what is perceived

Valence
= how the perception is appraised, received, tolerated, resisted, or affectively coloured

Desire
= motivational or affective orientation toward contact, continuation, intimacy, object, person, idea, or experience

Symbolic Meaning
= interpretation or significance assigned downstream
```

A sensation may exist without valence.

A sensation may shift valence over time.

Pleasure, discomfort, neutrality, ambiguity, aversion, and relief may all attach to perception without defining the underlying sensation.

## Candidate Valence Categories

| Valence Category | Definition | Notes |
|---|---|---|
| Pleasure | Positive, wanted, relieving, satisfying, intensifying, or affirming appraisal of perceived sensation | Governed in [[Pleasure Register]] |
| Discomfort | Unpleasant, irritating, painful, strained, distressing, or aversive appraisal of perceived sensation | Candidate category; does not define diagnosis |
| Neutral Valence | Perception registered without positive or negative appraisal | Candidate category |
| Ambivalent Valence | Mixed, uncertain, conflicting, or unstable appraisal | Candidate category |
| Unwanted Sensation | Sensation received as unwelcome or resisted | Not consent or refusal by itself |
| Relief | Sensation appraised as lessening strain, tension, discomfort, or burden | May overlap with Pleasure but should remain distinguishable where needed |
| Intensity Without Valence | Strong or noticeable perception without positive or negative appraisal | Prevents intensity from being mistaken for pleasure or discomfort |

## Boundary Rules

Sensory Valence records must not define:

```text
canonical anatomy
activation mechanics
fluid production, release, or surface presence
mirror correspondence
localized sensory quality itself
desire or motivational orientation
consent state
symbolic meaning
authorial terminology
corpus truth
diagnosis
```

Valence is not consent.

Pleasure is not consent.

Discomfort is not refusal by itself.

Neutrality is not consent.

Ambivalence is not consent.

Relief is not consent.

## Relationship to Pleasure Register

[[Pleasure Register]] remains the governed register for positive, wanted, relieving, satisfying, intensifying, or affirming sensory valence.

This register provides the broader valence map so Pleasure does not become the only governed valence outcome.

## Candidate Inputs

Valence may be referenced downstream from:

| Source Layer | Candidate Source | Relationship |
|---|---|---|
| Sensory Layer | Sensory Profile | May provide perceived sensation for valence appraisal |
| Somatic Layer | Somatic Profile | May provide body-state experience that receives valence |
| Activation Layer | Activation Profile | May provide physiological context without defining valence |
| Fluid Layer | Fluid Entity / Fluid Profile | May provide perceivable qualities such as wetness, warmth, taste, odour, surface presence, or flow |
| Mirror Layer | Mirror Profile | May provide traversal context that becomes perceptually salient |

These are candidate relationships only. This register does not define those source layers.

## Candidate Outputs

Valence may later be referenced by:

| Downstream Record | Purpose |
|---|---|
| Desire Register | May interact with motivational orientation without becoming desire |
| Symbolic Meaning Register | May interpret valence symbolically without defining valence here |
| Authorial Term Register | May govern how valence is described, withheld, complicated, or reframed |
| Corpus Annotation | May record where valence is present, absent, ambiguous, resisted, or changing in a work |

## Relationship Statements

```text
Sensory Valence Register DEFINES_SENSORY_VALENCE Sensory Valence
Sensory Valence Register DEFINES_VALENCE_CATEGORY Pleasure
Sensory Valence Register DEFINES_VALENCE_CATEGORY Discomfort
Sensory Valence Register DEFINES_VALENCE_CATEGORY Neutral Valence
Sensory Valence Register DEFINES_VALENCE_CATEGORY Ambivalent Valence
Sensory Valence Register DEFINES_VALENCE_CATEGORY Unwanted Sensation
Sensory Valence Register DEFINES_VALENCE_CATEGORY Relief
Sensory Valence Register DEFINES_VALENCE_CATEGORY Intensity Without Valence
Sensory Valence Register MAY_REFERENCE Sensory Profile
Sensory Valence Register MAY_REFERENCE Somatic Profile
Sensory Valence Register MAY_BE_CONTEXTUALIZED_BY Activation Profile
Sensory Valence Register MAY_BE_ASSOCIATED_WITH Fluid Profile
Sensory Valence Register MAY_BE_ROUTED_BY Mirror Profile
Sensory Valence Register MAY_INFORM Desire Register
Sensory Valence Register MAY_BE_INTERPRETED_BY Symbolic Meaning Register
Sensory Valence Register MAY_BE_USED_BY Authorial Term Register
Sensory Valence Register MAY_BE_ANNOTATED_IN Corpus Annotation
```

Relationship names remain draft until repeated valence use validates them.

Valence-category terms are controlled candidate values, not standalone ontology nodes unless promoted later.

## Activation Boundary Example

```text
Female - Pelvic Floor Contraction Activation Profile
→ may enable muscular contraction, support, tension, or release

Female - Pelvic Floor Sensory Profile
→ may define perceived pressure, tension, pulsing, support, or release

Sensory Valence Register
→ may define the perception as pleasurable, uncomfortable, neutral, ambiguous, relieving, unwanted, or intense-without-valence
```

The Activation Profile must not define valence directly.

## Consent Boundary

```text
Activation is not consent.
Sensation is not consent.
Valence is not consent.
Pleasure is not consent.
Discomfort is not refusal by itself.
Relief is not consent.
Neutrality is not consent.
Ambivalence is not consent.
Desire is not consent.
Symbolic meaning is not consent.
```

## Review Questions

1. Should Discomfort become its own register parallel to Pleasure Register?
2. Should Neutral Valence and Ambivalent Valence remain categories inside this register or become separate registers?
3. Should Relief be governed under Pleasure, Discomfort resolution, or its own category?
4. How should intensity be kept distinct from pleasure and discomfort?
5. Which Sensory Profiles should be used to validate the first valence categories?

## Status

Draft v0.1.

Initial broad valence register created to prevent Pleasure from becoming the only governed sensory-valence pathway.