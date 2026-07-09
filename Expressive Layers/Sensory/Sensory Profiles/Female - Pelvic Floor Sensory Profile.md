---
tags:
  - Ontology Node
  - Expressive Layer
  - Sensory Profile
  - Female Embodiment
  - Status/Draft
title: Female - Pelvic Floor Sensory Profile
file_class: Ontology Node
node_type: Sensory Profile
layer: Expressive Layers
expressive_sub_layer: Sensory
status: Draft
version: 0.2
sensory_scope: Local
primary_sensory_anchor: Female - Pelvic Floor
validation_status: Candidate
---

# Female - Pelvic Floor Sensory Profile

## Purpose

This node defines perceived sensory qualities associated with [[Female - Pelvic Floor]] in contexts where [[Female - Pelvic Floor Contraction Activation Profile]] may enable or contextualize local muscular contraction, shortening, tension, support, or release.

It defines sensory perception only. It does not define pelvic-floor anatomy, activation mechanics, reflex mechanics, mirror correspondence, sensory valence, pleasure, desire, symbolic meaning, authorial language, corpus usage, or consent.

## Sensory Classification

| Field | Value |
|---|---|
| Node Type | Sensory Profile |
| Layer | Expressive Layers |
| Expressive Sublayer | Sensory |
| Sensory Scope | Local |
| Primary Sensory Anchor | [[Female - Pelvic Floor]] |
| Validation Status | Candidate |

## Source Context

| Source | Role | Notes |
|---|---|---|
| [[Female - Pelvic Floor Contraction Activation Profile]] | May Enable / Contextualize | Supported upstream Motor / Kinetic Activation Profile; does not define sensation directly |
| [[Female - Pelvic Floor]] | Primary Sensory Anchor | Canonical anatomical context; not redefined here |
| [[Female - Perineum to Female - Pelvic Floor Mirror Profile]] | Optional Traversal Context | May become perceptually salient as boundary-to-support traversal; not sensory mechanism |
| [[Female - Perineum]] | Boundary Context | Nearby external boundary region; not the primary sensory anchor |
| [[Female - Vaginal Opening]] | Adjacent Context | Boundary-adjacent site; not required for core pelvic-floor sensation |
| [[Female - Anus]] | Adjacent Context | Boundary-adjacent site; not required for core pelvic-floor sensation |

## Referenced Canonical Nodes

| Canonical Node | Sensory Role | Notes |
|---|---|---|
| [[Female - Pelvic Floor]] | Primary Sensory Anchor | Local contractile support structure that may be perceived through tension, pressure, support, or release |
| [[Female - Perineum]] | Boundary Context | External boundary region may help localize or interpret pelvic-floor sensation without becoming the primary anchor |
| [[Female - Vaginal Opening]] | Adjacent Context | May be contextually felt as nearby boundary pressure or opening-level proximity; not required |
| [[Female - Anus]] | Adjacent Context | May be contextually felt as nearby boundary pressure or reflex-adjacent proximity; not required |

## Referenced Activation Profiles

| Activation Profile | Role | Notes |
|---|---|---|
| [[Female - Pelvic Floor Contraction Activation Profile]] | May Enable / Contextualize | Activation owns motor recruitment, contraction, tension, support, and release; this profile owns perception only |

## Referenced Fluid Entities / Profiles

No Fluid Entity or Fluid Profile is required for the core sensory definition.

Fluid presence, wetness, or surface moisture may co-occur in other contexts, but this profile does not depend on Fluid Layer content.

## Referenced Mirror Routes

| Mirror Profile | Sensory Role | Notes |
|---|---|---|
| [[Female - Perineum to Female - Pelvic Floor Mirror Profile]] | May Contextualize Boundary-to-Support Perception | Mirror remains traversal only; it does not define sensation or contraction mechanics |

## Sensory Qualities

| Sensory Quality | Possible Presentation | Notes |
|---|---|---|
| Pressure | Present / Absent / Variable | Perceived local pressure or support; not activation mechanics |
| Tension | Present / Absent / Variable | Perceived contraction or holding quality; not Tissue-State Activation |
| Tightness | Present / Absent / Variable | Perceived local constriction; not desire, refusal, or emotional meaning by itself |
| Release | Present / Absent / Variable | Perceived lessening or letting go of local tension; not consent |
| Pulsing | Present / Absent / Variable | Perceived rhythm or intermittent contraction; does not define activation sequence |
| Support | Present / Absent / Variable | Perceived structural holding or lift; not symbolic meaning by itself |
| Ache | Present / Absent / Variable | Sensory quality only; does not define discomfort valence, pain diagnosis, or emotional meaning |
| Fullness | Present / Absent / Variable | Perceived local fullness or pressure only; not fluid identity |

Sensory-quality terms are controlled candidate values. They are not standalone ontology nodes unless promoted later.

## Intensity / Rhythm / Location

| Dimension | Possible Range | Notes |
|---|---|---|
| Intensity | Low / Moderate / High / Variable | Does not imply pleasure, discomfort, desire, or consent |
| Rhythm | Steady / Pulsed / Intermittent / Absent / Variable | Does not define motor sequence |
| Location | Localized / Diffuse / Boundary-Aware / Unclear | Does not redefine anatomy |
| Duration | Brief / Sustained / Recurrent / Variable | Does not define temporal structure unless linked to a Temporal profile |
| Directionality | Inward / Upward / Downward / Releasing / Unclear / Variable | Perceived orientation only; not propagation mechanics |

## Valence Boundary

```text
Pelvic-floor sensation is not valence.
Pelvic-floor sensation is not pleasure.
Pelvic-floor sensation is not discomfort.
Pelvic-floor sensation is not desire.
Pelvic-floor sensation is not consent.
```

This profile may later reference [[Sensory Valence Register]], [[Pleasure Register]], or a future more specific discomfort/neutral-valence record, but it does not define valence itself.

## Somatic Boundary

```text
Female - Pelvic Floor Sensory Profile
= perceived local qualities such as pressure, tension, pulsing, support, and release

Female - Pelvic Floor Somatic Profile
= whole-body or body-state experience such as bracing, holding, steadiness, collapse, grounding, guarding, or letting go
```

Do not duplicate Somatic Profile content here.

## Desire Boundary

```text
Pelvic-floor sensation may be desired, undesired, ignored, resisted, ambiguous, or unnoticed.
Pelvic-floor sensation does not define desire by itself.
```

## Symbolic Boundary

```text
Pelvic-floor sensation may later be interpreted symbolically.
Pelvic-floor sensation does not define symbolic meaning by itself.
```

## Consent Boundary

```text
Pelvic-floor sensation is not consent.
Pelvic-floor contraction is not consent.
Pelvic-floor release is not consent.
Reflexive contraction is not consent.
Voluntary muscular recruitment is not consent by itself.
Valence is not consent.
Pleasure is not consent.
Discomfort is not refusal by itself.
Desire is not consent.
Symbolic meaning is not consent.
```

## Relationship Statements

```text
Female - Pelvic Floor Sensory Profile IS_SENSORY_PROFILE
Female - Pelvic Floor Sensory Profile HAS_SENSORY_SCOPE Local
Female - Pelvic Floor Sensory Profile HAS_PRIMARY_SENSORY_ANCHOR Female - Pelvic Floor
Female - Pelvic Floor Sensory Profile MAY_BE_ENABLED_BY Female - Pelvic Floor Contraction Activation Profile
Female - Pelvic Floor Sensory Profile MAY_REFERENCE_ANATOMICAL_SITE Female - Pelvic Floor
Female - Pelvic Floor Sensory Profile MAY_REFERENCE_ANATOMICAL_SITE Female - Perineum
Female - Pelvic Floor Sensory Profile MAY_REFERENCE_ANATOMICAL_SITE Female - Vaginal Opening
Female - Pelvic Floor Sensory Profile MAY_REFERENCE_ANATOMICAL_SITE Female - Anus
Female - Pelvic Floor Sensory Profile MAY_REFERENCE_MIRROR_ROUTE Female - Perineum to Female - Pelvic Floor Mirror Profile
Female - Pelvic Floor Sensory Profile MAY_DEFINE_SENSORY_QUALITY Pressure
Female - Pelvic Floor Sensory Profile MAY_DEFINE_SENSORY_QUALITY Tension
Female - Pelvic Floor Sensory Profile MAY_DEFINE_SENSORY_QUALITY Tightness
Female - Pelvic Floor Sensory Profile MAY_DEFINE_SENSORY_QUALITY Release
Female - Pelvic Floor Sensory Profile MAY_DEFINE_SENSORY_QUALITY Pulsing
Female - Pelvic Floor Sensory Profile MAY_DEFINE_SENSORY_QUALITY Support
Female - Pelvic Floor Sensory Profile MAY_DEFINE_SENSORY_QUALITY Ache
Female - Pelvic Floor Sensory Profile MAY_DEFINE_SENSORY_QUALITY Fullness
Female - Pelvic Floor Sensory Profile MAY_HAVE_VALENCE Sensory Valence Register
Female - Pelvic Floor Sensory Profile MAY_HAVE_VALENCE Pleasure Register
Female - Pelvic Floor Sensory Profile MAY_CONTEXTUALIZE Desire Register
Female - Pelvic Floor Sensory Profile MAY_BE_INTERPRETED_BY Symbolic Meaning Register
Female - Pelvic Floor Sensory Profile MAY_BE_USED_BY Authorial Term Register
Female - Pelvic Floor Sensory Profile MAY_BE_ANNOTATED_IN Corpus Annotation
```

## Review Questions

1. Are Pressure, Tension, Tightness, Release, Pulsing, Support, Ache, and Fullness acceptable first-generation Sensory Quality terms, or should they become governed nodes later?
2. Should Directionality remain a sensory dimension, or should directional spread belong to Propagation or Somatic profiles?
3. Should Ache reference a future Discomfort Register rather than remain neutral here?
4. Does Boundary-Aware location adequately handle perineal mirror context without making the mirror sensory mechanism?
5. Is [[Sensory Valence Register]] sufficient for first-pass non-pleasure valence routing, or is a separate Discomfort Register needed?

## Status

Draft v0.2.

First Sensory Profile pilot. Updated to route valence through [[Sensory Valence Register]] while preserving the distinction between sensory perception, valence, pleasure, desire, symbolic meaning, and consent.