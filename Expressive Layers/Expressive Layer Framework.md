---
tags:
  - Document/Framework
  - Layer/Expressive
  - Governance/Layer
  - Status/Draft
title: Expressive Layer Framework
file_class: Document
document_type: Framework
layer: Expressive Layers
status: Draft
version: 0.1
last_updated: 2026-07-03
---

# Expressive Layer Framework

## Purpose

This framework governs the Expressive Layers of the Somatic Meaning Engine.

Expressive Layers define how embodied processes, sensory states, affective orientations, symbolic interpretations, environmental conditions, sonic textures, liturgical structures, and temporal patterns may be perceived or interpreted.

Expressive Layers do not define canonical anatomy, biological mechanism, fluid identity, activation mechanics, mirror correspondence, authorial style, or corpus truth.

## Architectural Position

```text
Canonical Embodiment Layer
= what exists

Fluid Layer
= what fluids are and how they are locally related to anatomy

Mirror Layer
= governed correspondence and traversal routes

Activation Layer
= physiological process, movement, release, contraction, alteration, or state change

Expressive Layers
= perceived, felt, interpreted, environmental, sonic, symbolic, temporal, or ritual experience

Authorial Layers
= language, voice, cadence, register, and compositional style

Corpus
= situated usage in specific works
```

## Expressive Sublayers

| Sublayer | Defines | Does Not Define |
|---|---|---|
| Sensory | Perceived qualities of experience such as pressure, wetness, warmth, ache, texture, intensity, location, rhythm, taste, odour, sound, or contact | Activation mechanics, pleasure, desire, symbolic meaning, consent |
| Somatic | Whole-body or body-state experience such as bracing, heaviness, opening, tightening, release, steadiness, collapse, fatigue, grounding, or dissociation | Local sensory quality, biological mechanism, diagnosis, authorial metaphor |
| Emotional / Motivational | Affective or motivational orientation such as desire, refusal, ambivalence, longing, appetite, aversion, fear, relief, or attachment | Sensory perception, pleasure as valence, consent, symbolic meaning |
| Symbolic | Interpretation, significance, archetype, motif, or meaning assigned downstream from embodied or expressive material | Objective biology, activation, sensation itself, authorial wording |
| Sonic | Heard, rhythmic, resonant, tonal, musical, or acoustic expression | Biological hearing anatomy, authorial lineation, symbolic interpretation by default |
| Environmental | Place-based, atmospheric, weather, pressure, spatial, seasonal, or material experience | Objective setting inventory unless modelled elsewhere, biological mechanism |
| Liturgical | Ritual structure, repetition, offering, invocation, sacrament, vow, or ceremonial sequencing | Theology as truth, biological process, authorial style by default |
| Temporal | Felt duration, anticipation, delay, recurrence, simultaneity, interruption, time loss, or cyclic experience | Objective chronology unless recorded in corpus or structural systems |

## Core Separation Rules

```text
Activation enables or contextualizes possible experience.
Sensory defines what is perceived.
Somatic defines body-state or embodied orientation.
Pleasure defines valence applied to perceived sensation.
Desire defines motivational or affective orientation.
Symbolic Meaning defines interpretation or significance.
Authorial systems define wording and style.
Corpus records situated use.
```

A physiological response may occur without sensory awareness.

A sensation may occur without pleasure.

Pleasure may occur without desire.

Desire may occur without consent.

Symbolic meaning may be assigned without changing the underlying biology.

## Profile Types

| Profile Type | Purpose |
|---|---|
| Sensory Profile | Defines perceived qualities associated with an anatomical site, fluid, activation, mirror route, or contextual condition |
| Somatic Profile | Defines whole-body or body-state experience associated with activation, posture, emotional state, environment, rhythm, or narrative condition |
| Emotional Profile | Defines affective states distinct from desire and symbolic interpretation |
| Motivational Register | Defines orientation such as desire, refusal, ambivalence, approach, avoidance, or redirection |
| Symbolic Meaning Register | Defines interpretive meaning without redefining biology or sensation |
| Sonic Profile | Defines sound, rhythm, resonance, or acoustic experience |
| Environmental Profile | Defines atmospheric, spatial, material, or weather-related experiential context |
| Liturgical Profile | Defines ritual or ceremonial structure |
| Temporal Profile | Defines felt temporal experience |

## Sensory and Somatic Distinction

```text
Sensory Profile
= localized or modality-specific perceived qualities

Somatic Profile
= whole-body, posture-level, body-state, or embodied orientation
```

Example:

```text
Female - Pelvic Floor Sensory Profile
= pressure, tension, pulsing, contraction, release, location, intensity

Female - Pelvic Floor Somatic Profile
= bracing, holding, support, steadiness, collapse, letting go, grounding
```

These may reference the same Activation Profile but must not duplicate each other.

## Pleasure, Desire, and Consent Boundary

Pleasure belongs downstream from sensation as valence.

Desire belongs downstream as motivational or affective orientation.

Consent must remain separately governable and must never be inferred from activation, sensation, pleasure, desire, fluid presence, contraction, release, symbolic meaning, or authorial framing.

```text
Activation is not consent.
Sensation is not consent.
Pleasure is not consent.
Desire is not consent.
Somatic readiness is not consent.
Symbolic meaning is not consent.
Authorial emphasis is not consent.
```

## Relationship Governance

Candidate Expressive relationships may include:

```text
MAY_BE_ENABLED_BY Activation Profile
MAY_REFERENCE_ANATOMICAL_SITE Canonical Anatomical Node
MAY_REFERENCE_FLUID_ENTITY Fluid Entity
MAY_REFERENCE_FLUID_PROFILE Fluid Profile
MAY_REFERENCE_MIRROR_ROUTE Mirror Profile
MAY_DEFINE_SENSORY_QUALITY Sensory Quality
MAY_DEFINE_SOMATIC_STATE Somatic State
MAY_HAVE_VALENCE Pleasure Register / Discomfort Register / Neutral Valence
MAY_CONTEXTUALIZE Desire Register
MAY_BE_INTERPRETED_BY Symbolic Meaning Register
MAY_BE_USED_BY Authorial Term Register
MAY_BE_ANNOTATED_IN Corpus Annotation
```

These relationships remain draft until repeated profile use validates them.

## Boundary Rules

Expressive Layer nodes must not define:

```text
canonical anatomy
biological mechanism
fluid identity
fluid production
activation sequence
mirror correspondence
propagation mechanics
consent state
authorial voice or prose style
corpus truth
```

Expressive nodes may reference upstream layers, but they must not overwrite them.

## First Validation Path

The first recommended validation path is:

```text
Supported Activation Profile
→ Sensory Profile
→ Pleasure / Discomfort / Neutral Valence Register
→ Somatic Profile if whole-body state is required
→ Desire Register if motivational orientation is present
→ Symbolic Meaning Register if interpretation is present
→ Authorial Register
→ Corpus Annotation
```

Preferred first pilot:

```text
Female - Pelvic Floor Contraction Activation Profile
→ Female - Pelvic Floor Sensory Profile
```

This provides a clean test because the source Activation Profile is fluid-independent, Local in scope, and already Supported.

## Review Questions

1. Should Pleasure remain inside Sensory, or should Valence become a separate expressive sublayer?
2. Should Desire remain inside Emotional, or should Motivational become a separate expressive sublayer?
3. Which sensory qualities require governed controlled vocabularies before baseline?
4. Which somatic states require controlled vocabularies before baseline?
5. Should Environmental, Sonic, Liturgical, and Temporal profiles share the same profile template shape or require separate templates?

## Status

Draft v0.1.

Initial framework for governing the Expressive Layers before creating Sensory and Somatic pilot profiles.