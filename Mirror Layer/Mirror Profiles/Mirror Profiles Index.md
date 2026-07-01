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
version: 0.8
last_updated: 2026-07-01
---

# Mirror Profiles Index

## Purpose

This index lists mirror profile nodes in the Mirror Layer.

Mirror profiles define governed correspondences between ontology objects without redefining the objects being mirrored.

## Registers

| Register | Purpose | Status |
|---|---|---|
| [[Female Mirror Candidate Register]] | Planning register for female embodiment mirror expansion | Draft v0.1 |

## Supported Validation Set

| Mirror Profile | Source Object | Target Object | Mirror Type | Directionality | Inverse Required | Anchor Level | Child Traversal | Descendant Candidates | Baseline Likelihood | Activation Dependency | Traversal Priority | Validation Status | Document Status |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| [[Female - Vulva to Female - Clitoral Complex Mirror Profile]] | [[Female - Vulva]] | [[Female - Clitoral Complex]] | Anatomical / Functional | Contextual | false | Mixed | true | false | High | Contextual | Primary | Supported | Draft v0.3 |
| [[Female - Clitoral Complex to Female - Breasts Mirror Profile]] | [[Female - Clitoral Complex]] | [[Female - Breasts]] | Anatomical / Sensory-Adjacent | Bidirectional | false | Composite | true | true | Moderate | Activation-Dependent | Primary | Supported | Draft v0.5 |
| [[Female - Vulva to Female - Anus Mirror Profile]] | [[Female - Vulva]] | [[Female - Anus]] | Boundary / Anatomical-Adjacent | Bidirectional | false | Mixed | true | true | Moderate | Contextual | Primary | Supported | Draft v0.3 |

## Female Expansion Candidate Set

These profiles use the validated Mirror Profile Template but are not yet part of the supported validation set.

| Mirror Profile | Source Object | Target Object | Mirror Type | Directionality | Inverse Required | Anchor Level | Child Traversal | Descendant Candidates | Baseline Likelihood | Activation Dependency | Traversal Priority | Validation Status | Document Status |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| [[Female - Vulva to Female - Breasts Mirror Profile]] | [[Female - Vulva]] | [[Female - Breasts]] | Anatomical / Sensory-Adjacent | Bidirectional | false | Composite | true | true | Moderate | Contextual | Primary | Candidate | Draft v0.1 |
| [[Female - Nipples to Female - Vaginal Canal Mirror Profile]] | [[Female - Nipples]] | [[Female - Vaginal Canal]] | Anatomical / Sensory-Adjacent | Contextual | false | Mixed | true | false | Moderate | Activation-Dependent | Primary | Candidate | Draft v0.1 |
| [[Female - Skene's Glands to Female - Urethral Opening Mirror Profile]] | [[Female - Skene's Glands]] | [[Female - Urethral Opening]] | Anatomical / Functional | Contextual | false | Mixed | true | false | High | Contextual | Primary | Candidate | Draft v0.1 |
| [[Female - Perineum to Female - Pelvic Floor Mirror Profile]] | [[Female - Perineum]] | [[Female - Pelvic Floor]] | Anatomical / Functional / Boundary | Bidirectional | false | Mixed | true | true | High | Activation-Dependent | Primary | Candidate | Draft v0.1 |

## Index Column Notes

`Document Status` records the file maturity and version.

`Validation Status` records whether the mirror profile is supported, candidate, or blocked.

These are intentionally separate fields and should not be collapsed.

## Controlled Mirror Types Currently Used

```text
Anatomical
Functional
Sensory-Adjacent
Boundary
Anatomical-Adjacent
```

Other controlled mirror types remain available in the framework and template but are not yet used by the validation set.

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

## Boundary Region References

Boundary region references are allowed only as traversal aids.

```text
REFERENCES_BOUNDARY_REGION
```

This relationship may identify a canonical boundary region that helps explain a mirror route, but it must not redefine anatomy.

Current use:

```text
Female - Vulva to Female - Anus Mirror Profile REFERENCES_BOUNDARY_REGION Female - Perineum
Female - Perineum to Female - Pelvic Floor Mirror Profile REFERENCES_BOUNDARY_REGION Female - Perineum
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
boundary-region references are traversal aids, not anatomical definitions
```

## Validation Notes

The first supported validation set intentionally stays close to canonical anatomy.

It tests:

```text
composite-to-component correspondence
composite-to-composite correspondence with child traversal
external pelvic boundary correspondence
explicit directionality
lightweight routing hints
boundary-region references
```

The female expansion candidate set tests additional routes before Activation Layer construction:

```text
composite external body-region mirroring
focal output-site to internal-canal mirroring
paraurethral glandular to urinary-output boundary mirroring
boundary-region to support-structure mirroring
Fluid Layer adjacency without fluid definition
Activation dependency as routing hint only
```

## Status

Draft v0.8.
