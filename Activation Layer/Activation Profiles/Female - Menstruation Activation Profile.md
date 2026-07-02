---
tags:
  - Ontology Node
  - Activation Layer
  - Activation Profile
  - Female Embodiment
  - Status/Draft
title: Female - Menstruation Activation Profile
file_class: Ontology Node
node_type: Activation Profile
layer: Activation Layer
status: Draft
version: 0.1
activation_type: Composite Activation
activation_components:
  - Hormonal / Cyclical Activation
  - Tissue-State Activation
  - Fluid Activation
activation_scope: Regional
embodiment_scope: Female / Anatomy-Dependent
primary_anatomical_anchor: Female - Uterus
validation_status: Candidate
---

# Female - Menstruation Activation Profile

## Purpose

This node defines menstruation as a recurring, hormonally influenced activation process involving uterine tissue-state change, [[Menstrual Fluid]] formation or release, and passage through nearby reproductive anatomy.

It defines activation and temporal sequence only. It does not define Hormone Entities, endocrine mechanisms, anatomy, fluid identity, sensation, emotional meaning, symbolism, authorial language, corpus usage, or consent.

## Activation Classification

| Field | Value |
|---|---|
| Node Type | Activation Profile |
| Layer | Activation Layer |
| Activation Type | Composite Activation |
| Activation Components | Hormonal / Cyclical Activation; Tissue-State Activation; Fluid Activation |
| Activation Scope | Regional |
| Embodiment Scope | Female / Anatomy-Dependent |
| Primary Anatomical Anchor | [[Female - Uterus]] |
| Validation Status | Candidate |

## Trigger or Condition

| Trigger / Condition | Role | Notes |
|---|---|---|
| Menstrual-cycle phase context | May Initiate / Contextualize | Cyclical context only |
| Hormonal or cyclical transition | May Initiate / Modulate | Neutral influence; no Hormone Entity is defined |
| Uterine tissue-state transition | May Initiate / Coordinate | Local physiological state change |
| Pregnancy, postpartum state, menopause, medication, surgery, illness, stress, nutrition, or endocrine condition | May Modulate / Inhibit | Context only; no diagnosis is defined |

## Participating Canonical Nodes

| Anatomical Node | Role In Activation | Notes |
|---|---|---|
| [[Female - Uterus]] | Primary Anchor / Origin Site | Primary tissue-state and fluid-origin context |
| [[Female - Cervix]] | Transitional Participant | Conducts between uterus and vaginal canal |
| [[Female - Vaginal Canal]] | Conduit / Receiving Participant | Conducts Menstrual Fluid toward output territory |
| [[Female - Vaginal Opening]] | Output / Transition Participant | External output boundary |
| [[Female - Vulva]] | Surface Context | External surface presence only; not source |

## Referenced Mirror Routes

No Mirror Profile is required for the core menstruation process.

## Referenced Fluid Entities

| Fluid Entity | Activation Role | Notes |
|---|---|---|
| [[Menstrual Fluid]] | May Form / Release / Move / Expose | Identity remains defined in Fluid Layer |

## Referenced Fluid Profiles

| Fluid Profile | Role | Notes |
|---|---|---|
| [[Female - Vaginal Canal Fluid Profile]] | Conduit / Receiving Context | Existing local fluid relationship |
| [[Female - Vulva Fluid Profile]] | Surface / Adjacent Context | External presence only; not source |

No uterus-specific or cervix-specific Fluid Profile is silently assumed. Those may be created later if independently useful.

## Fluid Property Alterations

| Fluid Property | Possible Change | Notes |
|---|---|---|
| [[Volume]] | May Increase / Decrease / Cease | Cyclical quantity change |
| [[Flow]] | May Initiate / Continue / Alter / Cease | Movement through the regional route |
| [[Viscosity]] | May Vary | Neutral property change |
| [[Colour]] | May Vary | Neutral property change |
| [[Opacity]] | May Vary | Neutral property change |
| [[Cyclicity]] | Recurring / Phase-Dependent | Temporal property only |
| [[Surface Presence]] | May Increase / Expose / Cease | Output or external presence |

## Temporal or Phase Sequence

```text
1. Menstrual-cycle context enters a phase in which menstruation may occur.
2. A hormonally influenced transition becomes relevant without defining specific hormone mechanisms.
3. Uterine tissue state changes and Menstrual Fluid may form or become releasable.
4. Fluid release begins, continues, varies, or ceases over time.
5. The active phase completes.
6. Recurrence remains possible within a later cycle.
```

## Activation Sequence

```text
1. Female - Uterus enters activation context as primary anchor.
2. Uterine tissue-state change supports Menstrual Fluid formation or release.
3. Female - Cervix directly participates as transitional anatomy.
4. Female - Vaginal Canal receives and conducts Menstrual Fluid.
5. Female - Vaginal Opening functions as output boundary.
6. Female - Vulva may provide external surface context without becoming the source.
7. Existing Fluid Profiles provide canal and surface relationship context.
8. Downstream systems may later reference the activation.
```

## Modulators and Inhibitors

| Factor | Role | Notes |
|---|---|---|
| Cycle regularity | May Modulate | Temporal context only |
| Hormonal or endocrine context | May Modulate / Inhibit | No detailed endocrine mechanism defined |
| Pregnancy, postpartum state, or menopause | May Inhibit / Alter / Contextualize | Anatomy-dependent context |
| Medication, surgery, illness, nutrition, fatigue, or stress | May Modulate / Inhibit | Context only |
| Structural or tissue condition | May Alter | Requires separate canonical or medical governance if expanded |

## Candidate Downstream Links

| Downstream Record | Purpose |
|---|---|
| Menstrual Fluid Sensory Profile | May define perception of fluid properties |
| Female - Uterus Sensory Profile | May define uterine perception |
| Female - Cervix Sensory Profile | May define cervical perception |
| Female - Vaginal Canal Sensory Profile | May define canal-related perception |
| Propagation Profile | May define wider spread or transferred effects if needed |
| [[Pleasure Register]] | May define valence where relevant |
| [[Desire Register]] | May define motivational orientation where relevant |
| [[Symbolic Meaning Register]] | May define interpretation |
| Authorial Term Register | May govern language |
| Corpus Annotation | May record situated use |

## Boundary Rules

Do not define:

```text
specific hormone entities or levels
endocrine pathways or receptor mechanisms
canonical anatomy
Menstrual Fluid identity
sensory perception
pain or pleasure as valence
emotional or symbolic meaning
consent
authorial language
corpus examples
propagation mechanics
clinical diagnosis
```

## Consent Boundary

```text
Hormonal state is not consent.
Cyclical state is not consent.
Menstruation is not consent.
Fluid release is not consent.
Surface presence is not consent.
Pleasure is not consent.
Desire is not consent.
Symbolic meaning is not consent.
```

## Relationship Statements

```text
Female - Menstruation Activation Profile IS_ACTIVATION_PROFILE
Female - Menstruation Activation Profile HAS_ACTIVATION_TYPE Composite Activation
Female - Menstruation Activation Profile HAS_ACTIVATION_COMPONENT Hormonal / Cyclical Activation
Female - Menstruation Activation Profile HAS_ACTIVATION_COMPONENT Tissue-State Activation
Female - Menstruation Activation Profile HAS_ACTIVATION_COMPONENT Fluid Activation
Female - Menstruation Activation Profile HAS_ACTIVATION_SCOPE Regional
Female - Menstruation Activation Profile ACTIVATES_ANATOMICAL_SITE Female - Uterus
Female - Menstruation Activation Profile INVOLVES_ANATOMICAL_NODE Female - Cervix
Female - Menstruation Activation Profile INVOLVES_ANATOMICAL_NODE Female - Vaginal Canal
Female - Menstruation Activation Profile INVOLVES_ANATOMICAL_NODE Female - Vaginal Opening
Female - Menstruation Activation Profile REFERENCES_ADJACENT_ANATOMICAL_SITE Female - Vulva
Female - Menstruation Activation Profile INVOLVES_FLUID_ENTITY Menstrual Fluid
Female - Menstruation Activation Profile REFERENCES_FLUID_PROFILE Female - Vaginal Canal Fluid Profile
Female - Menstruation Activation Profile REFERENCES_FLUID_PROFILE Female - Vulva Fluid Profile
Female - Menstruation Activation Profile MAY_ALTER_FLUID_PROPERTY Volume
Female - Menstruation Activation Profile MAY_ALTER_FLUID_PROPERTY Flow
Female - Menstruation Activation Profile MAY_ALTER_FLUID_PROPERTY Viscosity
Female - Menstruation Activation Profile MAY_ALTER_FLUID_PROPERTY Colour
Female - Menstruation Activation Profile MAY_ALTER_FLUID_PROPERTY Opacity
Female - Menstruation Activation Profile MAY_ALTER_FLUID_PROPERTY Cyclicity
Female - Menstruation Activation Profile MAY_ALTER_FLUID_PROPERTY Surface Presence
Female - Menstruation Activation Profile MAY_HAND_OFF_TO Propagation Profile
Female - Menstruation Activation Profile MAY_ENABLE Menstrual Fluid Sensory Profile
Female - Menstruation Activation Profile MAY_BE_INTERPRETED_BY Symbolic Meaning Register
Female - Menstruation Activation Profile MAY_BE_USED_BY Authorial Term Register
Female - Menstruation Activation Profile MAY_BE_ANNOTATED_IN Corpus Annotation
```

## Review Questions

1. Is Regional scope correct for uterus, cervix, vaginal canal, and vaginal opening as direct participants?
2. Does the profile distinguish cyclical context from unmodelled endocrine mechanisms?
3. Should uterine tissue shedding remain within Tissue-State Activation without an endometrium node?
4. Are cervix and vaginal opening direct participants or transition/output context only?
5. Are missing uterus and cervix Fluid Profiles non-blocking?
6. Does the sequence separate Activation from future Propagation?
7. Should a later Cycle Regulation Activation Profile be distinct from Menstruation?

## Status

Draft v0.1.

Candidate Hormonal / Cyclical validation profile.
