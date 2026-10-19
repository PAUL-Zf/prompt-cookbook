# Prompt Cookbook

个人 Prompt 配方库，沉淀编程开发、科研分析、Agent 协作和产品技术研究中的可复用提示词。

以真实任务为起点，明确目标、材料、边界、交付物和验收方式，让每次与 AI 的协作更具体、更容易复用。

## 快速开始

1. 从下方索引中选择适合当前任务的 Prompt。
2. 打开对应 Markdown 文件，复制完整内容。
3. 在具备所需材料或代码访问权限的 AI Agent 中使用，并按实际情况补充背景与约束。
4. 检查输出是否满足交付要求，尤其关注事实依据、文件引用和待确认事项。

### 示例：快速理解一个代码项目

使用 [项目快速理解 Prompt](coding/understand-project.md)：

1. 在本地打开**待分析项目的根目录**，启动能够读取本地代码的 Agent。
2. 将该 Prompt 的完整内容粘贴给 Agent。
3. Agent 按“全局认知 → 模块解析 → 核心调用链 → 关键设计 → 快速上手”的顺序分析，输出《项目快速理解报告》。

这里的“当前代码仓库”指你希望分析的目标项目。该 Prompt 要求只读分析；运行与调试方法、小型修改任务作为建议输出，不要求实际执行。

## 使用约定

- 将 Prompt 中的方括号占位内容替换为实际需求，删除不适用项；不必填写与当前任务无关的信息。
- 调试、重构和 Skill 创建提供分析或实施模式；需要实际修改时，请明确选择实施模式并指定范围。
- 审查、调研、规划与上下文审计默认只读；上下文审计需要在批准清理方案后才能修改配置。
- 多 Agent 协作根据任务收益和环境能力启用，不支持时转为单 Agent 执行。
- 对来源、推断与实测结果分别标注；“已收录”表示内容可用，不表示已在所有 Agent 平台验证。

## Prompt 索引

| 分类 | Prompt | 用途 | 状态 |
| --- | --- | --- | --- |
| 编程开发 | [understand-project](coding/understand-project.md) | 快速理解陌生项目的架构、模块、调用链与关键设计 | 已收录 |
| 编程开发 | [debug-code](coding/debug-code.md) | 问题定位与调试 | 已收录 |
| 编程开发 | [code-review](coding/code-review.md) | 代码审查 | 已收录 |
| 编程开发 | [refactoring](coding/refactoring.md) | 代码重构 | 已收录 |
| 科研分析 | [literature-review](research/literature-review.md) | 文献调研与综述 | 已收录 |
| 科研分析 | [paper-analysis](research/paper-analysis.md) | 论文阅读与分析 | 已收录 |
| 科研分析 | [idea-brainstorming](research/idea-brainstorming.md) | 科研想法探索 | 已收录 |
| Agent 协作 | [context-audit](agent/context-audit.md) | 审计自定义指令、Skills 与记忆等上下文配置，按收益排序提出清理建议 | 已收录 |
| Agent 协作 | [task-planning](agent/task-planning.md) | 任务拆解与执行规划 | 已收录 |
| Agent 协作 | [multi-agent-collaboration](agent/multi-agent-collaboration.md) | 多 Agent 分工与协作 | 已收录 |
| Agent 协作 | [skill-creation](agent/skill-creation.md) | Skill 创建 | 已收录 |
| 产品与技术 | [technical-research](product/technical-research.md) | 技术调研 | 已收录 |
| 产品与技术 | [feasibility-analysis](product/feasibility-analysis.md) | 方案可行性分析 | 已收录 |
| 通用模板 | [universal-prompt-template](templates/universal-prompt-template.md) | 通用 Prompt 编写框架 | 已收录 |

## 仓库目录

目前共收录 14 份 Prompt，覆盖编程开发、科研分析、Agent 协作、产品与技术以及通用模板。

```text
prompt-cookbook/
├── README.md
├── coding/
│   ├── understand-project.md
│   ├── debug-code.md
│   ├── code-review.md
│   └── refactoring.md
├── research/
│   ├── literature-review.md
│   ├── paper-analysis.md
│   └── idea-brainstorming.md
├── agent/
│   ├── context-audit.md
│   ├── task-planning.md
│   ├── multi-agent-collaboration.md
│   └── skill-creation.md
├── product/
│   ├── technical-research.md
│   └── feasibility-analysis.md
└── templates/
    └── universal-prompt-template.md
```

## 编写与维护约定

- **一份文件，一个主要场景**：文件名使用小写英文与连字符，便于检索和引用。
- **描述具体**：优先写清目标、输入材料、执行边界、交付物与验收方式。
- **基于事实**：要求区分已确认事实、推断和待验证内容，重要结论提供依据。
- **明确操作范围**：区分只读分析与允许修改的任务，按实际需求设置权限。
- **持续迭代**：根据实际使用效果改进 Prompt，新增内容时同步更新索引。
