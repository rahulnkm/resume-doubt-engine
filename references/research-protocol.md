# Phase 1: market model, clean room

## The clean-room rule

Researchers never see the candidate's resume, bullets, past titles or numbers. If they do, the keywords they return are the candidate's own vocabulary reflected back, which proves nothing and tailors to the wrong thing.

Dispatch each researcher with the target role family and nothing else. Keep fact intake (phase 3) in a separate conversation branch from research.

## What to gather

**Demand side: postings.** 25 to 40 current postings for the role family, read in full, not summaries from an aggregator. Company job boards expose JSON:

- Ashby: `https://api.ashbyhq.com/posting-api/job-board/<org>?includeCompensation=true`
- Greenhouse: `https://boards-api.greenhouse.io/v1/boards/<org>/jobs?content=true`
- Lever: `https://api.lever.co/v0/postings/<org>?mode=json`

Count how many postings use each term. Counts are vocabulary signals, not market statistics, and get labeled that way.

**Hiring side: voices.** People who hire for or work in the role, in their own words: posts, podcast transcripts, newsletters, hiring guides, interview-question threads. Aim for at least 50 distinct sources and prefer practitioners over vendors.

## Source labels

Label every quote with one of:

- **practitioner** - speaking about their own hiring or their own work
- **vendor** - selling a tool, course or recruiting service
- **company** - official posting or careers material
- **unverified** - role could not be confirmed

A vendor quote can still be true. It just cannot be the only support for a chain.

## Rules for researchers

- Quote verbatim, with the link and the speaker. No paraphrase in the quote field.
- Mark anything that could not be re-checked against the source.
- Report blocked sources as blocked, never as empty. Name them in the gaps section.
- Never invent a persona, a fear or a quote to complete the map.

## Gaps disclosure

The map ends with what is missing: blocked domains, personas with no direct voice, quotes that could not be re-checked, and stages of the loop nobody described. A hole that is named is usable. A hole that is papered over corrupts every bullet built on it.
