# Case Record Template

Use this reference when converting chats into reusable deal memory.

## Principle

Every client conversation should leave two assets:

1. A deal record for this client.
2. A reusable business rule for future clients.
3. A trigger phrase that helps the user recognize the pattern next time.

Keep records append-only. Do not rewrite history unless the user asks.

## Deal Record

```markdown
## 案例：<客户/项目匿名名>

### 客户需求

### 当前阶段

### 客户心理

### 已发送报价

### 推荐报价策略

### 交付范围

### 不包含项

### 付款方式

### 后续跟进话术

### 最新进展

### 可复用经验
```

## Reusable Experience

Use this compact pattern:

```markdown
### 经验：<一句话规则>

- 触发条件：
- 客户信号：
- 错误做法：
- 推荐做法：
- 可复用话术：
```

Examples:

```markdown
### 经验：分成不能替代基础建设费

- 触发条件：客户提出后续营业额分成，想降低当前固定费用。
- 客户信号：认可长期合作，但当前预算或付款优先级不足。
- 错误做法：口头答应分成并继续免费推进。
- 推荐做法：基础建设费先结算，分成作为上线后增值合作另谈。
- 可复用话术：分成后面可以聊，但建议和当前基础建设费用分开。
```

```markdown
### 经验：拖延补资料时要切换到付款门槛

- 触发条件：客户多次说会补资料，但没有明确时间和付款动作。
- 客户信号：认可方向，但项目优先级不足。
- 错误做法：继续生成完整方案或深度 Demo。
- 推荐做法：发资料清单、截止日、启动款和重新排期规则。
- 可复用话术：资料和启动款确认后，我再排具体交付时间。
```

## Output Format

When the user asks to remember or continue a deal, output:

```text
建议追加到台账
可复用经验
下次触发条件
下一步动作
```

If a file path is provided, ask before writing. If no explicit write request exists, provide ready-to-paste Markdown only.

## Readability Rules

Keep the record useful under pressure:

- write facts in short bullets
- keep one experience to one rule
- do not store raw full chat unless the user asks
- do not mix private client facts into the general reusable rule
- prefer "next time, when X happens, do Y" over abstract lessons

## Experience Extraction Examples

| Client signal | Reusable rule |
|---|---|
| "后面有营业额给你分成" | Separate current build fee from later growth share. |
| "你先做个完整 demo 我看看" | Offer paid test or limited sample; do not deliver full workflow for free. |
| "资料我过两天发你" then no follow-up | Set deadline, starter fee, and re-quote/re-schedule rule. |
| "为什么这么贵" | Explain scope, risk, value, and alternatives; do not defend with personal effort. |
