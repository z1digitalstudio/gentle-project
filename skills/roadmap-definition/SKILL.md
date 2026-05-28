---
name: roadmap-definition
description: Use when research is already usable and Codex needs to turn evidence and opportunity framing into product priorities, MVP cuts, sequencing logic, and a roadmap that combines text, structure, and visual clarity.
domain: discovery
phase: roadmap-definition
outputs:
  - management/ROADMAP.md
  - management/DECISIONS.md
  - product/artifacts/Feature-Prioritization.md
  - product/artifacts/MVP-Cuts.md
recommended_previous:
  - design-research
next_steps:
  - scope-definition
---

# Roadmap Definition

Turn research into product priorities, MVP scope, and sequencing.

This skill exists to translate research and framing into a usable roadmap. It should make prioritization logic visible, distinguish MVP from later opportunities, and leave the project ready for PRD and user-story work.

## When to Use

Use this skill when:
- `product/RESEARCH.md` already exists in usable form
- the project needs a first real prioritization pass
- the team needs to distinguish MVP from later scope
- product opportunities are visible, but roadmap sequencing is not yet explicit

Do **not** use this skill when:
- research is still too weak or ambiguous to support prioritization
- the project is still clarifying kickoff-level framing
- the request is already to write PRD or user stories

## Required Reading

Read these files before producing output when they exist:

- `product/RESEARCH.md`
- `docs/PROJECT-SUMMARY.md`
- `management/RISKS.md`
- `management/ROADMAP.md`
- `management/DECISIONS.md`

If one or more files are missing, continue and treat that as missing context rather than a blocker, except for `product/RESEARCH.md`, which is normally required.

## Minimum Inputs

Require at least:

- `product/RESEARCH.md`

If research does not yet provide enough clarity to differentiate priorities, say that `design-research` needs more work first.

## Recommended Inputs

Use these when available:

- `docs/PROJECT-SUMMARY.md`
- `management/RISKS.md`
- kickoff closeout context
- commercial or technical constraints
- feature wishlist or backlog fragments
- stakeholder inputs on value, urgency, or feasibility

## Workflow

### 1. Confirm that roadmap work is justified

Verify that:
- research is already usable
- there are enough opportunity signals to prioritize
- the project now needs scope ordering rather than more raw discovery

If not, say what is still missing.

### 2. Rebuild the prioritization context

Extract and normalize:

- product goal
- main opportunities
- target users
- major constraints
- already-known risks
- implicit MVP assumptions hiding inside earlier discovery work

### 3. Translate research into prioritization logic

Make explicit:

- which opportunities matter most now
- which features belong in MVP
- which ones should be later
- what is out of scope for now
- what sequencing dependencies exist

Do not present instinct as logic. Show the rationale.

### 4. Produce or update `management/ROADMAP.md`

Create or update `management/ROADMAP.md` as the canonical output.

When useful, read `references/roadmap-template.md` for the historical table shape, but do not reduce the roadmap to that table alone.

The recommended roadmap combines three layers:

#### A. Narrative explanation

Include at least:

1. `Product Goal`
2. `Prioritization Principles`
3. `MVP Scope`
4. `Post-MVP / Later Opportunities`
5. `Sequencing Logic`
6. `Main Dependencies`
7. `Open Prioritization Decisions`

#### B. Structured feature table

Prefer columns like:

- Feature Name
- Release
- Opportunity Statement
- Target User
- Requirements
- Assumptions & Exclusions
- Comparable Solutions
- Reach
- Impact
- Frequency
- Priority

#### C. Mermaid visualization

Add a Mermaid diagram that makes one of these visible, whichever is most useful:

- MVP vs later releases
- grouped functional blocks
- sequencing dependencies
- phased rollout shape

### 5. Produce optional working artifacts when they add value

Generate these only when they help the team reason better:

- `product/artifacts/Feature-Prioritization.md`
- `product/artifacts/MVP-Cuts.md`

### 6. Update supporting project memory

When roadmap work sharpens the project framing, update:

- `docs/PROJECT-SUMMARY.md`
- `management/RISKS.md`
- `management/DECISIONS.md` when prioritization or scope decisions should be preserved explicitly

## Output Contract

Your output must include all of the following:

### A. Roadmap status

State one of:

- `Created roadmap draft`
- `Updated existing roadmap`
- `Prepared roadmap for review`
- `Roadmap definition blocked — research insufficient`

### B. Canonical document target

State where `management/ROADMAP.md` should live or confirm that it was updated there.

### C. Prioritization summary

List:

- MVP features or feature groups
- later opportunities
- explicit out-of-scope items when visible
- the main logic behind the prioritization

### D. Visual roadmap summary

State what the Mermaid diagram represents:

- MVP vs later
- dependencies
- release sequence
- functional grouping

### E. Risks and decisions

List:

- new or reframed risks
- decisions captured in `management/DECISIONS.md`
- prioritization questions that remain open

### F. Optional artifacts produced or skipped

State explicitly:

- whether `Feature-Prioritization.md` was created
- whether `MVP-Cuts.md` was created
- why each optional artifact was produced or skipped

### G. Next skill

State one of:

- `Next: scope-definition`
- `Next: design-research`
- `Next: gather better prioritization inputs`

Choose based on the actual state of the project.

### H. Human review checklist

End with a short checklist for the responsible person to validate:

- MVP is not overloaded
- prioritization logic is explicit
- roadmap is not pretending certainty it does not have
- Mermaid diagram is actually useful
- scope work can now begin

## Guardrails

Do not:

- fake certainty where tradeoffs are still unresolved
- depend on templates outside this skill folder at runtime
- reduce the roadmap to a naked feature table with no reasoning
- jump into detailed PRD or user stories
- promote nice-to-haves into MVP without explicit rationale
- ignore business, delivery, or feasibility constraints

## Success Criteria

The skill succeeds when `management/ROADMAP.md` exists in usable form, combines narrative + structure + Mermaid, makes MVP vs later explicit, and leaves the project ready for `scope-definition`.
