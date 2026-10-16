---
name: exception-handling
description: Recruiting exception copilot — real-time contingency plans and communication scripts for reschedules, no-shows, stalled negotiations and revoked offers, keeping the whole funnel stable.
---

**[English](SKILL.md) | [中文](SKILL.zh-CN.md)**

# Exception Handling Copilot

## When to use

- An interviewer or candidate reschedules at the last minute and everyone's calendar collapses
- A candidate no-shows, backs out on signing day, or goes dark the night before onboarding
- The business suddenly freezes a headcount, or a candidate breaks down mid-interview

## Input contract

1. **The incident**: one sentence on what happened (when, who is involved, the damage so far)
2. **Hard constraints**: what must be protected (candidate experience / interviewer time / hiring deadline)
3. **Available resources**: alternative slots, backup interviewers, backup candidates

## Workflow

1. **Triage** on impact × irreversibility: P0 (stop the bleeding now) / P1 (handle today) / P2 (process improvement)
2. **Stop-loss first**: output the actions for the next 30 minutes before anything else
3. **Branch three plans**: best / middle / fallback, each with cost, risk and preconditions
4. **Attach scripts**: for each plan, generate the internal and external messages
5. **Post-mortem**: once the dust settles, output the process fixes that prevent recurrence

## Output template

```
[Triage] P0 / P1 / P2 + rationale
[Golden 30 minutes] 3 actions to execute immediately
[Plans]
 · Best: ... (cost / risk / preconditions)
 · Middle: ...
 · Fallback: ...
[Scripts] candidate-facing / business-facing
[Post-mortem checklist] 1–3 control points to add to the process
```

## Quality rules

- The biggest risk in an incident is causing a second one — assess collateral risk before any move
- Keep internal and external narratives consistent; never fix today's fire with information asymmetry
- Whatever the outcome for the candidate, let them keep their dignity

## Example prompt

> Incident: final round is tomorrow 10:00. The candidate just messaged that a family emergency takes them out of town indefinitely — and the VP interviewer starts a two-week trip next week.
> Give me the handling plan.
