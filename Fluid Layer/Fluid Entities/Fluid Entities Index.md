---
tags:
  - Document/Index
  - Layer/Fluid
  - Fluid Entities
  - Status/Draft
title: Fluid Entities Index
file_class: Document
document_type: Index
layer: Fluid Layer
status: Draft
version: 0.1
last_updated: 2026-06-30
---

# Fluid Entities Index

## Purpose

This index lists reusable fluid entity nodes in the Fluid Layer.

Fluid entities define fluids independently from any single anatomical site, activation event, sensory perception, symbolic meaning, authorial usage, or corpus instance.

## Validation Set

| Fluid Entity | Primary Role | Embodiment Scope | Status |
|---|---|---|---|
| [[Tears]] | Lacrimal / expressive-adjacent fluid | Cross-Embodiment | Draft v0.1 |
| [[Urine]] | Urinary fluid | Cross-Embodiment | Draft v0.1 |
| [[Menstrual Fluid]] | Reproductive / cyclical fluid | Anatomy-Dependent | Draft v0.1 |
| [[Vaginal Fluid]] | Mucosal / reproductive tract fluid | Anatomy-Dependent | Draft v0.1 |
| [[Milk]] | Lactation fluid | Conditional / Anatomy-Dependent | Draft v0.1 |
| [[Blood]] | Circulatory fluid | Cross-Embodiment | Draft v0.1 |
| [[Sweat]] | Surface / thermoregulatory fluid | Cross-Embodiment | Draft v0.1 |
| [[Saliva]] | Oral / digestive fluid | Cross-Embodiment | Draft v0.1 |

## Governance Notes

Fluid entities should be referenced by anatomical fluid profiles and activation profiles rather than redefined inside them.

```text
Fluid Entity
= what the fluid is

Fluid Profile
= how that fluid relates to an anatomical anchor

Activation Profile
= what process produces, releases, moves, exposes, withholds, or alters the fluid
```

## Review Questions

1. Should fluid entities remain in a dedicated `Fluid Entities` subfolder?
2. Should there be a separate `Fluid Profiles` subfolder for anatomical fluid profiles?
3. Should Surface Moisture be a fluid entity, a quality, or a relationship type?
4. Which entities require embodiment-specific variants?

## Status

Draft v0.1.
