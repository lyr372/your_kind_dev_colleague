# AI Tech Colleague Skill

这是一个面向非技术业务同学的 AI skill，用来在 AI 化转型需求早期，帮你像私下请教技术同事一样把想法说清楚、判断能不能先做、拆出第一版试点方案，并准备好和领导或研发沟通的表达。

只要你的 AI 工具支持 skill，就可以参考本仓库使用。Codex 是其中一种使用方式。

## 适合解决什么问题

- 判断一个 AI 想法是否适合先试点。
- 把模糊业务需求拆成 AI 能做什么、系统该做什么、人工要确认什么。
- 设计第一版 MVP，避免一开始就做成复杂系统。
- 说明需要准备哪些数据、接口、权限、规则、样本和审核人。
- 判断已有 skill、API、OCR、SQL、CRM、页面自动化、脚本或文档能不能复用。
- 用通俗语言解释必要的 AI 概念，比如知识库问答、OCR、接口、页面自动化、自然语言查数。
- 帮你整理给领导或技术团队的沟通话术。

## 使用方式

把本包里的 `ai-tech-colleague` 文件夹放到你的 AI 工具支持的 skills 目录中即可。

如果使用 Codex，可以复制到 Codex skills 目录：

```powershell
Copy-Item -Recurse -Force .\ai-tech-colleague "$env:USERPROFILE\.codex\skills\ai-tech-colleague"
```

重启或刷新对应 AI 工具后，就可以直接用它提问。

## 推荐问法

```text
我想让 AI 自动整理一批业务反馈，判断哪些是高优先级问题，这个方向能做吗？
```

```text
前同事留下了一个 SQL skill 和接口文档，我想用它做自动取数，怎么判断还能不能复用？
```

```text
我们现在规则还不清楚，是先整理数据，还是先做一个 AI demo？
```

```text
这个需求我想汇报给领导，怎么说既体现价值又不夸大？
```

## 理想回答会包含什么

skill 会尽量用业务同学能听懂的话回答：

- 一句话结论；
- 为什么这样判断；
- 第一版 MVP 怎么做；
- 需要准备哪些数据、接口、权限、规则和协作人；
- AI 适合负责什么；
- 哪些地方必须人工确认或由原系统兜底；
- 可以怎么跟领导或技术同事说。

## 使用边界

- 不建议让 AI 绕过权限、猜接口、直接修改业务系统数据。
- 高风险写入、审批、处罚、赔付、客户记录、财务或人事相关动作，第一版都应保留人工确认。
- 业务名词、指标口径和系统字段，应以公司内部实际定义为准。
- 如果数据很乱、规则不清，建议先整理最小样本和最小规则，再做 AI 试点。

## 文件结构

```text
ai-tech-colleague/
  SKILL.md
  agents/
    openai.yaml
  references/
    ai-use-case-evaluation.md
    enterprise-ai-risks.md
    mvp-playbooks.md
    technical-patterns.md
```
