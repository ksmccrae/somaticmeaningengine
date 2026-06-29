---
tags:
  - Template/Canonical
  - Template/Anatomical Site
  - Status/Draft
aliases:
  - Anatomical Site Template
  - Canonical Anatomical Site Template
title: Anatomical Site Template
file_class: Template
template_type: Canonical
node_type: Anatomical Site
layer: Canonical Embodiment
status: Draft
version: 0.1
last_updated: 2026-06-29
---

# Anatomical Site Template

## Purpose

This template defines the required structure for canonical anatomical site nodes in the Somatic Meaning Engine.

An anatomical site node defines anatomical existence, placement, containment, boundaries, and canonical relationships.

It does not define sensory experience, symbolic meaning, authorial language, activation behaviour, propagation behaviour, or corpus usage. Those belong to downstream layers.

---

## File Naming Rule

Anatomical site nodes should use the pattern:

```text
Embodiment - Anatomical Node.md
```

Examples:

```text
Female - Vulva.md
Female - Nipple.md
Male - Nipple.md
Trans Feminine - Chest.md
Trans Masculine - Pelvic Floor.md
```

---

## YAML Pattern

```yaml
---
tags:
  - Ontology Node
  - Canonical Embodiment
  - Anatomical Site
  - Status/Draft
aliases:
  - Alternate Name
title: Embodiment - Anatomical Node
canonical_name: Anatomical Node
file_class: Ontology Node
node_type: Anatomical Site
layer: Canonical Embodiment
embodiment_scope: Embodiment
classification: Composite Anatomical Node
status: Draft
version: 0.1
parent: Embodiment - Parent Node
paired: false
distributed: false
transitional: false
---
```

---

# Embodiment - Anatomical Node

## Purpose

This node defines `[Anatomical Node]` as a canonical anatomical site within `[Embodiment]` Embodiment.

It exists to describe anatomical structure, containment relationships, boundaries, and canonical placement in the Somatic Meaning Engine.

This node does not define activation, sensory register, somatic experience, symbolic meaning, authorial usage, or corpus annotation.

---

## Canonical Definition

Define the anatomical site in clear, neutral, canonical language.

The definition should answer:

- What is this structure?
- Where does it belong anatomically?
- What structures does it contain, border, or organize?
- What should it not be confused with?

---

## Ontological Classification

| Field | Value |
|---|---|
| Node Type | Anatomical Site |
| Classification | Composite / Atomic / Distributed / Transitional |
| Layer | Canonical Embodiment |
| Embodiment Scope | Embodiment |
| Parent | Embodiment - Parent Node |
| Region | Embodiment - Region |
| External / Internal | External / Internal / Mixed |
| Paired | true / false |
| Distributed | true / false |
| Transitional | true / false |

---

## Parent Relationships

```text
Embodiment - Anatomical Node BELONGS_TO Embodiment - Parent Node
Embodiment - Parent Node BELONGS_TO Embodiment - Region
Embodiment - Region BELONGS_TO Embodiment Root
```

---

## Child Structures

Use this section when the anatomical site is composite.

| Child Structure | Proposed Node | Classification |
|---|---|---|
| Child Structure | [[Embodiment - Child Structure]] | Composite / Atomic / Review |

If the node is atomic, state:

```text
This node has no child structures at the current modelling resolution.
```

---

## Containment Relationships

Use this section when the node contains or organizes child structures.

```text
Embodiment - Anatomical Node CONTAINS Embodiment - Child Structure
```

If containment is not appropriate, use a controlled relationship more suited to the anatomical relationship once approved.

---

## Boundary Notes

Describe nearby or easily confused structures.

| Nearby Structure | Distinction |
|---|---|
| [[Embodiment - Nearby Structure]] | How this structure differs from the current node |

---

## Anatomical Notes

Use this section for canonical anatomical clarification only.

Do not include:

- sensory response
- erotic or authorial language
- symbolic meaning
- emotional associations
- propagation patterns
- mirror behaviour
- corpus usage

---

## Layer Separation

The following concerns are intentionally excluded from canonical anatomical nodes and should be modelled in later layers.

| Concern | Target Layer |
|---|---|
| Sensory response | Sensory Layer |
| Somatic experience | Somatic Layer |
| Mirror relationships | Mirror Layer |
| Propagation pathways | Propagation Layer |
| Symbolic meaning | Symbolic Layer |
| Emotional associations | Emotional Layer |
| Fluid behaviour | Fluid Layer |
| Authorial terminology | Authorial Systems or Term Register |
| Corpus usage | Corpus Annotation |

---

## Candidate Downstream Links

Use this section to identify likely future records without defining them inside the canonical node.

| Future Record | Purpose |
|---|---|
| Embodiment - Anatomical Node Sensory Profile | Sensory response and tactile qualities |
| Embodiment - Anatomical Node Somatic Profile | Embodied experience and internal sensation |
| Embodiment - Anatomical Node Mirror Profile | Mirror relationships |
| Embodiment - Anatomical Node Propagation Profile | Activation movement and pathways |
| Embodiment - Anatomical Node Symbolic Profile | Symbolic or ritual associations |
| Embodiment - Anatomical Node Term Register | Allowed, restricted, and banned language |
| Embodiment - Anatomical Node Corpus Annotations | Usage across stories, songs, essays, or research |

---

## Review Questions

Use this section to capture unresolved ontology questions before the node becomes canonical.

1. Is this node Composite, Atomic, Distributed, Transitional, or a combination?
2. Does this node require child structures now, or can they wait?
3. Is pairedness a property of this node?
4. Are the parent and region relationships correct?
5. Are any downstream-layer details accidentally included in this canonical node?

---

## Status

Draft v0.1.

This node should be reviewed before being marked Canonical.
