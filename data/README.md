# 结构化数据集目录 (Structured Data)

本目录存放机器可读的 JSON 格式数据集元数据，是未来 Data Hub 的核心维护方式。

## 优势

- 便于程序验证、搜索、同步到 Hugging Face
- 支持 rich metadata（HF ID、最后验证日期、状态等）
- 未来可自动生成各分类的 Markdown 表格

## 文件命名规范

- `ner.json`
- `qa.json`
- `sentiment_analysis.json`
- `text_classification.json`
- `text_matching.json`
- `text_summarization.json`
- `machine_translation.json`
- `knowledge_graph.json`
- `corpus.json`
- `reading_comprehension.json`

## 贡献方式

1. 在对应 JSON 文件中添加新对象（参考 `ner.json` 示例）
2. 运行验证脚本（未来提供）
3. 提交 PR

我们会逐步把原有 Markdown 表格迁移/同步到 JSON。