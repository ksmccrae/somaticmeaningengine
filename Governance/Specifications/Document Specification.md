---
tags:
  - Document/Specification
  - Governance/Specifications
  - Status/Baseline
file_class: Document
document_type: Specification
title: Document Specification
status: Baseline
version: 2.0
---

# Document Specification

## Purpose

This specification defines repository documents.

A document explains, governs, specifies, guides, or records a decision. It is distinct from an ontology node, which defines domain knowledge.

## Required Properties

| Property | Purpose |
|---|---|
| file_class | Repository function |
| document_type | Document subtype |
| title | Human-readable title |
| status | Lifecycle status |
| tags | Obsidian discovery |

## Common Document Types

- README
- Specification
- Standard
- Guide
- Reference
- Roadmap
- ADR

## Rule

Documents may describe ontology structures, but they should not become ontology nodes themselves unless they are intentionally modelling repository knowledge.
