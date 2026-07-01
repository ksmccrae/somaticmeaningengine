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
version: 0.5
last_updated: 2026-06-30
---

# Fluid Layer Framework

## Purpose

The Fluid Layer models bodily fluids as reusable ontology objects and defines their properties and relationships to anatomy, activation, sensory perception, symbolic meaning, authorial systems, and corpus annotation.

This layer exists so fluids and fluid properties are not duplicated inside anatomical nodes, activation nodes, sensory profiles, or symbolic registers.

Fluid records define fluid identity, fluid properties, and local fluid relationships. They do not redefine anatomy, activation mechanics, sensory experience, symbolic meaning, authorial language, or corpus usage.

---

## Layer Position

The Fluid Layer sits between Canonical Embodiment and downstream expressive systems.

```text
Canonical Embodiment
→ defines anatomical structures and systems

Fluid Layer
→ defines reusable fluid properties, fluid entities, and local anatomical fluid relationships

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

## Folder Structure

Fluid Layer records are organized into dedicated subfolders.

```text
Fluid Layer
├── Fluid Layer Framework.md
├── Fluid Properties
│   ├── Fluid Properties Index.md
│   ├── Viscosity.md
│   ├── Density.md
│   ├── Colour.md
│   ├── Opacity.md
│   ├── Odour.md
│   ├── Taste.md
│   ├── Temperature.md
│   ├── Volume.md
│   ├── Flow.md
│   ├── Cyclicity.md
│   └── Surface Presence.md
├── Fluid Entities
│   ├── Fluid Entities Index.md
│   ├── Tears.md
│   ├── Urine.md
│   ├── Menstrual Fluid.md
│   ├── Vaginal Fluid.md
│   ├── Cervical Mucus.md
│   ├── Paraurethral Glandular Fluid.md
│   ├── Milk.md
│   ├── Blood.md
│   ├── Sweat.md
│   └── Saliva.md
└── Fluid Profiles
    ├── Fluid Profiles Index.md
    ├── Female - Vulva Fluid Profile.md
    ├── Female - Vaginal Canal Fluid Profile.md
    ├── Female - Skene's Glands Fluid Profile.md
    └── Female - Breasts Fluid Profile.md
```

This structure separates reusable fluid properties, reusable fluid entities, and local anatomical fluid profiles.

---

## Core Architectural Rule

Fluid modelling uses a three-part structure.

```text
Fluid Property
= reusable quality or attribute

Fluid Entity
= what the fluid is

Fluid Profile
= how that fluid relates to a specific anatomical anchor
```

Activation profiles may later connect one or more fluid entities across one or more anatomical sites and may alter one or more fluid properties.

This prevents any one anatomical node, fluid entity, or activation profile from owning the full meaning or behaviour of a fluid.

---

## Fluid Properties

Fluid properties define reusable observable, measurable, or physiologically grounded qualities.

Examples:

```text
Viscosity
Density
Colour
Opacity
Odour
Taste
Temperature
Volume
Flow
Cyclicity
Surface Presence
```

Fluid properties may be referenced by fluid entities and local fluid profiles.

They are sensory-adjacent, but they are not sensory profiles.

Example:

```text
Odour
= fluid property

Odour Sensory Profile
= how odour is perceived, tolerated, desired, rejected, remembered, or interpreted
```

---

## Fluid Entities

Fluid entities define reusable fluids independent of any single anatomical site.

Current validation entities:

```text
Tears
Urine
Menstrual Fluid
Vaginal Fluid
Cervical Mucus
Paraurethral Glandular Fluid
Milk
Blood
Sweat
Saliva
```

Additional future candidate entities may include:

```text
Semen
Pre-Ejaculate
Surface Moisture
```

Fluid entities should reference fluid properties rather than redefine property categories locally.

They may reference common sources, conduits, and output sites, but they should not become local anatomical profiles.

---

## Surface Moisture Rule

Surface Moisture may be either a relationship type or a fluid entity depending on modelling need.

By default, use Surface Moisture as a relationship type when describing local presence of another identifiable fluid on a surface.

Examples:

```text
Vaginal Fluid HAS_SURFACE_PRESENCE_ON Female - Vulva
Urine HAS_ADJACENT_SURFACE_PRESENCE_NEAR Female - Vulva
Milk HAS_SURFACE_PRESENCE_ON Female - Nipples
Sweat HAS_SURFACE_PRESENCE_ON Skin Surface
```

Create Surface Moisture as a fluid entity only when the moisture itself becomes reusable, mixed, nonspecific, accumulated, transferred, or compositionally meaningful enough to be referenced directly.

Examples:

```text
Skin Surface Moisture
Mixed Surface Moisture
Transferred Surface Moisture
Environmental Surface Moisture
```

This prevents premature creation of a vague fluid entity while preserving the option to model surface wetness as its own reusable object later.

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

Local fluid profiles may reference fluid properties only where local anatomical context alters or foregrounds a property.

---

## Activation Relationship

The Fluid Layer does not define activation mechanics.

Activation profiles define events or processes that produce, release, move, expose, withhold, or alter one or more fluids across one or more anatomical sites.

Activation profiles may also alter fluid properties such as volume, flow, temperature, opacity, colour, or surface presence.

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

Activation is therefore not owned by one anatomical site, one fluid, or one property.

---

## Expressive Layer Relationship

Fluid entities, fluid properties, and fluid profiles may be referenced by expressive records, but expressive meaning is not defined inside the Fluid Layer.

Examples:

```text
Tears Sensory Profile
Tears Symbolic Profile
Blood Symbolic Profile
Sweat Sensory Profile
Menstrual Fluid Symbolic Profile
Milk Symbolic Profile
Colour Sensory Profile
Odour Sensory Profile
Viscosity Sensory Profile
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
| [[Fluid Property Template]] | Defines reusable fluid properties. | Draft v0.1 |
| [[Fluid Entity Template]] | Defines reusable fluid entities independent of one anatomical site. | Draft v0.1 |
| [[Fluid Profile Template]] | Defines local relationships between anatomical anchors and reusable fluid entities. | Draft v0.3 |

---

## Current Validation Set

Fluid property validation set:

```text
Viscosity
Density
Colour
Opacity
Odour
Taste
Temperature
Volume
Flow
Cyclicity
Surface Presence
```

Fluid entity validation set:

```text
Tears
Urine
Menstrual Fluid
Vaginal Fluid
Cervical Mucus
Paraurethral Glandular Fluid
Milk
Blood
Sweat
Saliva
```

Fluid profile validation set:

```text
Female - Vulva Fluid Profile
Female - Vaginal Canal Fluid Profile
Female - Skene's Glands Fluid Profile
Female - Breasts Fluid Profile
```

---

## Governance Notes

The Fluid Layer should preserve the following rules:

```text
anatomy does not own fluid
fluid does not own activation
activation does not own meaning
meaning does not redefine biology
properties do not become perception
```

This allows graph traversal from fluid properties and entities into anatomy, activation, sensory perception, symbolism, authorial systems, and corpus annotation without duplication.

---

## Resolved Decisions

1. Fluid properties use a dedicated `Fluid Properties` subfolder.
2. Fluid entities use a dedicated `Fluid Entities` subfolder.
3. Anatomical fluid profiles use a dedicated `Fluid Profiles` subfolder.
4. Existing validation profiles have been migrated out of the Fluid Layer root.
5. Surface Moisture is a relationship type by default, but may become a fluid entity when it is mixed, nonspecific, accumulated, transferred, or independently reusable.
6. Cervical Mucus and Paraurethral Glandular Fluid are current Fluid Entity validation nodes, not candidate-only placeholders.

---

## Open Review Questions

1. Which fluid properties should be full nodes and which should remain controlled values?
2. Which additional fluid entities are required before the Fluid Entity Template is frozen?
3. Which activation profiles must exist before fluid modelling can be considered stable?
4. Which missing canonical anatomical anchors are required before urinary and reproductive fluid validation?
5. Should Surface Moisture remain outside the entity register until it becomes mixed, nonspecific, accumulated, transferred, or independently reusable?

---

## Status

Draft v0.5.

This framework reflects the current split between Fluid Property, Fluid Entity, and Fluid Profile modelling, the adopted subfolder structure, the current ten-entity validation set, and the conditional Surface Moisture rule.
