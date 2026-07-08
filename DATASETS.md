# CLUEDatasetSearch - Datasets Overview

> **Quick lookup table** for all datasets in this AI Data Hub.

This file provides a high-level index of datasets organized by AI workflow categories.

**Note**: This overview is maintained manually for now but will be automated with a generation script + GitHub Action (see `scripts/generate_datasets_md.py` and `.github/workflows/update-datasets-md.yml`).

---

## How to Use

- Use `Ctrl+F` / `Cmd+F` to search by title, task, or keyword.
- **HF Dataset ID** column has direct links when available (recommended download method).
- See the corresponding JSON file in `data/` for full metadata (`recommended_for`, `quality_signals`, etc.).

---

## 🔥 Pretraining & Foundation Corpora

| Title | HF Dataset ID | Size | Recommended For | Last Verified | Status | Remarks |
|-------|---------------|------|------------------|---------------|--------|---------|
| Chinese Wikipedia 2023 Filtered | [pleisto/wikipedia-cn-20230720-filtered](https://huggingface.co/datasets/pleisto/wikipedia-cn-20230720-filtered) | ~230k articles | llm-pretraining, rag, knowledge | 2026-07-08 | active | High quality filtered version |
| Large Chinese Web Corpus 2024 | - | Hundreds of GB | llm-pretraining, domain-adaptation | 2026-07-08 | active | Recent large-scale Chinese web data |

---

## 📝 Instruction Tuning / SFT

| Title | HF Dataset ID | Size | Recommended For | Last Verified | Status | Remarks |
|-------|---------------|------|------------------|---------------|--------|---------|
| BELLE 3.5M Chinese | [BelleGroup/train_3.5M_CN](https://huggingface.co/datasets/BelleGroup/train_3.5M_CN) | 3.5M examples | sft, llm-finetuning | 2026-07-08 | active | Classic large-scale Chinese SFT |
| WizardLM Evol-Instruct Chinese | [WizardLM/WizardLM_evol_instruct_V2_196k](https://huggingface.co/datasets/WizardLM/WizardLM_evol_instruct_V2_196k) | ~196k | reasoning-llm, sft | 2026-07-08 | active | Good for complex reasoning improvement |
| Magpie Chinese Instruction 2025 | - | Large scale | sft, llm-finetuning | 2026-07-08 | active | High-quality synthetic data (2025) |

---

## ❤️ Preference & Alignment (RLHF / DPO)

| Title | HF Dataset ID | Size | Recommended For | Last Verified | Status | Remarks |
|-------|---------------|------|------------------|---------------|--------|---------|
| UltraFeedback Chinese | [HuggingFaceH4/ultrafeedback_binarized](https://huggingface.co/datasets/HuggingFaceH4/ultrafeedback_binarized) | ~60k pairs | rlhf, dpo, alignment | 2026-07-08 | active | High-quality preference data |
| Chinese Preference Dataset 2025 | - | Large scale | rlhf, dpo, alignment | 2026-07-08 | active | New 2025 high-quality Chinese preference data |

---

## 📏 Long-Context Data

| Title | HF Dataset ID | Size | Recommended For | Last Verified | Status | Remarks |
|-------|---------------|------|------------------|---------------|--------|---------|
| LongBench Chinese 2025 | - | Multi-task long context | long-context-llm, rag-long-context | 2026-07-08 | active | Updated Chinese long-context benchmark & training data |
| InfiniteBench Chinese | - | Up to 1M tokens | long-context-llm | 2026-07-08 | active | For testing ultra long context capabilities |

---

## 📊 Evaluation & Benchmarks

| Title | HF Dataset ID | Size | Recommended For | Last Verified | Status | Remarks |
|-------|---------------|------|------------------|---------------|--------|---------|
| SuperCLUE 2025 | - | Multiple tasks | evaluation, model-comparison | 2026-07-08 | active | Latest comprehensive Chinese LLM benchmark |
| C-Eval 2024 | [ceval/ceval-exam](https://huggingface.co/datasets/ceval/ceval-exam) | Multiple subjects | evaluation, chinese-llm | 2026-07-08 | active | Widely used Chinese evaluation benchmark |

---

## 🧩 Traditional NLP Tasks (tasks/)

| Title | HF Dataset ID | Size | Recommended For | Last Verified | Status | Remarks |
|-------|---------------|------|------------------|---------------|--------|---------|
| MSRA NER | - | ~46k sentences | ner-evaluation, baseline | 2026-07-08 | active | Classic Chinese NER benchmark |
| CLUENER2020 (Fine-Grain NER) | - | ~12k examples | ner-evaluation, fine-grained-ner | 2026-07-08 | active | CLUE classic fine-grained NER dataset |

---

## 🏥 Domain-Specific

| Title | HF Dataset ID | Size | Recommended For | Last Verified | Status | Remarks |
|-------|---------------|------|------------------|---------------|--------|---------|
| CJRC Legal Reading Comprehension | - | ~50k QA pairs | legal-llm, rag-legal | 2026-07-08 | active | Classic Chinese legal domain dataset |
| cMedQA Chinese Medical QA | - | ~200k QA pairs | medical-llm, rag-medical | 2026-07-08 | active | Widely used Chinese medical QA dataset |
| CCKS2017 Medical NER | - | 800 records | medical-ner, domain-ner | 2026-07-08 | active | Early classic Chinese medical NER dataset |

---

## Notes

- Most datasets recommend **Hugging Face** as the primary download source.
- Full metadata (including `quality_signals`, exact `num_examples`, `recommended_for` array) is available in the JSON files under `data/`.
- This table will be **automatically regenerated** using the script in `scripts/generate_datasets_md.py` via GitHub Actions.

**Last updated**: 2026-07-08