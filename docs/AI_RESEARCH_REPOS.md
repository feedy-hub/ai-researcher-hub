# AI Research 常用 GitHub 仓库索引

> 更新时间：2026-07-01  
> 默认 GitHub 命名空间：`feedy-hub`  
> 当前存放仓库：`feedy-hub/ai-researcher-hub`  
> 文件用途：为日常 AI research、论文复现、baseline 对比、RAG/Agent 工具开发、多模态与语音研究建立一份可持续维护的仓库导航。

---

## 0. 使用原则

这个文件不是简单的 Star 榜单，而是按科研工作流组织的仓库地图。后续维护时建议优先记录：

- 仓库名称与链接
- 研究方向 / 工程方向
- 是否适合论文复现
- 是否适合工程集成
- 依赖复杂度
- 许可证与商用风险
- 最近维护状态
- 是否适合作为本项目 baseline / toolkit / reference implementation

建议后续每次新增仓库时使用下面格式：

```md
| repo | 链接 | 方向 | 推荐用途 | 备注 |
```

---

## 1. 论文检索、论文代码与 Awesome List

| repo / 项目 | 链接 | 方向 | 推荐用途 | 备注 |
|---|---|---|---|---|
| Papers with Code | https://github.com/paperswithcode | 论文代码索引 | 找论文实现、榜单、数据集 | 优先入口 |
| arxiv-sanity-lite | https://github.com/karpathy/arxiv-sanity-lite | 论文过滤系统 | 借鉴论文推荐产品形态 | 适合做 AI-Paper 工具参考 |
| Awesome Machine Learning | https://github.com/josephmisiti/awesome-machine-learning | ML 资源大全 | 入门工具索引 | 覆盖面广 |
| Awesome Deep Learning Papers | https://github.com/terryum/awesome-deep-learning-papers | 经典论文 | 补基础阅读 | 偏经典 |
| Awesome LLM | https://github.com/Hannibal046/Awesome-LLM | LLM 论文 | 跟踪 LLM 方向 | 适合定期更新 |
| Awesome Multimodal LLM | https://github.com/BradyFU/Awesome-Multimodal-Large-Language-Models | 多模态大模型 | VLM/MLLM 论文跟踪 | 多模态必看 |
| RAG Survey | https://github.com/Tongji-KGLLM/RAG-Survey | RAG 论文综述 | 知识库 / 检索增强研究 | 适合做路线图 |
| Awesome AI Agents | https://github.com/e2b-dev/awesome-ai-agents | Agent 资源 | Agent 框架与项目导航 | 工具型项目很多 |

---

## 2. 基础深度学习框架与训练基础设施

| repo | 链接 | 方向 | 推荐用途 | 备注 |
|---|---|---|---|---|
| PyTorch | https://github.com/pytorch/pytorch | 深度学习框架 | 论文复现主框架 | 研究默认首选 |
| JAX | https://github.com/jax-ml/jax | 自动微分 / XLA | 高性能研究、函数式训练 | 大模型和强化学习常见 |
| TensorFlow | https://github.com/tensorflow/tensorflow | 深度学习框架 | 旧论文 / 工业模型复现 | 仍需兼容部分历史代码 |
| PyTorch Lightning | https://github.com/Lightning-AI/pytorch-lightning | 训练工程化 | 快速管理训练循环 | 对小团队友好 |
| Accelerate | https://github.com/huggingface/accelerate | 分布式训练封装 | Hugging Face 训练脚手架 | 轻量易用 |
| DeepSpeed | https://github.com/microsoft/DeepSpeed | 大模型训练优化 | ZeRO、并行训练、显存优化 | 大模型训练常用 |
| Megatron-LM | https://github.com/NVIDIA/Megatron-LM | 大模型训练系统 | Transformer 大规模预训练 | 系统复杂度高 |
| Ray | https://github.com/ray-project/ray | 分布式计算 | 多实验调度、分布式服务 | 适合大规模 pipeline |
| Hydra | https://github.com/facebookresearch/hydra | 配置管理 | 科研实验配置 | 强烈推荐 |
| OmegaConf | https://github.com/omry/omegaconf | 配置系统 | YAML 配置组合 | 常与 Hydra 搭配 |
| Weights & Biases | https://github.com/wandb/wandb | 实验追踪 | 训练日志、曲线、表格 | 云端依赖需注意 |
| MLflow | https://github.com/mlflow/mlflow | 实验管理 | 可本地化实验追踪 | 适合私有部署 |

---

## 3. Transformer、LLM 训练与微调

| repo | 链接 | 方向 | 推荐用途 | 备注 |
|---|---|---|---|---|
| Transformers | https://github.com/huggingface/transformers | Transformer 模型库 | LLM/NLP/VLM 基础库 | 必备 |
| Datasets | https://github.com/huggingface/datasets | 数据集加载 | 训练数据与评测数据 | 与 HF 生态高度绑定 |
| Tokenizers | https://github.com/huggingface/tokenizers | 分词器 | tokenizer 训练与推理 | 高性能 Rust 实现 |
| PEFT | https://github.com/huggingface/peft | 参数高效微调 | LoRA、AdaLoRA、Prefix tuning | 轻量微调必备 |
| TRL | https://github.com/huggingface/trl | RLHF / DPO / SFT | LLM 对齐训练 | 适合指令微调与偏好优化 |
| bitsandbytes | https://github.com/bitsandbytes-foundation/bitsandbytes | 量化训练 | 8-bit/4-bit 训练与推理 | QLoRA 常用 |
| Axolotl | https://github.com/axolotl-ai-cloud/axolotl | LLM 微调框架 | 快速 SFT / LoRA / DPO | 配置驱动 |
| Unsloth | https://github.com/unslothai/unsloth | 高效微调 | 低显存微调 | 适合个人 GPU |
| LLaMA-Factory | https://github.com/hiyouga/LLaMA-Factory | 中文友好 LLM 微调 | SFT、LoRA、DPO、Web UI | 国内常用 |
| LitGPT | https://github.com/Lightning-AI/litgpt | LLM 训练与微调 | 教学、预训练、微调 | 代码相对清晰 |
| nanoGPT | https://github.com/karpathy/nanoGPT | 极简 GPT 训练 | 理解 Transformer 训练流程 | 教学价值高 |
| minGPT | https://github.com/karpathy/minGPT | 极简 GPT | 学习 Transformer | 更偏教学 |

---

## 4. LLM 推理、Serving 与本地部署

| repo | 链接 | 方向 | 推荐用途 | 备注 |
|---|---|---|---|---|
| vLLM | https://github.com/vllm-project/vllm | 高吞吐 LLM 推理 | 服务端推理、batch serving | 生产和实验都常用 |
| SGLang | https://github.com/sgl-project/sglang | LLM/VLM Serving | Agent、结构化生成、高性能 serving | 新框架值得关注 |
| Text Generation Inference | https://github.com/huggingface/text-generation-inference | LLM Serving | HF 模型部署 | 工业化程度高 |
| llama.cpp | https://github.com/ggml-org/llama.cpp | 本地 CPU/GPU 推理 | GGUF、本地部署、边缘设备 | 工程参考价值高 |
| Ollama | https://github.com/ollama/ollama | 本地模型运行 | 快速拉起本地 LLM | 适合产品原型 |
| LMDeploy | https://github.com/InternLM/lmdeploy | 推理部署 | TensorRT-LLM / TurboMind | 中文生态常用 |
| TensorRT-LLM | https://github.com/NVIDIA/TensorRT-LLM | 高性能推理 | NVIDIA GPU 极致性能 | 工程复杂度较高 |
| OpenLLM | https://github.com/bentoml/OpenLLM | LLM 应用部署 | BentoML 生态 | 可用于服务封装 |

---

## 5. RAG、知识库、检索与向量数据库

| repo | 链接 | 方向 | 推荐用途 | 备注 |
|---|---|---|---|---|
| LlamaIndex | https://github.com/run-llama/llama_index | RAG 框架 | 文档解析、索引、检索、Agentic RAG | 知识库项目优先看 |
| LangChain | https://github.com/langchain-ai/langchain | LLM 应用框架 | Chains、Tools、RAG、Agent | 生态大但抽象较重 |
| LangGraph | https://github.com/langchain-ai/langgraph | Agent 工作流 | 有状态 Agent、图式流程 | 适合复杂任务编排 |
| Haystack | https://github.com/deepset-ai/haystack | RAG / QA | 企业级检索问答 | 比较稳健 |
| txtai | https://github.com/neuml/txtai | Embedding DB / RAG | 轻量知识库 | 易本地化 |
| Chroma | https://github.com/chroma-core/chroma | 向量数据库 | 本地 RAG 原型 | 轻量易用 |
| Milvus | https://github.com/milvus-io/milvus | 向量数据库 | 大规模向量检索 | 生产级 |
| Qdrant | https://github.com/qdrant/qdrant | 向量数据库 | RAG 服务化 | Rust 实现，部署方便 |
| Weaviate | https://github.com/weaviate/weaviate | 向量数据库 | 企业知识库 | 功能完整 |
| FAISS | https://github.com/facebookresearch/faiss | 向量检索库 | 高性能相似度搜索 | 经典必备 |
| RAGAS | https://github.com/explodinggradients/ragas | RAG 评测 | 检索质量、答案质量评估 | RAG 项目推荐 |

---

## 6. Agent、AI 应用框架与工作流

| repo | 链接 | 方向 | 推荐用途 | 备注 |
|---|---|---|---|---|
| AutoGen | https://github.com/microsoft/autogen | 多 Agent 框架 | 多智能体协作实验 | 适合 Agent 研究 |
| OpenHands | https://github.com/All-Hands-AI/OpenHands | 软件工程 Agent | 类 Devin 编码助手 | 适合 Codex/Dev Agent 参考 |
| CrewAI | https://github.com/crewAIInc/crewAI | 多 Agent 编排 | 角色协作、任务拆解 | 工程上手快 |
| MetaGPT | https://github.com/FoundationAgents/MetaGPT | 软件公司式 Agent | 需求、设计、代码生成流程 | 产品化思路好 |
| Dify | https://github.com/langgenius/dify | LLM 应用平台 | 工作流、RAG、Agent、API | 适合搭建可视化应用 |
| Open WebUI | https://github.com/open-webui/open-webui | LLM Web UI | 本地模型前端、知识库 | 适合个人工作台 |
| Flowise | https://github.com/FlowiseAI/Flowise | 可视化 LLM 工作流 | 拖拽式 RAG/Agent | 适合低代码原型 |
| n8n | https://github.com/n8n-io/n8n | 自动化工作流 | 与 LLM、API、Webhook 集成 | 非纯 AI，但很实用 |

---

## 7. 评测、Benchmark 与安全对齐

| repo | 链接 | 方向 | 推荐用途 | 备注 |
|---|---|---|---|---|
| lm-evaluation-harness | https://github.com/EleutherAI/lm-evaluation-harness | LLM 评测 | 标准 benchmark 跑分 | 必备 |
| OpenAI Evals | https://github.com/openai/evals | 模型评测 | 自定义 eval 任务 | 适合构建项目评测集 |
| HELM | https://github.com/stanford-crfm/helm | 大模型综合评测 | 系统性 benchmark | 学术参考价值高 |
| promptfoo | https://github.com/promptfoo/promptfoo | Prompt / LLM 应用评测 | 回归测试、红队测试 | 适合应用开发 |
| DeepEval | https://github.com/confident-ai/deepeval | LLM 应用评测 | 单元测试式评测 | 工程易用 |
| OpenCompass | https://github.com/open-compass/opencompass | 中文/通用大模型评测 | 中文生态模型评测 | 国内常用 |
| FastChat | https://github.com/lm-sys/FastChat | 对话模型评测/服务 | Arena 风格评测参考 | 也可作 serving 参考 |
| JailbreakBench | https://github.com/JailbreakBench/jailbreakbench | 安全评测 | 越狱攻击/防御研究 | 安全方向可关注 |
| Garak | https://github.com/NVIDIA/garak | LLM 漏洞扫描 | 安全红队评测 | 工程安全有用 |

---

## 8. 多模态、视觉语言模型与视觉基础模型

| repo | 链接 | 方向 | 推荐用途 | 备注 |
|---|---|---|---|---|
| LLaVA | https://github.com/haotian-liu/LLaVA | 视觉语言模型 | 多模态指令学习 | 经典 VLM 实现 |
| LLaVA-NeXT | https://github.com/LLaVA-VL/LLaVA-NeXT | 多模态大模型 | LLaVA 系列后续 | 跟踪新模型 |
| OpenCLIP | https://github.com/mlfoundations/open_clip | 图文对比学习 | CLIP 复现与变体 | 多模态基础 |
| CLIP | https://github.com/openai/CLIP | 图文模型 | CLIP 原始实现 | 经典基线 |
| Segment Anything | https://github.com/facebookresearch/segment-anything | 图像分割基础模型 | SAM 基线与工具 | 视觉研究常用 |
| Detectron2 | https://github.com/facebookresearch/detectron2 | 检测/分割框架 | CV baseline | 经典工程框架 |
| MMDetection | https://github.com/open-mmlab/mmdetection | 目标检测 | 检测复现实验 | OpenMMLab 生态 |
| MMSegmentation | https://github.com/open-mmlab/mmsegmentation | 语义分割 | 分割复现实验 | 配置化强 |
| MMPreTrain | https://github.com/open-mmlab/mmpretrain | 视觉预训练 | 分类/自监督/基础模型 | OpenMMLab 生态 |
| timm | https://github.com/huggingface/pytorch-image-models | 视觉模型库 | ViT/CNN baseline | 视觉研究必备 |

---

## 9. 语音、音频与音视频研究

| repo | 链接 | 方向 | 推荐用途 | 备注 |
|---|---|---|---|---|
| Whisper | https://github.com/openai/whisper | ASR | 语音识别 baseline | 经典通用 ASR |
| ESPnet | https://github.com/espnet/espnet | 语音工具箱 | ASR/TTS/SE/SS 论文复现 | 学术语音研究常用 |
| SpeechBrain | https://github.com/speechbrain/speechbrain | 语音工具箱 | ASR、说话人、增强、分离 | PyTorch 友好 |
| NeMo | https://github.com/NVIDIA/NeMo | 语音/LLM/多模态 | ASR、TTS、LLM 训练 | 工程完整 |
| Asteroid | https://github.com/asteroid-team/asteroid | 语音分离 | Conv-TasNet/DPRNN 等 | 分离研究常用 |
| torchaudio | https://github.com/pytorch/audio | 音频处理 | PyTorch 音频 I/O 与特征 | 基础依赖 |
| librosa | https://github.com/librosa/librosa | 音频分析 | STFT、mel、特征提取 | 研究脚本常用 |
| audiocraft | https://github.com/facebookresearch/audiocraft | 生成式音频 | MusicGen / AudioGen | 音频生成参考 |
| EnCodec | https://github.com/facebookresearch/encodec | 神经音频 codec | codec-based speech/audio research | 与 AV-Codec/AVSE 相关 |
| SoundStream | https://github.com/wesbz/SoundStream | 神经音频 codec | codec 结构学习参考 | 非官方实现需核查 |
| AV-HuBERT | https://github.com/facebookresearch/av_hubert | 音视频自监督 | AVSR/AVSE 视觉前端参考 | AV 研究重要基线 |
| FlowAVSE | https://github.com/kaistmm/FlowAVSE | Audio-Visual Speech Enhancement | AVSE baseline | 与当前研究方向相关 |
| AVSE Challenge | https://github.com/cogmhear/avse_challenge | AVSE Challenge | 数据与评测流程参考 | 适合任务规范化 |
| tinyAVSE | https://github.com/Zikovich/tinyAVSE | 轻量 AVSE | 轻量化模型参考 | 可作为工程参考 |

---

## 10. Diffusion、生成模型与图像/视频生成

| repo | 链接 | 方向 | 推荐用途 | 备注 |
|---|---|---|---|---|
| diffusers | https://github.com/huggingface/diffusers | Diffusion 模型库 | 图像/视频/音频扩散模型 | 生成模型必备 |
| Stable Diffusion WebUI | https://github.com/AUTOMATIC1111/stable-diffusion-webui | 图像生成 WebUI | 插件生态、交互原型 | 工程参考 |
| ComfyUI | https://github.com/comfyanonymous/ComfyUI | 节点式生成工作流 | 图像/视频生成 pipeline | 可视化工作流强 |
| k-diffusion | https://github.com/crowsonkb/k-diffusion | Diffusion sampler | 采样器研究 | 理论/算法参考 |
| ControlNet | https://github.com/lllyasviel/ControlNet | 可控生成 | 条件控制、结构控制 | 经典方法 |
| AnimateDiff | https://github.com/guoyww/AnimateDiff | 视频生成 | 动画/视频扩散 | 研究参考 |
| VideoCrafter | https://github.com/AILab-CVC/VideoCrafter | 视频生成 | Text-to-Video baseline | 视频生成方向 |

---

## 11. 数据处理、标注与科研工具

| repo | 链接 | 方向 | 推荐用途 | 备注 |
|---|---|---|---|---|
| pandas | https://github.com/pandas-dev/pandas | 数据分析 | 实验表格、结果处理 | 基础工具 |
| polars | https://github.com/pola-rs/polars | 高性能 DataFrame | 大规模数据处理 | 速度快 |
| DVC | https://github.com/iterative/dvc | 数据版本管理 | 数据集与模型版本追踪 | 适合可复现工程 |
| Label Studio | https://github.com/HumanSignal/label-studio | 数据标注 | 图像、文本、音频标注 | 可本地部署 |
| FiftyOne | https://github.com/voxel51/fiftyone | 数据集可视化 | CV 数据检查 | 适合数据诊断 |
| ClearML | https://github.com/clearml/clearml | MLOps / 实验管理 | 私有化实验平台 | 功能完整 |
| Airflow | https://github.com/apache/airflow | 工作流调度 | 数据/训练流水线 | 工程复杂度高 |
| Prefect | https://github.com/PrefectHQ/prefect | 工作流调度 | 更现代的数据流水线 | 易用性较好 |

---

## 12. 对当前 Feedy Hub / AI Researcher Hub 最值得优先跟进的仓库

### P0：必须熟悉

| repo | 用途 |
|---|---|
| PyTorch | 主实验框架 |
| Transformers | 预训练模型与多模态模型接口 |
| Accelerate / DeepSpeed | 多 GPU 训练与显存优化 |
| Hydra / OmegaConf | 实验配置管理 |
| ESPnet / SpeechBrain | 语音增强、ASR、TTS、分离 baseline 参考 |
| EnCodec | codec prior / codec target recovery 相关研究 |
| AV-HuBERT | 音视频自监督与视觉前端 |
| FlowAVSE | AVSE 关键外部 baseline |
| Whisper | WER / ASR downstream evaluation |

### P1：建议纳入工具链

| repo | 用途 |
|---|---|
| W&B / MLflow | 实验追踪与结果归档 |
| DVC | 数据版本与 checkpoint 管理 |
| lm-evaluation-harness / OpenAI Evals | 如果后续加入 LLM 评测 |
| LlamaIndex / LangChain / Dify | 如果把论文库和实验日志做成知识库 |
| vLLM / Ollama | 如果需要本地或服务化模型调用 |

### P2：长期关注

| repo | 用途 |
|---|---|
| LLaVA / OpenCLIP | 多模态表示学习参考 |
| diffusers | 生成式建模与 diffusion baseline |
| AutoGen / OpenHands | AI research assistant / coding agent 参考 |
| RAGAS / promptfoo | 论文知识库和 Agent 的评测工具 |

---

## 13. 建议的本地维护结构

建议后续在仓库中形成如下结构：

```text
docs/
  AI_RESEARCH_REPOS.md              # 当前文件：仓库总索引
  BASELINE_TRACKER.md               # 论文 baseline 跟踪表
  REPRODUCE_STATUS.md               # 已复现/待复现/失败原因
  DATASET_INDEX.md                  # 数据集、路径、协议、许可证
  EVALUATION_PROTOCOL.md            # 指标、脚本、评测规范
  CODE_READING_NOTES/               # 代码阅读笔记
    encodec.md
    flowavse.md
    avhubert.md
    espnet.md
```

---

## 14. Baseline 复现状态模板

```md
# Baseline: <repo-name>

- Repository: <url>
- Paper: <paper-url>
- Task: AVSE / ASR / SE / SS / LLM / RAG / Agent / VLM
- License: <license>
- Dataset: <dataset>
- Environment: <CUDA / Python / PyTorch>
- Checkpoint: available / unavailable / self-trained
- Reproduce status: not started / running / reproduced / failed
- Metrics:
  - PESQ:
  - STOI:
  - SI-SDR:
  - DNSMOS:
  - WER:
- Notes:
  - Key implementation detail:
  - Risk:
  - Difference from paper:
```

---

## 15. 后续维护规则

1. 新增仓库前先判断它属于：baseline、toolkit、framework、survey、product reference、evaluation tool。
2. 不要只因为 Star 高就加入；优先加入能服务当前研究目标的仓库。
3. 对论文 baseline 仓库，必须记录 commit、环境、数据集、评测脚本。
4. 对工程框架，必须记录部署方式、许可证、依赖复杂度。
5. 对 AVSE / AVSS / codec / speech 相关仓库，优先补充复现状态和可对比指标。
6. 至少每月检查一次 P0/P1 仓库维护状态。

---

## 16. 下一步建议

建议下一步补三个文件：

1. `docs/BASELINE_TRACKER.md`：专门跟踪 AVSE/AVSS/codec/speech/LLM/RAG baseline。
2. `docs/REPRODUCE_STATUS.md`：记录每个外部 repo 是否已经跑通。
3. `docs/EVALUATION_PROTOCOL.md`：统一 PESQ、STOI、SI-SDR、DNSMOS、WER、RTF、参数量统计方式。

这样 `ai-researcher-hub` 后续就不是单纯存链接，而是逐步变成一个“AI research operating system / paper engineering hub”。
