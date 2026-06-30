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
version: 0.1
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

---

## File Naming Rule

Mirror profile nodes should use the pattern:

```text
Source Object to Target Object Mirror Profile.md
```

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
mirror_type: Anatomical / Functional / Sensory / Symbolic / Relational / Inversion / Echo / Contrast / Boundary
source_object: Source Object
target_object: Target Object
directionality: Bidirectional / Source-to-Target / Target-to-Source / Contextual
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
| Mirror Type | Anatomical / Functional / Sensory / Symbolic / Relational / Inversion / Echo / Contrast / Boundary |
| Source Object | [[Source Object]] |
| Target Object | [[Target Object]] |
| Directionality | Bidirectional / Source-to-Target / Target-to-Source / Contextual |
| Validation Status | Supported / Candidate / Blocked |

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
```

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
```

---

## Candidate Downstream Uses

| Future Record | Purpose |
|---|---|
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
Source Object to Target Object Mirror Profile HAS_CORRESPONDENCE_BASIS Basis
Source Object to Target Object Mirror Profile MAY_SUPPORT Expressive Profile
```

---

## Review Questions

1. Are both mirrored objects already valid ontology nodes?
2. Is the mirror anatomical, functional, sensory, symbolic, relational, contrastive, or boundary-based?
3. Is directionality clear?
4. Does this mirror accidentally redefine anatomy or meaning?
5. Does this mirror require candidate downstream profiles before baseline?

---

## Status

Draft v0.1.

This template should be validated with a small mirror profile set before being marked Baseline.
