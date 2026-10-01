# 售前智能导购

> 意图识别→知识库检索→话术→商品推荐

工作流 `wf-ecom-cs-presale-guide`　·　归属 智能客服+售后　·　触发 事件（买家消息）　·　
复杂度 M　·　阶段 P0

## 调用链

- `文档问答（RAG）`（doc-qa-rag）
- `议价话术`（negotiation-copy）

## 文档

- [`WORKFLOW.md`](WORKFLOW.md) — 完整编排、闸门、降级与验收标准
- [`tests/cases.yaml`](tests/cases.yaml) — 端到端 / 闸门 / 降级用例

## 一句话试用

```text
帮我跑 智能客服+售后 的「售前智能导购」：<你的输入>
```
