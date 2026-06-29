---
tags:
  - Document/Framework
  - Layer/Fluid
  - Status/Draft
title: Fluid Layer Framework
file_class: Document
document_type: Framework
layer: Fluid Layer
status: Draft
version: 0.1
last_updated: 2026-06-29
---

# Fluid Layer Framework

## Purpose

The Fluid Layer models bodily fluids as reusable ontology objects and defines their relationships to anatomy, activation, sensory perception, symbolic meaning, authorial systems, and corpus annotation.

This layer exists so fluids are not duplicated inside anatomical nodes, activation nodes, sensory profiles, or symbolic registers.

Fluid records define fluid identity and local fluid relationships. They do not redefine anatomy, activation mechanics, sensory experience, symbolic meaning, authorial language, or corpus usage.

---

## Layer Position

The Fluid Layer sits between Canonical Embodiment and downstream expressive systems.

```text
Canonical Embodiment
→ defines anatomical structures and systems

Fluid Layer
→ defines reusable fluid entities and local anatomical fluid relationships

Activation Layer
→ defines processes that produce, release, move, expose, withhold, or alter fluids

Expressive Layers
→ define sensory, symbolic, emotional, temporal, environmental, and other experiential meanings

Authorial Systems
→ define language, register, stylistic treatment, and controlled authorial use

Corpus
→ records how fluids appear in specific works
```

---

## Core Architectural Rule

Fluid modelling uses a two-part structure.

```text
Fluid Entity
= what the fluid is

Fluid Profile
= how that fluid relates to a specific anatomical anchor
```

Activation profiles may later connect one or more fluid entities across one or more anatomical sites.

This prevents any one anatomical node from owning the full meaning or behaviour of a fluid.

---

## Fluid Entities

Fluid entities define reusable fluids independent of any single anatomical site.

Examples:

```text
Tears
Blood
Sweat
Saliva
Urine
Menstrual Fluid
Vaginal Fluid
Cervical Mucus
Paraurethral Glandular Fluid
Milk
Semen
Pre-Ejaculate
Surface Moisture
```

Fluid entities may include neutral physiological qualities such as viscosity, density, colour, opacity, odour, taste, volume, flow, and cyclicity.

They may reference common sources, conduits, and output sites, but they should not become local anatomical profiles.

---

## Fluid Profiles

Fluid profiles describe the local relationship between an anatomical anchor and one or more fluid entities.

Examples:

```text
Female - Vulva Fluid Profile
Female - Vaginal Canal Fluid Profile
Female - Skene's Glands Fluid Profile
Female - Breasts Fluid Profile
Female - Eye Fluid Profile
Female - Mouth Fluid Profile
```

A fluid profile may define whether the anatomical anchor:

```text
produces a fluid
stores a fluid
conducts a fluid
receives a fluid
acts as an output site
has surface presence
is adjacent to a fluid source or output site
```

Fluid profiles should separate source, conduit, output site, and adjacent site so fluids are not assigned to nearby structures incorrectly.

---

## Activation Relationship

The Fluid Layer does not define activation mechanics.

Activation profiles define events or processes that produce, release, move, expose, withhold, or alter one or more fluids across one or more anatomical sites.

Example:

```text
Crying Activation Profile
→ may involve tears, lacrimal anatomy, face, breathing, voice, and emotional expression

Urination Activation Profile
→ may involve urine, bladder, urethra, urethral opening, pelvic floor, and release control

Menstruation Activation Profile
→ may involve menstrual fluid, uterus, cervix, vaginal canal, cycle timing, and hormonal regulation

Smack Activation Profile
→ may involve skin, hand, local tissue, blood, sweat, saliva, tears, surface moisture, and multiple sensory consequences
```

Activation is therefore not owned by one anatomical site or one fluid.

---

## Expressive Layer Relationship

Fluid entities and fluid profiles may be referenced by expressive records, but expressive meaning is not defined inside the Fluid Layer.

Examples:

```text
Tears Sensory Profile
Tears Symbolic Profile
Blood Symbolic Profile
Sweat Sensory Profile
Menstrual Fluid Symbolic Profile
Milk Symbolic Profile
```

The Fluid Layer may describe neutral qualities such as colour, odour, taste, viscosity, or volume.

The Sensory Layer describes how those qualities are perceived.

The Symbolic Layer describes what those qualities may mean.

The Authorial Systems layer governs language, register, restraint, and stylistic treatment.

---

## Boundary Rules

Fluid Layer records must not include:

```text
canonical anatomical definitions
activation mechanics
sensory pleasure or discomfort
emotional interpretation
symbolic meaning
authorial terminology
story examples
corpus usage
```

Those concerns belong to their own layers.

---

## Current Templates

| Template | Purpose | Status |
|---|---|---|
| [[Fluid Entity Template]] | Defines reusable fluid entities independent of one anatomical site. | Draft v0.1 |
| [[Fluid Profile Template]] | Defines local relationships between anatomical anchors and reusable fluid entities. | Draft v0.3 |

---

## Current Validation Set

Fluid modelling is currently being validated through a small Female Embodiment set:

```text
Female - Vulva Fluid Profile
Female - Vaginal Canal Fluid Profile
Female - Skene's Glands Fluid Profile
Female - Breasts Fluid Profile
```

The next validation set should include reusable fluid entities such as:

```text
Tears
Urine
Menstrual Fluid
Vaginal Fluid
Milk
Blood
Sweat
Saliva
```

---

## Governance Notes

The Fluid Layer should preserve the following rules:

```text
anatomy does not own fluid
fluid does not own activation
activation does not own meaning
meaning does not redefine biology
```

This allows graph traversal from fluid entities into anatomy, activation, sensory perception, symbolism, authorial systems, and corpus annotation without duplication.

---

## Review Questions

1. Should fluid entities live directly in the Fluid Layer root or in a dedicated Fluid Entities subfolder?
2. Should anatomical fluid profiles live directly in the Fluid Layer root or in a dedicated Fluid Profiles subfolder?
3. Which fluid entities should be validated before the Fluid Entity Template is frozen?
4. Should Surface Moisture be a fluid entity, a quality, or a relationship type?
5. Which activation profiles must exist before fluid modelling can be considered stable?

---

## Status

Draft v0.1.

This framework reflects the current split between Fluid Entity and Fluid Profile modelling and should be reviewed before the Fluid Layer is marked Baseline.
