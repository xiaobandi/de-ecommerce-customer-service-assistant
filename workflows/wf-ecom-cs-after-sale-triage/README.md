# 售后工单分流与安抚

> 情绪识别→分级→安抚话术/转人工

工作流 `wf-ecom-cs-after-sale-triage`　·　归属 智能客服+售后　·　触发 事件　·　
复杂度 M　·　阶段 P0

## 调用链

- `评论情绪识别`（review-sentiment-tag）
- `转人工分流`（handoff-to-human）

## 文档

- [`WORKFLOW.md`](WORKFLOW.md) — 完整编排、闸门、降级与验收标准
- [`tests/cases.yaml`](tests/cases.yaml) — 端到端 / 闸门 / 降级用例

## 一句话试用

```text
帮我跑 智能客服+售后 的「售后工单分流与安抚」：<你的输入>
```
