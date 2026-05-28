---
name: kickoff-closeout
description: Use after kickoff when notes, transcript evidence, or decisions exist and Codex needs to turn that evidence into reliable project memory without overstating certainty.
domain: discovery
phase: onboarding-kickoff
outputs:
  - docs/PROJECT-SUMMARY.md
  - management/RISKS.md
  - product/artifacts/Kickoff-Closeout-Summary.md
recommended_previous:
  - kickoff-prep
next_steps:
  - design-research
---

# Kickoff Closeout

Turn kickoff evidence into reliable project memory.

This skill is not for writing a polished meeting recap. Its purpose is to separate what the kickoff actually clarified from what remains open, then update the project's living context without inventing certainty.

## When to Use

Use this skill when:
- kickoff already happened
- there are usable notes, transcript excerpts, decisions, or follow-ups
- the team needs to update project memory before starting `design-research`
- context from the kickoff is still trapped in chat, calls, or scattered notes

Do **not** use this skill when:
- kickoff has not happened yet
- there is still no usable evidence from the meeting
- the right next step is `kickoff-prep`
- the project already moved far beyond kickoff and another artifact now supersedes it

## Required Reading

Read these files before producing output when they exist:

- `docs/PROJECT-SUMMARY.md`
- `management/RISKS.md`
- `management/ROADMAP.md`
- `product/artifacts/Kick-off-Meeting-Prep.md`
- `product/artifacts/Kickoff-Closeout-Summary.md`

If one or more files are missing, continue and treat that as missing context rather than a blocker.

## Minimum Inputs

Require usable kickoff evidence from at least one of these:

- kickoff notes
- full or partial transcript
- decisions captured live
- action items or follow-ups
- another reliable post-kickoff summary

`Kick-off-Meeting-Prep.md` is helpful when it exists, but it is **not required**.

If the meeting has not happened yet, or if only raw audio exists with no usable notes or transcript, stop and say that `kickoff-closeout` should not proceed yet.

## Evidence Rules

Treat source reliability explicitly:

- prefer direct quotes or transcript-backed statements over paraphrases
- prefer confirmed decisions over speculative remarks
- treat facilitator assumptions as assumptions unless the meeting clearly validated them
- if sources disagree, surface the inconsistency instead of resolving it silently

## Workflow

### 1. Confirm that closeout is possible

Verify that:
- kickoff actually happened
- there is enough usable evidence to reconstruct what changed
- the project still benefits from updating kickoff-level memory before `design-research`

If not, say what is missing.

### 2. Reconstruct what the kickoff actually clarified

Extract:

- confirmed decisions
- unresolved questions
- commitments or follow-ups
- newly surfaced risks
- reframed project goals or constraints

Separate what was discussed from what was actually decided.

### 3. Compare expected vs. actual outcome when prep exists

If `product/artifacts/Kick-off-Meeting-Prep.md` exists, compare:

- what the team wanted to validate
- what the meeting really answered
- what remains open

If no prep exists, skip this comparison and work directly from the available evidence.

### 4. Produce a structured kickoff summary

Create a concise summary with this preferred structure:

1. `What Was Confirmed`
2. `What Changed`
3. `Open Questions`
4. `Risks And Constraints`
5. `Next Actions`

Do not optimize for elegant prose. Optimize for recoverable project memory.

### 5. Update canonical project memory

Prepare concrete updates for:

- `docs/PROJECT-SUMMARY.md`
- `management/RISKS.md`
- `management/ROADMAP.md` only when the kickoff justifies a first preliminary sequence of work

Treat roadmap updates carefully:

- do not imply planning certainty that the meeting did not create
- do not sequence work beyond what the evidence supports
- make it explicit when a roadmap note is provisional

### 6. Mark uncertainty explicitly

Always distinguish between:

- confirmed decision
- likely interpretation
- unresolved ambiguity
- follow-up required

If a single stakeholder expressed a view but no agreement was reached, do not write it as project consensus.

## Output Contract

Your output must include all of the following:

### A. Kickoff closeout status

State one of:

- `Created kickoff closeout summary`
- `Updated kickoff closeout summary`
- `Prepared kickoff closeout summary for review`
- `Kickoff closeout blocked — usable meeting evidence missing`

### B. Structured kickoff summary

Include:

- confirmed decisions
- open questions
- new or reframed risks
- next actions

### C. Proposed canonical updates

Provide proposed updates for:

- `docs/PROJECT-SUMMARY.md`
- `management/RISKS.md`
- `management/ROADMAP.md` when applicable

If one of these should not be updated yet, say why.

### D. Confidence and ambiguity notes

List:

- low-confidence interpretations
- places where the transcript or notes are incomplete
- decisions that still need explicit confirmation

### E. Next skill

State one of:

- `Next: design-research`
- `Next: kickoff-prep`
- `Next: gather better kickoff evidence`

Choose based on the actual state of the project.

### F. Human review checklist

End with a short checklist for the responsible person to validate:

- no invented consensus
- no isolated opinion presented as a decision
- risks and commitments correctly interpreted
- roadmap not made more certain than the evidence allows
- research can now start without depending on oral context

## Guidance for `management/RISKS.md`

When proposing or updating risks, prefer this structure:

1. Risk
2. Why it matters
3. Current evidence
4. Impact
5. Likelihood
6. Mitigation
7. Owner
8. Status
9. Review trigger / next check

## Guardrails

Do not:

- proceed before the meeting happened
- require `Kick-off-Meeting-Prep.md` when usable kickoff evidence exists without it
- depend on templates outside this skill folder at runtime
- treat raw audio as usable evidence without notes or transcript
- rewrite `product/PRD.md`
- rewrite `product/USER-STORIES.md`
- rewrite design or technical specs as if Discovery were already complete
- present a tentative interpretation as confirmed agreement

## Success Criteria

The skill succeeds when kickoff evidence has been converted into reliable project memory, important uncertainties remain visible, and the repo is cleanly prepared to move into `design-research`.
