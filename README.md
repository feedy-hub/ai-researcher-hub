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
  <a href="#自动科研精选项目">自动科研精选</a> ·
  <a href="#ai-research-基础设施">AI Research 基础设施</a> ·
  <a href="#推荐组合">推荐组合</a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Focus-Automated%20Research-blue" />
  <img src="https://img.shields.io/badge/Research-Agentic%20Workflow-purple" />
  <img src="https://img.shields.io/badge/Default-简体中文-red" />
  <img src="https://img.shields.io/badge/Status-Curated%20Hub-brightgreen" />
</p>

---

<a id="简体中文"></a>

## 简体中文

> **AI Researcher Hub** 旨在收集、筛选和跟踪当前高质量、高关注度、真正服务科研流程的自动科研与 AI Research 开源项目。

它不是普通 AI 工具链接大全，而是一个面向研究者的：

<table>
  <tr>
    <td><strong>自动科研项目聚合仓库</strong><br/>收集 Deep Research、Paper QA、自动综述、科研 Agent、代码实验 Agent。</td>
    <td><strong>AI Research Workflow Hub</strong><br/>整理从文献调研、论文阅读、实验复现到评测归档的完整科研工作流。</td>
    <td><strong>Paper Engineering Hub</strong><br/>关注 baseline 复现、代码阅读、实验管理、指标评测和论文工程化。</td>
  </tr>
</table>

### 这个仓库解决什么问题？

现在自动科研和 AI Research 相关项目很多，但信息分散、质量参差不齐、维护状态变化快。这个仓库希望回答三个问题：

1. **哪些开源项目真正能帮助科研？**
2. **哪些项目适合本地运行、私有论文库、复现实验？**
3. **如何把 Deep Research、Paper QA、Agent、RAG、Coding Agent、训练框架、评测工具组合成真实可用的科研工作流？**

---

## 自动科研精选项目

> 更完整的列表见 [`docs/AUTO_RESEARCH_PROJECTS.md`](docs/AUTO_RESEARCH_PROJECTS.md)。下面的 Stars 使用 GitHub 动态 badge，打开 README 时会显示当前 star 数。

### Deep Research / 自动调研与报告生成

| 项目 | Stars | 仓库 | 适合用途 |
|---|---:|---|---|
| **STORM** | ![stars](https://img.shields.io/github/stars/stanford-oval/storm?style=social) | [stanford-oval/storm](https://github.com/stanford-oval/storm) | 主题调研、大纲生成、带引用的长文报告 |
| **GPT Researcher** | ![stars](https://img.shields.io/github/stars/assafelovic/gpt-researcher?style=social) | [assafelovic/gpt-researcher](https://github.com/assafelovic/gpt-researcher) | Web / local deep research、资料检索、来源追踪、报告生成 |
| **Open Deep Research** | ![stars](https://img.shields.io/github/stars/langchain-ai/open_deep_research?style=social) | [langchain-ai/open_deep_research](https://github.com/langchain-ai/open_deep_research) | 基于 LangGraph 的可配置 Deep Research Agent |
| **Deep Research** | ![stars](https://img.shields.io/github/stars/dzhng/deep-research?style=social) | [dzhng/deep-research](https://github.com/dzhng/deep-research) | 极简 deep research agent，适合理解核心逻辑 |
| **Alibaba DeepResearch** | ![stars](https://img.shields.io/github/stars/Alibaba-NLP/DeepResearch?style=social) | [Alibaba-NLP/DeepResearch](https://github.com/Alibaba-NLP/DeepResearch) | Web Agent、Search Agent、Agentic RAG、Deep Research 系统参考 |
| **Skywork DeepResearchAgent** | ![stars](https://img.shields.io/github/stars/SkyworkAI/DeepResearchAgent?style=social) | [SkyworkAI/DeepResearchAgent](https://github.com/SkyworkAI/DeepResearchAgent) | 层级多智能体科研任务执行 |

### Paper QA / Scientific RAG / 论文知识库

| 项目 | Stars | 仓库 | 适合用途 |
|---|---:|---|---|
| **PaperQA2** | ![stars](https://img.shields.io/github/stars/Future-House/paper-qa?style=social) | [Future-House/paper-qa](https://github.com/Future-House/paper-qa) | 科学论文问答、引用支撑回答、本地文献库 QA |
| **OpenPaper** | ![stars](https://img.shields.io/github/stars/khoj-ai/openpaper?style=social) | [khoj-ai/openpaper](https://github.com/khoj-ai/openpaper) | 论文阅读、文献辅助分析 |
| **LlamaIndex** | ![stars](https://img.shields.io/github/stars/run-llama/llama_index?style=social) | [run-llama/llama_index](https://github.com/run-llama/llama_index) | 构建论文库、实验日志库、代码文档 RAG |
| **LangChain** | ![stars](https://img.shields.io/github/stars/langchain-ai/langchain?style=social) | [langchain-ai/langchain](https://github.com/langchain-ai/langchain) | RAG、工具调用、Agent 应用集成 |
| **R2R** | ![stars](https://img.shields.io/github/stars/SciPhi-AI/R2R?style=social) | [SciPhi-AI/R2R](https://github.com/SciPhi-AI/R2R) | 面向私有知识库的服务化 RAG 引擎 |

### Research Agent / 多智能体科研工作流

| 项目 | Stars | 仓库 | 适合用途 |
|---|---:|---|---|
| **LangGraph** | ![stars](https://img.shields.io/github/stars/langchain-ai/langgraph?style=social) | [langchain-ai/langgraph](https://github.com/langchain-ai/langgraph) | 有状态、可控、可恢复的科研 Agent 工作流 |
| **AutoGen** | ![stars](https://img.shields.io/github/stars/microsoft/autogen?style=social) | [microsoft/autogen](https://github.com/microsoft/autogen) | 多智能体科研讨论、Reviewer / Coder / Researcher 协作 |
| **CrewAI** | ![stars](https://img.shields.io/github/stars/crewAIInc/crewAI?style=social) | [crewAIInc/crewAI](https://github.com/crewAIInc/crewAI) | 轻量角色式 Agent 编排 |
| **MetaGPT** | ![stars](https://img.shields.io/github/stars/FoundationAgents/MetaGPT?style=social) | [FoundationAgents/MetaGPT](https://github.com/FoundationAgents/MetaGPT) | 角色分工、任务拆解、结构化多 Agent 流程 |
| **Dify** | ![stars](https://img.shields.io/github/stars/langgenius/dify?style=social) | [langgenius/dify](https://github.com/langgenius/dify) | 可视化 RAG / Agent 应用入口 |

### Code Agent / 实验复现 / Paper Engineering

| 项目 | Stars | 仓库 | 适合用途 |
|---|---:|---|---|
| **OpenHands** | ![stars](https://img.shields.io/github/stars/All-Hands-AI/OpenHands?style=social) | [All-Hands-AI/OpenHands](https://github.com/All-Hands-AI/OpenHands) | 读代码、改代码、跑测试、迭代实验仓库 |
| **Aider** | ![stars](https://img.shields.io/github/stars/Aider-AI/aider?style=social) | [Aider-AI/aider](https://github.com/Aider-AI/aider) | 交互式修改研究代码和实验脚本 |
| **SWE-agent** | ![stars](https://img.shields.io/github/stars/SWE-agent/SWE-agent?style=social) | [SWE-agent/SWE-agent](https://github.com/SWE-agent/SWE-agent) | 仓库级自动修复、测试驱动代码修改 |

### Evaluation / 自动科研质量控制

| 项目 | Stars | 仓库 | 适合用途 |
|---|---:|---|---|
| **RAGAS** | ![stars](https://img.shields.io/github/stars/explodinggradients/ragas?style=social) | [explodinggradients/ragas](https://github.com/explodinggradients/ragas) | RAG 检索质量、回答一致性、忠实度评测 |
| **promptfoo** | ![stars](https://img.shields.io/github/stars/promptfoo/promptfoo?style=social) | [promptfoo/promptfoo](https://github.com/promptfoo/promptfoo) | LLM 应用回归测试、Prompt 评测、红队测试 |
| **DeepEval** | ![stars](https://img.shields.io/github/stars/confident-ai/deepeval?style=social) | [confident-ai/deepeval](https://github.com/confident-ai/deepeval) | 类单元测试的 LLM / RAG 应用评测 |
| **OpenAI Evals** | ![stars](https://img.shields.io/github/stars/openai/evals?style=social) | [openai/evals](https://github.com/openai/evals) | 自定义模型与科研 Agent 评测任务 |
| **lm-evaluation-harness** | ![stars](https://img.shields.io/github/stars/EleutherAI/lm-evaluation-harness?style=social) | [EleutherAI/lm-evaluation-harness](https://github.com/EleutherAI/lm-evaluation-harness) | 标准 LLM benchmark 评测 |

---

## AI Research 基础设施

> 这一部分收录通用 AI Research 开发、训练、评测和工程化常用仓库。它们不一定是“自动科研 Agent”，但经常是构建科研系统和复现实验的底座。

### 训练框架 / 实验基础设施

| 项目 | Stars | 仓库 | 适合用途 |
|---|---:|---|---|
| **PyTorch** | ![stars](https://img.shields.io/github/stars/pytorch/pytorch?style=social) | [pytorch/pytorch](https://github.com/pytorch/pytorch) | 深度学习主框架，论文复现默认首选 |
| **Transformers** | ![stars](https://img.shields.io/github/stars/huggingface/transformers?style=social) | [huggingface/transformers](https://github.com/huggingface/transformers) | LLM / NLP / VLM 预训练模型库 |
| **Datasets** | ![stars](https://img.shields.io/github/stars/huggingface/datasets?style=social) | [huggingface/datasets](https://github.com/huggingface/datasets) | 数据集加载、处理、共享 |
| **Accelerate** | ![stars](https://img.shields.io/github/stars/huggingface/accelerate?style=social) | [huggingface/accelerate](https://github.com/huggingface/accelerate) | 多 GPU / 混合精度 / 分布式训练封装 |
| **DeepSpeed** | ![stars](https://img.shields.io/github/stars/microsoft/DeepSpeed?style=social) | [microsoft/DeepSpeed](https://github.com/microsoft/DeepSpeed) | ZeRO、显存优化、大模型训练 |
| **Hydra** | ![stars](https://img.shields.io/github/stars/facebookresearch/hydra?style=social) | [facebookresearch/hydra](https://github.com/facebookresearch/hydra) | 科研实验配置管理 |
| **Weights & Biases** | ![stars](https://img.shields.io/github/stars/wandb/wandb?style=social) | [wandb/wandb](https://github.com/wandb/wandb) | 实验日志、曲线、表格、结果追踪 |
| **MLflow** | ![stars](https://img.shields.io/github/stars/mlflow/mlflow?style=social) | [mlflow/mlflow](https://github.com/mlflow/mlflow) | 实验管理、模型管理、可本地化追踪 |

### LLM 微调 / 推理 / 本地部署

| 项目 | Stars | 仓库 | 适合用途 |
|---|---:|---|---|
| **PEFT** | ![stars](https://img.shields.io/github/stars/huggingface/peft?style=social) | [huggingface/peft](https://github.com/huggingface/peft) | LoRA、Prefix tuning、参数高效微调 |
| **TRL** | ![stars](https://img.shields.io/github/stars/huggingface/trl?style=social) | [huggingface/trl](https://github.com/huggingface/trl) | SFT、DPO、RLHF、偏好优化 |
| **LLaMA-Factory** | ![stars](https://img.shields.io/github/stars/hiyouga/LLaMA-Factory?style=social) | [hiyouga/LLaMA-Factory](https://github.com/hiyouga/LLaMA-Factory) | 中文友好 LLM 微调与 Web UI |
| **Unsloth** | ![stars](https://img.shields.io/github/stars/unslothai/unsloth?style=social) | [unslothai/unsloth](https://github.com/unslothai/unsloth) | 低显存高效微调 |
| **vLLM** | ![stars](https://img.shields.io/github/stars/vllm-project/vllm?style=social) | [vllm-project/vllm](https://github.com/vllm-project/vllm) | 高吞吐 LLM 推理服务 |
| **SGLang** | ![stars](https://img.shields.io/github/stars/sgl-project/sglang?style=social) | [sgl-project/sglang](https://github.com/sgl-project/sglang) | LLM / VLM serving、结构化生成、Agent serving |
| **llama.cpp** | ![stars](https://img.shields.io/github/stars/ggml-org/llama.cpp?style=social) | [ggml-org/llama.cpp](https://github.com/ggml-org/llama.cpp) | GGUF、本地 CPU/GPU 推理、边缘部署 |
| **Ollama** | ![stars](https://img.shields.io/github/stars/ollama/ollama?style=social) | [ollama/ollama](https://github.com/ollama/ollama) | 快速拉起本地 LLM |

### RAG / 向量数据库 / 知识库

| 项目 | Stars | 仓库 | 适合用途 |
|---|---:|---|---|
| **Chroma** | ![stars](https://img.shields.io/github/stars/chroma-core/chroma?style=social) | [chroma-core/chroma](https://github.com/chroma-core/chroma) | 本地 RAG 原型和轻量向量库 |
| **Qdrant** | ![stars](https://img.shields.io/github/stars/qdrant/qdrant?style=social) | [qdrant/qdrant](https://github.com/qdrant/qdrant) | 服务化向量数据库，适合 RAG 系统 |
| **Milvus** | ![stars](https://img.shields.io/github/stars/milvus-io/milvus?style=social) | [milvus-io/milvus](https://github.com/milvus-io/milvus) | 大规模向量检索和生产级 RAG |
| **FAISS** | ![stars](https://img.shields.io/github/stars/facebookresearch/faiss?style=social) | [facebookresearch/faiss](https://github.com/facebookresearch/faiss) | 高性能相似度搜索基础库 |
| **Haystack** | ![stars](https://img.shields.io/github/stars/deepset-ai/haystack?style=social) | [deepset-ai/haystack](https://github.com/deepset-ai/haystack) | 企业级 RAG / QA pipeline |
| **txtai** | ![stars](https://img.shields.io/github/stars/neuml/txtai?style=social) | [neuml/txtai](https://github.com/neuml/txtai) | 轻量 Embedding DB 与本地知识库 |

### 多模态 / 视觉 / 语音音频

| 项目 | Stars | 仓库 | 适合用途 |
|---|---:|---|---|
| **LLaVA** | ![stars](https://img.shields.io/github/stars/haotian-liu/LLaVA?style=social) | [haotian-liu/LLaVA](https://github.com/haotian-liu/LLaVA) | 视觉语言模型、多模态指令学习 |
| **OpenCLIP** | ![stars](https://img.shields.io/github/stars/mlfoundations/open_clip?style=social) | [mlfoundations/open_clip](https://github.com/mlfoundations/open_clip) | CLIP 复现、图文对比学习、多模态表征 |
| **Segment Anything** | ![stars](https://img.shields.io/github/stars/facebookresearch/segment-anything?style=social) | [facebookresearch/segment-anything](https://github.com/facebookresearch/segment-anything) | 图像分割基础模型 |
| **timm** | ![stars](https://img.shields.io/github/stars/huggingface/pytorch-image-models?style=social) | [huggingface/pytorch-image-models](https://github.com/huggingface/pytorch-image-models) | 视觉模型库、ViT / CNN baseline |
| **Whisper** | ![stars](https://img.shields.io/github/stars/openai/whisper?style=social) | [openai/whisper](https://github.com/openai/whisper) | ASR、WER 评测、语音转写 |
| **ESPnet** | ![stars](https://img.shields.io/github/stars/espnet/espnet?style=social) | [espnet/espnet](https://github.com/espnet/espnet) | ASR / TTS / SE / SS 语音研究工具箱 |
| **SpeechBrain** | ![stars](https://img.shields.io/github/stars/speechbrain/speechbrain?style=social) | [speechbrain/speechbrain](https://github.com/speechbrain/speechbrain) | 语音增强、分离、说话人、ASR baseline |
| **EnCodec** | ![stars](https://img.shields.io/github/stars/facebookresearch/encodec?style=social) | [facebookresearch/encodec](https://github.com/facebookresearch/encodec) | 神经音频 codec、codec-based speech/audio research |
| **AV-HuBERT** | ![stars](https://img.shields.io/github/stars/facebookresearch/av_hubert?style=social) | [facebookresearch/av_hubert](https://github.com/facebookresearch/av_hubert) | 音视频自监督、AVSR / AVSE 视觉前端参考 |

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

### 4. 通用 AI Research 实验栈

```text
PyTorch / Transformers
+ Accelerate / DeepSpeed
+ Hydra / W&B / MLflow
+ vLLM / Ollama
+ RAGAS / lm-evaluation-harness
```

适合：快速搭建可复现、可记录、可评测的 AI research 实验环境。

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
- [x] 给 README 首页项目增加实时 Stars 展示。
- [x] 将 AI Research 基础设施项目加入 README 首页。
- [ ] 增加 `data/projects.yaml` 机器可读项目库。
- [ ] 增加 `PROJECT_SCORECARD.md` 标准化项目评分卡。
- [ ] 增加 `refresh_github_stats.py` 自动刷新 stars、forks、issues、last commit。
- [ ] 为 STORM、GPT Researcher、PaperQA2、Open Deep Research 增加复现笔记。
- [ ] 增加中文自动科研工作流指南。

---

## 维护原则

1. 优先收录真正服务科研流程的项目，而不是泛泛收集所有 AI 工具。
2. Star 数只作为参考，必须结合活跃度、可运行性、引用质量和科研适配度判断。
3. 首页 Star 数使用 GitHub 动态 badge；如果后续需要排序和快照归档，应使用 `data/projects.yaml` 和刷新脚本固化数值。
4. 对重点项目记录：repo、类型、stars 快照、license、是否可本地运行、是否支持引用、是否支持本地文档、是否有评测。
5. 对 baseline / paper engineering 项目记录：paper、commit、环境、数据集、评测脚本和复现状态。
6. 每月至少刷新一次重点项目的 stars、forks、open issues、last commit、release 和 license。

---

## 贡献方向

欢迎补充：

- 新的自动科研项目
- 新的 AI Research 基础设施项目
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

**AI Researcher Hub** is a curated hub for high-quality open-source projects that support automated research workflows and general AI research infrastructure.

It covers two major layers:

| Layer | Scope |
|---|---|
| Automated Research | Deep research agents, paper QA, literature review automation, coding agents, research workflow agents, and evaluation tools. |
| AI Research Infrastructure | Training frameworks, LLM fine-tuning, inference serving, RAG systems, vector databases, multimodal models, speech/audio toolkits, and experiment management. |

### Featured Project Groups

| Category | Examples |
|---|---|
| Deep Research | STORM, GPT Researcher, Open Deep Research, Deep Research, Alibaba DeepResearch, Skywork DeepResearchAgent |
| Paper QA / Scientific RAG | PaperQA2, OpenPaper, LlamaIndex, LangChain, R2R |
| Research Agent Frameworks | LangGraph, AutoGen, CrewAI, MetaGPT, Dify |
| Code / Experiment Agents | OpenHands, Aider, SWE-agent |
| Evaluation | RAGAS, promptfoo, DeepEval, OpenAI Evals, lm-evaluation-harness |
| AI Research Infrastructure | PyTorch, Transformers, Accelerate, DeepSpeed, PEFT, vLLM, Ollama, Chroma, Qdrant, Milvus, FAISS, Whisper, ESPnet, EnCodec, AV-HuBERT |

### Indexes

| File | Purpose |
|---|---|
| [`docs/AUTO_RESEARCH_PROJECTS.md`](docs/AUTO_RESEARCH_PROJECTS.md) | Curated automated research project index. |
| [`docs/AI_RESEARCH_REPOS.md`](docs/AI_RESEARCH_REPOS.md) | General AI research repository index. |

A good project entry should answer: **What research workflow does this project automate, and can a researcher actually run it?**
