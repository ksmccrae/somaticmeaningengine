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
version: 0.3
last_updated: 2026-06-30
---

# Fluid Entities Index

## Purpose

This index lists reusable fluid entity nodes in the Fluid Layer.

Fluid entities define fluids independently from any single anatomical site, activation event, sensory perception, symbolic meaning, authorial usage, or corpus instance.

## Validation Set

| Fluid Entity | Primary Role | Embodiment Scope | Status |
|---|---|---|---|
| [[Tears]] | Lacrimal / expressive-adjacent fluid | Cross-Embodiment | Draft v0.2 |
| [[Urine]] | Urinary fluid | Cross-Embodiment | Draft v0.2 |
| [[Menstrual Fluid]] | Reproductive / cyclical fluid | Anatomy-Dependent | Draft v0.2 |
| [[Vaginal Fluid]] | Mucosal / reproductive tract fluid | Anatomy-Dependent | Draft v0.2 |
| [[Cervical Mucus]] | Cervical / reproductive mucosal fluid | Anatomy-Dependent | Draft v0.1 |
| [[Paraurethral Glandular Fluid]] | Paraurethral glandular fluid | Anatomy-Dependent | Draft v0.1 |
| [[Milk]] | Lactation fluid | Conditional / Anatomy-Dependent | Draft v0.2 |
| [[Blood]] | Circulatory fluid | Cross-Embodiment | Draft v0.2 |
| [[Sweat]] | Surface / thermoregulatory fluid | Cross-Embodiment | Draft v0.2 |
| [[Saliva]] | Oral / digestive fluid | Cross-Embodiment | Draft v0.2 |

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

Fluid entities should reference fluid property nodes through `HAS_FLUID_PROPERTY` relationship statements rather than redefining property categories locally.

## Surface Moisture Note

Surface Moisture is not listed as a fluid entity by default.

Current governance treats Surface Moisture primarily as a relationship or property state unless mixed, nonspecific, accumulated, transferred, or independently reusable surface wetness requires a standalone fluid entity.

## Review Questions

1. Which entities require embodiment-specific variants?
2. Should Cervical Mucus require a dedicated Cervical Canal anatomical node before baseline?
3. Should Paraurethral Glandular Fluid require refined gland opening anatomy before baseline?
4. Should Surface Moisture remain outside the entity register for now?
5. Should all current validation entities be migrated to Draft v0.2 after confirming property-node pattern parity?

## Status

Draft v0.3.
