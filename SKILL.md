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

## Ordering rule: real proof first

Within a role, bullets go in this order:

1. **Real users or a measured result.** Test cases, demos and internal runs are not users. A bullet that only looks like it answers "does anyone use it?" does not get the top slot.
2. **A system someone else now runs** goes before work only the candidate did.
3. **With no users, the build with a named company and numbers** goes first among the builds.
4. **Breadth before plumbing:** where it was applied goes before monitoring, cost tracking or data access.
5. **Exception, first hire or sole owner of a function:** a bullet stating that scope ("Stood up marketing as the sole marketing hire at...") goes above everything, then the rules above. It answers the header's "how big was this job?" before the number. Only when the facts state the scope outright; never invent a scope bullet.

When these rules do not decide, obvious doubts go above subtle ones. The most obvious doubt is the one a skeptical reader forms from the role's header alone: title, company, dates, industry. Obviousness ladder, most to least: doubts the header raises (unknown company, short tenure, title that outruns the scope, solo work, seniority) → whether the core job was actually done → craft and depth → working with other people. When two bullets tie on both, the stronger proof goes first.

Jobs come first on the page, then side projects and open source, then education and skills.

## Hook: a verb, then the result

Every bullet opens with a plain past-tense verb. Never open with the number itself: "Revenue grew 4x..." or "6 of 40 questions..." reads as AI-written.

- **Measured result exists:** a result verb, the number, then "by" and how. "Grew trial-to-paid conversion from 4% to 9% by..." Keep all of the how, even at 2 lines.
- **No measured result:** "Built [thing] that [does a, b and c]." Never word it so it implies an outcome nobody measured.
- **Stopped on purpose:** "Ran [thing]..., then killed it after data showed..." The kill goes at the end, never as the opening verb.

Full house style in `references/bullet-style.md`.

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
- A test case, demo or internal run placed above real proof as if it were a user.
- A rewrite that reads like a different author from the candidate's own untouched bullets.
