---
tags:
  - Template/Translation
  - Template/Mirror Profile
  - Status/Draft
aliases:
  - Mirror Profile Template
  - Mirror Relationship Template
title: Mirror Profile Template
file_class: Template
template_type: Translation
node_type: Mirror Profile
layer: Mirror Layer
status: Draft
version: 0.5
last_updated: 2026-06-30
---

# Mirror Profile Template

## Purpose

This template defines reusable mirror profile nodes in the Somatic Meaning Engine.

A mirror profile defines a governed correspondence between two or more ontology objects. It does not redefine the objects being mirrored.

---

## Architectural Rule

Mirror profiles describe correspondence.

They do not define anatomy, activation mechanics, fluid behaviour, sensory experience, symbolic meaning, authorial language, or corpus usage.

```text
Mirror Profile
= correspondence record

Mirrored Object
= ontology object referenced by the mirror
```

A single mirror profile may be bidirectional, directional, or contextual. Do not create duplicate inverse mirror files unless the inverse relationship has a different correspondence basis, different layer boundary, or different governance rule.

---

## Lightweight Routing Rule

Mirror profiles may include lightweight routing hints so the graph can prioritize plausible routes.

Routing hints are not activation mechanics and not expressive interpretation.

```text
Mirror Layer may rank plausible correspondence routes.
Mirror Layer must not define when, how strongly, or with what felt meaning those routes activate.
```

Use routing hints to answer:

```text
Is this mirror a likely route?
Is this mirror usually primary or secondary?
Does this mirror depend on activation, expressive framing, or corpus use?
```

Do not use routing hints to answer:

```text
What causes the response?
How intense is the response?
How is it felt?
What does it mean symbolically?
How should it be written?
```

Those belong to Activation, Expressive, Symbolic, Authorial, and Corpus layers.

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

## Descendant Mirror Candidate Rule

Composite-first mirror profiles may name possible descendant mirrors without creating them immediately.

This allows the graph to preserve future routes while avoiding unnecessary node proliferation.

Examples:

```text
Female - Nipples ↔ Female - Vaginal Canal
Female - Nipples ↔ Female - Anus
Female - Areolae ↔ Female - Vestibule
Female - Breast Skin ↔ Female - Vulva
```

These candidate descendant mirrors should become standalone mirror profiles only when a downstream activation, sensory, symbolic, authorial, or corpus use makes the narrower correspondence independently meaningful.

Use canonical anatomical names for candidate mirrors. For example, use `Female - Vaginal Canal` rather than informal wording such as vaginal tunnel.

---

## File Naming Rule

Mirror profile nodes should use the pattern:

```text
Source Object to Target Object Mirror Profile.md
```

The source and target in the filename identify the authored record, not necessarily a one-way relationship.

Examples:

```text
Female - Vulva to Female - Clitoral Complex Mirror Profile.md
Female - Clitoral Complex to Female - Breasts Mirror Profile.md
Female - Vulva to Female - Anus Mirror Profile.md
```

---

## YAML Pattern

```yaml
---
tags:
  - Ontology Node
  - Mirror Layer
  - Mirror Profile
  - Status/Draft
title: Source Object to Target Object Mirror Profile
file_class: Ontology Node
node_type: Mirror Profile
layer: Mirror Layer
status: Draft
version: 0.1
mirror_type: Anatomical / Functional / Sensory-Adjacent / Symbolic / Relational / Inversion / Echo / Contrast / Boundary
source_object: Source Object
target_object: Target Object
directionality: Bidirectional / Source-to-Target / Target-to-Source / Contextual
inverse_profile_required: true / false
anchor_level: Composite / Atomic / Mixed / Contextual
child_traversal_allowed: true / false
descendant_mirror_candidates: true / false
baseline_mirror_likelihood: High / Moderate / Low / Contextual / Unknown
activation_dependency: Independent / Activation-Dependent / Expressive-Dependent / Corpus-Dependent / Unknown
traversal_priority: Primary / Secondary / Tertiary / Candidate / Unknown
validation_status: Supported / Candidate / Blocked
---
```

---

# Source Object to Target Object Mirror Profile

## Purpose

This node defines a mirror relationship between `Source Object` and `Target Object`.

It records the basis of correspondence without redefining either object.

---

## Mirror Classification

| Field | Value |
|---|---|
| Node Type | Mirror Profile |
| Layer | Mirror Layer |
| Mirror Type | Anatomical / Functional / Sensory-Adjacent / Symbolic / Relational / Inversion / Echo / Contrast / Boundary |
| Source Object | [[Source Object]] |
| Target Object | [[Target Object]] |
| Directionality | Bidirectional / Source-to-Target / Target-to-Source / Contextual |
| Inverse Profile Required | true / false |
| Anchor Level | Composite / Atomic / Mixed / Contextual |
| Child Traversal Allowed | true / false |
| Descendant Mirror Candidates | true / false |
| Baseline Mirror Likelihood | High / Moderate / Low / Contextual / Unknown |
| Activation Dependency | Independent / Activation-Dependent / Expressive-Dependent / Corpus-Dependent / Unknown |
| Traversal Priority | Primary / Secondary / Tertiary / Candidate / Unknown |
| Validation Status | Supported / Candidate / Blocked |

---

## Routing Hints

Use this section to give the graph enough guidance to prioritize traversal without defining activation or expressive experience.

| Field | Value | Boundary |
|---|---|---|
| Baseline Mirror Likelihood | High / Moderate / Low / Contextual / Unknown | Plausibility of mirror route only |
| Activation Dependency | Independent / Activation-Dependent / Expressive-Dependent / Corpus-Dependent / Unknown | Points to dependency, does not define mechanism |
| Traversal Priority | Primary / Secondary / Tertiary / Candidate / Unknown | Graph priority, not intensity |

---

## Directionality Rule

Mirror profiles must explicitly state directionality.

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

Do not create an inverse mirror profile if `directionality: Bidirectional` and `inverse_profile_required: false`.

Create an inverse profile only if the reverse traversal has a meaningfully different structure, governance rule, or correspondence basis.

---

## Correspondence Basis

Describe the neutral basis of correspondence.

Examples:

```text
shared tissue sensitivity
paired boundary role
structural adjacency
functional echo
surface-to-surface relationship
inside/outside contrast
front/back contrast
central/peripheral contrast
focal-site to focal-site correspondence
composite-to-composite correspondence
composite-to-component correspondence
```

---

## Hierarchy-Level Check

Mirror profiles should compare objects at the highest useful hierarchy level.

Examples:

```text
Clitoral Complex ↔ Breasts
= broad composite-to-composite mirror with child traversal allowed

Clitoral Glans ↔ Nipples
= focal anatomical site to focal anatomical site mirror, used only if lower-level correspondence is independently meaningful

Vulva ↔ Anus
= external pelvic site to external pelvic site boundary mirror
```

If hierarchy levels are mismatched, explain why the mismatch is useful or choose a cleaner composite anchor.

---

## Child Traversal

Use this section when the primary mirror anchors are composite nodes.

| Side | Child Node | Traversal Role | Notes |
|---|---|---|---|
| Source | [[Source Child Node]] | Candidate child traversal | Does not redefine mirror anchor |
| Target | [[Target Child Node]] | Candidate child traversal | Does not redefine mirror anchor |

Child traversal identifies likely lower-level nodes that may participate in downstream activation, sensory, symbolic, authorial, or corpus work.

It does not create separate mirror profiles unless those lower-level correspondences become independently meaningful.

---

## Descendant Mirror Candidates

Use this section to list possible child or descendant mirror routes that may later become standalone mirror profiles.

| Candidate Mirror | Basis | Baseline Likelihood | Traversal Priority | Status | Notes |
|---|---|---|---|---|---|
| [[Source Child Node]] to [[Target Child Node]] | Candidate basis | Contextual | Candidate | Candidate | Do not create until independently needed |

Candidate descendant mirrors should preserve traversal possibilities without overbuilding the Mirror Layer.

---

## Included Layers

List layers this mirror may reference without redefining them.

| Layer | Referenced Object | Role |
|---|---|---|
| Canonical Embodiment | [[Object]] | Mirrored object |
| Fluid Layer | [[Object]] | Candidate downstream relationship |
| Activation Layer | [[Object]] | Candidate downstream relationship |
| Expressive Layer | [[Object]] | Candidate downstream relationship |
| Authorial Systems | [[Object]] | Candidate downstream use |
| Corpus | [[Object]] | Candidate annotation use |

---

## Excluded Interpretations

State what this mirror does not claim.

Examples:

```text
This mirror does not claim anatomical equivalence.
This mirror does not define activation behaviour.
This mirror does not define sensory pleasure or discomfort.
This mirror does not define symbolic meaning.
This mirror does not create authorial language rules.
This mirror does not define intensity, felt meaning, or narrative effect.
```

---

## Candidate Downstream Uses

| Future Record | Purpose |
|---|---|
| Activation Mirror Mapping | May define when this mirror is activated and with what strength |
| Sensory Profile | May reference mirrored sensory correspondence |
| Symbolic Profile | May reference mirrored symbolic correspondence |
| Activation Profile | May reference coordinated activation or response |
| Authorial Register | May govern language use of the mirror |
| Corpus Annotation | May record use in a work |

---

## Relationship Statements

Use controlled relationship language.

```text
Source Object to Target Object Mirror Profile MIRRORS Source Object
Source Object to Target Object Mirror Profile MIRRORS Target Object
Source Object to Target Object Mirror Profile HAS_MIRROR_TYPE Mirror Type
Source Object to Target Object Mirror Profile HAS_DIRECTIONALITY Directionality
Source Object to Target Object Mirror Profile HAS_ANCHOR_LEVEL Anchor Level
Source Object to Target Object Mirror Profile ALLOWS_CHILD_TRAVERSAL true / false
Source Object to Target Object Mirror Profile HAS_DESCENDANT_MIRROR_CANDIDATES true / false
Source Object to Target Object Mirror Profile HAS_BASELINE_MIRROR_LIKELIHOOD Likelihood
Source Object to Target Object Mirror Profile HAS_ACTIVATION_DEPENDENCY Dependency
Source Object to Target Object Mirror Profile HAS_TRAVERSAL_PRIORITY Priority
Source Object to Target Object Mirror Profile HAS_CORRESPONDENCE_BASIS Basis
Source Object to Target Object Mirror Profile MAY_SUPPORT Expressive Profile
```

---

## Review Questions

1. Are both mirrored objects already valid ontology nodes?
2. Is the mirror anchored at the highest useful composite level?
3. Is child traversal needed?
4. Are descendant mirror candidates useful, or would they overbuild the layer?
5. Is the mirror anatomical, functional, sensory-adjacent, symbolic, relational, contrastive, or boundary-based?
6. Is directionality explicit?
7. Is an inverse profile actually required, or does directionality solve it?
8. Are routing hints lightweight enough, or have they crossed into Activation or Expressive layers?
9. Are the mirrored objects at compatible hierarchy levels?
10. Does this mirror accidentally redefine anatomy or meaning?
11. Does this mirror require candidate downstream profiles before baseline?

---

## Status

Draft v0.5.

This template should be validated with a small mirror profile set before being marked Baseline.
