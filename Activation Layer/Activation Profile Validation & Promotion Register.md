---
tags:
  - Document/Register
  - Layer/Activation
  - Governance/Validation
  - Status/Draft
title: Activation Profile Validation & Promotion Register
file_class: Document
document_type: Governance Register
layer: Activation Layer
status: Draft
version: 0.1
last_updated: 2026-07-02
---

# Activation Profile Validation & Promotion Register

## Purpose

This register defines the evidence required to move an Activation Profile from Candidate to Supported.

It separates document maturity from profile validation status.

```text
Document status
= Draft / Validated / Baseline

Profile validation status
= Candidate / Supported / Blocked
```

A profile may be mechanically mature while remaining Candidate.

## Promotion Rule

An Activation Profile may be promoted from Candidate to Supported only when every required criterion passes.

A deferred downstream node is not automatically a blocker unless the profile depends on that node to justify its own classification, scope, anatomy, fluid identity, mirror route, or process sequence.

## Required Criteria

| Criterion | Required Evidence |
|---|---|
| Mechanical completeness | All required template sections are present; YAML, body, Index, and relationship statements agree |
| Controlled classification | `activation_type`, `activation_components`, `activation_scope`, embodiment scope, and validation status use governed values |
| Scope accuracy | Scope follows direct participation under the validated scope decision rule |
| Canonical anatomy accuracy | Primary anchor and participants exist and are referenced without redefinition |
| Process coherence | Trigger, state change, sequence, modulators, and outcomes describe one coherent activation process |
| Cross-layer discipline | Anatomy, Fluid, Mirror, Propagation, Sensory, Pleasure, Desire, Meaning, Authorial, and Corpus boundaries are preserved |
| Mirror accuracy | Referenced Mirror Profile exists; its Candidate or Supported status is represented accurately; mirror traversal is not treated as mechanism |
| Fluid accuracy | Where applicable, Fluid Entities, Fluid Profiles, and Fluid Properties exist and remain distinct |
| Adjacency accuracy | Adjacent anatomy or fluid is not treated as active, source, or identity-defining by proximity alone |
| Consent boundary | Physiological response, fluid release, pleasure, desire, and symbolic meaning are not treated as consent |
| Wikilink integrity | Existing nodes resolve; nonexistent candidate records remain plain text |
| Audit evidence | At least one focused audit has found no blocking mechanical or governance defect |
| Replicability evidence | The profile uses a pattern already demonstrated by at least one contrasting Activation Profile |
| Unresolved-question review | Open questions are classified as blocking or non-blocking rather than merely listed |

## Blocking Conditions

A profile remains Candidate or becomes Blocked when any of the following applies:

```text
primary anatomical anchor is unresolved or inaccurate
activation scope conflicts with direct participation
fluid identity is collapsed or unsupported
mirror status is misstated
activation component is essential but ungoverned
process sequence combines distinct processes without justification
relationship verbs imply participation that the body does not support
consent boundary is absent or weakened
mechanical drift remains unresolved
```

`Blocked` should be used only when the profile cannot progress without upstream architectural or canonical work.

## Non-Blocking Conditions

The following may remain open without preventing Supported status when they do not undermine the profile's core definition:

```text
missing downstream Sensory Profile
missing Authorial Term Register
missing Corpus Annotation
candidate Propagation handoff
future child-level anatomy
future corpus examples
future symbolic interpretation
```

## Promotion Decision Record

Each profile assessment should record:

| Field | Allowed Value |
|---|---|
| Mechanical Result | Pass / Warning / Fail |
| Governance Result | Pass / Warning / Fail |
| Blocking Defect | None or concise defect |
| Non-Blocking Open Questions | Concise list |
| Promotion Recommendation | Remain Candidate / Promote to Supported / Blocked |
| Review Date | YYYY-MM-DD |

## Current Profile Assessments

### Female - Vulvar Lubrication Activation Profile

| Field | Assessment |
|---|---|
| Mechanical Result | Pass |
| Governance Result | Warning |
| Blocking Defect | None currently demonstrated |
| Non-Blocking Open Questions | Future Sensory profiles; possible Propagation handoff; name remains narrower than broader genital activation |
| Promotion Recommendation | Remain Candidate pending promotion audit against this register |
| Review Date | 2026-07-02 |

Notes:

```text
classification normalized
scope and anatomy currently coherent
Vaginal Fluid and fluid-property boundaries preserved
Supported mirror route represented accurately
consent boundary explicit
```

### Female - Paraurethral Glandular Release Activation Profile

| Field | Assessment |
|---|---|
| Mechanical Result | Pass |
| Governance Result | Warning |
| Blocking Defect | Canonical role of Female - Vestibular Gland Openings remains under review; Autonomic Activation remains provisional |
| Non-Blocking Open Questions | Future Sensory profiles; possible Propagation handoff |
| Promotion Recommendation | Remain Candidate |
| Review Date | 2026-07-02 |

Notes:

```text
Paraurethral Glandular Fluid remains distinct from Urine
Skene's Glands remains source anatomy
Urethral Opening remains adjacent territory
Candidate mirror route represented accurately
```

### Female - Pelvic Floor Contraction Activation Profile

| Field | Assessment |
|---|---|
| Mechanical Result | Pass |
| Governance Result | Warning |
| Blocking Defect | Motor / Kinetic Activation and Reflex Activation promotion criteria require further governance before Supported status |
| Non-Blocking Open Questions | Candidate Propagation handoff; future Sensory profiles |
| Promotion Recommendation | Remain Candidate |
| Review Date | 2026-07-02 |

Notes:

```text
Local scope now follows one active anatomical anchor
Perineum is boundary and mirror context rather than direct participant
Fluid Layer independence is explicit
Candidate mirror route represented accurately
```

## Promotion Sequence

```text
1. Apply this register to the profile.
2. Resolve all blocking defects.
3. Run a focused promotion audit.
4. Record the audit result here.
5. Update the profile validation_status.
6. Update the Activation Profiles Index and README.
7. Do not promote the governing Framework, Template, or Index merely because a profile is promoted.
```

## Current Recommendation

No live Activation Profile is promoted by this first register pass.

The closest profile to Supported is:

```text
Female - Vulvar Lubrication Activation Profile
```

It requires a focused promotion audit rather than new ontology construction.

## Status

Draft v0.1.

This register establishes Candidate-to-Supported promotion governance but has not yet been validated through an actual profile promotion.
