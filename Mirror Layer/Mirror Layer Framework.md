---
tags:
  - Document/Framework
  - Layer/Mirror
  - Status/Draft
title: Mirror Layer Framework
file_class: Document
document_type: Framework
layer: Mirror Layer
status: Draft
version: 0.2
last_updated: 2026-06-30
---

# Mirror Layer Framework

## Purpose

The Mirror Layer models governed correspondences between ontology objects.

A mirror is not an anatomical structure, activation process, sensory experience, symbolic meaning, authorial device, or corpus example. It is a reusable relationship pattern that allows two or more ontology objects to be compared, reflected, echoed, paired, contrasted, traversed, or held in boundary relation without duplicating their definitions.

Mirror records help the graph preserve relational routes while keeping canonical, activation, fluid, expressive, authorial, and corpus layers distinct.

---

## Layer Position

The Mirror Layer sits between canonical knowledge and downstream interpretive systems.

```text
Canonical Embodiment
→ defines what exists

Fluid Layer
→ defines fluid properties, entities, and profiles

Activation Layer
→ defines processes and responses

Mirror Layer
→ defines structured correspondences and traversal routes

Expressive Layers
→ define perceived, emotional, symbolic, sensory, and temporal experience

Authorial Systems
→ define controlled authorial use

Corpus
→ records specific instances in works
```

---

## Folder Structure

```text
Mirror Layer
├── Mirror Layer Framework.md
└── Mirror Profiles
    ├── Mirror Profiles Index.md
    ├── Female - Vulva to Female - Clitoral Complex Mirror Profile.md
    ├── Female - Clitoral Complex to Female - Breasts Mirror Profile.md
    └── Female - Vulva to Female - Anus Mirror Profile.md
```

Mirror profiles live in a dedicated `Mirror Profiles` subfolder.

---

## Core Architectural Rule

Mirrors describe correspondence. They do not redefine the things being mirrored.

```text
Mirror Profile
= reusable correspondence record

Mirrored Object
= anatomical node, fluid entity, activation profile, sensory profile, symbolic profile, authorial device, or corpus annotation
```

A mirror profile may link objects across the same layer or across different layers, provided it does not collapse their categories.

---

## Mirror Types

Initial controlled mirror types include:

```text
Anatomical
Functional
Sensory-Adjacent
Symbolic
Relational
Inversion
Echo
Contrast
Boundary
Anatomical-Adjacent
```

These should remain controlled values until repeated patterns justify more detailed subtypes.

---

## Directionality

Every mirror profile must state directionality.

```text
Bidirectional
= traversal is valid in either direction using the same correspondence basis

Source-to-Target
= traversal is valid primarily from source object to target object

Target-to-Source
= traversal is valid primarily from target object to source object

Contextual
= traversal direction depends on activation, expressive, authorial, or corpus context
```

A bidirectional profile does not require a duplicate inverse file unless the inverse route has a different correspondence basis, layer boundary, or governance rule.

---

## Composite-First Mirror Rule

Mirror profiles should usually anchor at the highest meaningful composite node that contains the mirror field.

This prevents prematurely narrowing a mirror to one atomic child when multiple child structures may participate downstream.

Example:

```text
Female - Clitoral Complex ↔ Female - Breasts
= composite-first mirror

Potential child traversal:
Female - Clitoral Glans
Female - Clitoral Hood
Female - Clitoral Body
Female - Clitoral Crura
Female - Vestibular Bulbs

Potential child traversal:
Female - Nipples
Female - Areolae
Female - Breast Skin
Female - Mammary Tissue
```

A lower-level focal mirror may still be created later, but only when the narrower correspondence has a distinct modelling purpose.

---

## Descendant Mirror Candidates

Composite-first mirror profiles may name possible descendant mirrors without creating standalone mirror files immediately.

This preserves future traversal routes while avoiding unnecessary node proliferation.

Examples:

```text
Female - Nipples ↔ Female - Vaginal Canal
Female - Nipples ↔ Female - Anus
Female - Areolae ↔ Female - Vestibule
Female - Breast Skin ↔ Female - Vulva
Female - Clitoral Glans ↔ Female - Nipples
```

Candidate descendant mirrors should become standalone mirror profiles only when downstream activation, sensory, symbolic, authorial, or corpus use makes the narrower correspondence independently meaningful.

---

## Lightweight Routing Hints

Mirror profiles may include lightweight routing hints so the graph can prioritize plausible routes.

Routing hints are not activation mechanics and not expressive interpretation.

```text
Mirror Layer may rank plausible correspondence routes.
Mirror Layer must not define when, how strongly, or with what felt meaning those routes activate.
```

Allowed routing fields:

```text
baseline_mirror_likelihood: High / Moderate / Low / Contextual / Unknown
activation_dependency: Independent / Activation-Dependent / Expressive-Dependent / Corpus-Dependent / Unknown
traversal_priority: Primary / Secondary / Tertiary / Candidate / Unknown
```

Activation and Expressive layers later decide what actually fires, how strongly, and how it is experienced.

---

## Relationship to Activation

Mirror is not activation.

Activation describes response initiation, physiological process, or change.

Mirror describes correspondence and route plausibility.

Example:

```text
Nipple Touch Activation Profile
→ may activate or weight a mirror route

Female - Clitoral Complex to Female - Breasts Mirror Profile
→ records a composite correspondence route that may become salient under activation
```

A mirror may be activated by an event, but the mirror itself is not the event.

---

## Relationship to Expressive Layers

Mirror profiles may support expressive interpretation, but they do not define expressive meaning directly.

Example:

```text
Tears to Rain Mirror Profile
→ records correspondence between tears and rain

Tears Symbolic Profile
→ defines symbolic meanings of tears

Rain Symbolic Profile
→ defines symbolic meanings of rain

Corpus Annotation
→ records a work where tears and rain are used together
```

---

## Boundary Rules

Mirror Layer records must not include:

```text
canonical anatomical definitions
activation mechanics
fluid definitions
sensory pleasure or discomfort
emotional interpretation as definition
symbolic meaning as definition
authorial language rules
corpus examples as canonical truth
intensity, felt meaning, or narrative effect
```

They may point to these layers as candidate downstream uses.

---

## Relationship Statements

Use controlled relationship language.

```text
Mirror Profile MIRRORS Source Object
Mirror Profile MIRRORS Target Object
Mirror Profile HAS_MIRROR_TYPE Mirror Type
Mirror Profile HAS_DIRECTIONALITY Directionality
Mirror Profile HAS_ANCHOR_LEVEL Anchor Level
Mirror Profile ALLOWS_CHILD_TRAVERSAL true / false
Mirror Profile HAS_DESCENDANT_MIRROR_CANDIDATES true / false
Mirror Profile HAS_BASELINE_MIRROR_LIKELIHOOD Likelihood
Mirror Profile HAS_ACTIVATION_DEPENDENCY Dependency
Mirror Profile HAS_TRAVERSAL_PRIORITY Priority
Mirror Profile HAS_CORRESPONDENCE_BASIS Basis
Mirror Profile MAY_SUPPORT Expressive Profile
Mirror Profile MAY_BE_USED_BY Authorial System
Mirror Profile MAY_BE_ANNOTATED_IN Corpus Annotation
```

---

## Current Validation Set

```text
Female - Vulva to Female - Clitoral Complex Mirror Profile
Female - Clitoral Complex to Female - Breasts Mirror Profile
Female - Vulva to Female - Anus Mirror Profile
```

These test:

```text
composite-to-component correspondence
composite-to-composite correspondence with child traversal
external pelvic boundary correspondence
explicit directionality
lightweight routing hints
```

---

## Governance Notes

Mirrors should preserve the following rules:

```text
mirror does not redefine anatomy
mirror does not initiate activation
mirror does not create symbolic meaning by itself
mirror does not authorialize language
mirror supports traversal without collapsing layers
mirror may guide route priority without defining response intensity
```

---

## Review Questions

1. Which mirror types should become controlled values?
2. Should Sensory-Adjacent remain a mirror type, or become only a downstream candidate?
3. Which candidate descendant mirrors should remain hints rather than standalone nodes?
4. Are routing hints lightweight enough, or have they crossed into Activation or Expressive layers?
5. Which mirror profiles are needed before Activation Layer validation?
6. Which mirror profiles are needed before Expressive Layer validation?

---

## Status

Draft v0.2.

This framework reflects the current Mirror Profile Template, composite-first anchoring, descendant mirror candidates, explicit directionality, and lightweight routing hints.
