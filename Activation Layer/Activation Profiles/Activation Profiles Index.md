---
tags:
  - Document/Index
  - Layer/Activation
  - Activation Profiles
  - Status/Draft
title: Activation Profiles Index
file_class: Document
document_type: Index
layer: Activation Layer
status: Draft
version: 0.2
last_updated: 2026-07-01
---

# Activation Profiles Index

## Purpose

This index lists Activation Profile nodes in the Activation Layer.

Activation profiles define governed physiological, embodied, and processual state changes without redefining anatomy, fluids, mirrors, sensory experience, pleasure, desire, symbolic meaning, authorial language, or corpus usage.

## Current Validation Set

| Activation Profile | Primary Anchor | Activation Type | Activation Components | Activation Scope | Embodiment Scope | Referenced Fluid Entity | Referenced Mirror Route | Validation Status | Document Status |
|---|---|---|---|---|---|---|---|---|---|
| [[Female - Vulvar Lubrication Activation Profile]] | [[Female - Vulva]] | Composite Activation | Tissue-State Activation; Fluid Activation; Mirror-Route Activation | Regional | Female / Anatomy-Dependent | [[Vaginal Fluid]] | [[Female - Vulva to Female - Clitoral Complex Mirror Profile]] | Candidate | Draft v0.2 |
| [[Female - Paraurethral Glandular Release Activation Profile]] | [[Female - Skene's Glands]] | Composite Activation | Fluid Activation; Mirror-Route Activation; Autonomic Activation | Regional | Female / Anatomy-Dependent | [[Paraurethral Glandular Fluid]] | [[Female - Skene's Glands to Female - Urethral Opening Mirror Profile]] | Candidate | Draft v0.1 |

## Classification Rule

```text
Activation Type
= one controlled structural class

Activation Components
= one or more controlled process families

Activation Scope
= Local / Regional / Cross-System
```

Composite profiles use:

```text
activation_type: Composite Activation
activation_components: governed YAML list
```

## Validation Purpose

The two-profile validation set tests whether Activation can coordinate:

```text
canonical anatomical participants
Fluid Layer references
Fluid Property alterations
Mirror Layer route availability
composite activation classification
candidate downstream links
consent boundary discipline
fluid identity separation
adjacent anatomy without anatomical collapse
```

without collapsing into anatomy definitions, fluid definitions, mirror definitions, sensory perception, pleasure, desire, symbolic meaning, authorial wording, or corpus usage.

## Controlled Activation Components Currently Used

```text
Tissue-State Activation
Fluid Activation
Mirror-Route Activation
Autonomic Activation
```

`Composite Activation` is used as the structural activation type when multiple components are coordinated.

## Index Column Notes

`Document Status` records file maturity and version.

`Validation Status` records whether the profile is Supported, Candidate, or Blocked.

These are intentionally separate fields.

## Governance Notes

```text
activation defines process, not anatomy
activation coordinates fluid involvement, not fluid identity
activation may engage mirror routes, not define mirror correspondence
activation may hand off to propagation, not define propagation
activation may enable sensation, pleasure, desire, or symbolic meaning downstream, not define them
activation never implies consent
```

## Candidate Future Activation Profiles

| Candidate Activation Profile | Reason Deferred |
|---|---|
| Female - Pelvic Floor Contraction Activation Profile | Requires motor / kinetic activation governance |
| Female - Clitoral Complex Arousal Activation Profile | Requires Sensory and Pleasure boundary validation |
| Female - Breast / Nipple Arousal Activation Profile | Requires child-level mirror route decisions |
| Menstruation Activation Profile | Requires hormonal / cyclical activation governance |
| Letdown Activation Profile | Requires mammary/lactation activation governance |
| Crying Activation Profile | Likely cross-embodiment and requires lacrimal anatomy expansion |
| Sweating Activation Profile | Likely cross-embodiment and requires skin/surface profile expansion |

## Review Questions

1. Do both profiles demonstrate the normalized type/component/scope model?
2. Should Autonomic Activation remain a component of the paraurethral profile or become a modulator?
3. Are adjacent anatomy and adjacent fluid relationships sufficiently governed?
4. Which profile should be built third to test a non-fluid activation family?
5. When should Candidate profiles be promoted to Supported?

## Status

Draft v0.2.
