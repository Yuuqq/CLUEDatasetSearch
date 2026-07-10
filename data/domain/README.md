# Domain-Specific Datasets · 垂直领域数据集

> 法律 · 金融（研报/财报/年报）· 代码 · 医疗 等高价值垂直领域数据

本目录 (`domain.json`) 聚焦**垂直领域大模型 / RAG / Agent** 所需的中文高质量数据集。

## 当前覆盖（2026-07 更新，共 23+ 条）

### ⚖️ 法律 (Legal)
- **CAIL2018** — 大规模判决预测（2.6M+ 案件）
- **CAIL2019-SCM** — 相似案例匹配
- **JEC-QA** — 国家司法考试 QA
- **LeCaRD** — 法律案例检索
- **DISC-Law-SFT** — 复旦高质量法律指令微调
- CJRC、tw-legal-qa-3M 等

### 💰 金融 (Finance · 研报 / 财报 / 年报)
- **FinRpt** — 股票研报生成（CSI800，双语）
- **CFQA** — 上市公司年报/财报 QA（带页面 grounding）
- **CFLUE** — 中文金融理解评测（考试 + 应用任务）
- **DocFEE** — 文档级金融事件抽取（公告）
- **FinChina SA** — 细粒度金融情感分析（企业预警）
- **FinCUGE**、**FinGPT-FinEval**、Finance-Chinese-2025、Finance-Instruct-500k 等

### 💻 代码 (Code)
- **Gitee Chinese Code Corpus** — 3M+ 仓库中文代码语料
- **GitCode Chinese Code Corpus** — 补充 GitCode 源
- **Ling-Coder-SFT** — 5M+ 中英双语代码指令
- **Evol-Code-ZH (CodeAlpaca-CN)** — 中文 CodeAlpaca 进化版

### 🏥 医疗 (Medical)
- cMedQA、CCKS2017 Medical NER、shibing624/medical

## 使用建议

- **Legal LLM / 类案检索 / 法律 RAG** → CAIL 系列 + JEC-QA + LeCaRD + DISC-Law-SFT
- **金融研报 / 年报分析 / 金融 Agent** → FinRpt + CFQA + DocFEE + CFLUE
- **中文 Code LLM 预训练 / SFT** → Gitee/GitCode + Ling-Coder-SFT + Evol-Code-ZH

完整元数据（HF ID、paper、size、recommended_for 等）见 `domain.json`。  
总览表见根目录 [DATASETS.md](../../DATASETS.md) 的 **Domain-Specific** 部分。

欢迎继续补充更多垂直领域高质量数据集！
