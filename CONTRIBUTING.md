# 贡献指南 | Contributing Guide

欢迎为 **CLUEDatasetSearch** 贡献力量！  
我们目标是把这个仓库打造成**长期活跃、结构化、易维护**的中文 NLP Data Hub。

---

## 📌 贡献方式（推荐顺序）

### 1. 最简单：报告问题
- 数据集链接失效、描述错误、许可信息过时
- 使用 GitHub Issue 模板：
  - [Broken Link / 数据集链接失效](https://github.com/Yuuqq/CLUEDatasetSearch/issues/new?template=broken_link.md)
  - 其他问题直接开 issue 即可

### 2. 添加新数据集（最欢迎！）
推荐两种方式：

**方式 A（推荐）：直接提交 PR**
1. 在对应类别的 `data/<category>.json` 中添加新条目（结构见下文）
2. 可选：在对应类别的 `README.md` 表格中同步添加（未来会自动生成）
3. 提交 PR 时请描述清楚数据集来源、论文链接、HF ID（如有）

**方式 B：先开 Issue**
使用 [New Dataset Issue 模板](https://github.com/Yuuqq/CLUEDatasetSearch/issues/new?template=new_dataset.md)

### 3. 改进结构与工具
- 改进验证脚本
- 添加 Hugging Face Dataset 自动同步
- 优化 README / 搜索体验
- 非常欢迎！

---

## 📋 数据集元数据结构（JSON 格式）

我们正在逐步迁移到结构化 JSON，便于程序处理和未来自动化。

**推荐字段（data/xxx.json 中的对象）：**

```json
{
  "id": 101,
  "title": "数据集全称",
  "update_date": "2025-06",
  "provider": "机构/作者",
  "license": "Apache-2.0 / CC-BY-4.0 / 未知",
  "description": "简要说明（支持 Markdown）",
  "keywords": ["\u4e2d\u6587", "NER", "\u7ec6\u7c92度"],
  "category": "NER",
  "paper_url": "https://arxiv.org/abs/xxxx",
  "hf_dataset_id": "username/dataset-name",   // Hugging Face ID（强烈推荐）
  "download_url": "https://...",
  "size": "约 12GB / 50万条",
  "language": "\u4e2d\u6587",
  "tasks": ["ner", "entity-linking"],
  "last_verified": "2026-07-01",
  "status": "active",           // active / broken / deprecated
  "remarks": "额外备注"
}
```

**必填字段**：`title`, `description`, `category`  
**强烈推荐**：`hf_dataset_id`, `paper_url`, `license`

---

## ✅ 质量标准（我们优先收录）

- 有明确论文或技术报告
- 有开源许可或明确可商用/研究使用声明
- 数据可公开下载或通过 HF 便捷获取
- 信息相对准确（描述、链接、规模）
- 2023 年以后发布或仍有维护的数据集优先

---

## 🛠️ 开发与验证

仓库根目录提供一些脚本（持续完善中）：

```bash
# 未来计划
python scripts/validate_datasets.py          # 验证 JSON 格式 + 链接可访问性
python scripts/sync_from_huggingface.py      # 同步 HF 热门中文数据集
```

---

## 📜 行为准则

- 尊重原作者劳动成果
- 提交前请确保信息尽量准确
- 欢迎建设性讨论，保持友好

---

**感谢每一位贡献者！**  
你的每一个 PR 都在让中文 NLP 社区变得更好。

有任何问题欢迎在 issue 或 QQ 群（836811304）讨论。