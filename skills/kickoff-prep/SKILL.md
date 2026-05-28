---
name: kickoff-prep
description: Use when kickoff framing is already usable and Codex needs to turn that context into a focused kickoff agenda, strategic questions, risks to validate, and expected decisions.
domain: discovery
phase: onboarding-kickoff
outputs:
  - product/artifacts/Kick-off-Meeting-Prep.md
recommended_previous:
  - discovery-onboarding
next_steps:
  - kickoff-closeout
---

# Kickoff Prep

Turn usable project framing into a focused `Kick-off Meeting Prep`.

This skill is for preparing a better kickoff conversation, not for polishing a static document. It should leave the team with a clear agenda, the right questions, visible risks, and explicit decisions worth attempting during the meeting.

## When to Use

Use this skill when:
- kickoff has not happened yet
- project framing is already usable
- the team needs a stronger kickoff agenda, talking points, and validation questions
- there is enough context to prepare the meeting, whether it came from `discovery-onboarding`, an external `Opportunity Brief`, or equivalent materials

Do **not** use this skill when:
- kickoff framing is still too weak or contradictory and `discovery-onboarding` should run first
- kickoff already happened and the right next step is `kickoff-closeout`
- the repo already has a solid, current `Kick-off Meeting Prep` and only minor execution is needed

## Required Reading

Read these files before producing output when they exist:

- `docs/PROJECT-SUMMARY.md`
- `management/RISKS.md`
- `product/artifacts/Opportunity-Brief.md`
- `product/artifacts/Kick-off-Meeting-Prep.md`

If one or more files are missing, continue and treat that as missing context rather than a blocker.

## Minimum Inputs

Require usable framing from at least one of these:

- `product/artifacts/Opportunity-Brief.md`
- externally provided `Opportunity Brief`
- framing synthesized by `discovery-onboarding`
- another external document set that already captures the project problem, objective, stakeholders, and constraints

If framing is still too weak to support a useful kickoff, stop and say that `discovery-onboarding` should run first.

## Recommended Inputs

Use these when available:

- externally provided `Vision & Collaboration Goals`
- internal team notes
- commercial or contractual constraints
- prior client questions
- rough MVP ideas or scope assumptions
- known risks already captured in `management/RISKS.md`

Treat `Vision & Collaboration Goals` as optional input, not required output.

## Workflow

### 1. Validate that kickoff prep is the right next move

Confirm that:
- kickoff has not happened yet
- framing is strong enough to prepare the meeting
- the main uncertainty is now about what to validate and decide live

If those conditions are not true, say which skill should come first instead.

### 2. Rebuild the current project framing

Extract and normalize:

- project objective
- problem framing
- target user or stakeholder context
- known constraints
- open questions
- early signals of scope or MVP direction

Treat contradictions as explicit items to validate during the meeting.

### 3. Read the repo's operating context

Use repo context to understand whether kickoff prep should emphasize:

- unresolved risks
- assumptions already captured elsewhere
- dependencies or sequencing concerns
- business, collaboration, or delivery tensions that should be surfaced early

Do not duplicate large sections of existing documentation without improving the structure of the meeting.

### 4. Draft or update the Kick-off Meeting Prep

Produce or update `product/artifacts/Kick-off-Meeting-Prep.md` when it adds value.

The skill should interiorize the expected structure and may read `references/kickoff-meeting-prep-template.md` when it needs the canonical template shape.

Prefer this structure:

1. `Project Snapshot`
2. `Executive Summary`
3. `Main Problem`
4. `Initial Solution Direction`
5. `Preliminary MVP Signals`
6. `Risks To Validate`
7. `Strategic Questions`
8. `Kickoff Objectives`
9. `Expected Decisions`
10. `Agenda`

Keep it practical. The goal is to drive a better meeting, not to produce a polished strategy artifact.

### 5. Build the meeting agenda and decision prompts

Always include:

- a short agenda with clear outcomes per section
- talking points for the facilitator
- strategic questions that reach the real uncertainty
- risks that should be validated live
- decisions worth attempting during the meeting

Do not turn assumptions into decisions. Frame them as items to confirm, reject, or refine.

## Output Contract

Your output must include all of the following:

### A. Kick-off Meeting Prep status

State one of:

- `Created Kick-off Meeting Prep draft`
- `Updated existing Kick-off Meeting Prep`
- `Prepared Kick-off Meeting Prep for review`
- `Kickoff prep blocked — run discovery-onboarding first`

### B. Recommended document target

Use this preference order:

1. existing `product/artifacts/Kick-off-Meeting-Prep.md`
2. `product/artifacts/Kick-off-Meeting-Prep.md`
3. markdown draft in the current working context if the repo should not be edited yet

If you do not write the file directly, say where it should live.

### C. Agenda

Provide a short agenda with:

- topic
- goal of the section
- why it matters now

### D. Strategic questions and risks

List:

- the highest-signal questions to ask
- the main risks to validate during the call
- the decisions worth attempting

### E. Next skill

State one of:

- `Next: kickoff-closeout`
- `Next: discovery-onboarding`

Choose based on the actual state of the project.

### F. Human review checklist

End with a short checklist for the responsible person to validate:

- agenda order
- missing delicate topics
- quality of the strategic questions
- whether preliminary scope is being presented too strongly
- whether kickoff is ready to run

## Guardrails

Do not:

- proceed when framing is too weak and `discovery-onboarding` should run first
- depend on templates outside this skill folder at runtime
- treat `Vision & Collaboration Goals` as a required output
- close `management/ROADMAP.md`
- rewrite `product/PRD.md`
- present preliminary MVP scope as a committed decision
- hide political or stakeholder-sensitive questions

## Success Criteria

The skill succeeds when the team can enter the kickoff with a clear agenda, visible gaps, prioritized questions, and explicit risks and decisions to validate live.
