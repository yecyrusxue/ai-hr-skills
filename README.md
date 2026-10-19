# AI × HR Skills · Recruiting Workflow Skill Library

**[English](README.md) | [中文文档](README.zh-CN.md)**

> Engineering LLM capabilities into reusable recruiting workflows.

A collection of AI Skills covering the full recruiting lifecycle, written in the standard `SKILL.md` agent-skill format. Load any of them into Kimi / Claude / GPT and put them to work in minutes.

Author: [@yecyrusxue](https://github.com/yecyrusxue) · HR (Recruiting)

## Skills

| # | Skill | Stage | What it solves |
|---|-------|-------|----------------|
| 1 | [resume-screening](skills/resume-screening/SKILL.md) | Screening | Structures the role profile, scores every resume on one rubric — HR only reads the resumes worth reading |
| 2 | [talent-mapping](skills/talent-mapping/SKILL.md) | Mapping | Systematic org inference + candidate profiling that turns scattered clues into a searchable talent pool |
| 3 | [candidate-outreach](skills/candidate-outreach/SKILL.md) | Outreach | Personalized first-touch messages that lift reply and show-up rates |
| 4 | [communication-playbooks](skills/communication-playbooks/SKILL.md) | Communication | Structured scripts for first touch, follow-ups, offer negotiation and rejections |
| 5 | [candidate-nurturing](skills/candidate-nurturing/SKILL.md) | Nurturing | Cadenced care plans that keep long-cycle candidates from going cold |
| 6 | [exception-handling](skills/exception-handling/SKILL.md) | Exceptions | Real-time playbooks for reschedules, no-shows and stalled negotiations |

## System map

The six skills are not a grab bag — each one takes a position on the recruiting funnel, and all of them share a single input/output contract, so the output of one stage becomes the input of the next:

```
SOURCING            SCREENING            ENGAGEMENT                OFFER & BEYOND
──────────────      ───────────────      ─────────────────────     ─────────────────────
talent-mapping  →   resume-screening  →  candidate-outreach     →  communication-playbooks
                                         (first touch)             (negotiation · rejection)
                                              ↓
                                     candidate-nurturing  ····▶  exception-handling
                                     (long-cycle care)          (spans every stage)
```

The funnel is the system: structured input in, structured output out, at every stage.

## Design principles

- **AI as leverage, humans as judges** — Skills handle structure, scale and memory; HR keeps insight, empathy and the final call
- **Embedded in the funnel, not bolted on** — every Skill anchors to a specific recruiting stage and hands structured output to the next
- **Reusable and iterable** — uniform input/output contracts so new teammates are productive on day one, and hard-won lessons get encoded into prompts

## How to use

1. Open the `SKILL.md` of the skill you need
2. Paste the full text into any major LLM (Kimi / Claude / GPT, etc.)
3. Provide your role and candidate materials per the **Input Contract**
4. Review the structured output and make the final decision yourself

## Disclaimer

This repository contains generic methodology only — no proprietary company data and no candidate PII. When using these skills, process candidate information in compliance with applicable privacy laws (e.g. PIPL/GDPR): anonymize first, collect the minimum necessary.

## License

MIT
