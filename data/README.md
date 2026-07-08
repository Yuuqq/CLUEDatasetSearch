# Structured Data Directory (AI Data Hub)

This directory contains machine-readable JSON metadata for datasets, organized by modern AI development workflows.

## New Folder Structure

```
data/
├── README.md
├── pretraining/          # Large-scale pretraining corpora
├── instruction/          # SFT / Instruction tuning data
├── preference/           # RLHF / Preference / Alignment data
├── evaluation/           # Benchmarks & Evaluation datasets
└── domain/               # Vertical domain datasets (legal, medical, finance, code...)
```

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
  "category": "pretraining",
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
  "last_verified": "2026-07-08",
  "status": "active",
  "remarks": "High quality filtered version"
}
```

**New/Recommended fields**:
- `recommended_for`: array of use cases (e.g. "llm-pretraining", "sft", "rag", "evaluation", "agent")
- `quality_signals`: object with boolean flags
- `num_examples`, `size`

We are gradually migrating old data into this new structure.