---
name: resume-screening
description: Intelligent resume screening — structure the role profile, let AI evaluate every resume on one rubric, and get match points, risk flags and a recommendation grade for each candidate.
---

**[English](SKILL.md) | [中文](SKILL.zh-CN.md)**

# Intelligent Resume Screening

## When to use

- A single opening attracts 50+ resumes and manual screening becomes the bottleneck
- Multiple HR partners or interviewers apply inconsistent standards for "a good resume"
- You need an auditable rationale for every reject, not gut feelings

## Input contract

1. **Role profile**: title, hard requirements (degree/years/must-have skills), nice-to-haves, team preferences
2. **Resumes**: anonymized text (strip name, phone, ID number and other sensitive fields)
3. **Optional**: profiles of past top performers as calibration anchors

## Workflow

1. **Deconstruct the role** into four layers: hard gates / core competencies / bonus points / deal-breakers. If information is missing, ask the HR partner — never invent requirements
2. **Extract evidence**: pull objective facts from the resume (companies, titles, projects, metrics) mapped to each layer. Quote the source text only; never fill gaps by imagination
3. **Score on 5 dimensions** (1–5): experience match, skill depth, stability & motivation, growth potential, risk signals
4. **Decide**: output a recommendation grade with a one-line rationale

## Output template

```
[Grade] A strongly recommend / B recommend / C borderline / D reject
[One-line conclusion] ...
[Match points] (up to 3, each citing resume evidence)
[Risk flags] (up to 3: job-hopping, gaps, compensation mismatch, ...)
[Questions to probe] (2–3 items to verify in the interview)
[Scores] experience x/5 · depth x/5 · motivation x/5 · growth x/5 · risk x/5
```

## Quality rules

- Never score on protected characteristics: gender, age, location, marital or family status
- If the resume doesn't say it, output "not mentioned" — never speculate
- Every score must carry evidence traceable to the resume text

## Example prompt

> Role: HRBP, growth team (3–5 yrs, internet industry, familiar with OKRs and org diagnostics)
> Hard gates: bachelor's degree, 3+ years HR experience
> Please screen the following 10 anonymized resumes per this SKILL and output a ranked grade table.
