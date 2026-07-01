---
tags:
  - Template/Translation
  - Template/Fluid Entity
  - Status/Draft
aliases:
  - Fluid Entity Template
  - Fluid Register Entity Template
title: Fluid Entity Template
file_class: Template
template_type: Translation
node_type: Fluid Entity
layer: Fluid Layer
status: Draft
version: 0.2
last_updated: 2026-06-30
---

# Fluid Entity Template

## Purpose

This template defines the required structure for reusable fluid entity nodes in the Somatic Meaning Engine.

A fluid entity defines the fluid itself, independent of any single anatomical site, activation event, sensory interpretation, symbolic meaning, authorial usage, or corpus instance.

Fluid entities may be referenced by multiple anatomical fluid profiles and multiple activation profiles.

---

## Architectural Rule

Fluid entities are reusable knowledge objects.

They should not be defined separately inside every anatomical site.

Use this pattern:

```text
Fluid Entity
→ defines what the fluid is

Anatomical Fluid Profile
→ defines how the fluid relates to a local anatomical anchor

Activation Profile
→ defines what process produces, releases, moves, exposes, withholds, or alters the fluid

Expressive Profiles
→ define sensory, symbolic, emotional, authorial, or corpus meaning
```

---

## File Naming Rule

Fluid entity nodes should use clear fluid names.

Examples:

```text
Tears.md
Blood.md
Sweat.md
Saliva.md
Urine.md
Menstrual Fluid.md
Vaginal Fluid.md
Cervical Mucus.md
Paraurethral Glandular Fluid.md
Milk.md
```

---

## YAML Pattern

```yaml
---
tags:
  - Ontology Node
  - Fluid Layer
  - Fluid Entity
  - Status/Draft
title: Fluid Name
canonical_name: Fluid Name
file_class: Ontology Node
node_type: Fluid Entity
layer: Fluid Layer
status: Draft
version: 0.1
primary_system: System Name
embodiment_scope: Cross-Embodiment / Female / Male / Trans Feminine / Trans Masculine
fluid_class: Exocrine / Urinary / Reproductive / Circulatory / Surface / Mixed
---
```

---

# Fluid Name

## Purpose

This node defines `[Fluid Name]` as a reusable fluid entity in the Somatic Meaning Engine.

It defines the fluid itself, not a local anatomical relationship, activation process, sensory perception, symbolic meaning, authorial language, or corpus use.

---

## Canonical Definition

Define the fluid in neutral physiological language.

The definition should answer:

- What is this fluid?
- Which system or systems is it associated with?
- Is it cross-embodiment or embodiment-specific?
- What anatomical profiles may reference it?
- What activation profiles may produce, move, release, or alter it?

---

## Fluid Classification

| Field | Value |
|---|---|
| Node Type | Fluid Entity |
| Layer | Fluid Layer |
| Fluid Class | Exocrine / Urinary / Reproductive / Circulatory / Surface / Mixed |
| Primary System | System Name |
| Embodiment Scope | Cross-Embodiment / Embodiment-Specific |
| Typical State | Liquid / Semi-fluid / Mucosal / Variable |
| Cyclical | true / false / conditional |
| Conditional | true / false |

---

## Common Anatomical Sources

List common source structures without making the fluid belong to only one anatomical site.

| Anatomical Source | Relationship | Notes |
|---|---|---|
| [[Anatomical Node]] | Produces / Stores / Conducts / Receives / Exposes | Neutral note only |

---

## Common Anatomical Output or Surface Sites

List common output, surface, or visible sites.

| Anatomical Site | Relationship | Notes |
|---|---|---|
| [[Anatomical Node]] | Output / Surface Presence / Conducts / Adjacent | Neutral note only |

---

## Fluid Properties

Use this section for neutral observable or physiologically grounded properties.

Fluid entities should reference fluid property nodes rather than redefine property categories locally.

| Fluid Property | Range / Description | Notes |
|---|---|---|
| [[Viscosity]] | Thin / watery / thick / variable | Neutral description only |
| [[Density]] | Low / moderate / high / variable | Use only if meaningful at this modelling resolution |
| [[Colour]] | Clear / white / yellow / red / brown / variable | Neutral description only |
| [[Opacity]] | Clear / translucent / opaque / variable | Neutral description only |
| [[Odour]] | None / mild / strong / variable | Neutral description only |
| [[Taste]] | Neutral / saline / metallic / bitter / variable | Use only where relevant and not authorialized |
| [[Volume]] | Trace / low / moderate / high / variable | Neutral description only |
| [[Flow]] | Static / surface / discharge / stream / cyclical / variable | Neutral description only |
| [[Cyclicity]] | None / cyclical / hormonal / reproductive / contextual | Neutral description only |
| [[Surface Presence]] | None / trace / local / surface / adjacent / transferred / variable | Use when the fluid is commonly present on surfaces |

Do not use this section to define how the property is perceived. Perception belongs to the Sensory Layer.

---

## Common Activation Processes

Activation processes should be referenced, not defined here.

| Activation Process | Relationship | Notes |
|---|---|---|
| Activation Profile | Produces / Releases / Moves / Alters / Exposes | Defined in Activation Layer |

---

## Expressive Layer Hooks

Fluid entities may later be interpreted downstream.

| Future Record | Purpose |
|---|---|
| Fluid Name Sensory Profile | Perception of fluid qualities |
| Fluid Name Symbolic Profile | Symbolic associations and meaning |
| Fluid Name Emotional Profile | Emotional context or affective charge |
| Fluid Name Term Register | Authorial language rules |
| Fluid Name Corpus Annotations | Usage across works |

---

## Boundary Rules

Do not include:

- local anatomical placement beyond common source/output references
- activation mechanics
- sensory pleasure or discomfort
- symbolic meaning
- emotional interpretation
- authorial language
- corpus examples

---

## Relationship Statements

Use controlled relationship language.

```text
Fluid Name IS_FLUID_ENTITY
Fluid Name HAS_COMMON_SOURCE Anatomical Node
Fluid Name HAS_COMMON_OUTPUT_SITE Anatomical Node
Fluid Name HAS_FLUID_PROPERTY Fluid Property
Fluid Name MAY_BE_PRODUCED_BY Activation Profile
Fluid Name MAY_BE_REFERENCED_BY Anatomical Node Fluid Profile
```

---

## Review Questions

1. Is this fluid cross-embodiment or embodiment-specific?
2. Is the fluid entity being defined separately from local anatomical profiles?
3. Are activation mechanics excluded from this node?
4. Are sensory and symbolic meanings excluded from this node?
5. Should this fluid be atomic, composite, or a category containing sub-fluids?
6. Does this fluid require embodiment-specific variants?
7. Are fluid properties referenced as property nodes rather than redefined locally?

---

## Status

Draft v0.2.

This template should be validated before fluid entities are populated broadly. It now uses the `Fluid Properties` wikilink pattern used by the current Cervical Mucus and Paraurethral Glandular Fluid validation nodes.
