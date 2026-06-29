---
tags:
  - Document/Index
  - Templates/Translation
  - Status/Draft
title: Translation Templates Index
file_class: Document
document_type: Index
status: Draft
last_updated: 2026-06-29
---

# Translation Templates Index

## Purpose

This index lists reusable templates for translation-layer records.

Translation-layer records link canonical anatomical anchors to fluid, activation, propagation, mirror, sensory, or other downstream systems without redefining canonical anatomy.

## Templates

| Template | Purpose | Status |
|---|---|---|
| [[Fluid Entity Template]] | Defines reusable fluid entities independent of one anatomical site. | Draft v0.1 |
| [[Fluid Profile Template]] | Defines local relationships between canonical anatomical anchors and reusable fluid entities. | Draft v0.3 |

## Fluid Architecture Rule

Fluid modelling now uses a two-part structure:

```text
Fluid Entity
= what the fluid is

Fluid Profile
= how that fluid relates to a specific anatomical anchor
```

Activation profiles will later describe processes that produce, release, move, expose, withhold, or alter one or more fluid entities across one or more anatomical sites.

## Validation Plan

The Fluid Entity Template and Fluid Profile Template should be validated together before either is marked Baseline.

Recommended validation entities:

```text
Tears
Urine
Menstrual Fluid
Vaginal Fluid
Milk
Blood
Sweat
Saliva
```

Recommended validation profiles:

```text
Female - Vulva Fluid Profile
Female - Vaginal Canal Fluid Profile
Female - Skene's Glands Fluid Profile
Female - Breasts Fluid Profile
```

This should test direct, adjacent, conditional, cyclical, glandular-source, cross-body, and multi-site fluid relationships.
