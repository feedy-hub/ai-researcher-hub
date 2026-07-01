# AI Researcher Hub

<p align="center">
  <strong>自动科研项目聚合仓库 · AI Research Agent 导航 · Paper Engineering Hub</strong>
</p>

<p align="center">
  <a href="#简体中文">🇨🇳 简体中文</a> ·
  <a href="#english">🇺🇸 English</a>
</p>

<p align="center">
  <a href="docs/AUTO_RESEARCH_PROJECTS.md">自动科研项目索引</a> ·
  <a href="docs/AI_RESEARCH_REPOS.md">AI Research 仓库索引</a> ·
  <a href="#精选项目">精选项目</a> ·
  <a href="#推荐组合">推荐组合</a> ·
  <a href="#路线图">路线图</a>
</p>

---

<a id="简体中文"></a>

## 简体中文

> **AI Researcher Hub** 旨在收集、筛选和跟踪当前高质量、高关注度、真正服务科研流程的自动科研开源项目。

它不是普通的 AI 工具链接大全，而是一个面向研究者的：

<table>
  <tr>
    <td><strong>自动科研项目聚合仓库</strong><br/>收集 Deep Research、Paper QA、自动综述、科研 Agent、代码实验 Agent。</td>
    <td><strong>AI Research Workflow Hub</strong><br/>整理从文献调研、论文阅读、实验复现到评测归档的完整科研工作流。</td>
    <td><strong>Paper Engineering Hub</strong><br/>关注 baseline 复现、代码阅读、实验管理、指标评测和论文工程化。</td>
  </tr>
</table>

### 这个仓库解决什么问题？

现在自动科研相关项目很多，但信息分散、质量参差不齐、维护状态变化快。这个仓库希望回答三个问题：

1. **哪些开源项目真正能帮助科研？**
2. **哪些项目适合本地运行、私有论文库、复现实验？**
3. **如何把 Deep Research、Paper QA、Agent、RAG、Coding Agent 组合成真实可用的科研工作流？**

---

## 精选项目

> 更完整的列表见 [`docs/AUTO_RESEARCH_PROJECTS.md`](docs/AUTO_RESEARCH_PROJECTS.md)。Star 数和活跃度会变化，这里优先展示“高关注 + 强科研相关 + 值得重点跟踪”的项目。

### Deep Research / 自动调研与报告生成

| 项目 | 仓库 | 适合用途 |
|---|---|---|
| **STORM** | [stanford-oval/storm](https://github.com/stanford-oval/storm) | 主题调研、大纲生成、带引用的长文报告 |
| **GPT Researcher** | [assafelovic/gpt-researcher](https://github.com/assafelovic/gpt-researcher) | Web / local deep research、资料检索、来源追踪、报告生成 |
| **Open Deep Research** | [langchain-ai/open_deep_research](https://github.com/langchain-ai/open_deep_research) | 基于 LangGraph 的可配置 Deep Research Agent |
| **Deep Research** | [dzhng/deep-research](https://github.com/dzhng/deep-research) | 极简 deep research agent，适合理解核心逻辑 |
| **Alibaba DeepResearch** | [Alibaba-NLP/DeepResearch](https://github.com/Alibaba-NLP/DeepResearch) | Web Agent、Search Agent、Agentic RAG、Deep Research 系统参考 |
| **Skywork DeepResearchAgent** | [SkyworkAI/DeepResearchAgent](https://github.com/SkyworkAI/DeepResearchAgent) | 层级多智能体科研任务执行 |

### Paper QA / Scientific RAG / 论文知识库

| 项目 | 仓库 | 适合用途 |
|---|---|---|
| **PaperQA2** | [Future-House/paper-qa](https://github.com/Future-House/paper-qa) | 科学论文问答、引用支撑回答、本地文献库 QA |
| **OpenPaper** | [khoj-ai/openpaper](https://github.com/khoj-ai/openpaper) | 论文阅读、文献辅助分析 |
| **LlamaIndex** | [run-llama/llama_index](https://github.com/run-llama/llama_index) | 构建论文库、实验日志库、代码文档 RAG |
| **LangChain** | [langchain-ai/langchain](https://github.com/langchain-ai/langchain) | RAG、工具调用、Agent 应用集成 |
| **R2R** | [SciPhi-AI/R2R](https://github.com/SciPhi-AI/R2R) | 面向私有知识库的服务化 RAG 引擎 |

### Research Agent / 多智能体科研工作流

| 项目 | 仓库 | 适合用途 |
|---|---|---|
| **LangGraph** | [langchain-ai/langgraph](https://github.com/langchain-ai/langgraph) | 有状态、可控、可恢复的科研 Agent 工作流 |
| **AutoGen** | [microsoft/autogen](https://github.com/microsoft/autogen) | 多智能体科研讨论、Reviewer / Coder / Researcher 协作 |
| **CrewAI** | [crewAIInc/crewAI](https://github.com/crewAIInc/crewAI) | 轻量角色式 Agent 编排 |
| **MetaGPT** | [FoundationAgents/MetaGPT](https://github.com/FoundationAgents/MetaGPT) | 角色分工、任务拆解、结构化多 Agent 流程 |
| **Dify** | [langgenius/dify](https://github.com/langgenius/dify) | 可视化 RAG / Agent 应用入口 |

### Code Agent / 实验复现 / Paper Engineering

| 项目 | 仓库 | 适合用途 |
|---|---|---|
| **OpenHands** | [All-Hands-AI/OpenHands](https://github.com/All-Hands-AI/OpenHands) | 读代码、改代码、跑测试、迭代实验仓库 |
| **Aider** | [Aider-AI/aider](https://github.com/Aider-AI/aider) | 交互式修改研究代码和实验脚本 |
| **SWE-agent** | [SWE-agent/SWE-agent](https://github.com/SWE-agent/SWE-agent) | 仓库级自动修复、测试驱动代码修改 |

### Evaluation / 自动科研质量控制

| 项目 | 仓库 | 适合用途 |
|---|---|---|
| **RAGAS** | [explodinggradients/ragas](https://github.com/explodinggradients/ragas) | RAG 检索质量、回答一致性、忠实度评测 |
| **promptfoo** | [promptfoo/promptfoo](https://github.com/promptfoo/promptfoo) | LLM 应用回归测试、Prompt 评测、红队测试 |
| **DeepEval** | [confident-ai/deepeval](https://github.com/confident-ai/deepeval) | 类单元测试的 LLM / RAG 应用评测 |
| **OpenAI Evals** | [openai/evals](https://github.com/openai/evals) | 自定义模型与科研 Agent 评测任务 |
| **lm-evaluation-harness** | [EleutherAI/lm-evaluation-harness](https://github.com/EleutherAI/lm-evaluation-harness) | 标准 LLM benchmark 评测 |

---

## 推荐组合

### 1. 自动综述 / Topic Survey

```text
STORM / GPT Researcher
+ PaperQA2
+ LlamaIndex / LangGraph
+ RAGAS / promptfoo
```

适合：自动调研主题、生成综述大纲、整理引用、对本地论文库做问答。

### 2. 个人科研助手 / Personal Research Agent

```text
LangGraph / AutoGen / CrewAI
+ GPT Researcher / Open Deep Research
+ LlamaIndex / R2R
+ Dify / Open WebUI
```

适合：管理论文、想法、实验记录、代码库和研究知识图谱。

### 3. 论文工程化 / Paper Engineering

```text
OpenHands / Aider / SWE-agent
+ GitHub Actions
+ MLflow / W&B
+ Codebase RAG
```

适合：读论文代码、改 baseline、跑实验、整理复现状态和实验结果。

---

## 项目筛选标准

| 维度 | 判断问题 |
|---|---|
| 科研适配度 | 它是否直接服务科研流程，而不是泛泛的聊天或娱乐工具？ |
| 社区关注度 | 是否有较高 Star、讨论度、使用案例或论文引用？ |
| 活跃度 | 最近 commit、issue、release 是否活跃？ |
| 可运行性 | 是否容易本地运行？是否支持私有文档和本地论文库？ |
| 引用质量 | 是否支持来源追踪、引用、证据链和可验证输出？ |
| 可扩展性 | 是否支持自定义模型、检索器、工具、MCP、API？ |
| 可复现性 | 是否有 demo、examples、docker、benchmark 或测试？ |
| 许可证 | 是否适合研究、复现和二次开发？ |

推荐分级：

- **A**：强相关、高关注、可运行、可扩展，重点跟踪。
- **B**：方向相关，但需要进一步验证复现和维护状态。
- **C**：有启发价值，但暂不作为核心依赖。
- **Watch**：新项目或潜力项目，先观察。

---

## 仓库结构规划

```text
ai-researcher-hub/
  README.md
  docs/
    AUTO_RESEARCH_PROJECTS.md        # 自动科研项目聚合索引
    AI_RESEARCH_REPOS.md             # AI research 通用仓库索引
    BASELINE_TRACKER.md              # baseline / repo 复现跟踪表
    REPRODUCE_STATUS.md              # 复现状态表
    EVALUATION_PROTOCOL.md           # 自动科研评测协议
    PROJECT_SCORECARD.md             # 项目评分标准
    COMMERCIAL_TOOLS.md              # 闭源/商业科研工具
    CODE_READING_NOTES/              # 代码阅读笔记
  data/
    projects.yaml                    # 机器可读项目库
    tags.yaml                        # 标签定义
  scripts/
    refresh_github_stats.py          # 自动刷新 stars/forks/issues/last_commit
    validate_project_links.py        # 检查链接是否失效
```

---

## 路线图

- [x] 初始化 AI Researcher Hub。
- [x] 增加 AI research 通用仓库索引。
- [x] 增加自动科研项目聚合索引。
- [x] 将精选自动科研项目链接放到 README 首页。
- [x] 增加中英文切换入口，默认简体中文。
- [ ] 增加 `data/projects.yaml` 机器可读项目库。
- [ ] 增加 `PROJECT_SCORECARD.md` 标准化项目评分卡。
- [ ] 增加 `refresh_github_stats.py` 自动刷新 stars、forks、issues、last commit。
- [ ] 为 STORM、GPT Researcher、PaperQA2、Open Deep Research 增加复现笔记。
- [ ] 增加中文自动科研工作流指南。

---

## 维护原则

1. 优先收录真正服务科研流程的项目，而不是泛泛收集所有 AI 工具。
2. Star 数只作为参考，必须结合活跃度、可运行性、引用质量和科研适配度判断。
3. 对重点项目记录：repo、类型、stars 快照、license、是否可本地运行、是否支持引用、是否支持本地文档、是否有评测。
4. 对 baseline / paper engineering 项目记录：paper、commit、环境、数据集、评测脚本和复现状态。
5. 每月至少刷新一次重点项目的 stars、forks、open issues、last commit、release 和 license。

---

## 贡献方向

欢迎补充：

- 新的自动科研项目
- 项目复现笔记
- 项目评分卡
- 自动科研工作流
- Paper QA / Deep Research / Research Agent benchmark
- 中文使用指南

一个好的条目应该回答：**这个项目自动化了哪一类科研流程？研究者能不能真实跑起来？**

---

<a id="english"></a>

## English

<p align="right"><a href="#简体中文">Back to 简体中文</a></p>

**AI Researcher Hub** is a curated hub for high-quality open-source projects that support automated research workflows, including deep research agents, scientific paper QA, literature review automation, research agents, coding agents, and evaluation tools.

This repository is designed as:

<table>
  <tr>
    <td><strong>Automated Research Project Index</strong><br/>Curated projects for deep research, paper QA, survey generation, research agents, and coding agents.</td>
    <td><strong>AI Research Workflow Hub</strong><br/>A structured map from literature search and paper reading to experiment reproduction and evaluation.</td>
    <td><strong>Paper Engineering Hub</strong><br/>A practical space for baseline reproduction, code reading, experiment tracking, and research evaluation.</td>
  </tr>
</table>

### Featured Projects

| Category | Projects |
|---|---|
| Deep Research | [STORM](https://github.com/stanford-oval/storm), [GPT Researcher](https://github.com/assafelovic/gpt-researcher), [Open Deep Research](https://github.com/langchain-ai/open_deep_research), [dzhng/deep-research](https://github.com/dzhng/deep-research), [Alibaba DeepResearch](https://github.com/Alibaba-NLP/DeepResearch), [Skywork DeepResearchAgent](https://github.com/SkyworkAI/DeepResearchAgent) |
| Paper QA / Scientific RAG | [PaperQA2](https://github.com/Future-House/paper-qa), [OpenPaper](https://github.com/khoj-ai/openpaper), [LlamaIndex](https://github.com/run-llama/llama_index), [LangChain](https://github.com/langchain-ai/langchain), [R2R](https://github.com/SciPhi-AI/R2R) |
| Research Agent Frameworks | [LangGraph](https://github.com/langchain-ai/langgraph), [AutoGen](https://github.com/microsoft/autogen), [CrewAI](https://github.com/crewAIInc/crewAI), [MetaGPT](https://github.com/FoundationAgents/MetaGPT), [Dify](https://github.com/langgenius/dify) |
| Code / Experiment Agents | [OpenHands](https://github.com/All-Hands-AI/OpenHands), [Aider](https://github.com/Aider-AI/aider), [SWE-agent](https://github.com/SWE-agent/SWE-agent) |
| Evaluation | [RAGAS](https://github.com/explodinggradients/ragas), [promptfoo](https://github.com/promptfoo/promptfoo), [DeepEval](https://github.com/confident-ai/deepeval), [OpenAI Evals](https://github.com/openai/evals), [lm-evaluation-harness](https://github.com/EleutherAI/lm-evaluation-harness) |

### Indexes

| File | Purpose |
|---|---|
| [`docs/AUTO_RESEARCH_PROJECTS.md`](docs/AUTO_RESEARCH_PROJECTS.md) | Curated automated research project index. |
| [`docs/AI_RESEARCH_REPOS.md`](docs/AI_RESEARCH_REPOS.md) | General AI research repository index. |

### Recommended Stacks

| Scenario | Stack |
|---|---|
| Literature Review | STORM / GPT Researcher + PaperQA2 + LlamaIndex / LangGraph + RAGAS |
| Personal Research Agent | LangGraph / AutoGen / CrewAI + Open Deep Research + LlamaIndex / R2R |
| Paper Engineering | OpenHands / Aider / SWE-agent + GitHub Actions + MLflow / W&B + Codebase RAG |

A good project entry should answer: **What research workflow does this project automate, and can a researcher actually run it?**
