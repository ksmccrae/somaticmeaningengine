---
tags:
  - convention
  - governance
---
**Type:** Vault Convention
**Status:** Draft v1
**Scope:** Anatomical Site nodes (02_Anatomical_Sites)

> The rule of thumb: a convention is only worth keeping if it makes future linking and filtering easier. When in doubt, optimise for "links always resolve" and "tags always filter."

---

## 1. Node Naming (canonical rule)

Each anatomical structure is **one note, titled by its canonical anatomical name** — e.g. `Urethra`, `Clitoral Complex`, `Vaginal Wall`. This is the single source of truth.

- All `[[wikilinks]]` must use the exact canonical title, because `[[Urethra]]` and `[[Urethral Opening]]` are two different graph nodes in Obsidian.
- Hierarchy/spec documents (e.g. *Female Genitalia Hierarchy*) must refer to children using these same canonical titles — not descriptive variants like "Urethral Opening."
- Other accepted names (clinical, neutral, slang) go in the note's `aliases:` frontmatter, **not** in the title. Aliases still resolve in `[[ ]]` autocomplete, so you keep natural-language linking without creating duplicate notes.

**One structure = one note = one canonical name. Everything else is an alias.**

---

## 2. Folder Layout

Nodes live under `02_Anatomical_Sites/<embodiment>/` — e.g. `02_Anatomical_Sites/female/`. Cross-embodiment structures go under `shared/`. Higher-level hierarchy/spec documents stay at the `02_Anatomical_Sites/` root.

---

## 3. Node Types

| Type | Tag | Meaning |
|------|-----|---------|
| Composite | `type/composite` | Container/organisational node that holds child nodes (e.g. Vulva, Clitoral Complex). |
| Atomic | `type/atomic` | A discrete structure with no children (e.g. Mons Pubis, Clitoral Glans). |
| Functional | `type/functional` | An experiential/somatic/propagative concept treated as a tag rather than a standalone structure (e.g. Pelvic Floor) until promoted. |

Composite nodes list their **direct children only** by canonical name. Grandchildren belong to the intermediate composite, not the grandparent (e.g. Vestibular Bulbs sit under Clitoral Complex, not directly under Vulva).

---

## 4. Tag Namespacing

Use nested tags so the tag pane filters cleanly. Keep structural type and ontological role in separate namespaces:

- `type/…` — node type: `type/composite`, `type/atomic`, `type/functional`
- `role/…` — ontological role: `role/sensory-hub`, `role/mirror-hub`, `role/symbolic-site`, `role/propagation-hub`, `role/transition-zone`
- `register/…` — expressive register affinity: `register/somatic`, `register/sensory`, `register/symbolic`, `register/mirror`

Do **not** use inline tags with markdown formatting (e.g. `#**Composite**` will not parse). Put tags in frontmatter, or use plain inline tags like `#type/composite`.

---

## 5. Template

New nodes start from `02_Anatomical_Sites/anatomical_site_template.md`. Fill every placeholder or delete the section — avoid leaving raw `<...>` placeholders in finished notes. The template mirrors the structure of `female/Vulva.md`, which is the reference example.

---

## 6. Terms & Governance

The `Terms` section tiers vocabulary by register (clinical / neutral / restricted / banned). Scope any "banned" entry to the register it applies to — e.g. "clinical distancing" is disallowed *within the erotic register* but allowed in medical/educational contexts, which the `governance.thresholds.clinical.allowed_contexts` block already permits. Wording the scope explicitly prevents future-you reading it as a contradiction.

---

## 7. Revision Gate

These conventions inherit from the master README governance. Changes to naming, node types, or tag namespaces should be made here first, then propagated — and significant changes warrant a version bump on this note.

---

## Related
- [[README]]
- [[Female Genitalia Hierarchy]]
- [[Female]]
