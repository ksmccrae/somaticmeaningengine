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
version: 0.2
last_updated: 2026-06-29
---

# Fluid Profile Template

## Purpose

This template defines the required structure for fluid profile nodes in the Somatic Meaning Engine.

A fluid profile describes how bodily fluids relate to a canonical anatomical anchor.

It does not redefine anatomy, sensory experience, symbolic meaning, activation behaviour, propagation behaviour, authorial language, or corpus usage.

---

## Layer Boundary

Fluid profiles may describe observable or physiologically grounded fluid qualities.

Examples:

```text
viscosity
thickness
density
colour
opacity
odour
taste
volume
flow
cyclicity
presence / absence
```

These are treated as fluid-layer qualities when described neutrally.

The Sensory Layer describes embodied perception of those qualities, such as how wetness, dryness, thickness, odour, taste, temperature, pressure, or texture are experienced.

The Symbolic, Emotional, Authorial, and Corpus layers may interpret or use these qualities, but they should not be defined inside the fluid profile.

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

## Fluid Categories

Use this section to list relevant fluids or fluid categories without converting them into sensory, symbolic, or authorial meaning.

| Fluid Category | Relationship | Notes |
|---|---|---|
| Fluid Name | Present / Conditional / Cyclical / Adjacent | Neutral physiological note only |

Common Female Embodiment fluid categories may include:

```text
urine
menstrual fluid
vaginal fluid
cervical mucus
paraurethral glandular fluid
lactation fluid / milk
surface moisture
```

Only include categories relevant to the anatomical anchor.

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

## Fluid Qualities

Use this section for neutral observable or physiologically grounded properties of the fluid.

Do not describe subjective experience here.

| Quality | Range / Description | Notes |
|---|---|---|
| Viscosity | Thin / watery / thick / variable | Neutral description only |
| Density | Low / moderate / high / variable | Use only if meaningful at this modelling resolution |
| Colour | Clear / white / yellow / red / brown / variable | Neutral description only |
| Opacity | Clear / translucent / opaque / variable | Neutral description only |
| Odour | None / mild / strong / variable | Neutral description only |
| Taste | Neutral / saline / metallic / bitter / variable | Use only where relevant and not authorialized |
| Volume | Trace / low / moderate / high / variable | Neutral description only |
| Flow | Static / surface / discharge / stream / cyclical / variable | Neutral description only |
| Cyclicity | None / cyclical / hormonal / reproductive / contextual | Neutral description only |

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
Embodiment - Anatomical Node Fluid Profile HAS_FLUID_CATEGORY Fluid Category
Embodiment - Anatomical Node Fluid Profile HAS_FLUID_QUALITY Fluid Quality
```

---

## Candidate Downstream Links

Use this section to identify likely future records without defining them here.

| Future Record | Purpose |
|---|---|
| Embodiment - Anatomical Node Activation Profile | Activation behaviour involving fluid changes |
| Embodiment - Anatomical Node Sensory Profile | Sensory experience of moisture, pressure, dryness, smell, taste, or texture |
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
6. Are fluid qualities neutral and observable, or have they crossed into sensory interpretation?
7. Are urine and menstrual fluid represented where relevant without collapsing urinary and reproductive systems into the same node?

---

## Status

Draft v0.2.

This template should be validated against a small set of Female genital and breast anatomical nodes before being marked Baseline.
