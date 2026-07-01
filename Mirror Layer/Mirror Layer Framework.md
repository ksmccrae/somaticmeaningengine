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
version: 0.4
last_updated: 2026-07-01
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
    ├── Female Mirror Candidate Register.md
    ├── Female - Vulva to Female - Clitoral Complex Mirror Profile.md
    ├── Female - Clitoral Complex to Female - Breasts Mirror Profile.md
    ├── Female - Vulva to Female - Anus Mirror Profile.md
    ├── Female - Vulva to Female - Breasts Mirror Profile.md
    ├── Female - Nipples to Female - Vaginal Canal Mirror Profile.md
    ├── Female - Skene's Glands to Female - Urethral Opening Mirror Profile.md
    └── Female - Perineum to Female - Pelvic Floor Mirror Profile.md
```

Mirror profiles and candidate registers live in the dedicated `Mirror Profiles` subfolder.

---

## Supported and Candidate Status Model

The Mirror Layer separates profile maturity into at least two operational groups.

```text
Supported Validation Set
= profiles already audited against the validated Mirror Profile Template and confirmed as mechanically clean

Expansion Candidate Set
= structurally governed draft profiles created for traversal testing but not yet promoted to Supported

Candidate Register
= planning document for possible mirror routes, deferred candidates, and construction criteria
```

Document status and validation status must remain separate.

```text
Document Status
= file maturity and version, for example Draft v0.1

Validation Status
= whether the profile is Supported, Candidate, or Blocked
```

Candidate profiles may be useful for Activation planning without being part of the Supported validation set.

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

`Fluid-Adjacent` is not currently a controlled mirror type. Fluid adjacency may be described in prose under Anatomical, Functional, Boundary, or other governed mirror types unless an ADR or later governance decision promotes it to a controlled value.

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

## Boundary Region References

Mirror profiles may reference a boundary region when the mirrored route depends on shared or adjacent anatomical territory.

The boundary reference is a traversal aid. It must not redefine canonical anatomy.

Examples:

```text
Female - Vulva to Female - Anus Mirror Profile
REFERENCES_BOUNDARY_REGION Female - Perineum

Female - Perineum to Female - Pelvic Floor Mirror Profile
REFERENCES_BOUNDARY_REGION Female - Perineum
```

This means the perineum helps explain the boundary route. It does not create a new anatomical definition of the perineum, vulva, anus, or pelvic floor.

---

## Relationship to Fluid Layer

Mirror profiles may reference Fluid Layer profiles or fluid entities as candidate downstream traversal hooks.

They must not define fluid entities, fluid properties, fluid production, fluid release, or fluid activation mechanics.

Example:

```text
Female - Skene's Glands to Female - Urethral Opening Mirror Profile
→ may reference Paraurethral Glandular Fluid and Urine as boundary-sensitive traversal objects
→ must not collapse those fluids or define their activation
```

Fluid-adjacent prose is allowed as a boundary note. `Fluid-Adjacent` is not currently a controlled mirror type.

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
Mirror Profile REFERENCES_BOUNDARY_REGION Boundary Region
Mirror Profile MAY_SUPPORT Expressive Profile
Mirror Profile MAY_BE_USED_BY Authorial System
Mirror Profile MAY_BE_ANNOTATED_IN Corpus Annotation
```

---

## Current Supported Validation Set

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
boundary-region references
```

---

## Current Female Expansion Candidate Set

```text
Female - Vulva to Female - Breasts Mirror Profile
Female - Nipples to Female - Vaginal Canal Mirror Profile
Female - Skene's Glands to Female - Urethral Opening Mirror Profile
Female - Perineum to Female - Pelvic Floor Mirror Profile
```

These candidate profiles test:

```text
composite external body-region mirroring
focal output-site to internal-canal mirroring
paraurethral glandular to urinary-output boundary mirroring
boundary-region to support-structure mirroring
Fluid Layer adjacency without fluid definition
Activation dependency as routing hint only
```

They remain Candidate until a later audit promotes them.

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
boundary-region references are traversal aids, not anatomical definitions
```

---

## Review Questions

1. Which mirror types should become controlled values?
2. Should Sensory-Adjacent remain a mirror type, or become only a downstream candidate?
3. Which candidate descendant mirrors should remain hints rather than standalone nodes?
4. Are routing hints lightweight enough, or have they crossed into Activation or Expressive layers?
5. Are boundary-region references sufficiently constrained as traversal aids?
6. Which mirror profiles are needed before Activation Layer validation?
7. Which mirror profiles are needed before Expressive Layer validation?
8. Should any female expansion candidates be promoted from Candidate to Supported after audit?
9. Should Fluid-Adjacent remain descriptive prose, or become a governed mirror type in a later ADR?

---

## Status

Draft v0.4.

This framework reflects the current Mirror Profile Template, composite-first anchoring, descendant mirror candidates, explicit directionality, lightweight routing hints, formal boundary-region reference support, the Supported/Candidate split, and the first female mirror expansion candidate set.
