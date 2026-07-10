# Chinese AI Data Hub

> **A high-quality Chinese Data Hub built for AI / LLM developers**  
> Discover, access, and contribute high-quality datasets — supporting LLM pretraining, instruction tuning, preference alignment, long-context, and domain-specific applications.

[![Stars](https://img.shields.io/github/stars/Yuuqq/CLUEDatasetSearch?style=social)](https://github.com/Yuuqq/CLUEDatasetSearch)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/Yuuqq/CLUEDatasetSearch/pulls)
[![Issues](https://img.shields.io/github/issues/Yuuqq/CLUEDatasetSearch)](https://github.com/Yuuqq/CLUEDatasetSearch/issues)

---

## 🔍 Quick Dataset Lookup

Need a fast overview of all available datasets?

→ **[DATASETS.md](DATASETS.md)** — Comprehensive overview table grouped by AI workflow categories (searchable with Ctrl+F).

**Recent Focus Additions (July 2026)**:
- **Legal**: CAIL2018 / CAIL2019-SCM / JEC-QA / LeCaRD / DISC-Law-SFT
- **Finance (Research Reports / Annual Reports)**: FinRpt, CFQA, CFLUE, DocFEE, FinChina SA, FinCUGE, FinGPT
- **Code**: Gitee + GitCode Chinese code corpora, Ling-Coder-SFT, Evol-Code-ZH (CodeAlpaca-CN)

---

## 🎯 Who is this Data Hub for?

- **LLM Developers**: Looking for pretraining corpora, SFT/instruction data, and preference data
- **RAG / Agent Developers**: Domain knowledge, long-context, and tool-use datasets
- **Researchers**: High-quality evaluation benchmarks and ablation datasets
- **Industry Teams**: Vertical domain data (**legal, medical, finance, code**, education)

---

## 🚀 Quick Start (for AI Developers)

### 1. Online Search (Fastest)
https://www.cluebenchmarks.com/dataSet_search.html

### 2. Local Clone + Structured Data
```bash
git clone https://github.com/Yuuqq/CLUEDatasetSearch.git
cd CLUEDatasetSearch
```

We recommend starting with the structured JSON files in the `data/` directory.

---

## 📍a Recommended Categories for AI Workflows

We organize datasets according to the modern AI development pipeline:

### 🔥 Pretraining & Foundation Corpora
- Large-scale Chinese web, books, code, and encyclopedia data
- Ideal for continued pretraining or domain adaptation

### 📝 Instruction Tuning / SFT
- High-quality QA, conversation, and task instruction data
- Recommended for Supervised Fine-Tuning

### ❤️ Preference & Alignment (RLHF / DPO)
- Human preference data and reward model training data
- For DPO, PPO, ORPO, and other alignment methods

### 📊 Evaluation & Benchmarks
- Chinese comprehensive capability benchmarks (SuperCLUE, CLUE, etc.)
- Specific capability evaluation (reasoning, long-context, code, math)

### 🏥 Domain-Specific  ← **Actively Expanding**
- **Legal**: CAIL series, JEC-QA, LeCaRD, DISC-Law-SFT and more
- **Finance**: Research report generation (FinRpt), Annual report QA (CFQA), Event extraction (DocFEE), Fine-grained sentiment (FinChina SA), CFLUE, etc.
- **Code**: Gitee/GitCode Chinese code corpora, Ling-Coder-SFT, CodeAlpaca-CN (Evol-Code-ZH)
- Medical, education, government, etc.
- Perfect for vertical LLMs or RAG applications

See `data/domain/domain.json` and the Domain-Specific table in [DATASETS.md](DATASETS.md).

---

## 📂 Repository Structure (AI-Friendly)

```
chinese-ai-data-hub/
├── README.md / README_EN.md
├── DATASETS.md                 # Auto-generated overview table
├── CONTRIBUTING.md
├── data/
│   ├── pretraining/
│   ├── instruction/
│   ├── preference/
│   ├── long_context/
│   ├── evaluation/
│   ├── tasks/
│   └── domain/                 # Legal / Finance / Code / Medical (priority)
├── scripts/
└── .github/
```

---

## ✨ Featured Recommendations (2026 Update)

**Domain Highlights**:
- **Legal**: CAIL2018 (judgment prediction), JEC-QA (judicial exam), DISC-Law-SFT
- **Finance**: FinRpt (research report generation), CFQA (annual report QA), CFLUE, DocFEE
- **Code**: Gitee/GitCode Chinese code corpora, Ling-Coder-SFT, Evol-Code-ZH

**General**:
- **Pretraining**: `pleisto/wikipedia-cn-20230720-filtered`, BAAI CCI3-HQ
- **Instruction**: Qwen Instruct 2025 / BELLE / Infinity-Instruct / Magpie
- **Evaluation**: SuperCLUE series, C-Eval, AgentBench Chinese 2026

More high-quality 2025–2026 datasets are being added rapidly.

---

## 📥 How to Download Datasets?

Recommended sources (in order of preference):

1. **Hugging Face Datasets** (Strongly Recommended)
2. **ModelScope** (Often faster in China)
3. Original sources (GitHub / paper homepages)

---

## 🤝 Contribution Guide

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details.

PRs that add new vertical-domain entries to `data/domain/domain.json` are especially welcome!

---

## 📜 Disclaimer

This repository only indexes publicly available dataset information. All copyrights belong to the original authors.

---

## 🔗 Related Resources

- **CLUE Official**: https://www.cluebenchmarks.com/
- **Hugging Face Chinese Datasets**: https://huggingface.co/datasets?language=zh

---

## 🔄 Relationship with the Original Repository

This repository is a **community-maintained and modernized fork** of [CLUEbenchmark/CLUEDatasetSearch](https://github.com/CLUEbenchmark/CLUEDatasetSearch).

### Key Differences:

| Aspect              | Original (CLUEbenchmark)          | This Repo (Chinese AI Data Hub)                  |
|---------------------|-----------------------------------|-----------------------------------------------|
| **Maintenance**     | Largely inactive since 2022       | Actively maintained (2026 updates ongoing)    |
| **Goal**            | Static dataset list               | **Dynamic AI-oriented Data Hub**              |
| **Data Format**     | Markdown tables only              | **Structured JSON** + Markdown (dual-track)   |
| **Dataset Freshness**| Mostly 2017–2020 data             | Prioritizes 2023–2026 high-quality AI data    |
| **AI Focus**        | General NLP listing               | Categorized for Pretraining / SFT / RLHF / Eval / Long-Context / Domain |
| **Contribution**    | Traditional issues                | Standardized templates + JSON-first           |
| **Download**        | Few HF links                      | **HF-first** + ModelScope                     |
| **Documentation**   | Chinese only                      | **Bilingual** (README + README_EN)            |

**Our mission**: Preserve the spirit of the original project while transforming it into a **long-term maintainable, AI-developer-friendly** Chinese NLP / LLM Data Hub.

---

**Making Chinese AI dataset discovery and sharing simple and efficient!**

Suggestions and new dataset submissions via Issues or PRs are highly welcome.  
Star ⭐ to support ongoing maintenance!
