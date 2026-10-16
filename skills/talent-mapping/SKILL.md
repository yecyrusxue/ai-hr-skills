---
name: talent-mapping
description: Talent mapping — run systematic talent landscaping against target companies and roles, producing structured candidate profiles and outreach priorities that compound into a searchable talent pool.
---

**[English](SKILL.md) | [中文](SKILL.zh-CN.md)**

# Talent Mapping

## When to use

- A critical role stays open long-term and you need the full talent landscape of target companies
- A new business line launches and you must answer "where are the people, and who is worth a call" fast
- The talent pool needs to graduate from "a pile of resumes" to a searchable relationship network

## Input contract

1. **Target role**: level, core competencies, list of benchmark companies
2. **Available clues**: candidate fragments from public sources (Maimai/LinkedIn/company sites/talks/papers)
3. **Purpose**: immediate hire / pipeline building / market intelligence

## Workflow

1. **Infer the org chart** of each target company from public information; tag every inference with a confidence level
2. **Structure profiles**: file each candidate's fragments into the unified fields (see template)
3. **Prioritize** on three axes — fit × reachability × likelihood to move — and tag P0/P1/P2
4. **Gap analysis**: list uncovered departments and levels to guide the next search round

## Output template

```
[Candidate profile] (anonymized ID, e.g. P-001)
· Current: company / team / level / reporting line (confidence: high/med/low)
· Background: career arc, signature projects, verifiable achievements
· Motivation signals: tenure, recent activity, possible move windows
· Outreach plan: channel, opening angle, referral path
· Priority: P0 / P1 / P2 + one-line rationale
```

## Quality rules

- Public sources only — no pretexting, no deception, no privacy invasion
- Every fact carries a source and a confidence tag; never present inference as fact
- Keep pool fields uniform so a teammate can take over without a handover

## Example prompt

> Target role: multimodal algorithm expert (P7 equivalent)
> Benchmark companies: A, B, C
> Based on public information, infer the relevant team structures for each company, structure the following 20 clues into standard profiles, and output the P0 shortlist.
