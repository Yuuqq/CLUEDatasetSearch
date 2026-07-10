# Chinese AI Data Hub · 中文 AI 数据枢纽

> **为 AI / LLM 开发者打造的高质量中文数据枢纽**  
> 发现、获取、贡献高质量数据集 —— 支持大模型预训练、指令微调、偏好对齐、长上下文与垂直领域应用

[![Stars](https://img.shields.io/github/stars/Yuuqq/CLUEDatasetSearch?style=social)](https://github.com/Yuuqq/CLUEDatasetSearch)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/Yuuqq/CLUEDatasetSearch/pulls)
[![Issues](https://img.shields.io/github/issues/Yuuqq/CLUEDatasetSearch)](https://github.com/Yuuqq/CLUEDatasetSearch/issues)

---

## 🔍 快速查找数据集

需要快速浏览所有数据集？

→ **[DATASETS.md](DATASETS.md)** — 数据集快速总览表（按 AI 工作流分类，支持关键词搜索）

**最近重点补充（2026-07）**：
- **法律**：CAIL2018 / CAIL2019-SCM / JEC-QA / LeCaRD / DISC-Law-SFT
- **金融（研报/财报/年报）**：FinRpt、CFQA、CFLUE、DocFEE、FinChina SA、FinCUGE、FinGPT
- **代码**：Gitee + GitCode 中文代码语料、Ling-Coder-SFT、Evol-Code-ZH (CodeAlpaca-CN)

---

## 🎯 这个 Data Hub 适合谁？

- **大模型开发者**：寻找预训练语料、SFT/指令数据、偏好数据
- **RAG / Agent 开发者**：领域知识数据、长文本、工具使用数据
- **研究人员**：高质量评测 benchmark 和消融实验数据
- **企业落地团队**：垂直领域（**法律、医疗、金融、代码**、教育）数据

---

## 🚀 快速开始（面向 AI 开发者）

### 1. 在线搜索（最快）
https://www.cluebenchmarks.com/dataSet_search.html

### 2. 本地克隆 + 结构化数据
```bash
git clone https://github.com/Yuuqq/CLUEDatasetSearch.git
cd CLUEDatasetSearch
```

推荐优先查看 `data/` 目录下的 JSON 文件（机器可读 + 丰富元数据）。

---

## 📍a AI 场景推荐数据集分类

我们按照**现代 AI 开发流程**重新组织数据：

### 🔥 预训练 / 基础语料 (Pretraining & Corpus)
- 大规模中文网页、书籍、代码、百科数据
- 推荐用于继续预训练或领域适配

### 📝 指令微调 / SFT (Instruction Tuning)
- 高质量问答、对话、任务指令数据
- 推荐用于 Supervised Fine-Tuning

### ❤️ 偏好对齐 / RLHF (Preference & Alignment)
- 人类偏好数据、奖励模型训练数据
- 用于 DPO、PPO、ORPO 等对齐方法

### 📊 评测与 Benchmark (Evaluation)
- 中文综合能力评测（SuperCLUE、CLUE 等）
- 特定能力评测（推理、长文本、代码、数学等）

### 🏥 垂直领域 (Domain-Specific)  ← **重点持续扩展**
- **法律**：CAIL 系列、JEC-QA、LeCaRD、DISC-Law-SFT 等经典 + 现代数据集
- **金融**：研报生成 (FinRpt)、年报/财报 QA (CFQA)、事件抽取 (DocFEE)、细粒度情感 (FinChina SA)、CFLUE 等
- **代码**：Gitee/GitCode 中文代码语料、Ling-Coder-SFT、CodeAlpaca-CN (Evol-Code-ZH)
- 医疗、教育、政务等
- 适合垂直大模型或 RAG 应用

详见 `data/domain/domain.json` 与 [DATASETS.md](DATASETS.md) 中的 Domain-Specific 表格。

---

## 📂 仓库结构（AI 友好版）

```
chinese-ai-data-hub/
├── README.md / README_EN.md
├── DATASETS.md                 # 自动生成的数据集总览表
├── CONTRIBUTING.md
├── data/
│   ├── pretraining/
│   ├── instruction/
│   ├── preference/
│   ├── long_context/
│   ├── evaluation/
│   ├── tasks/
│   └── domain/                 # 法律 / 金融 / 代码 / 医疗 等垂直领域（重点）
├── scripts/
└── .github/
```

---

## ✨ 精选推荐（2026 更新）

**垂直领域亮点**：
- **法律**：CAIL2018（判决预测）、JEC-QA（司法考试）、DISC-Law-SFT
- **金融**：FinRpt（研报生成）、CFQA（年报QA）、CFLUE（金融评测）、DocFEE（事件抽取）
- **代码**：Gitee/GitCode 中文代码语料、Ling-Coder-SFT、Evol-Code-ZH

**通用**：
- **预训练**：`pleisto/wikipedia-cn-20230720-filtered`、BAAI CCI3-HQ
- **指令数据**：Qwen Instruct 2025 / BELLE / Infinity-Instruct / Magpie
- **评测**：SuperCLUE 系列、C-Eval、AgentBench Chinese 2026

更多高质量 2025–2026 年数据集持续补充中。

---

## 📥 如何下载数据集？

优先级推荐：

1. **Hugging Face Datasets**（最推荐）
2. **ModelScope**（国内更快）
3. 原始来源（GitHub / 论文主页）

---

## 🤝 贡献指南

详细请阅读 [CONTRIBUTING.md](CONTRIBUTING.md)

欢迎直接提交 PR 到 `data/domain/domain.json` 添加新垂直领域数据集！

---

## 📜 声明

本仓库仅做数据集信息整理与索引。所有版权归原作者所有。

---

## 🔗 相关资源

- **CLUE 官方**：https://www.cluebenchmarks.com/
- **Hugging Face 中文数据集**：https://huggingface.co/datasets?language=zh

---

## 🔄 与原仓库的关系与区别

本仓库是 [CLUEbenchmark/CLUEDatasetSearch](https://github.com/CLUEbenchmark/CLUEDatasetSearch) 的**社区维护与现代化改造版本**（fork）。

### 主要区别：

| 维度           | 原仓库 (CLUEbenchmark)          | 本仓库 (Chinese AI Data Hub)                  |
|---------------------|-----------------------------------|-----------------------------------------------|
| **维护状态**   | 2022 年后代码基本停止更新        | 持续活跃维护（2026 年仍在更新）        |
| **目标定位**   | 静态数据集列表                   | **面向 AI 的动态 Data Hub**                    |
| **数据格式**   | 仅 Markdown 表格                     | **结构化 JSON** + Markdown（双轨制）         |
| **数据时效性** | 多为 2017-2020 年数据                 | 优先补充 2023-2026 年高质量 AI 数据         |
| **AI 友好度**   | 通用 NLP 列表                     | 按预训练/SFT/RLHF/评测/长上下文/垂直领域分类         |
| **贡献流程**   | 传统 Issue                       | 标准化 Issue 模板 + JSON 优先                |
| **下载推荐**   | 较少 HF 链接                     | **HF 优先** + ModelScope                       |
| **文档**         | 中文主导                         | **中英双语** (README + README_EN)              |

**我们的目标**：在保留原项目精神的基础上，把它打造成**长期可维护、AI 开发者友好**的中文 NLP / LLM 数据枢纽。

---

**让中文 AI 数据集的发现和共享变得简单高效！**

有任何建议或想添加的数据集，欢迎直接开 Issue 或提交 PR。  
Star ⭐ 支持我们持续维护！
