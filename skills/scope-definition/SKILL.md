---
name: scope-definition
description: Use when roadmap priorities are already usable and Codex needs to turn MVP decisions into a PRD, prioritized user stories, explicit non-goals, and a clean handoff toward design, specification, or development.
domain: discovery
phase: scope-definition
outputs:
  - product/PRD.md
  - product/USER-STORIES.md
  - product/artifacts/MVP-Scope-Notes.md
  - product/artifacts/Open-Product-Questions.md
recommended_previous:
  - roadmap-definition
next_steps:
  - design
  - specification
  - development
---

# Scope Definition

Turn roadmap priorities into actionable product scope.

This skill exists to close Discovery by making MVP scope explicit, documenting non-goals, and translating roadmap priorities into a usable PRD and prioritized user stories. It should reduce ambiguity for design and development without pretending that every detail is already settled.

## When to Use

Use this skill when:
- `management/ROADMAP.md` already exists in usable form
- MVP priorities are clear enough to turn into product requirements
- the team needs a PRD and user stories before moving into design, spec, or implementation
- roadmap work is done, but the delivery-facing scope is still too vague

Do **not** use this skill when:
- the roadmap is still unstable
- MVP vs later is not yet clear
- the work is still about research or prioritization rather than requirements
- the request is really for technical design or implementation planning

## Required Reading

Read these files before producing output when they exist:

- `management/ROADMAP.md`
- `product/RESEARCH.md`
- `docs/PROJECT-SUMMARY.md`
- `management/RISKS.md`
- `management/DECISIONS.md`
- `product/PRD.md`
- `product/USER-STORIES.md`

If one or more files are missing, continue and treat that as missing context rather than a blocker, except for `management/ROADMAP.md`, which is normally required.

## Minimum Inputs

Require at least:

- `management/ROADMAP.md`

If the roadmap still does not make MVP boundaries clear enough to define scope, say that `roadmap-definition` needs more work first.

## Recommended Inputs

Use these when available:

- `product/RESEARCH.md`
- `docs/PROJECT-SUMMARY.md`
- `management/RISKS.md`
- `management/DECISIONS.md`
- business notes or validation feedback
- important open questions from stakeholders

## Workflow

### 1. Confirm that scope work is justified

Verify that:
- roadmap priorities are already usable
- MVP boundaries are clear enough to document
- the project is ready to move from prioritization into requirements

If not, say what is still missing.

### 2. Rebuild the scope context

Extract and normalize:

- product goal
- MVP definition from the roadmap
- target users
- functional priorities
- key flows implied by the roadmap
- risks, dependencies, and unresolved questions that affect scope

### 3. Define the real MVP scope

Make explicit:

- what is in scope now
- what is out of scope for now
- what is still uncertain but important
- which requirements are essential for design and development to start

Do not hide uncertainty just to make the document look complete.

### 4. Produce or update `product/PRD.md`

Create or update `product/PRD.md` as the canonical product definition output.

Prefer this structure:

1. `Problem Statement`
2. `Product Goal`
3. `MVP Definition`
4. `Target Users`
5. `Functional Scope`
6. `Non-Goals`
7. `Key Flows`
8. `Constraints`
9. `Risks / Open Questions`
10. `Success Signals`

### 5. Produce or update `product/USER-STORIES.md`

Create or update `product/USER-STORIES.md` as the canonical user-story output.

At minimum, stories should be:

- prioritized
- grouped by feature or epic
- written in user-centered language
- clear enough for design and development to start
- explicit about important doubts when certainty is still incomplete

### 6. Produce optional working artifacts when they add value

Generate these only when they help clarify scope:

- `product/artifacts/MVP-Scope-Notes.md`
- `product/artifacts/Open-Product-Questions.md`

### 7. Update supporting project memory

When scope work sharpens the framing, update:

- `docs/PROJECT-SUMMARY.md`
- `management/RISKS.md`
- `management/DECISIONS.md` when scope decisions should be preserved explicitly

## Output Contract

Your output must include all of the following:

### A. Scope status

State one of:

- `Created scope draft`
- `Updated existing scope`
- `Prepared scope for review`
- `Scope definition blocked — roadmap insufficient`

### B. Canonical document targets

State where these should live or confirm they were updated there:

- `product/PRD.md`
- `product/USER-STORIES.md`

### C. Scope summary

List:

- what is clearly in MVP
- what is explicitly out of scope
- the most important open questions
- the key flows that now shape design and development

### D. Risks and decisions

List:

- new or reframed risks
- decisions captured in `management/DECISIONS.md`
- scope questions that remain open

### E. Optional artifacts produced or skipped

State explicitly:

- whether `MVP-Scope-Notes.md` was created
- whether `Open-Product-Questions.md` was created
- why each optional artifact was produced or skipped

### F. Next phase

State one or more of:

- `Next: design`
- `Next: specification`
- `Next: development`
- `Next: roadmap-definition`

Choose based on the actual state of the project.

### G. Human review checklist

End with a short checklist for the responsible person to validate:

- MVP is truly bounded
- non-goals are visible
- stories are actionable enough
- uncertainty is not hidden
- design and development can now begin with less ambiguity

## Guardrails

Do not:

- fake precision where major ambiguity still exists
- depend on templates outside this skill folder at runtime
- write detailed technical design or implementation plans
- mix PRD language with UI design specification
- mix user stories with engineering task breakdowns
- hide non-goals or open questions just to make the output look complete

## Success Criteria

The skill succeeds when `product/PRD.md` and `product/USER-STORIES.md` exist in usable form, the MVP is clearly bounded, non-goals are visible, and the project is ready to move from Discovery into design, specification, or development.
