---
tags:
  - Document/Register
  - Layer/Expressive
  - Governance/Validation
  - Status/Draft
title: Expressive Profile Validation & Promotion Register
file_class: Document
document_type: Governance Register
layer: Expressive Layers
status: Draft
version: 0.4
last_updated: 2026-07-09
---

# Expressive Profile Validation & Promotion Register

## Purpose

This register defines evidence required to move an Expressive Profile from Candidate to Supported and records later cross-layer alignment revisions.

```text
Document status = Draft / Validated / Baseline
Profile validation status = Candidate / Supported / Blocked
```

This register covers first-generation Expressive Profile types, especially Sensory Profiles and Somatic Profiles.

## Required Criteria

| Criterion | Required Evidence |
|---|---|
| Mechanical completeness | Required sections present; YAML, body, Index, and relationships agree |
| Controlled classification | Sublayer, profile type, scope, anchor, and validation status use governed values |
| Source discipline | Upstream Activation, Fluid, Mirror, Canonical, Environmental, Sonic, Temporal, or Emotional sources are referenced without being redefined |
| Sensory / Somatic separation | Sensory Profiles define perceived qualities; Somatic Profiles define body-state or embodied orientation |
| Valence separation | Sensation and somatic state remain distinct from valence, pleasure, discomfort, relief, neutrality, and ambiguity |
| Desire separation | Desire and motivational orientation are referenced downstream rather than defined inside Sensory or Somatic profiles |
| Symbolic separation | Symbolic meaning remains downstream and does not overwrite sensation, somatic state, or valence |
| Authorial separation | Language, cadence, voice, register, and prose style remain Authorial concerns |
| Corpus separation | Profile does not treat situated work examples as ontology definitions |
| Consent boundary | Activation, sensation, somatic state, valence, pleasure, discomfort, desire, and symbolic meaning are not treated as consent |
| Candidate value discipline | Sensory-quality, somatic-state, and valence-category terms remain plain text unless governed nodes exist |
| Relationship discipline | Draft relationship statements are used consistently and not treated as validated verbs before repetition |
| Graph traversal | Incoming and outgoing references support traversal without circular layer collapse |
| Review questions | Open questions are identified as blocking or non-blocking |

## Blocking Conditions

```text
unresolved profile type
scope conflict
source-layer redefinition
sensory / somatic duplication
valence collapsed into sensation or somatic state
desire collapsed into sensation, somatic state, or pleasure
symbolic meaning collapsed into sensation, somatic state, or valence
consent boundary weakened
candidate values wikilinked as false nodes
unsupported relationship statements
incoherent upstream / downstream routing
```

Missing downstream Authorial, Corpus, Symbolic, Emotional, or additional profile coverage is non-blocking unless the Expressive Profile depends on it.

## Profile Type Validation Notes

### Sensory Profiles

Sensory Profiles must define perceived qualities.

They may reference upstream Activation, Fluid, Mirror, Canonical, Environmental, Sonic, or Temporal context, but they must not define those upstream layers.

```text
Sensory Profile
= pressure, tension, wetness, warmth, ache, texture, taste, odour, sound, contact, movement, rhythm, location, intensity, etc.
```

Sensory Profiles must not define sensory valence, pleasure, desire, symbolic meaning, authorial language, corpus truth, or consent.

### Somatic Profiles

Somatic Profiles must define body-state, posture-level, whole-body, or embodied-orientation experience.

They may reference Sensory Profiles or Activation Profiles, but they must not duplicate localized sensory qualities.

```text
Somatic Profile
= bracing, holding, support, collapse, grounding, guarding, release, approach, withdrawal, steadiness, etc.
```

Somatic Profiles must not define localized sensory perception by itself, diagnosis, valence, pleasure, desire, symbolic meaning, authorial language, corpus truth, or consent.

## Candidate Relationship Validation State

The following relationship statements are currently draft-pattern relationships.

They may be used in Supported records but should not be treated as baseline relationship verbs until repeated profile validation confirms them.

```text
IS_SENSORY_PROFILE
IS_SOMATIC_PROFILE
HAS_SENSORY_SCOPE
HAS_SOMATIC_SCOPE
HAS_PRIMARY_SENSORY_ANCHOR
HAS_PRIMARY_SOMATIC_ANCHOR
MAY_BE_ENABLED_BY
MAY_REFERENCE_ANATOMICAL_SITE
MAY_REFERENCE_FLUID_ENTITY
MAY_REFERENCE_FLUID_PROFILE
MAY_REFERENCE_MIRROR_ROUTE
MAY_REFERENCE_SENSORY_PROFILE
MAY_DEFINE_SENSORY_QUALITY
MAY_DEFINE_SOMATIC_STATE
MAY_HAVE_VALENCE
MAY_CONTEXTUALIZE
MAY_BE_INTERPRETED_BY
MAY_BE_USED_BY
MAY_BE_ANNOTATED_IN
```

## Promotion and Alignment Decisions

### Female - Pelvic Floor Sensory Profile

| Field | Assessment |
|---|---|
| Mechanical Result | Pass |
| Governance Result | Pass |
| Blocking Defect | None |
| Non-Blocking Open Questions | Sensory-quality value governance; directionality boundary; ache/discomfort routing; mirror context; future Discomfort Register |
| Promotion Recommendation | Promote to Supported |
| Decision Applied | Supported / Draft v0.3 |
| Review Date | 2026-07-03 |

Evidence:

```text
light internal consistency review confirmed required sections are present
Sensory Profile defines perceived qualities rather than activation mechanics
upstream Female - Pelvic Floor Contraction Activation Profile remains the source Activation context
Female - Pelvic Floor remains the primary sensory anchor
Mirror route remains contextual traversal only
Fluid Layer independence is preserved
Sensory Valence Register and Pleasure Register remain downstream only
Desire, Symbolic Meaning, Authorial, and Corpus systems remain downstream
sensory-quality terms remain controlled candidate values, not wikilinked nodes
consent boundary remains explicit
```

### Female - Vulva Sensory Profile

| Field | Assessment |
|---|---|
| Mechanical Result | Pass |
| Governance Result | Pass |
| Blocking Defect | None |
| Non-Blocking Open Questions | Sensory-quality value governance; surface-relation perception vs Fluid Profile relationship; taste/odour governance; future Discomfort Register |
| Promotion Recommendation | Retain Supported |
| Decision Applied | Supported / Draft v0.3 |
| Original Review Date | 2026-07-03 |
| Cross-Layer Alignment Date | 2026-07-09 |

Evidence:

```text
light internal consistency review confirmed required sections are present
Sensory Profile defines perceived qualities rather than activation mechanics
Female - Vulva remains the primary sensory anchor
Regional sensory scope is justified by vulva, vestibule, vaginal opening, vaginal canal, and fluid-surface context
Vaginal Fluid identity remains Fluid Layer content
Female - Vulva Fluid Profile and Female - Vaginal Canal Fluid Profile provide context without defining sensation
wetness, surface presence, flow, taste, and odour remain sensory qualities, not fluid identity or production mechanics
surface relation records perception only and does not replace Fluid Profile anatomical relationships
Mirror route remains contextual traversal only
upstream Female - Vulvar Lubrication Activation Profile now uses the same Mirror boundary and no longer treats Mirror traversal as an Activation component
Sensory Valence Register and Pleasure Register remain downstream only
Desire, Symbolic Meaning, Authorial, and Corpus systems remain downstream
sensory-quality terms remain controlled candidate values, not wikilinked nodes
consent boundary explicitly rejects wetness, lubrication, fluid surface presence, taste, odour, pleasure, desire, and symbolic meaning as consent
```

### Female - Pelvic Floor Somatic Profile

| Field | Assessment |
|---|---|
| Mechanical Result | Pass |
| Governance Result | Pass |
| Blocking Defect | None |
| Non-Blocking Open Questions | Somatic-state value governance; Local / Whole-Body scope replication; guarding boundary; letting-go phrasing; future Discomfort Register |
| Promotion Recommendation | Promote to Supported |
| Decision Applied | Supported / Draft v0.3 |
| Review Date | 2026-07-03 |

Evidence:

```text
light internal consistency review confirmed required sections are present
Somatic Profile defines body-state and embodied orientation rather than localized sensory qualities
Female - Pelvic Floor Contraction Activation Profile remains upstream Activation context
Female - Pelvic Floor Sensory Profile may inform but does not define somatic body-state
Local / Whole-Body scope is retained as first-pass expression of local source with possible whole-body echo
Somatic-state terms remain controlled candidate values, not wikilinked nodes
Sensory Valence Register and Pleasure Register remain downstream only
Desire, Symbolic Meaning, Authorial, and Corpus systems remain downstream
no diagnosis, trauma inference, refusal inference, or consent inference is made
consent boundary remains explicit
```

## First Validation Path

```text
Female - Pelvic Floor Contraction Activation Profile
→ Female - Pelvic Floor Sensory Profile
→ Female - Pelvic Floor Somatic Profile
→ Sensory Valence Register
→ Pleasure Register / Desire Register / Symbolic Meaning Register downstream
```

This path is useful because the upstream Activation Profile is Supported, Local, fluid-independent, and Motor / Kinetic only.

## Fluid-Involving Validation Path

```text
Female - Vulvar Lubrication Activation Profile
→ Vaginal Fluid / Female - Vulva Fluid Profile / Female - Vaginal Canal Fluid Profile
→ Female - Vulva Sensory Profile
→ Sensory Valence Register
→ Pleasure Register / Desire Register / Symbolic Meaning Register downstream
```

This path validates that Sensory Profiles can reference Fluid Layer content without redefining fluid identity, production, anatomical path, valence, desire, symbolic meaning, or consent.

The upstream Activation profile and downstream Sensory profile now share the same Mirror boundary: traversal may be referenced, but Mirror is not a physiological or sensory mechanism.

## Consent Boundary

```text
Activation is not consent.
Sensation is not consent.
Somatic state is not consent.
Valence is not consent.
Wetness is not consent.
Lubrication is not consent.
Fluid surface presence is not consent.
Taste is not consent.
Odour is not consent.
Pleasure is not consent.
Discomfort is not refusal by itself.
Relief is not consent.
Neutrality is not consent.
Ambivalence is not consent.
Desire is not consent.
Symbolic meaning is not consent.
Authorial emphasis is not consent.
Corpus usage is not consent.
```

## Status

Draft v0.4.

This register has governed three Supported Expressive Profile pilots and now records the first explicit cross-layer alignment revision between a Supported Activation Profile and its downstream Sensory Profile.