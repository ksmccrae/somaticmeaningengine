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
version: 0.3
last_updated: 2026-06-30
---

# Mirror Profiles Index

## Purpose

This index lists mirror profile nodes in the Mirror Layer.

Mirror profiles define governed correspondences between ontology objects without redefining the objects being mirrored.

## Validation Set

| Mirror Profile | Mirror Type | Directionality | Source | Target | Status |
|---|---|---|---|---|---|
| [[Female - Vulva to Female - Clitoral Complex Mirror Profile]] | Anatomical / Functional | Contextual | [[Female - Vulva]] | [[Female - Clitoral Complex]] | Draft v0.1 |
| [[Female - Clitoral Glans to Female - Nipples Mirror Profile]] | Anatomical / Sensory-Adjacent | Bidirectional | [[Female - Clitoral Glans]] | [[Female - Nipples]] | Draft v0.1 |
| [[Female - Vulva to Female - Anus Mirror Profile]] | Boundary / Anatomical-Adjacent | Bidirectional | [[Female - Vulva]] | [[Female - Anus]] | Draft v0.1 |

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
focal-site to focal-site correspondence
external pelvic boundary correspondence
explicit directionality
```

## Status

Draft v0.3.
