# resume-doubt-engine

A Claude Code skill for writing, auditing and tailoring resumes.

The idea: the candidate is the product and the hiring committee is the market. Every bullet has to flip one specific doubt in one specific reader's head. A bullet that answers no doubt gets cut, and a number that cannot be verified never gets written.

## What it does

Six phases, each ending at a gate you answer before the next starts:

1. **Market model** - research the target role's hiring committee from job postings and hiring-side voices, without ever showing the researchers your resume.
2. **Committee map** - turn that research into doubt chains per persona (recruiter, hiring manager, technical evaluator, etc.).
3. **Fact intake** - fill a facts template with only what you confirm this run.
4. **Keyword sheet** - cross-check the map, the specific job description and recruiter search terms.
5. **Bullet construction** - write bullets ordered from most obvious doubt to least, each opening on its strongest honest hook.
6. **Audit** - bullet-to-doubt matrix, coverage, quick fixes, fact-check landmines and story prompts.

## Install

```bash
git clone https://github.com/rahulnkm/resume-doubt-engine ~/.claude/skills/resume-doubt-engine
```

Claude Code picks it up automatically. Ask it to audit or rewrite your resume for a target role.

## Files

- `SKILL.md` - the workflow and hard rules
- `references/` - per-phase protocols
- `assets/` - templates for the committee map and fact intake

## License

MIT
