---
tags:
  - Document/Standard
  - Governance/Standards
  - Status/Baseline
file_class: Document
document_type: Standard
title: Metadata Standard
status: Baseline
version: 2.0
---

# Metadata Standard

## Purpose

This standard defines how metadata is used across the Somatic Meaning Engine repository.

Metadata allows files to be discovered, filtered, validated, and interpreted consistently in Obsidian, GitHub, future parsers, and future graph tooling.

## Core Principle

Metadata should identify the function of a file without overloading it.

Every file should declare what kind of repository object it is before declaring its subtype.

## Core Properties

| Property | Purpose | Required |
|---|---|---|
| file_class | Defines the repository function of the file | Yes |
| title | Human-readable title | Yes |
| status | Lifecycle status | Yes |
| tags | Obsidian discovery and filtering | Yes |
| aliases | Alternate names or search terms | Optional |
| version | Version marker for governed documents | Optional |

## File Class Values

| Value | Function |
|---|---|
| Document | Explains, governs, specifies, or guides |
| Ontology Node | Defines a domain knowledge object |
| Template | Defines reusable structure |
| Corpus Annotation | Annotates a work or research object |
| ADR | Records an architectural decision |
| Scratchpad | Holds temporary work |

## Subtype Properties

Subtype properties depend on `file_class`.

| File Class | Subtype Property |
|---|---|
| Document | document_type |
| Ontology Node | node_type |
| Template | template_type |
| Corpus Annotation | corpus_type |
| ADR | document_type |

## Common Status Values

| Status | Meaning |
|---|---|
| Draft | Early working version |
| Review | Requires review before acceptance |
| Baseline | Accepted as part of the current architecture |
| Canonical | Accepted as the current source of truth |
| Deprecated | Retained but no longer preferred |
| Archived | Historical reference only |

## Rule

Metadata should remain useful, minimal, and stable.

If a property is only useful once, it should not become part of the standard.
