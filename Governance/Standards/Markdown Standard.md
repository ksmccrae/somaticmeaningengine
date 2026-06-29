---
tags:
  - Document/Standard
  - Governance/Standards
  - Status/Baseline
file_class: Document
document_type: Standard
title: Markdown Standard
status: Baseline
version: 2.0
---

# Markdown Standard

## Purpose

This standard defines Markdown conventions for the Somatic Meaning Engine.

The goal is readable Markdown that works well in GitHub, Obsidian, PDF export, and future tooling.

## Heading Rules

- Use one level-one heading per file.
- Use clear section headings.
- Avoid decorative heading patterns that reduce parser clarity.
- Prefer consistent heading names across related files.

## Link Rules

Use Obsidian wiki links for internal conceptual links when working inside the vault.

```markdown
[[Node Specification]]
```

Use relative Markdown links when a GitHub-readable navigation link is needed.

```markdown
[Node Specification](Governance/Specifications/Node%20Specification.md)
```

## Tables

Use tables for compact comparisons, definitions, and classification summaries.

Tables should remain simple enough to export cleanly to PDF.

## Code Blocks

Use fenced code blocks for:

- YAML examples
- Text hierarchy examples
- Mermaid diagrams
- Query examples

Always specify the language where useful.

## Mermaid Diagrams

Use Mermaid diagrams for architecture, flow, hierarchy, and traversal examples.

Mermaid diagrams should support understanding rather than decoration.

## Tone

Governance and specification documents should be precise, calm, and architectural.

## Rule

Markdown should serve both human reading and future machine interpretation.
