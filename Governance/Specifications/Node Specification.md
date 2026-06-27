---
tags:
  - Document/Specification
  - Governance/Specifications
  - Status/Baseline
file_class: Document
document_type: Specification
title: Node Specification
status: Baseline
version: 2.0
---

# Node Specification

## Purpose

This specification defines ontology nodes.

An ontology node is a domain knowledge object represented as a Markdown file.

## Required Questions

Every node should answer:

1. What am I?
2. How am I connected?
3. How do I participate?
4. How am I governed?

## Required Properties

| Property | Purpose |
|---|---|
| file_class | Must be `Ontology Node` |
| node_type | Class of knowledge object |
| layer | Ontology layer |
| status | Lifecycle status |
| title | Human-readable node name |
| tags | Obsidian discovery |

## Rule

Nodes define reusable knowledge. They should not duplicate material that belongs in another node, template, or specification.
