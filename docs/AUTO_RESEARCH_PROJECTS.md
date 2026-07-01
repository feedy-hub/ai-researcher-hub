# 自动科研项目聚合索引

> 更新时间：2026-07-01  
> 仓库定位：收集、筛选、跟踪当前比较好的、高关注度的自动科研相关开源项目。  
> 目标：把 `ai-researcher-hub` 做成一个面向 AI Researcher / Research Agent / Paper Engineering 的聚合仓库，而不是普通 AI 工具链接大全。

---

## 0. 核心定位

`ai-researcher-hub` 的主线应聚焦在：

> **自动科研项目聚合 + 可复现科研工作流 + AI Research Agent 基础设施。**

它关注的不是所有 AI 项目，而是能帮助研究者完成以下任务的项目：

1. 自动检索资料、网页、论文、数据集。
2. 自动生成研究问题、检索计划、综述大纲。
3. 自动阅读论文、回答文献问题、生成带引用的总结。
4. 自动形成 research report、survey、technical note、benchmark note。
5. 自动运行或辅助运行代码实验、baseline 复现、指标评测。
6. 自动管理论文库、实验记录、代码阅读笔记和研究知识图谱。

---

## 1. 收录边界

### 1.1 优先收录

| 类型 | 说明 | 示例 |
|---|---|---|
| Deep Research Agent | 能自动搜索、递归研究、生成报告 | GPT Researcher、Open Deep Research、STORM |
| Scientific Paper QA | 面向论文 PDF / 科学文献的 RAG 问答 | PaperQA2 |
| Literature Review / Survey Agent | 自动综述、生成大纲、比较工作 | STORM、OpenPaper |
| Research Workflow Agent | 能规划、拆解、执行科研任务 | DeepResearchAgent、AutoGen、MetaGPT |
| Code / Experiment Agent | 能读代码、改代码、跑实验或辅助复现 | OpenHands、Aider、SWE-agent |
| Evaluation / Benchmark | 用来评测 Research Agent 或 RAG 质量 | Deep Research Bench、RAGAS、promptfoo |
| Meta Index / Awesome List | 聚合 Agent、RAG、LLM 工具 | awesome-ai-agents、Awesome-LLM |

### 1.2 暂不优先收录

| 类型 | 原因 |
|---|---|
| 纯聊天机器人 | 不直接服务科研流程 |
| 单纯 UI 壳项目 | 除非对科研工作流有明确价值 |
| 只有 demo、无 README、无维护的项目 | 难以长期跟踪 |
| 闭源 SaaS 工具 | 可以另建 `COMMERCIAL_TOOLS.md`，不混入开源项目主索引 |
| 与科研无关的通用 Agent | 除非具备可迁移到科研任务的架构价值 |

---

## 2. 评价维度

每个项目建议按以下维度打分，后续可以转成 YAML/JSON 数据源：

| 维度 | 说明 |
|---|---|
| Stars | GitHub star 数，反映社区关注度；必须标注采集日期 |
| Activity | 最近 commit、issue、release 是否活跃 |
| Research Fit | 是否直接服务科研流程 |
| Reproducibility | 是否容易本地跑通，是否有 demo / docker / examples |
| Citation Quality | 输出是否带来源、引用、证据链 |
| Extensibility | 是否支持自定义模型、检索器、工具、MCP、API |
| Local-first | 是否支持本地运行、私有知识库、私有文档 |
| License | Apache-2.0 / MIT 优先；不明许可证需谨慎 |
| Benchmark | 是否有公开评测、leaderboard、paper 或 technical report |

推荐分级：

- **A 级**：高关注、强相关、可运行、可扩展，适合重点跟踪。
- **B 级**：方向相关，但需要验证复现或维护状态。
- **C 级**：有启发价值，但暂不作为核心依赖。
- **Watch**：新项目或潜力项目，先观察。

---

## 3. A 级：重点跟踪的自动科研项目

> Star 数是易变信息，下面仅作为 2026-07-01 左右的快照参考；后续应由脚本自动刷新。

| 项目 | 仓库 | 类型 | 关注度快照 | 推荐理由 | 初步等级 |
|---|---|---|---|---|---|
| STORM | https://github.com/stanford-oval/storm | 自动资料调研 / 大纲 / 长文报告 | 约 29.7k stars | Stanford OVAL 项目，面向带引用的 Wikipedia-like report 生成，具有 Pre-writing + Writing 两阶段设计 | A |
| GPT Researcher | https://github.com/assafelovic/gpt-researcher | Deep Research Agent | 约 28k stars | 面向 web/local research 的自动研究 Agent，支持多 Agent、报告生成、来源追踪、PDF/Word 导出、MCP | A |
| Alibaba DeepResearch | https://github.com/Alibaba-NLP/DeepResearch | Deep Research Agent / Web Agent | 约 19.6k stars | 通义 DeepResearch，包含模型、推理、评测、Web Agent / Search Agent / Agentic RAG 方向材料 | A |
| dzhng/deep-research | https://github.com/dzhng/deep-research | 极简 Deep Research Agent | 约 19.2k stars | 代码极简，适合理解递归搜索、方向扩展、报告生成的核心逻辑 | A |
| LangChain Open Deep Research | https://github.com/langchain-ai/open_deep_research | Deep Research Agent / LangGraph | 约 11.9k stars | 可配置、开源、支持多模型/搜索/MCP，并提供 Deep Research Bench 评测流程 | A |
| PaperQA2 | https://github.com/Future-House/paper-qa | Scientific Paper QA / RAG | 约 8.8k stars | 面向科学文献的高精度 RAG，支持 PDF/文档/源码问答和引用 | A |
| Skywork DeepResearchAgent | https://github.com/SkyworkAI/DeepResearchAgent | 层级多智能体 / Deep Research | 约 3.5k stars | 层级多 Agent 架构，适合研究任务拆解、规划和复杂任务执行参考 | A- |

---

## 4. B 级：值得观察和补充验证的项目

| 项目 | 仓库 | 类型 | 推荐理由 | 待验证点 | 初步等级 |
|---|---|---|---|---|---|
| OpenPaper | https://github.com/khoj-ai/openpaper | 论文阅读 / 文献助手 | 面向论文阅读和研究辅助，适合补充到文献工作流 | 需要验证功能边界、维护状态、可运行性 | B |
| HKUDS Auto-Deep-Research | https://github.com/HKUDS/Auto-Deep-Research | Deep Research Agent | 与自动深度研究直接相关 | 需要验证成熟度、文档、评测 | B |
| nickscamara/open-deep-research | https://github.com/nickscamara/open-deep-research | Open Deep Research | 自动研究方向相关 | 需要确认是否仍活跃、与 dzhng/langchain 版本关系 | B |
| ResearchClaw | https://github.com/ymx10086/ResearchClaw | Research Assistant | 搜索结果中相关，但需进一步审阅 | 需要确认质量和完整性 | Watch |
| deep_research_bench | https://github.com/Ayanami0730/deep_research_bench | Research Agent Benchmark | 可能用于自动科研 Agent 评测 | 需要验证数据集、指标和使用方式 | Watch |

---

## 5. 支撑层：Agent / Coding Agent / Workflow 项目

这些项目未必是“自动科研项目”，但对搭建自动科研系统很关键。

| 项目 | 仓库 | 类型 | 与自动科研的关系 | 初步等级 |
|---|---|---|---|---|
| AutoGen | https://github.com/microsoft/autogen | 多 Agent 框架 | 可用于设计论文阅读 Agent、实验复现 Agent、多角色科研讨论 Agent | A |
| OpenHands | https://github.com/All-Hands-AI/OpenHands | Coding Agent | 可用于自动读代码、改代码、复现实验、生成 PR | A |
| MetaGPT | https://github.com/FoundationAgents/MetaGPT | 多 Agent 软件流程 | 可借鉴“角色—流程—产物”的科研任务组织方式 | B+ |
| CrewAI | https://github.com/crewAIInc/crewAI | 多 Agent 编排 | 易于快速搭建 researcher / reviewer / engineer 多角色系统 | B+ |
| Aider | https://github.com/Aider-AI/aider | AI pair programming | 适合论文代码修改、实验脚本迭代 | A- |
| SWE-agent | https://github.com/SWE-agent/SWE-agent | 软件工程 Agent | 适合借鉴自动修 bug、跑测试、改 repo 的流程 | B+ |
| LangGraph | https://github.com/langchain-ai/langgraph | Agent 工作流图 | 适合构建可控、可追踪、可恢复的科研 Agent 流程 | A |
| Dify | https://github.com/langgenius/dify | LLM 应用平台 | 可用于快速搭建论文知识库、研究助手、RAG 工作流 | B+ |

---

## 6. 支撑层：RAG / Knowledge Base / 文献知识库项目

| 项目 | 仓库 | 类型 | 与自动科研的关系 | 初步等级 |
|---|---|---|---|---|
| LlamaIndex | https://github.com/run-llama/llama_index | RAG / 数据索引框架 | 适合构建论文库、实验日志库、代码库问答 | A |
| LangChain | https://github.com/langchain-ai/langchain | LLM 应用框架 | 可用于工具调用、检索、Agent、RAG pipeline | A- |
| Haystack | https://github.com/deepset-ai/haystack | RAG / QA | 适合企业级文档检索问答 | B+ |
| R2R | https://github.com/SciPhi-AI/R2R | RAG 引擎 | 适合构建可服务化的研究知识库 | B+ |
| txtai | https://github.com/neuml/txtai | Embedding / RAG | 轻量本地知识库方案 | B |
| Chroma | https://github.com/chroma-core/chroma | 向量数据库 | 本地 RAG 原型 | B+ |
| Qdrant | https://github.com/qdrant/qdrant | 向量数据库 | 服务化、生产级 RAG | A- |
| Milvus | https://github.com/milvus-io/milvus | 向量数据库 | 大规模向量检索 | A- |
| FAISS | https://github.com/facebookresearch/faiss | 向量检索库 | 高性能相似度搜索基础库 | A |

---

## 7. 支撑层：评测与质量控制

自动科研项目最容易的问题是“看起来像研究，实际可能幻觉、引用不准、遗漏关键文献”。所以评测项目必须单独维护。

| 项目 | 仓库 | 类型 | 用途 | 初步等级 |
|---|---|---|---|---|
| RAGAS | https://github.com/explodinggradients/ragas | RAG 评测 | 评估检索质量、答案一致性、引用质量 | A- |
| promptfoo | https://github.com/promptfoo/promptfoo | LLM 应用测试 | 回归测试、prompt 评测、红队测试 | A- |
| DeepEval | https://github.com/confident-ai/deepeval | LLM 应用评测 | 单元测试式评测 LLM/RAG 应用 | B+ |
| OpenAI Evals | https://github.com/openai/evals | Eval 框架 | 构建自定义科研 Agent 评测任务 | B+ |
| lm-evaluation-harness | https://github.com/EleutherAI/lm-evaluation-harness | LLM Benchmark | 模型能力评测 | B+ |
| HELM | https://github.com/stanford-crfm/helm | 综合模型评测 | 学术评测参考 | B |

---

## 8. 推荐的仓库结构升级

建议把 `ai-researcher-hub` 做成如下结构：

```text
ai-researcher-hub/
  README.md
  docs/
    AUTO_RESEARCH_PROJECTS.md        # 自动科研项目聚合索引，本文件
    AI_RESEARCH_REPOS.md             # AI research 通用仓库索引
    BASELINE_TRACKER.md              # baseline / repo 复现跟踪表
    REPRODUCE_STATUS.md              # 复现状态表
    EVALUATION_PROTOCOL.md           # 自动科研评测协议
    PROJECT_SCORECARD.md             # 项目评分标准
    COMMERCIAL_TOOLS.md              # 可选：闭源/商业科研工具
    CODE_READING_NOTES/
      gpt-researcher.md
      storm.md
      paperqa.md
      open-deep-research.md
  data/
    projects.yaml                    # 机器可读项目库
    tags.yaml                        # 标签定义
  scripts/
    refresh_github_stats.py          # 自动刷新 stars/forks/issues/last_commit
    validate_project_links.py        # 检查链接是否失效
```

---

## 9. 项目卡片模板

```md
## <Project Name>

- Repository: <url>
- Category: Deep Research / Paper QA / Literature Review / Coding Agent / RAG / Evaluation
- Stars snapshot: <number> as of <YYYY-MM-DD>
- License: <MIT / Apache-2.0 / Other>
- Core capability:
- Best use case:
- Local runnable: yes / no / unknown
- Requires API keys: yes / no / unknown
- Supports citations: yes / no / partial
- Supports local documents: yes / no / partial
- Supports MCP/tools: yes / no / partial
- Evaluation available: yes / no / partial
- Maturity: A / B / C / Watch
- Notes:
```

---

## 10. `projects.yaml` 建议结构

后续建议把核心项目转成机器可读格式，便于生成 README 表格、自动刷新、自动排序：

```yaml
- name: GPT Researcher
  repo: assafelovic/gpt-researcher
  url: https://github.com/assafelovic/gpt-researcher
  category: deep-research-agent
  level: A
  stars_snapshot: "28k"
  snapshot_date: "2026-07-01"
  license: Apache-2.0
  local_runnable: true
  supports_citations: true
  supports_local_documents: true
  supports_mcp: true
  notes: "Autonomous agent for web/local deep research and report generation."
```

---

## 11. 最小可行路线图

### Phase 1：手工聚合

- 建立 `AUTO_RESEARCH_PROJECTS.md`。
- 先收录 30 个项目。
- 每个项目至少记录：repo、类型、用途、等级、待验证点。

### Phase 2：半自动维护

- 增加 `data/projects.yaml`。
- 写 `refresh_github_stats.py` 自动刷新 stars、forks、open issues、last commit。
- README 表格由 YAML 自动生成。

### Phase 3：科研工作流化

- 给每个重点项目写代码阅读笔记。
- 建立“是否能本地跑通”的复现记录。
- 建立 automatic research agent 评测协议。

### Phase 4：成为真正的 Hub

- 做成 Awesome List 风格主页。
- 增加标签、目录、徽章、自动更新状态。
- 增加“推荐组合”：例如 `STORM + PaperQA + LangGraph + RAGAS`。
- 建立中文科研使用指南：如何用这些项目做真实论文调研、综述、baseline 复现。

---

## 12. 初始推荐组合

### 12.1 自动综述 / Topic Survey

- STORM：生成大纲和长文报告。
- GPT Researcher：补充 web/local 深度调研。
- PaperQA2：针对本地论文 PDF 做精确问答。
- RAGAS：评估 RAG 输出质量。

### 12.2 自动科研助手 / Research Agent

- LangGraph：编排 researcher / reviewer / coder / evaluator。
- Open Deep Research：作为可运行 deep research baseline。
- AutoGen 或 CrewAI：快速做多 Agent 原型。
- Dify：做可视化应用入口。

### 12.3 自动复现实验 / Paper Engineering

- OpenHands：自动读代码、修改脚本、跑测试。
- Aider：交互式论文代码修改。
- SWE-agent：借鉴 repo-level 自动修复和测试流程。
- MLflow / W&B：记录实验结果。

---

## 13. 维护提醒

这个领域变化非常快，Star 数和活跃度会频繁变化。建议每月刷新一次：

- stars
- forks
- open issues
- last commit
- latest release
- license
- 是否 archive
- 是否仍可运行
- 是否有新 benchmark / paper

最终目标不是“收藏夹”，而是一个**可筛选、可复现、可比较、可扩展的自动科研项目索引库**。
