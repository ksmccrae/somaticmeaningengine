---
tags:
  - Document/Standard
  - Governance/Standards
  - Status/Baseline
file_class: Document
document_type: Standard
title: Repository Lifecycle Standard
status: Baseline
version: 2.0
---

# Repository Lifecycle Standard

## Purpose

This standard defines lifecycle states for repository objects.

Lifecycle status makes it clear whether a file is temporary, under review, accepted, deprecated, or historical.

## Lifecycle States

| Status | Meaning |
|---|---|
| Scratchpad | Temporary working material |
| Draft | Early structured version |
| Review | Ready for architectural or content review |
| Baseline | Accepted as part of the current architecture |
| Canonical | Accepted as source of truth for ontology content |
| Deprecated | Retained but no longer preferred |
| Archived | Historical reference only |

## Recommended Flow

```text
Scratchpad
↓
Draft
↓
Review
↓
Baseline or Canonical
↓
Deprecated
↓
Archived
```

## Documents

Governance documents usually move toward `Baseline`.

## Ontology Nodes

Ontology nodes usually move toward `Canonical`.

## Templates

Templates may begin as `Draft`, move to `Review`, and become `Baseline` once they are stable enough to instantiate repeated nodes.

## Rule

A file should not be treated as accepted until its lifecycle status says so.
