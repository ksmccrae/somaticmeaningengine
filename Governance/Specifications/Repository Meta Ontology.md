---
tags:
  - Document/Specification
  - Governance/Specifications
  - Status/Baseline
file_class: Document
document_type: Specification
title: Repository Meta Ontology
status: Baseline
version: 2.0
---

# Repository Meta Ontology

## Purpose

This document defines how Markdown files are classified within the Somatic Meaning Engine repository.

Every Markdown file belongs to the repository, but not every Markdown file has the same function.

## Core File Classes

| File Class | Function |
|---|---|
| Document | Explains, governs, specifies, or guides |
| Ontology Node | Defines a domain knowledge object |
| Template | Defines reusable structure |
| Corpus Annotation | Annotates a creative or research work |
| ADR | Records an architectural decision |
| Scratchpad | Holds temporary work |

## Rule

The `file_class` property identifies the repository function of a file.

Secondary properties define the subtype.

Examples include `document_type`, `node_type`, `template_type`, and `corpus_type`.

## Governance

This model is part of the v2 architecture baseline and should remain stable unless an ADR justifies a change.
