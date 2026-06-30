---
tags:
  - Document/Index
  - Layer/Mirror
  - Mirror Profiles
  - Status/Draft
title: Mirror Profiles Index
file_class: Document
document_type: Index
layer: Mirror Layer
status: Draft
version: 0.5
last_updated: 2026-06-30
---

# Mirror Profiles Index

## Purpose

This index lists mirror profile nodes in the Mirror Layer.

Mirror profiles define governed correspondences between ontology objects without redefining the objects being mirrored.

## Validation Set

| Mirror Profile | Mirror Type | Directionality | Anchor Level | Child Traversal | Baseline Likelihood | Activation Dependency | Traversal Priority | Status |
|---|---|---|---|---|---|---|---|---|
| [[Female - Vulva to Female - Clitoral Complex Mirror Profile]] | Anatomical / Functional | Contextual | Mixed | true | High | Contextual | Primary | Draft v0.2 |
| [[Female - Clitoral Complex to Female - Breasts Mirror Profile]] | Anatomical / Sensory-Adjacent | Bidirectional | Composite | true | Moderate | Activation-Dependent | Primary | Draft v0.4 |
| [[Female - Vulva to Female - Anus Mirror Profile]] | Boundary / Anatomical-Adjacent | Bidirectional | Mixed | true | Moderate | Contextual | Primary | Draft v0.2 |

## Composite-First Rule

Mirror profiles should usually anchor at the highest meaningful composite node that contains the mirror field.

This avoids prematurely reducing a mirror to one atomic child when multiple child structures may participate downstream.

```text
Female - Clitoral Complex ↔ Female - Breasts
= preferred composite-first mirror

Female - Clitoral Glans ↔ Female - Nipples
= possible future child-level mirror only if independently needed
```

## Descendant Mirror Candidate Rule

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

## Directionality Rule

Mirror profiles must state directionality.

A bidirectional mirror does not require a duplicate inverse file.

```text
Bidirectional
= either traversal direction is valid using the same correspondence basis

Source-to-Target
= traversal is primarily valid from source to target

Target-to-Source
= traversal is primarily valid from target to source

Contextual
= traversal depends on activation, expressive, authorial, or corpus context
```

## Lightweight Routing Rule

Mirror profiles may include lightweight routing hints so the graph can prioritize plausible routes.

```text
Mirror Layer may rank plausible correspondence routes.
Mirror Layer must not define when, how strongly, or with what felt meaning those routes activate.
```

Routing hints currently used:

```text
baseline_mirror_likelihood
activation_dependency
traversal_priority
```

## Governance Notes

Mirror profiles should preserve the following rules:

```text
mirror does not redefine anatomy
mirror does not initiate activation
mirror does not create symbolic meaning by itself
mirror does not authorialize language
mirror supports traversal without collapsing layers
mirror may guide route priority without defining response intensity
```

## Validation Notes

The first validation set intentionally stays close to canonical anatomy.

It tests:

```text
composite-to-component correspondence
composite-to-composite correspondence with child traversal
external pelvic boundary correspondence
explicit directionality
lightweight routing hints
```

## Status

Draft v0.5.
