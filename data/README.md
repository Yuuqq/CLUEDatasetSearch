# Structured Data Directory (AI Data Hub)

This directory contains machine-readable JSON metadata for datasets, organized by modern AI development workflows.

## Folder Structure

```
data/
├── README.md                 # This file
├── pretraining/              # Large-scale pretraining corpora
├── instruction/              # SFT / Instruction tuning data
├── preference/               # RLHF / Preference / Alignment data
├── long_context/             # Long-context training & evaluation
├── evaluation/               # Benchmarks & Evaluation datasets
├── tasks/                    # Traditional NLP tasks (NER etc.)
└── domain/                   # Vertical domain datasets ★ Priority
    ├── README.md             # Domain overview (legal / finance / code / medical)
    └── domain.json           # All domain entries (currently 23+)
```

## Domain Highlights (2026-07)

The `domain/` folder is actively expanded and currently covers:

- **Legal (法律)**: CAIL2018, CAIL2019-SCM, JEC-QA, LeCaRD, DISC-Law-SFT, CJRC, Taiwan Legal QA
- **Finance (金融 · 研报/财报/年报)**: FinRpt, CFQA, CFLUE, DocFEE, FinChina SA, FinCUGE, FinGPT-FinEval, Finance-Chinese-2025, Finance-Instruct-500k
- **Code (代码)**: Gitee Chinese Code Corpus, GitCode Chinese Code Corpus, Ling-Coder-SFT, Evol-Code-ZH (CodeAlpaca-CN)
- **Medical (医疗)**: cMedQA, CCKS2017-NER, shibing624/medical

See [DATASETS.md](../DATASETS.md) Domain-Specific section for the full searchable table.

## Improved JSON Schema (v2)

```json
{
  "id": "unique-id-or-slug",
  "title": "Dataset Full Name",
  "update_date": "2025-06",
  "provider": "Organization / Author",
  "license": "Apache-2.0",
  "description": "Short description",
  "keywords": ["chinese", "llm", "pretraining"],
  "category": "domain",
  "paper_url": "https://arxiv.org/abs/...",
  "hf_dataset_id": "username/dataset-name",
  "download_url": "https://...",
  "size": "120GB / 50M examples",
  "num_examples": 50000000,
  "language": "Chinese",
  "tasks": ["pretraining", "continued-pretraining"],
  "recommended_for": ["llm-pretraining", "domain-adaptation", "rag"],
  "quality_signals": {
    "license_clear": true,
    "human_annotated": false,
    "verified_2026": true
  },
  "last_verified": "2026-07-10",
  "status": "active",
  "remarks": "High quality filtered version"
}
```

**Key fields**:
- `recommended_for`: array of use cases (e.g. "legal-llm", "finance-llm", "code-sft", "rag-legal")
- `quality_signals`: object with boolean flags
- `num_examples`, `size`, `hf_dataset_id` (strongly preferred)

## How to Add a New Dataset

1. Add a new object to the appropriate `*.json` (prefer `data/domain/domain.json` for vertical domains).
2. Follow the schema above.
3. Submit a PR. The GitHub Action will automatically regenerate `DATASETS.md`.

We are gradually migrating legacy Markdown category folders into this structured format.
