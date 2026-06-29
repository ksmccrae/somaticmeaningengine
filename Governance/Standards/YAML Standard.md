---
tags:
  - Document/Standard
  - Governance/Standards
  - Status/Baseline
file_class: Document
document_type: Standard
title: YAML Standard
status: Baseline
version: 2.0
---

# YAML Standard

## Purpose

This standard defines how YAML front matter should be written across the repository.

The goal is valid, readable, Obsidian-compatible metadata that can also support future tooling.

## General Rules

- Use YAML front matter at the top of governed Markdown files.
- Use lowercase property keys with underscores where needed.
- Quote string values that contain colons or unusual punctuation.
- Use ISO dates in `YYYY-MM-DD` format.
- Use lists for multi-value fields.
- Keep front matter concise.

## Recommended Property Order

```yaml
---
tags:
aliases:
title:
file_class:
document_type:
node_type:
template_type:
corpus_type:
layer:
status:
version:
last_updated:
---
```

Not every file uses every field. Omit fields that do not apply.

## Strings

Use quotes when a value contains a colon.

```yaml
title: "K.S. McCrae Ontology: Somatic Meaning Engine"
```

## Lists

Use block lists for tags, aliases, relationships, and multi-value properties.

```yaml
tags:
  - Document/Standard
  - Governance/Standards
```

## Booleans

Use lowercase YAML booleans.

```yaml
paired: true
```

## Rule

YAML must remain valid before it is useful. If Obsidian flags an error, the metadata must be fixed before content work continues.
