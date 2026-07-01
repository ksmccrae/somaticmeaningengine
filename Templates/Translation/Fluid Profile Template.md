---
tags:
  - Template/Translation
  - Template/Fluid Profile
  - Status/Validated
aliases:
  - Fluid Profile Template
  - Fluid Layer Profile Template
title: Fluid Profile Template
file_class: Template
template_type: Translation
node_type: Fluid Profile
layer: Fluid Layer
status: Validated
version: 0.4
last_updated: 2026-06-30
---

# Fluid Profile Template

## Purpose

This template defines the required structure for anatomical fluid profile nodes in the Somatic Meaning Engine.

A fluid profile describes how one or more reusable fluid entities relate to a canonical anatomical anchor.

It does not define the fluid entity itself, redefine anatomy, define sensory experience, define symbolic meaning, define activation behaviour, define propagation behaviour, define authorial language, or describe corpus usage.

---

## Architectural Rule

Fluid profiles are relationship records.

They sit between canonical anatomy and reusable fluid entities.

```text
Fluid Entity
= what the fluid is

Anatomical Fluid Profile
= how one or more fluids relate to a local anatomical anchor

Activation Profile
= what process produces, moves, releases, exposes, withholds, or alters fluid across one or more anatomical sites
```

A fluid profile may reference multiple fluid entities.

A fluid entity may appear in multiple fluid profiles.

An activation profile may involve multiple anatomical sites and multiple fluid entities.

---

## Layer Boundary

Fluid profiles may describe local observable or physiologically grounded fluid qualities only where those qualities are specific to the anatomical relationship.

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

It links to the canonical anatomical node and reusable fluid entities without redefining either.

---

## Anatomical Anchor

| Field | Value |
|---|---|
| Anatomical Anchor | [[Embodiment - Anatomical Node]] |
| Anchor Layer | Canonical Embodiment |
| Fluid Layer Role | Present / Conditional / Adjacent / None |

---

## Referenced Fluid Entities

List fluid entities referenced by this anatomical profile.

| Fluid Entity | Relationship To Anchor | Notes |
|---|---|---|
| [[Fluid Entity]] | Produces / Stores / Conducts / Receives / Surface Presence / Adjacent / Output Site | Neutral relationship note only |

Only reference reusable fluid entity nodes here. Do not define the fluid entity inside the anatomical profile.

---

## Fluid Relationship Type

Describe the type of relationship between the anatomical anchor and each referenced fluid entity without using symbolic, sensory, or authorial language.

| Relationship Type | Description |
|---|---|
| Produces | The anatomical anchor produces or secretes a referenced fluid entity |
| Stores | The anatomical anchor stores a referenced fluid entity |
| Conducts | The anatomical anchor conducts a referenced fluid entity from another structure |
| Receives | The anatomical anchor receives or contains a referenced fluid entity from another structure |
| Output Site | A referenced fluid exits or becomes externally present at this anatomical anchor |
| Surface Presence | A referenced fluid is present on or across the anatomical surface |
| Cyclical | The relationship varies through hormonal or reproductive cycles |
| Contextual | The relationship appears only under specific physiological conditions |
| Adjacent | The fluid belongs to a nearby structure rather than this anchor directly |
| None | No meaningful fluid relationship at current modelling resolution |

---

## Anatomical Sources, Conduits, and Output Sites

Separate source, pathway, and output relationships so fluids are not incorrectly assigned to nearby external structures.

| Role | Anatomical Node | Fluid Entity | Notes |
|---|---|---|---|
| Source | [[Embodiment - Source Node]] | [[Fluid Entity]] | Produces or stores the fluid |
| Conduit | [[Embodiment - Conduit Node]] | [[Fluid Entity]] | Conducts the fluid |
| Output Site | [[Embodiment - Output Node]] | [[Fluid Entity]] | External or surface site where fluid appears |
| Adjacent Site | [[Embodiment - Adjacent Node]] | [[Fluid Entity]] | Nearby but not source or primary conduit |

---

## Local Fluid Qualities

Use this section for neutral observable or physiologically grounded properties only when those qualities are specific to the anatomical relationship.

Do not describe subjective experience here.

| Fluid Entity | Quality | Range / Description | Notes |
|---|---|---|---|
| [[Fluid Entity]] | Viscosity | Thin / watery / thick / variable | Neutral description only |
| [[Fluid Entity]] | Density | Low / moderate / high / variable | Use only if meaningful at this modelling resolution |
| [[Fluid Entity]] | Colour | Clear / white / yellow / red / brown / variable | Neutral description only |
| [[Fluid Entity]] | Opacity | Clear / translucent / opaque / variable | Neutral description only |
| [[Fluid Entity]] | Odour | None / mild / strong / variable | Neutral description only |
| [[Fluid Entity]] | Taste | Neutral / saline / metallic / bitter / variable | Use only where relevant and not authorialized |
| [[Fluid Entity]] | Volume | Trace / low / moderate / high / variable | Neutral description only |
| [[Fluid Entity]] | Flow | Static / surface / discharge / stream / cyclical / variable | Neutral description only |
| [[Fluid Entity]] | Cyclicity | None / cyclical / hormonal / reproductive / contextual | Neutral description only |

---

## Activation Hooks

Use this section to reference likely activation profiles without defining activation mechanics.

| Activation Profile | Fluid Entity | Role |
|---|---|---|
| Activation Profile | [[Fluid Entity]] | Produces / Releases / Moves / Withholds / Alters / Exposes |

Activation profiles may involve multiple anatomical sites and multiple fluid entities.

---

## Boundary Rules

Clarify what this fluid profile must not include.

Do not include:

- definitions of the fluid entity itself
- sensory pleasure or discomfort
- erotic terminology
- symbolic meaning
- emotional associations
- activation mechanics
- propagation routes
- authorial usage
- corpus examples

---

## Relationship Statements

Use controlled relationship language.

```text
Embodiment - Anatomical Node Fluid Profile DESCRIBES_FLUID_RELATIONSHIPS_OF Embodiment - Anatomical Node
Embodiment - Anatomical Node Fluid Profile REFERENCES_FLUID_ENTITY Fluid Entity
Embodiment - Anatomical Node Fluid Profile REFERENCES_FLUID_SOURCE Embodiment - Source Node
Embodiment - Anatomical Node Fluid Profile REFERENCES_FLUID_CONDUIT Embodiment - Conduit Node
Embodiment - Anatomical Node Fluid Profile REFERENCES_FLUID_OUTPUT_SITE Embodiment - Output Node
Embodiment - Anatomical Node Fluid Profile MAY_BE_CHANGED_BY Activation Profile
```

---

## Candidate Downstream Links

Use this section to identify likely future records without defining them here.

| Future Record | Purpose |
|---|---|
| Embodiment - Anatomical Node Activation Profile | Activation behaviour involving fluid changes |
| Fluid Entity Sensory Profile | Sensory perception of fluid qualities |
| Fluid Entity Symbolic Profile | Symbolic meaning attached to the fluid entity |
| Fluid Entity Term Register | Authorial terminology and language constraints |
| Fluid Entity Corpus Annotations | Story, song, essay, or research usage |

---

## Review Questions

Use this section to capture unresolved ontology questions before the node becomes canonical.

1. Is the fluid relationship direct, adjacent, conditional, cyclical, or absent?
2. Does this profile accidentally redefine anatomy from the canonical anchor?
3. Does this profile accidentally define the fluid entity rather than referencing it?
4. Does this profile accidentally include activation mechanics, sensory perception, symbolic meaning, or authorial material?
5. Are source, conduit, output site, and adjacent site separated clearly?
6. Should this profile exist for this anatomical anchor, or should fluid relationships be inherited from a parent node?
7. Are fluid qualities neutral and observable, or have they crossed into sensory interpretation?
8. Does this profile support multi-site, multi-fluid activation events?

---

## Validation Result

Validated against the current Female Fluid Profile validation set:

```text
Female - Vulva Fluid Profile
Female - Vaginal Canal Fluid Profile
Female - Skene's Glands Fluid Profile
Female - Breasts Fluid Profile
```

Validation confirmed:

```text
expected YAML fields present in checked profile nodes
expected sections present across validation set
profiles reference Fluid Entities rather than defining them locally
Cervical Mucus and Paraurethral Glandular Fluid are treated as existing Fluid Entity nodes, not candidate-only placeholders
Surface Moisture remains governed as a relationship/property state by default unless mixed, nonspecific, accumulated, transferred, or independently reusable
source, conduit, output site, surface presence, and adjacency are separated in live profiles
activation hooks are referenced but not defined
profiles do not redefine canonical anatomy, fluid entities, activation mechanics, sensory experience, symbolic meaning, authorial language, or corpus usage
no mechanical drift found in the checked validation set
```

This template is validated for continued construction use. It is not yet Baseline.

---

## Baseline Blockers

Before this template can be marked Baseline, resolve or formally defer:

```text
Whether all current Fluid Profile nodes should be individually audited again before Baseline.
Which additional anatomical anchors require Fluid Profiles before the layer is stable.
Whether Surface Moisture remains a relationship/property state or eventually becomes one or more standalone Fluid Entities.
Which activation profiles must exist before Fluid Profile modelling is stable.
Whether local fluid qualities should wikilink Fluid Property nodes in profile files or remain plain neutral descriptors.
Whether profile relationship statements need additional controlled verbs for adjacent output sites and adjacent surface presence.
Which cross-embodiment, trans feminine, trans masculine, male, or non-sex-specific profiles are needed before Baseline.
```

---

## Status

Validated v0.4.

This template is validated against the current Fluid Profile validation set and remains pre-Baseline pending governance resolution or formal deferral.
