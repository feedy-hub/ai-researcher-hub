# AI Researcher Hub

AI Researcher Hub 是一个面向**自动科研、AI Research Agent、论文复现、baseline 管理、实验评测、RAG/Agent 工具开发、多模态与语音研究**的资料与工作流聚合仓库。

它的核心目标不是做普通 AI 工具链接大全，而是构建一个可持续维护的：

> **自动科研项目聚合仓库 + AI Research Workflow Hub + Paper Engineering Hub**

## 当前内容

- [`docs/AUTO_RESEARCH_PROJECTS.md`](docs/AUTO_RESEARCH_PROJECTS.md)：自动科研项目聚合索引，重点收集高关注、高星、适合科研工作流的 Research Agent / Deep Research / Paper QA / 自动综述项目。
- [`docs/AI_RESEARCH_REPOS.md`](docs/AI_RESEARCH_REPOS.md)：AI research 常用 GitHub 仓库索引，按科研工作流分类整理。

## 重点关注方向

1. Deep Research Agent：自动检索、递归研究、生成带引用报告。
2. Paper QA / Scientific RAG：面向论文 PDF、科学文献、代码文档的高精度问答。
3. Literature Review Agent：自动综述、生成大纲、比较相关工作。
4. Research Workflow Agent：自动拆解研究任务、组织多 Agent 协作。
5. Code / Experiment Agent：辅助读代码、改代码、跑实验、复现 baseline。
6. Evaluation：评测 RAG、Research Agent、引用质量、报告质量。

## 建议后续扩展

```text
docs/
  AUTO_RESEARCH_PROJECTS.md  # 自动科研项目聚合索引
  AI_RESEARCH_REPOS.md       # 常用 AI research 仓库索引
  BASELINE_TRACKER.md        # baseline 跟踪表
  REPRODUCE_STATUS.md        # 复现状态记录
  DATASET_INDEX.md           # 数据集、路径、协议与许可证
  EVALUATION_PROTOCOL.md     # 统一评测协议
  PROJECT_SCORECARD.md       # 项目评分标准
  COMMERCIAL_TOOLS.md        # 闭源/商业科研工具，单独维护
  CODE_READING_NOTES/        # 代码阅读笔记

data/
  projects.yaml              # 机器可读项目库
  tags.yaml                  # 标签定义

scripts/
  refresh_github_stats.py    # 自动刷新 stars/forks/issues/last_commit
  validate_project_links.py  # 检查链接是否失效
```

## 维护原则

1. 不只按 Star 数收集仓库，优先收录能服务科研工作流的项目。
2. 对自动科研项目记录：repo、类型、stars 快照、许可证、是否可本地运行、是否支持引用、是否支持本地文档、是否有评测。
3. 对 baseline 仓库记录 paper、commit、环境、数据集、评测脚本和复现状态。
4. 对工具类仓库记录许可证、部署复杂度、是否适合本地化使用。
5. 对 AVSE / AVSS / codec / speech 相关项目优先补充实验指标和复现状态。
6. 每月至少刷新一次重点项目的 stars、forks、open issues、last commit、release 和 license。
