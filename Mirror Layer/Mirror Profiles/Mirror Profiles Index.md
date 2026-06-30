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
version: 0.4
last_updated: 2026-06-30
---

# Mirror Profiles Index

## Purpose

This index lists mirror profile nodes in the Mirror Layer.

Mirror profiles define governed correspondences between ontology objects without redefining the objects being mirrored.

## Validation Set

| Mirror Profile | Mirror Type | Directionality | Anchor Level | Child Traversal | Source | Target | Status |
|---|---|---|---|---|---|---|---|
| [[Female - Vulva to Female - Clitoral Complex Mirror Profile]] | Anatomical / Functional | Contextual | Mixed | true | [[Female - Vulva]] | [[Female - Clitoral Complex]] | Draft v0.1 |
| [[Female - Clitoral Complex to Female - Breasts Mirror Profile]] | Anatomical / Sensory-Adjacent | Bidirectional | Composite | true | [[Female - Clitoral Complex]] | [[Female - Breasts]] | Draft v0.2 |
| [[Female - Vulva to Female - Anus Mirror Profile]] | Boundary / Anatomical-Adjacent | Bidirectional | Composite / Atomic | true | [[Female - Vulva]] | [[Female - Anus]] | Draft v0.1 |

## Composite-First Rule

Mirror profiles should usually anchor at the highest meaningful composite node that contains the mirror field.

This avoids prematurely reducing a mirror to one atomic child when multiple child structures may participate downstream.

```text
Female - Clitoral Complex ↔ Female - Breasts
= preferred composite-first mirror

Female - Clitoral Glans ↔ Female - Nipples
= possible future child-level mirror only if independently needed
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

## Governance Notes

Mirror profiles should preserve the following rules:

```text
mirror does not redefine anatomy
mirror does not initiate activation
mirror does not create symbolic meaning by itself
mirror does not authorialize language
mirror supports traversal without collapsing layers
```

## Validation Notes

The first validation set intentionally stays close to canonical anatomy.

It tests:

```text
composite-to-component correspondence
composite-to-composite correspondence with child traversal
external pelvic boundary correspondence
explicit directionality
```

## Status

Draft v0.4.
