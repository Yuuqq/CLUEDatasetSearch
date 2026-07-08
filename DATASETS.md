# CLUEDatasetSearch - Datasets Overview

> **Quick lookup table** for all datasets in this AI Data Hub. Use `Ctrl+F` / `Cmd+F` to search by name, task, or keyword.

This file provides a high-level index. For detailed metadata, see the JSON files in each `data/` subfolder.

---

## 📚 How to Use This Table

- **Category**: Organized by modern AI workflow
- **HF Dataset ID**: Clickable link when available (recommended way to download)
- **Recommended For**: Suggested use cases
- **Status**: `active` / `deprecated`

---

## 🔥 Pretraining & Foundation Corpora

| Title | HF Dataset ID | Size | Recommended For | Last Verified | Status |emarks |
|-------|---------------|------|------------------|---------------|--------|--------|
| Chinese Wikipedia 2023 Filtered | [pleisto/wikipedia-cn-20230720-filtered](https://huggingface.co/datasets/pleisto/wikipedia-cn-20230720-filtered) | ~230k articles | LLM pretraining, RAG, Knowledge injection | 2026-07-08 | active | High quality filtered |
| Large Chinese Web Corpus 2024 | - | Hundreds of GB | Continued pretraining, Domain adaptation | 2026-07-08 | active | Recent large-scale web data |

---

## 📝 Instruction Tuning / SFT

| Title | HF Dataset ID | Size | Recommended For | Last Verified | Status | Remarks |
|-------|---------------|------|------------------|---------------|--------|---------|
| BELLE 3.5M Chinese | [BelleGroup/train_3.5M_CN](https://huggingface.co/datasets/BelleGroup/train_3.5M_CN) | 3.5M examples | SFT, LLM fine-tuning | 2026-07-08 | active | Classic large-scale Chinese SFT |
| WizardLM Evol-Instruct Chinese | [WizardLM/WizardLM_evol_instruct_V2_196k](https://huggingface.co/datasets/WizardLM/WizardLM_evol_instruct_V2_196k) | ~196k | Reasoning-focused SFT | 2026-07-08 | active | Good for complex reasoning |
| Magpie Chinese Instruction 2025 | - | Large scale | SFT, LLM fine-tuning | 2026-07-08 | active | High-quality synthetic data (2025) |

---

## ❤️ Preference & Alignment (RLHF / DPO)

| Title | HF Dataset ID | Size | Recommended For | Last Verified | Status | Remarks |
|-------|---------------|------|------------------|---------------|--------|---------|
| UltraFeedback Chinese | [HuggingFaceH4/ultrafeedback_binarized](https://huggingface.co/datasets/HuggingFaceH4/ultrafeedback_binarized) | ~60k pairs | DPO, RLHF, Alignment | 2026-07-08 | active | High-quality preference data |
| Chinese Preference Dataset 2025 | - | Large scale | DPO, RLHF, Alignment | 2026-07-08 | active | New 2025 high-quality Chinese preference data |

---

## 📏 Long-Context Data

| Title | HF Dataset ID | Size | Recommended For | Last Verified | Status | Remarks |
|-------|---------------|------|------------------|---------------|--------|---------|
| LongBench Chinese 2025 | - | Multi-task long context | Long-context LLM, Long RAG | 2026-07-08 | active | Updated Chinese long-context benchmark & training data |
| InfiniteBench Chinese | - | Up to 1M tokens | Ultra long-context modeling | 2026-07-08 | active | For testing very long context capabilities |

---

## 📊 Evaluation & Benchmarks

| Title | HF Dataset ID | Size | Recommended For | Last Verified | Status | Remarks |
|-------|---------------|------|------------------|---------------|--------|---------|
| SuperCLUE 2025 | - | Multiple tasks | LLM evaluation, Model comparison | 2026-07-08 | active | Latest comprehensive Chinese LLM benchmark |
| C-Eval 2024 | [ceval/ceval-exam](https://huggingface.co/datasets/ceval/ceval-exam) | Multiple subjects | Knowledge & reasoning evaluation | 2026-07-08 | active | Widely used Chinese evaluation benchmark |

---

## 🧩 Traditional NLP Tasks (tasks/)

| Title | HF Dataset ID | Size | Recommended For | Last Verified | Status | Remarks |
|-------|---------------|------|------------------|---------------|--------|---------|
| MSRA NER | - | ~46k sentences | NER baseline, Traditional NLP | 2026-07-08 | active | Classic Chinese NER benchmark |
| CLUENER2020 (Fine-Grain NER) | - | ~12k examples | Fine-grained NER evaluation | 2026-07-08 | active | CLUE classic fine-grained NER |

---

## 🏥 Domain-Specific

| Title | HF Dataset ID | Size | Recommended For | Last Verified | Status | Remarks |
|-------|---------------|------|------------------|---------------|--------|---------|
| CJRC Legal Reading Comprehension | - | ~50k QA pairs | Legal LLM, Legal RAG | 2026-07-08 | active | Classic Chinese legal domain dataset |
| cMedQA Chinese Medical QA | - | ~200k QA pairs | Medical LLM, Medical RAG | 2026-07-08 | active | Widely used Chinese medical QA |
| CCKS2017 Medical NER | - | 800 records | Medical NER | 2026-07-08 | active | Early classic Chinese medical NER |

---

## 📌 Notes

- Most datasets prioritize **Hugging Face** as the recommended download source.
- `recommended_for` values in JSON files include: `llm-pretraining`, `sft`, `rag`, `long-context-llm`, `alignment`, `evaluation`, etc.
- For full metadata (including `quality_signals`, exact `num_examples`, etc.), refer to the corresponding JSON file in `data/`.
- This table is manually maintained. Contributions to keep it updated are welcome!

---

**Last updated**: 2026-07-08

> Want to add a new dataset? See [CONTRIBUTING.md](CONTRIBUTING.md)