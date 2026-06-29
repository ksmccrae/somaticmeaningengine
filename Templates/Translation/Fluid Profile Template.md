---
tags:
  - Template/Translation
  - Template/Fluid Profile
  - Status/Draft
aliases:
  - Fluid Profile Template
  - Fluid Layer Profile Template
title: Fluid Profile Template
file_class: Template
template_type: Translation
node_type: Fluid Profile
layer: Fluid Layer
status: Draft
version: 0.1
last_updated: 2026-06-29
---

# Fluid Profile Template

## Purpose

This template defines the required structure for fluid profile nodes in the Somatic Meaning Engine.

A fluid profile describes how bodily fluids relate to a canonical anatomical anchor.

It does not redefine anatomy, sensory experience, symbolic meaning, activation behaviour, propagation behaviour, authorial language, or corpus usage.

---

## File Naming Rule

Fluid profile nodes should use the pattern:

```text
Embodiment - Anatomical Node Fluid Profile.md
```

Examples:

```text
Female - Vulva Fluid Profile.md
Female - Vaginal Canal Fluid Profile.md
Female - Skene's Glands Fluid Profile.md
Female - Breasts Fluid Profile.md
```

---

## YAML Pattern

```yaml
---
tags:
  - Ontology Node
  - Fluid Layer
  - Fluid Profile
  - Status/Draft
title: Embodiment - Anatomical Node Fluid Profile
file_class: Ontology Node
node_type: Fluid Profile
layer: Fluid Layer
embodiment_scope: Embodiment
status: Draft
version: 0.1
anatomical_anchor: Embodiment - Anatomical Node
canonical_layer_reference: Canonical Embodiment
fluid_relevance: Present / Conditional / Adjacent / None
---
```

---

# Embodiment - Anatomical Node Fluid Profile

## Purpose

This node defines fluid relationships associated with `Embodiment - Anatomical Node`.

It links to the canonical anatomical node without redefining anatomical structure.

---

## Anatomical Anchor

| Field | Value |
|---|---|
| Anatomical Anchor | [[Embodiment - Anatomical Node]] |
| Anchor Layer | Canonical Embodiment |
| Fluid Layer Role | Present / Conditional / Adjacent / None |

---

## Fluid Relationship Type

Describe the type of fluid relationship without using symbolic, sensory, or authorial language.

| Relationship Type | Description |
|---|---|
| Produces | The anatomical anchor produces or secretes fluid |
| Conducts | The anatomical anchor conducts fluid from another structure |
| Receives | The anatomical anchor receives or contains fluid from another structure |
| Surface Moisture | Fluid is present on or across the anatomical surface |
| Cyclical | Fluid relationship varies through hormonal or reproductive cycles |
| Contextual | Fluid relationship appears only under specific physiological conditions |
| Adjacent | Fluid belongs to a nearby structure rather than this anchor directly |
| None | No meaningful fluid relationship at current modelling resolution |

---

## Fluid Sources

List sources only when anatomically or physiologically appropriate.

| Source | Relationship | Notes |
|---|---|---|
| [[Embodiment - Source Node]] | Produces / Conducts / Receives / Adjacent | Canonical note only |

If no source applies, state:

```text
No direct fluid source is defined at the current modelling resolution.
```

---

## Fluid Outputs or Presence

Describe outputs, surface presence, or containment in neutral anatomical language.

| Fluid Presence | Relationship | Notes |
|---|---|---|
| Fluid Name | Present / Conditional / Cyclical / Adjacent | Canonical physiological note only |

---

## Boundary Rules

Clarify what this fluid profile must not include.

Do not include:

- sensory pleasure or discomfort
- erotic terminology
- symbolic meaning
- emotional associations
- activation pathways
- propagation routes
- authorial usage
- corpus examples

---

## Relationship Statements

Use controlled relationship language.

```text
Embodiment - Anatomical Node Fluid Profile DESCRIBES_FLUID_RELATIONSHIPS_OF Embodiment - Anatomical Node
Embodiment - Anatomical Node Fluid Profile REFERENCES_FLUID_SOURCE Embodiment - Source Node
```

---

## Candidate Downstream Links

Use this section to identify likely future records without defining them here.

| Future Record | Purpose |
|---|---|
| Embodiment - Anatomical Node Activation Profile | Activation behaviour involving fluid changes |
| Embodiment - Anatomical Node Sensory Profile | Sensory experience of moisture, pressure, or dryness |
| Embodiment - Anatomical Node Symbolic Profile | Symbolic meaning attached to fluid imagery |
| Embodiment - Anatomical Node Term Register | Authorial terminology and language constraints |
| Embodiment - Anatomical Node Corpus Annotations | Story, song, essay, or research usage |

---

## Review Questions

Use this section to capture unresolved ontology questions before the node becomes canonical.

1. Is the fluid relationship direct, adjacent, conditional, cyclical, or absent?
2. Does this profile accidentally redefine anatomy from the canonical anchor?
3. Does this profile accidentally include activation, sensory, symbolic, or authorial material?
4. Are fluid sources represented as anatomical nodes, fluid entities, or both?
5. Should this profile exist for this anatomical anchor, or should fluid relationships be inherited from a parent node?

---

## Status

Draft v0.1.

This template should be validated against a small set of Female genital and breast anatomical nodes before being marked Baseline.
