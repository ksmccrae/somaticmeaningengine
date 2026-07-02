---
tags:
  - Document/Index
  - Layer/Fluid
  - Fluid Properties
  - Status/Draft
title: Fluid Properties Index
file_class: Document
document_type: Index
layer: Fluid Layer
status: Draft
version: 0.3
last_updated: 2026-07-02
---

# Fluid Properties Index

## Purpose

This index lists reusable fluid property nodes in the Fluid Layer.

Fluid properties define observable, measurable, or physiologically grounded qualities that may be referenced by fluid entities or local fluid profiles.

They do not define fluid entities, anatomical sites, activation mechanics, sensory experience, symbolic meaning, authorial usage, or corpus examples.

## Property Register

| Property | Property Class | Primary Use | Status |
|---|---|---|---|
| [[Viscosity]] | Physical | Fluid Entity / Fluid Profile | Draft v0.1 |
| [[Density]] | Physical | Fluid Entity / Fluid Profile | Draft v0.1 |
| [[Colour]] | Visual | Fluid Entity / Fluid Profile | Draft v0.1 |
| [[Opacity]] | Visual | Fluid Entity / Fluid Profile | Draft v0.1 |
| [[Odour]] | Olfactory | Fluid Entity / Fluid Profile | Draft v0.1 |
| [[Taste]] | Gustatory | Fluid Entity / Fluid Profile | Draft v0.1 |
| [[Temperature]] | Thermal | Fluid Profile / Sensory Boundary | Draft v0.1 |
| [[Volume]] | Physical / Quantitative | Fluid Entity / Fluid Profile | Draft v0.1 |
| [[Flow]] | Relational / Physical | Fluid Profile / Activation Boundary | Draft v0.1 |
| [[Cyclicity]] | Temporal | Fluid Entity / Activation Boundary | Draft v0.1 |
| [[Surface Presence]] | Relational | Fluid Profile | Draft v0.1 |
| [[Coagulation State]] | Physical | Blood-containing Fluid Entity / Fluid Profile | Draft v0.1 |

## Governance Notes

Fluid properties sit between fluid entities and sensory interpretation.

```text
Colour
= fluid property

Seeing red, dark, bright, pale, alarming, beautiful, shameful, sacred, or dangerous
= sensory / symbolic / authorial interpretation depending on layer
```

Fluid properties may be referenced by fluid entities as general properties and by fluid profiles as local anatomical variations.

`Coagulation State` governs the values `Uncoagulated`, `Partially Coagulated`, and `Clotted`. `Clotted` is the terminal traversal level; clot size, frequency, morphology, and composition are not currently modelled.

## Validation Notes

The first validation set is intentionally broad enough to test physical, visual, olfactory, gustatory, thermal, temporal, and relational properties.

The next validation pass should check whether property value ranges are reusable enough across the first fluid entity set.

## Review Questions

1. Which properties require stricter governed value ranges?
2. Which properties should remain broad controlled values rather than expanding into subproperties?
3. Should Surface Presence remain a relationship property rather than a fluid entity?
4. Should Temperature and Flow be treated as activation-adjacent properties?

## Status

Draft v0.3.
