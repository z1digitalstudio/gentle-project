---
name: discovery-onboarding
description: Use when kickoff framing is weak, scattered, contradictory, or missing a usable brief, and Codex needs to normalize onboarding materials into kickoff-ready project context.
domain: discovery
phase: onboarding-kickoff
outputs:
  - product/artifacts/Opportunity-Brief.md
recommended_previous: []
next_steps:
  - kickoff-prep
---

# Discovery Onboarding

Normalize scattered onboarding context into kickoff-ready framing.

This skill is **not** for producing an `Opportunity Brief` by ritual. Its job is to make sure the team has enough context, gaps, and questions to run a useful kickoff.

## When to Use

Use this skill when:
- onboarding context is fragmented across notes, decks, emails, transcripts, or links
- there is no usable `Opportunity Brief`
- an existing brief is too weak, stale, or contradictory
- the team cannot yet prepare a solid kickoff agenda

Do **not** use this skill when:
- a usable `Opportunity Brief` or equivalent framing already exists
- the kickoff is already prepared and `kickoff-prep` can start directly
- the kickoff already happened and the right next step is `kickoff-closeout`

## Required Reading

Read these files before producing output when they exist:

- `docs/PROJECT-SUMMARY.md`
- `management/RISKS.md`
- `product/artifacts/Opportunity-Brief.md`

If one or more files are missing, continue and treat that as missing context rather than a blocker.

## Inputs To Prioritize

Prioritize these sources when available:

- sales notes
- proposal or commercial deck
- intake form
- emails or written summaries
- budget or timeline constraints
- call transcripts or rough notes
- early prototypes or product links
- externally provided `Opportunity Brief`
- externally provided `Vision & Collaboration Goals`

Treat source quality explicitly:

- prefer direct client language over internal paraphrases
- prefer recent material over stale material
- call out contradictions rather than resolving them silently
- treat `Vision & Collaboration Goals` as optional input, not required output

## Workflow

### 1. Determine whether onboarding is actually needed

Decide whether framing is insufficient.

If kickoff framing is already usable, do **not** force a new brief. Instead, say the repo can proceed to `kickoff-prep`.

### 2. Gather and normalize source context

Extract and normalize:

- client or company context
- problem statement or opportunity
- expected business outcome
- stakeholders and decision-makers
- known constraints
- supporting materials and links
- missing information that blocks good kickoff preparation

### 3. Reconcile with repo context

Use repo documents to:

- avoid restating outdated assumptions as current truth
- spot contradictions between onboarding inputs and project memory
- reuse validated framing when it already exists

### 4. Produce kickoff-ready framing

Your primary responsibility is to leave the project in one of these states:

- `Prepared framing from onboarding materials`
- `Created Opportunity Brief draft`
- `Updated existing Opportunity Brief`

Only create or update `product/artifacts/Opportunity-Brief.md` when writing the document adds real value.

If you create or update it, read `references/opportunity-brief-template.md` when you need the canonical template shape, then prefer this section structure:

1. `Context`
2. `Opportunity`
3. `Project Goal`
4. `Stakeholders`
5. `Known Constraints`
6. `Supporting Materials`
7. `Open Questions`

Keep it concise. It should prepare the kickoff, not replace later discovery artifacts.

### 5. Make a recommendation about Vision & Collaboration Goals

State one of:

- `Use existing Vision & Collaboration Goals`
- `Recommend creating Vision & Collaboration Goals`
- `Skip for now`

Recommend creating it only when kickoff quality would materially improve from clarifying:

- product vision
- value proposition
- collaboration expectations
- success criteria
- target users

Do not present it as a required repo output.

### 6. Surface gaps and contradictions

Always produce a short list of:

- missing critical information
- contradictions across sources
- assumptions that still need validation
- questions that should be answered before or during kickoff

Do not hide uncertainty inside polished prose.

## Output Contract

Your output must include all of the following:

### A. Framing status

State one of:

- `Prepared framing from onboarding materials`
- `Created Opportunity Brief draft`
- `Updated existing Opportunity Brief`
- `Kickoff framing already sufficient`

### B. Recommended document target

Use this preference order:

1. existing `product/artifacts/Opportunity-Brief.md`
2. `product/artifacts/Opportunity-Brief.md`
3. markdown draft in the current working context if the repo should not be edited yet

If no document needs to be written, say so explicitly.

### C. Vision & Collaboration Goals recommendation

State:

- recommendation
- reasoning
- minimum unanswered questions

### D. Gaps and contradictions

List only the highest-signal missing pieces.

### E. Next skill

State one of:

- `Next: kickoff-prep`
- `Next: kickoff-closeout`
- `Next: design-research`

Choose based on the actual state of the project.

### F. Human review checklist

End with a short checklist for the responsible person to validate:

- framing of the opportunity
- stakeholder completeness
- constraints accuracy
- whether kickoff can now be prepared
- whether `Vision & Collaboration Goals` adds real value

## Guardrails

Do not:

- force creation of an `Opportunity Brief` when framing is already usable
- treat `Vision & Collaboration Goals` as a required output
- depend on templates outside this skill folder at runtime
- close `management/RISKS.md`
- close `management/ROADMAP.md`
- rewrite `product/PRD.md` as if discovery were already complete
- present assumptions as confirmed facts
- infer stakeholder alignment without evidence

## Success Criteria

The skill succeeds when kickoff framing is usable, important gaps are visible, and the project can move cleanly into `kickoff-prep` without inventing context on the fly.
