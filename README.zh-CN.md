# AI × HR Skills · 招聘全流程 AI 技能库

**[English](README.md) | [中文文档](README.zh-CN.md)**

> 把大模型能力工程化，沉淀为招聘团队可复用的生产力资产。
> Engineering LLM capabilities into reusable recruiting workflows.

一套覆盖招聘全生命周期的 AI Skills 合集，采用业界通用的 `SKILL.md` 智能体技能格式编写，可直接加载到 Kimi / Claude / GPT 等大模型中使用。

作者：薛烨 · HR（招聘方向）

## 技能清单

| # | Skill | 场景 | 解决什么 |
|---|-------|------|----------|
| 1 | [resume-screening](skills/resume-screening/SKILL.md) | 简历初筛 | 岗位画像结构化 → 按维度打分，HR 只看最值得看的简历 |
| 2 | [talent-mapping](skills/talent-mapping/SKILL.md) | 人才 Mapping | 目标公司/岗位的系统化人才盘点与画像沉淀 |
| 3 | [candidate-outreach](skills/candidate-outreach/SKILL.md) | 邀约外联 | 千人千面的个性化触达，提升到面率 |
| 4 | [communication-playbooks](skills/communication-playbooks/SKILL.md) | 沟通话术 | 首触/跟进/offer 谈判/拒信安抚的全周期话术资产 |
| 5 | [candidate-nurturing](skills/candidate-nurturing/SKILL.md) | 跟进保温 | 长周期候选人的节奏化维护，防止流失 |
| 6 | [exception-handling](skills/exception-handling/SKILL.md) | 异常处置 | 改期/爽约/谈薪僵持等突发场景的预案生成 |

## 体系结构

六个技能不是散点，而是按招聘漏斗一一卡位，共用同一套输入输出契约——上一环节的产出，即下一环节的输入：

```
寻访                筛选                 触达与沟通                 offer 及之后
──────────────      ───────────────      ─────────────────────     ─────────────────────
talent-mapping  →   resume-screening  →  candidate-outreach     →  communication-playbooks
                                         （首触邀约）              （谈判 · 拒信）
                                              ↓
                                     candidate-nurturing  ····▶  exception-handling
                                     （长周期保温）              （贯穿全流程）
```

漏斗即体系：每个环节都是结构化输入、结构化输出。

## 设计理念

- **AI 做杠杆，人做判断**：Skills 负责结构化、规模化、不遗忘；HR 负责洞察、共情与最终决策
- **嵌入流程而非外挂**：每个 Skill 都锚定招聘漏斗的具体环节，输出直接对接下一步动作
- **可复用可迭代**：统一输入输出契约，团队新人开箱即用，踩过的坑沉淀进提示词

## 使用方法

1. 打开对应技能的 `SKILL.md`
2. 将全文粘贴给任意主流大模型（Kimi / Claude / GPT 等）
3. 按「输入契约」提供你的岗位信息与候选人材料
4. 拿到结构化输出后，由 HR 做最终判断

## 声明

本仓库为通用方法论沉淀，不含任何公司的机密信息、内部数据与候选人隐私。使用前请确保候选人信息的处理符合《个人信息保护法》要求：脱敏在先，最小必要。

## License

MIT
