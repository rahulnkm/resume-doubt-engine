---
name: resume-doubt-engine
description: Use when writing, rewriting, auditing or tailoring a resume, CV or its bullets for a target role, when deciding which experiences to keep or cut, or when asking what a resume is missing before applying.
---

# Resume Doubt Engine

## Overview

The candidate is the product. The hiring committee is the market. Every bullet exists to flip one specific doubt in one specific reader's head, and the proof behind it carries that reader's own words.

A bullet that kills no doubt gets cut. A number that cannot be verified never gets written.

## The six phases

Run them in order. Each ends at a gate the user answers before the next starts.

1. **Market model (clean room)** - research the target role's hiring committee from postings and hiring-side voices. The researchers never see the candidate's resume. See `references/research-protocol.md`.
2. **Committee map** - turn research into doubt chains, one per persona per fear, plus a rollup ranking proofs by how many personas each wins over. Schema and persona checklist in `references/committee-map.md`.
3. **Fact intake** - fill `assets/facts-template.md` from the candidate. Copy it into the working directory and fill it each run; never carry facts over from an old run or from memory without re-confirming them.
4. **Keyword sheet** - cross-check three sources: the clean-room map, the specific job description, and what recruiters and tracking systems search on. Both sides of every chain, the doubt words and the proof words, get carried. See `references/keyword-sheet.md`.
5. **Bullet construction** - write bullets under `references/bullet-style.md`, ordered by the rule below.
6. **Audit** - produce the three tables in `references/audit-format.md`: bullet-to-doubt matrix, coverage across every doubt, then gaps, quick fixes, fact-check landmines and ranked story prompts.

Editing a resume hosted in resume.lol: `references/resume-lol.md`.

## Ordering rule: obvious to subtle

Within a role, the doubts the bullets answer run from **most obvious at the top to least obvious at the bottom**.

The most obvious doubt is the one a skeptical reader forms from the role's header alone: title, company, dates, industry. The direction has to hold all the way down. Exact ranking does not matter, so 1-2-3-4-5 and 1-1-3-5-5 are both fine; 1-4-2-5 is not.

Test before locking a role: read its header line out loud, write the first three questions a skeptical reader asks, and check that the first bullet answers one of them. Never put a subtle doubt above an obvious one because its bullet is stronger.

When two bullets answer doubts of equal obviousness, the stronger proof goes first.

Obviousness ladder, most to least: doubts the header line itself raises (unknown company, short tenure, title that outruns the scope, solo work, seniority) → doubts about whether the core job was actually done → doubts about craft and depth → doubts about working with other people.

## Hook preference: result first

Each bullet is a Pain, a Problem, a Solution or a Result, and it opens with that. When the facts support more than one framing, pick the highest one on this ladder:

1. **Result** - the outcome and its number
2. **Solution** - the thing built and why it was clever
3. **Problem** - the knot that had to be untangled
4. **Pain** - the thing that was hurting

Drop a rung only when the rung above is not honestly available: no measured outcome, no built artifact, and so on. Never open with the pain when a real result exists.

This is a separate axis from the ordering rule. Obviousness decides which bullet goes where in the role; the ladder decides how each bullet opens.

## Hard rules

- Never invent a number, a user, a customer or a technique. Unknowns become questions for the candidate or things to go build.
- Every keyword must be true for the candidate. An untrue keyword is a gap, not a word choice.
- Every euphoria point and proof maps one-to-one to a mapped doubt. Free-floating virtues ("taste", "cost discipline") are irrelevant and get cut or reframed.
- Never cite test counts, node counts or other volume metrics as proof. Reviewers read them as inflation.
- Flag, in the audit and not silently, any claim a reader could check and find wrong.
- Apply agreed changes straight to the live resume, then report what changed. Verify after reload: page count, orphan lines, and that every edit saved. Ask first only when a change rests on a fact the candidate has not confirmed.

## Red flags - stop

- Writing a bullet before the doubt it kills is named.
- A number that came from a previous conversation rather than from the candidate this run.
- Researchers who have seen the resume, so the keywords echo it back.
- Two bullets on the same doubt while another doubt has none.
- A role whose bullets get more obvious as they go down.
