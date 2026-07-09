---
tags:
  - Document/README
  - Folder/Expressive Layers
  - Layer/Sensory
  - Status/Draft
file_class: Document
document_type: README
title: Sensory
layer: Expressive Layers
expressive_sub_layer: Sensory
status: Draft
version: 0.3
last_updated: 2026-07-03
---

# Sensory

The Sensory sublayer defines perceived qualities of embodied experience.

Sensory records describe what is perceived, not what biologically causes it and not what it means.

## Governing Framework

- [[Expressive Layer Framework]] — Draft v0.1

## Scope

Sensory may define perceived qualities such as:

```text
pressure
tension
wetness
warmth
coolness
ache
sharpness
softness
texture
contact
movement
pulsing
rhythm
intensity
location
spread
flow
heaviness
lightness
taste
odour
sound
```

Sensory does not define:

```text
canonical anatomy
activation mechanics
fluid identity
fluid production
mirror correspondence
somatic body-state
pleasure or discomfort as valence
desire or motivational orientation
symbolic meaning
consent state
authorial language
corpus truth
```

## Sensation, Valence, Pleasure, and Desire

```text
Sensation
= what is perceived

Sensory Valence
= how perception is appraised, received, tolerated, resisted, wanted, unwanted, relieving, distressing, neutral, mixed, or ambiguous

Pleasure
= positive, wanted, relieving, satisfying, or intensifying valence applied to perception

Desire
= motivational or affective orientation toward contact, continuation, intimacy, object, person, idea, or experience
```

A Sensory Profile may provide input to [[Sensory Valence Register]], [[Pleasure Register]], or [[Desire Register]], but it must not define any of them.

## Current Registers

- [[Sensory Valence Register]] — Draft v0.1
- [[Pleasure Register]] — Draft v0.1

## Current Profile Indexes

- [[Sensory Profiles Index]] — Draft v0.1

## Planned Profiles

| Planned Profile | Source | Purpose |
|---|---|---|
| [[Female - Pelvic Floor Sensory Profile]] | [[Female - Pelvic Floor Contraction Activation Profile]] | First fluid-independent Local sensory pilot |
| Female - Vulva Sensory Profile | [[Female - Vulvar Lubrication Activation Profile]] | Future tissue/fluid sensory pilot |
| Paraurethral Glandular Fluid Sensory Profile | [[Female - Paraurethral Glandular Release Activation Profile]] | Future fluid-boundary sensory pilot |
| Menstrual Fluid Sensory Profile | [[Female - Menstruation Activation Profile]] | Future cyclical/fluid sensory pilot |

## Relationship Pattern

```text
Sensory Profile MAY_BE_ENABLED_BY Activation Profile
Sensory Profile MAY_REFERENCE_ANATOMICAL_SITE Canonical Anatomical Node
Sensory Profile MAY_REFERENCE_FLUID_ENTITY Fluid Entity
Sensory Profile MAY_REFERENCE_FLUID_PROFILE Fluid Profile
Sensory Profile MAY_REFERENCE_MIRROR_ROUTE Mirror Profile
Sensory Profile MAY_DEFINE_SENSORY_QUALITY Sensory Quality
Sensory Profile MAY_HAVE_VALENCE Sensory Valence Register / Pleasure Register / Discomfort / Neutral Valence
Sensory Profile MAY_CONTEXTUALIZE Desire Register
Sensory Profile MAY_BE_INTERPRETED_BY Symbolic Meaning Register
Sensory Profile MAY_BE_USED_BY Authorial Term Register
Sensory Profile MAY_BE_ANNOTATED_IN Corpus Annotation
```

Relationship names remain draft until repeated Sensory Profile use validates them.

## Status

Draft v0.3.

Expanded to include broad Sensory Valence governance alongside Pleasure Register.