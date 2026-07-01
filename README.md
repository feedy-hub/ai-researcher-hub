# AI Researcher Hub

<p align="center">
  <strong>Curated Open-Source Projects for Automated Research, Deep Research Agents, Paper QA, Literature Review, and Paper Engineering.</strong>
</p>

<p align="center">
  <a href="docs/AUTO_RESEARCH_PROJECTS.md">Auto Research Projects</a> ·
  <a href="docs/AI_RESEARCH_REPOS.md">AI Research Repos</a> ·
  <a href="#featured-projects">Featured Projects</a> ·
  <a href="#roadmap">Roadmap</a>
</p>

---

## What is this?

**AI Researcher Hub** 是一个面向自动科研的开源项目聚合仓库，重点收集当前比较好的、高关注度的：

- Deep Research Agent
- AI Research Assistant
- Paper QA / Scientific RAG
- Literature Review / Survey Agent
- Code & Experiment Agent
- Research Workflow / Multi-Agent Framework
- RAG Evaluation / Agent Benchmark

它不是普通 AI 工具链接大全，而是一个可持续维护的：

> **自动科研项目聚合仓库 + AI Research Workflow Hub + Paper Engineering Hub**

目标是帮助研究者快速找到可以用于：**查文献、读论文、写综述、做调研、跑实验、复现 baseline、评估结果、构建个人科研助手**的开源项目。

---

## Featured Projects

> Star 数和活跃度变化很快，这里优先放“高关注 + 与自动科研强相关 + 值得重点跟踪”的项目。更完整列表见 [`docs/AUTO_RESEARCH_PROJECTS.md`](docs/AUTO_RESEARCH_PROJECTS.md)。

### Deep Research / Automated Report Generation

| Project | Repository | What it is good for |
|---|---|---|
| **STORM** | [stanford-oval/storm](https://github.com/stanford-oval/storm) | Topic research, outline synthesis, cited long-form report generation |
| **GPT Researcher** | [assafelovic/gpt-researcher](https://github.com/assafelovic/gpt-researcher) | Autonomous web/local research, source-grounded reports, research automation |
| **Open Deep Research** | [langchain-ai/open_deep_research](https://github.com/langchain-ai/open_deep_research) | LangGraph-based deep research agent, configurable research workflow |
| **Deep Research** | [dzhng/deep-research](https://github.com/dzhng/deep-research) | Minimal deep research agent, good for understanding core research-agent logic |
| **Alibaba DeepResearch** | [Alibaba-NLP/DeepResearch](https://github.com/Alibaba-NLP/DeepResearch) | Web agent, search agent, agentic RAG, deep research system reference |
| **Skywork DeepResearchAgent** | [SkyworkAI/DeepResearchAgent](https://github.com/SkyworkAI/DeepResearchAgent) | Hierarchical multi-agent deep research workflow |

### Paper QA / Scientific RAG

| Project | Repository | What it is good for |
|---|---|---|
| **PaperQA2** | [Future-House/paper-qa](https://github.com/Future-House/paper-qa) | Scientific paper QA, citation-grounded answers, local document research |
| **OpenPaper** | [khoj-ai/openpaper](https://github.com/khoj-ai/openpaper) | Paper reading and research assistance |
| **LlamaIndex** | [run-llama/llama_index](https://github.com/run-llama/llama_index) | Building paper libraries, research knowledge bases, document RAG |
| **LangChain** | [langchain-ai/langchain](https://github.com/langchain-ai/langchain) | General LLM application, RAG, tools, agent integration |
| **R2R** | [SciPhi-AI/R2R](https://github.com/SciPhi-AI/R2R) | Production-oriented RAG engine for private knowledge bases |

### Research Workflow / Multi-Agent Frameworks

| Project | Repository | What it is good for |
|---|---|---|
| **LangGraph** | [langchain-ai/langgraph](https://github.com/langchain-ai/langgraph) | Stateful and controllable research-agent workflow graphs |
| **AutoGen** | [microsoft/autogen](https://github.com/microsoft/autogen) | Multi-agent research discussion, reviewer/coder/researcher collaboration |
| **CrewAI** | [crewAIInc/crewAI](https://github.com/crewAIInc/crewAI) | Lightweight role-based agent workflow prototyping |
| **MetaGPT** | [FoundationAgents/MetaGPT](https://github.com/FoundationAgents/MetaGPT) | Role-based task decomposition and structured multi-agent workflow |
| **Dify** | [langgenius/dify](https://github.com/langgenius/dify) | Visual LLM workflow, RAG app, research assistant prototype |

### Code / Experiment / Paper Engineering Agents

| Project | Repository | What it is good for |
|---|---|---|
| **OpenHands** | [All-Hands-AI/OpenHands](https://github.com/All-Hands-AI/OpenHands) | Coding agent for reading, editing, testing, and iterating repositories |
| **Aider** | [Aider-AI/aider](https://github.com/Aider-AI/aider) | AI pair programming for research code and experiment scripts |
| **SWE-agent** | [SWE-agent/SWE-agent](https://github.com/SWE-agent/SWE-agent) | Repository-level bug fixing and test-driven code automation |

### Evaluation / Benchmark / Quality Control

| Project | Repository | What it is good for |
|---|---|---|
| **RAGAS** | [explodinggradients/ragas](https://github.com/explodinggradients/ragas) | RAG answer quality, retrieval quality, faithfulness evaluation |
| **promptfoo** | [promptfoo/promptfoo](https://github.com/promptfoo/promptfoo) | LLM app regression tests, prompt evaluation, red-team checks |
| **DeepEval** | [confident-ai/deepeval](https://github.com/confident-ai/deepeval) | Unit-test-like evaluation for LLM and RAG applications |
| **OpenAI Evals** | [openai/evals](https://github.com/openai/evals) | Custom evaluation tasks for models and research agents |
| **lm-evaluation-harness** | [EleutherAI/lm-evaluation-harness](https://github.com/EleutherAI/lm-evaluation-harness) | Standard LLM benchmark evaluation |

---

## Core Indexes

| File | Purpose |
|---|---|
| [`docs/AUTO_RESEARCH_PROJECTS.md`](docs/AUTO_RESEARCH_PROJECTS.md) | 自动科研项目聚合索引：Deep Research、Paper QA、自动综述、Research Agent、Coding Agent、评测工具 |
| [`docs/AI_RESEARCH_REPOS.md`](docs/AI_RESEARCH_REPOS.md) | AI research 常用仓库索引：训练框架、LLM、RAG、多模态、语音、评测、工具链 |

---

## Recommended Research Stacks

### 1. Automated Literature Review

```text
STORM / GPT Researcher
+ PaperQA2
+ LlamaIndex / LangGraph
+ RAGAS / promptfoo
```

适合：自动调研主题、生成综述大纲、整理引用、对本地论文库做问答。

### 2. Personal Research Agent

```text
LangGraph / AutoGen / CrewAI
+ GPT Researcher / Open Deep Research
+ LlamaIndex / R2R
+ Dify / Open WebUI
```

适合：构建自己的科研助手，管理论文、想法、实验记录和知识库。

### 3. Paper Engineering / Reproduction Agent

```text
OpenHands / Aider / SWE-agent
+ GitHub Actions
+ MLflow / W&B
+ RAG over codebase
```

适合：读论文代码、改 baseline、跑实验、整理复现状态。

---

## Project Selection Criteria

每个项目建议按以下维度维护：

| Dimension | Meaning |
|---|---|
| Research Fit | 是否直接服务科研工作流 |
| Stars / Community | 社区关注度和传播度 |
| Activity | 最近 commit、issue、release 是否活跃 |
| Local Runnable | 是否容易本地运行，是否支持私有文档 |
| Citation Quality | 是否支持来源追踪、引用、证据链 |
| Extensibility | 是否支持自定义模型、检索器、工具、MCP、API |
| Reproducibility | 是否有 demo、examples、docker、benchmark |
| License | 是否适合研究和二次开发 |

推荐分级：

- **A**：强相关、高关注、可运行、可扩展，重点跟踪。
- **B**：方向相关，但需要进一步验证复现和维护状态。
- **C**：有启发价值，但暂不作为核心依赖。
- **Watch**：新项目或潜力项目，先观察。

---

## Repository Plan

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

## Roadmap

- [x] Initialize AI Researcher Hub.
- [x] Add general AI research repository index.
- [x] Add automated research project index.
- [x] Put featured automated-research links directly in README.
- [ ] Add `data/projects.yaml` as a machine-readable project database.
- [ ] Add `PROJECT_SCORECARD.md` for standardized project evaluation.
- [ ] Add `refresh_github_stats.py` to update stars, forks, issues, and last commit.
- [ ] Add reproducibility notes for STORM, GPT Researcher, PaperQA2, and Open Deep Research.
- [ ] Add an automated research workflow guide in Chinese.

---

## Maintenance Principles

1. 优先收录真正服务科研流程的项目，而不是泛泛收集所有 AI 工具。
2. Star 数只作为参考，必须结合活跃度、可运行性、引用质量和科研适配度判断。
3. 对重点项目记录：repo、类型、stars 快照、license、是否可本地运行、是否支持引用、是否支持本地文档、是否有评测。
4. 对 baseline / paper engineering 项目记录：paper、commit、环境、数据集、评测脚本和复现状态。
5. 每月至少刷新一次重点项目的 stars、forks、open issues、last commit、release 和 license。

---

## Contribution Ideas

欢迎补充：

- 新的自动科研项目
- 项目复现笔记
- 项目评分卡
- 自动科研工作流
- Paper QA / Deep Research / Research Agent benchmark
- 中文使用指南

A good entry should answer: **What research workflow does this project automate, and can a researcher actually run it?**
