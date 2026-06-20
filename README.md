# 成交信号捕手

`deal-signal-hunter` 是一个面向 AI 自由职业者、一人公司和小型工作室的 BotLearn / OPC 销售流程 Skill。

它帮助个人识别客户需求、包装服务方案、生成报价话术、推进跟单复盘，把每一次客户沟通沉淀成可复用的成交经验。

## 适合谁

- AI 自由职业者
- 一人公司创始人
- 小型工作室主理人
- 正在接品牌站、AI 工作流、内容自动化、获客自动化项目的人
- 需要自己完成获客、报价、跟进和复盘的服务型个人

## 它解决什么问题

一人公司经常不是不会交付，而是卡在成交前：

- 不知道该先联系哪类客户
- 第一封破冰消息写得太泛
- 客户问价格时不知道怎么拆报价
- 客户要求免费完整 Demo 时不知道怎么设边界
- 客户拖延资料和付款时不知道怎么推进
- 客户提出“后续分成”时，不知道怎么保护当前建设费
- 每次谈单经验都散落在聊天记录里，下次又重新判断

## 它会输出什么

输入潜在客户线索或客户聊天记录后，它会把信息整理成一份可执行的售前行动单。

跟进 / 谈单场景会输出：

1. 结论
2. 下一步动作
3. 可直接发送的话术
4. 报价 / 边界建议
5. 成交台账记录
6. 可复用经验
7. 下次触发条件

获客场景会输出：

1. 目标客户画像
2. 最值得切入的痛点
3. 首封破冰话术
4. 三步跟进节奏
5. 线索评分表
6. 可复用获客经验

自我推广 / 服务展示场景会输出：

1. 定位一句话
2. 目标客户
3. 服务展示模块
4. 能力一页草稿
5. 案例页结构
6. 可直接发布的简介

## 推荐使用方式

这个 Skill 不只适用于 BotLearn。只要你的 Agent 支持读取 GitHub 仓库、Markdown 指令文件，或可以粘贴系统提示词，就可以使用。

如果你的 Agent 已经安装 / 导入了这个 Skill，直接使用：

```text
Use $deal-signal-hunter to turn my lead or client chat into a concise sales action sheet and reusable deal memory.

客户/线索类型：
客户最新聊天记录或公开线索：
我已经做了什么：
我最纠结的问题：
```

如果你的 Agent 还没有安装这个 Skill，可以复制下面这段提示词，让它临时读取 GitHub 仓库后再执行：

```text
请使用这个 GitHub 仓库里的 Skill 帮我处理售前问题：

https://github.com/S313S/deal-signal-hunter

请先读取仓库根目录的 SKILL.md，并按其中的规则工作。
如果需要参考资料，请读取同仓库 references/ 目录下的相关文件。

我的需求是：把下面的客户线索或客户聊天记录，整理成一份可执行的售前行动单。

请按这些栏目输出：
1. 结论
2. 下一步动作
3. 可直接发送的话术
4. 报价 / 边界建议
5. 成交台账记录
6. 可复用经验
7. 下次触发条件

客户/线索类型：
客户最新聊天记录或公开线索：
我已经做了什么：
我最纠结的问题：
```

## 示例 1：客户提出“后续分成”

```text
客户项目类型：
品牌独立站 + AI 视觉 + 前端上线

客户最新表达：
费用能不能再优化一些？我们现在也是初期阶段。后面如果网页产生营业额，你可以占一定百分比，这样对双方长期合作也比较好。

我已经做了什么：
已经帮客户做了品牌视觉方向、AI 氛围图、页面结构、文案和前端预览。之前只有少量辛苦费，还没有正式结算。

我最纠结的问题：
我不想直接拒绝长期合作，但也不想让未来不确定分成替代当前建设费。
```

这个场景下，Skill 会重点判断：

- 客户不是直接拒绝，而是在降低前期现金支出
- 核心风险是用未来不确定收益替代当前建设费
- 当前基础建设费和后续分成需要分开谈
- 如果降价，必须同步缩小范围或限定维护期

## 示例 2：生成获客破冰消息

```text
潜在客户类型：
小型品牌方，有官网/社媒内容，但页面展示和客户跟进路径比较弱。

我能提供：
AI 工作流、品牌独立站、内容自动化和售前跟进经验沉淀。

我最纠结的问题：
我不想一上来就说“我能帮你做 AI”，想找到一个客户更容易理解的切入点。
```

这个场景下，Skill 会输出：

- 目标客户画像
- 最值得切入的痛点
- 首封破冰话术
- 三步跟进节奏
- 线索评分表
- 可复用获客经验

## 设计重点

成交信号捕手不是普通销售话术生成器。它更像一个面向一人公司的售前判断框架。

每次输出都会尽量区分三件事：

| 层级 | 作用 |
| --- | --- |
| 本次客户事实 | 方便继续跟进当前客户 |
| 可复用经验 | 方便下次遇到类似客户时直接套用 |
| 下次触发条件 | 让你知道什么时候该复用这条经验 |

这样用户不是每次都从聊天记录里重新判断，而是在逐步建立自己的成交经验库。

## 隐私提醒

使用真实客户案例前，请先做匿名处理：

- 去掉客户姓名、公司名、微信号、手机号等身份信息
- 模糊具体金额、报价和内部计划
- 不暴露客户未公开的商业安排
- 公开发帖时只保留必要上下文和经过脱敏的聊天片段

## 项目结构

```text
SKILL.md
agents/openai.yaml
references/acquisition-playbook.md
references/case-record-template.md
references/contest-note-template.md
references/deal-diagnosis.md
references/follow-up-templates.md
references/marketing-case-library.md
references/pricing-playbooks.md
references/service-showcase-generator.md
```

## 参赛与推广资料

```text
demo.md
submission.md
botlearn-submission-page-pack.md
peer-evaluation-kit.md
practical-note-flagship.md
practical-note-acquisition.md
screenshot-board.html
contest-launch-plan.md
judge-comments.html
```

## BotLearn 导入方式

```text
Repository URL: https://github.com/S313S/deal-signal-hunter
Branch: main
Subpath: 留空
```

仓库根目录已经包含 `SKILL.md`，导入时不需要填写子路径。

## 其他 Agent 接入方式

这个仓库是纯 Skill 包，不需要安装 npm、Python 或其他运行时依赖。只要你的 Agent 平台支持加载 Markdown Skill / system prompt / instruction bundle，就可以按下面方式接入：

```text
Skill name: deal-signal-hunter
入口文件: SKILL.md
参考资料目录: references/
默认调用: Use $deal-signal-hunter ...
```

接入时需要保证：

- `SKILL.md` 位于 Skill 根目录。
- `references/` 和 `SKILL.md` 保持同级目录。
- Agent 能读取 `references/*.md`，因为 `SKILL.md` 会按场景加载这些参考资料。
- 如果平台支持 YAML 元数据，可以参考 `agents/openai.yaml` 里的展示名、简介和默认 Prompt。

最小可用配置示例：

```yaml
name: deal-signal-hunter
entrypoint: SKILL.md
references: references/
description: 识别客户需求、包装服务方案、生成报价话术和跟单复盘
```

注意：这个仓库不会自动让所有 Agent“自注册”。外部 Agent 仍然需要在自己的平台里配置入口文件或导入这个 GitHub 仓库。配置完成后，它不需要额外代码即可使用。
