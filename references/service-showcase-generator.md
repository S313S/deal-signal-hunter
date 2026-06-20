# Service Showcase Generator

Use this reference when the user wants to promote themselves or their company, turn past work into a public-facing service explanation, create an ability one-pager, or generate a case page from messy project material.

## Core Principle

Do not output a generic brand profile. Convert the user's work into a customer-facing proof asset.

The output must answer:

1. who this helps
2. what painful workflow it improves
3. what the user can deliver
4. what proof or artifact supports the claim
5. what the customer should do next

## Input Checklist

If information is missing, still draft a usable version and mark gaps.

| Field | What to ask for |
|---|---|
| 服务对象 | industry, role, company size, current stage |
| 典型痛点 | lead generation, content, website, support, follow-up, reporting |
| 已有作品 | links, screenshots, GitHub, demos, documents, client chats |
| 可验证证据 | before/after, demo, public case note, public page, testimonial, metric |
| 交付边界 | what is included, what is excluded, timeline, starter package |

## Output Contract

```text
定位一句话
目标客户
服务展示模块
能力一页草稿
案例页结构
可直接发布的简介
需要补充的信息
```

Keep the first draft short enough to paste into a Skill page, GitHub README, portfolio page, or client proposal.

## Service Showcase Modules

Use these modules in this order:

| Module | Purpose | Prompt |
|---|---|---|
| Hero line | explain the service in one sentence | 我帮 <客户类型> 把 <痛点流程> 做成 <结果> |
| Problem | show the customer you understand the pain | 你现在可能不是缺工具，而是 <断点> |
| Service | describe the deliverable | 我会交付 <具体资产/流程/系统> |
| Proof | make it credible | 可展示的证据是 <demo/case/before-after/page> |
| Next step | reduce friction | 先做 <小范围动作>，再决定是否扩展 |

## Ability One-Pager

```markdown
# <服务名>

## 一句话定位
我帮 <目标客户> 把 <低效/混乱流程> 变成 <可复用/可展示/可跟进系统>。

## 适合谁
- <客户类型 1>
- <客户类型 2>
- <客户类型 3>

## 能解决什么
| 痛点 | 交付物 | 客户得到什么 |
|---|---|---|
| <痛点 1> | <交付物 1> | <业务结果 1> |
| <痛点 2> | <交付物 2> | <业务结果 2> |

## 可展示证据
- Demo:
- GitHub / 页面:
- 截图 / 前后对比:
- 客户反馈 / 公开案例:

## 起步合作
先做 <小范围试点>，交付 <明确产物>，再按结果扩展。
```

## Case Page Generator

Use this when the user gives a past project, client chat, folder, screenshot, or delivery note.

```markdown
# 案例：<客户类型> 的 <问题> 改造

## 改造前
- <流程混乱点>
- <沟通/获客/内容/客服断点>
- <客户可感知损失>

## 我做了什么
- <动作 1>
- <动作 2>
- <动作 3>

## 改造后
- <更清晰的客户路径>
- <可复用的内容/话术/系统>
- <下一步可扩展方向>

## 可复用经验
<一句话总结这个案例以后怎么复用>

## 可对外展示版本
<匿名、短、能放到作品集或提案里的版本>
```

## Publishing Versions

### Skill Page Version

```text
这个 Skill 帮一人公司把线索、客户聊天和过往项目转成可直接使用的售前动作：获客切入点、报价边界、跟进话术、案例页和成交台账。它不是泛泛分析，而是优先输出下一步动作和可直接发送的话术。
```

### GitHub README Version

```text
Deal Signal Hunter is a sales workflow Skill for one-person companies. It helps AI freelancers and small studios turn messy leads, client chats, and project notes into outreach messages, pricing boundaries, follow-up plans, service one-pagers, case pages, and reusable deal memory.
```

### Client Proposal Version

```text
我可以先帮你把现有资料整理成一个小型售前展示包：一页服务说明、一个可对外案例页、三条客户跟进话术。这样你不用先做完整系统，也能更快看见这个方向是否值得继续投入。
```

## Guardrails

Do not:

- invent client names, metrics, awards, or testimonials
- claim public cases as the user's own work
- write vague slogans such as "empower business with AI"
- make the showcase only about tools or models
- hide the next step at the end of a long analysis

Use anonymized evidence when the user has real but private material.
