---
tags:
  - Document/Specification
  - Governance/Specifications
  - Status/Baseline
file_class: Document
document_type: Specification
title: Relationship Specification
status: Baseline
version: 2.0
---

# Relationship Specification

## Purpose

This specification defines the controlled ontology relationship language.

Relationships are expressed as single uppercase verbs in the form:

```text
Subject VERB Object
```

## Edge Families

| Family | Function |
|---|---|
| Canonical | Defines structural knowledge |
| Activation | Defines response and interaction |
| Interpretive | Defines meaning and representation |
| Governance | Defines requirements and constraints |

## Controlled Verb Rule

Relationship verbs should be compact, uppercase, and reusable.

## Tag Pattern

Relationship tags should use this pattern:

```text
Edge/Family/VERB
```

## Governance

The relationship vocabulary is part of the v2 architecture baseline. Future additions should be justified by repeated need across the ontology rather than by a single node.
