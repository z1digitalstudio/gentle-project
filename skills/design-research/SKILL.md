---
name: design-research
description: Use when kickoff context is already usable and agents needs to turn it into structured research, explicit evidence vs assumptions, and opportunity framing for roadmap decisions.
domain: discovery
phase: design-research
outputs:
  - product/RESEARCH.md
  - product/artifacts/Discovery-Insights.md
  - product/artifacts/Personas.md
  - product/artifacts/User-Journeys.md
recommended_previous:
  - kickoff-closeout
next_steps:
  - roadmap-definition
---

# Design Research

Turn post-kickoff context into usable research and opportunity framing.

This skill exists to separate evidence from assumptions, clarify users and market context, and leave the project ready for prioritization. It should not jump ahead into roadmap or PRD decisions as if research already resolved them.

## When to Use

Use this skill when:
- kickoff context is already usable
- the project needs structured research before prioritization
- user, market, competitor, or opportunity signals are still scattered
- the team needs a reliable `product/RESEARCH.md` before defining roadmap

Do **not** use this skill when:
- kickoff framing is still too weak and `discovery-onboarding` or `kickoff-closeout` should run first
- the work is already at the stage of prioritizing MVP and releases
- the request is really to write PRD or user stories

## Required Reading

Read these files before producing output when they exist:

- `docs/PROJECT-SUMMARY.md`
- `management/RISKS.md`
- `product/RESEARCH.md`
- `product/artifacts/Opportunity-Brief.md`
- `product/artifacts/Kickoff-Closeout-Summary.md`

If one or more files are missing, continue and treat that as missing context rather than a blocker.

## Minimum Inputs

Require usable project framing from at least one of these:

- `docs/PROJECT-SUMMARY.md`
- `product/artifacts/Opportunity-Brief.md`
- `product/artifacts/Kick-off-Meeting-Prep.md`
- `product/artifacts/Kickoff-Closeout-Summary.md`
- kickoff notes or equivalent external context
- other external documentation that already explains the problem, users, and goals

If there is still not enough context to distinguish signals from assumptions, stop and say which earlier skill should run first.

## Recommended Inputs

Use these when available:

- existing `management/RISKS.md`
- research notes or interviews
- benchmark or competitor review
- links to product, prototype, or adjacent solutions
- support, sales, or commercial data
- externally provided `Brand Personality` when the project has a design component

Treat `Brand Personality` as optional external input, not as output of this skill.

## Optional Outputs

Default behavior should prioritize `product/RESEARCH.md`.

Optional artifacts like `Discovery Insights`, `Personas`, and `User Journeys` should be produced only when they add clear value to product or design decisions.

## Workflow

### 1. Confirm that research is the right next step

Verify that:
- kickoff-level context is already usable
- the project still needs structured research before prioritization
- there is enough evidence or context to produce meaningful findings

If not, say which prerequisite is missing.

### 2. Rebuild the current context

Extract and normalize:

- problem framing
- project objective
- user or stakeholder context
- business and delivery constraints
- already-known risks
- major open questions

### 3. Separate evidence from assumptions

Explicitly distinguish:

- evidence backed by inputs
- repeated signals that look promising but still need validation
- assumptions that the team is making without enough proof
- contradictions across sources

Do not blur these categories.

### 4. Produce or update `product/RESEARCH.md`

Create or update `product/RESEARCH.md` as the canonical output.

Prefer this structure:

1. `Context`
2. `Research Inputs`
3. `User Signals`
4. `Pain Points`
5. `Market / Competitor Signals`
6. `Evidence vs Assumptions`
7. `Opportunity Areas`
8. `Open Questions`
9. `Implications for Roadmap`

### 5. Produce optional working artifacts when they add value

#### A. `Discovery Insights`

If the project needs a richer synthesis artifact, read `references/discovery-insights-template.md` for the canonical template shape.

When produced, `product/artifacts/Discovery-Insights.md` should capture:

1. metadata
2. product main goals
3. key opportunities
4. ideation / how-might-we
5. potential solutions explored
6. key insights and findings
7. feature list proposal
8. assumptions, constraints, dependencies, and open questions

#### B. `Personas`

Generate `product/artifacts/Personas.md` only when personas materially improve product or design decisions.

#### C. `User Journeys`

Generate `product/artifacts/User-Journeys.md` only when journey mapping materially improves understanding of flows, friction, or sequencing.

### 6. Update project memory

When research changes the framing materially, update:

- `docs/PROJECT-SUMMARY.md`
- `management/RISKS.md` if new uncertainties or discovery risks appear

## Output Contract

Your output must include all of the following:

### A. Research status

State one of:

- `Created research draft`
- `Updated existing research`
- `Prepared research for review`
- `Design research blocked — earlier discovery context insufficient`

### B. Canonical document target

State where `product/RESEARCH.md` should live or confirm that it was updated there.

### C. Evidence vs assumptions summary

List:

- strongest evidence
- strongest signals still needing validation
- assumptions that remain unresolved
- contradictions that matter

### D. Optional artifacts produced or skipped

State explicitly:

- whether `Discovery Insights` was created
- whether `Personas` were created
- whether `User Journeys` were created
- why each optional artifact was produced or skipped

### E. Risks and implications

List:

- new or reframed risks
- major open questions
- implications that should shape `roadmap-definition`

### F. Next skill

State one of:

- `Next: roadmap-definition`
- `Next: kickoff-closeout`
- `Next: gather better research evidence`

Choose based on the actual state of the project.

### G. Human review checklist

End with a short checklist for the responsible person to validate:

- evidence is not being overstated
- assumptions are explicitly labeled
- opportunities are clear enough to prioritize
- optional artifacts were created only when they added value
- roadmap work can now start

## Guardrails

Do not:

- invent certainty from weak research
- convert isolated opinions into user truth
- depend on templates outside this skill folder at runtime
- produce `Brand Personality` as a standard output
- write the PRD
- write detailed user stories
- treat research synthesis as final prioritization

## Success Criteria

The skill succeeds when `product/RESEARCH.md` exists in usable form, evidence and assumptions are clearly separated, opportunities are visible, and `roadmap-definition` can start without reinventing discovery context.
