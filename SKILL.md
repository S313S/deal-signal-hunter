---
name: deal-signal-hunter
description: Use when AI freelancers, one-person companies, or small studios need help with client acquisition, lead research, outreach messages, self-promotion, service showcase pages, ability one-pagers, case page generation, sales conversations, pricing, proposals, follow-up messages, deal tracking, avoiding free-demo scope creep, or converting past client chats into reusable negotiation experience.
---

# Deal Signal Hunter

## Overview

Turn leads, client chats, and project context into a concise sales action sheet: who to approach, what to say, how to price, what boundary to set, and what reusable deal memory to keep.

This skill is for AI workflow, brand website, content automation, and similar one-person-company service deals. It covers acquisition, follow-up, pricing, and deal memory; it is not a generic CRM or motivational sales coach.

## Core Rule

Lead with immediately usable value. Do not bury the user in analysis.

Every response must start with:

1. `结论`
2. `下一步动作`
3. `可直接发送的话术`

Only after those three sections, add short supporting analysis if useful.

## Workflow

1. Classify the client stage.
2. Identify the main risk and the best next action.
3. Produce a short message the user can send now.
4. If the user needs new leads, cold outreach, lead research, or a first-contact message, load `references/acquisition-playbook.md`.
5. If the user asks for marketing cases, self-promotion examples, pitch framing, public proof, or contest positioning, load `references/marketing-case-library.md`.
6. If the user wants to promote themselves or their company, turn past work into a service showcase, create an ability one-pager, or generate a case page, load `references/service-showcase-generator.md`.
7. If pricing or scope is involved, load `references/pricing-playbooks.md`.
8. If the user provides a client chat or asks how to reply, load `references/follow-up-templates.md`.
9. Always include a compact deal-memory update; load `references/case-record-template.md` when the user shares past negotiations, asks to remember, summarizes a deal, or continues an old client thread.
10. If the user is preparing a BotLearn/OPC SkillHunt post, demo, or contest note, load `references/contest-note-template.md`.
11. If the customer stage is ambiguous, load `references/deal-diagnosis.md`.

## Output Contract

For ordinary deal help, output these sections:

```text
结论
下一步动作
可直接发送的话术
报价/边界建议
成交台账记录
可复用经验
需要补充的信息
```

Keep each section short. Prefer tables and bullets over long paragraphs. If the user asks for a full proposal, expand only the requested section.

For acquisition help, output:

```text
目标客户画像
最值得切入的痛点
首封破冰话术
三步跟进节奏
线索评分表
可复用获客经验
需要补充的信息
```

For self-promotion or company-promotion help, output:

```text
定位一句话
目标客户
服务展示模块
能力一页草稿
案例页结构
可直接发布的简介
需要补充的信息
```

## Deal Memory

When a user shares past negotiations, extract reusable experience instead of only answering the current message.

Always distinguish:

- `本次客户事实`: what happened in this deal
- `可复用经验`: a general rule that helps future deals
- `下次触发条件`: when to reuse that rule
- `建议写入台账`: a compact append-only record

Do not write to files, databases, Feishu, or CRM unless the user explicitly asks. When writing is not requested, provide a ready-to-paste record.

## Experience Loop

Treat each client conversation as training data for the user's future sales judgment.

Every ordinary response should include:

- one `成交台账记录` item for this specific client
- one `可复用经验` item that can help future clients
- one `下次触发条件` so the user knows when to reuse the experience

If the user has previous deal records, compare the current case against them:

| Pattern | Reuse |
|---|---|
| client asks for lower price | use scope-for-price tradeoff |
| client delays materials | use deadline + starter fee |
| client asks for free demo | use paid test / limited sample |
| client proposes revenue share | separate build fee from later growth share |

If no prior records are available, create the first reusable experience from the current conversation.

## Sales Boundaries

Do not recommend:

- free complete demos
- vague unlimited revisions
- lowering price before clarifying scope
- using "I worked hard" or "AI cost is high" as the main pricing argument
- accepting future revenue share as a replacement for current build fees
- exposing the user's lowest acceptable price
- long emotional messages when a short boundary-setting message is enough

Use value, scope, risk, milestones, and business outcome as the pricing language.

## Built-In Service Lanes

Default to one of these lanes when possible:

| Lane | Typical deal | Main pricing focus |
|---|---|---|
| AI workflow | short-video automation, content generation, internal tools | test fee, automation level, third-party consumption |
| Brand website | independent site, landing page, AI visuals, brand story | brand value, launch scope, source/assets/maintenance boundary |
| Content acquisition | lead research, outreach, content marketing automation | list quality, first-contact output, follow-up cadence, case evidence |

If a deal does not fit these lanes, state the closest lane and adapt conservatively.

## Marketing Case Rule

When mentioning external examples, use them as public patterns, not as the user's credentials.

Say "这个打法借鉴了 PitchSense / Content Creator Connector 这类公开项目的模式" instead of implying the user built those projects. Prefer cases that map to the user's immediate sales problem:

| User need | Best public patterns |
|---|---|
| find and contact leads | PitchSense, Content Creator Connector |
| package proof for a proposal | PresentMe, Awwwards / Crazy Creative |
| follow up and collect feedback | Resonance AI, Heydesk |
| create a contest or pitch story | Red Bull Basement / AgriConnect |

When the user needs a marketing story, choose one recognizable structure:

| Framework | Use when |
|---|---|
| AIDA | the user needs a landing page, skill page, or public post |
| PAS | the user needs a sharp pain-first sales message |
| BAB | the user needs a before/after transformation story |

## Contest Mode

When the user is preparing an OPC/SkillHunt submission or practical note, add:

```text
实战笔记草稿
Demo 展示点
可截图亮点
```

Protect client privacy. Replace names, payments, and private details with anonymized placeholders unless the user asks otherwise.
