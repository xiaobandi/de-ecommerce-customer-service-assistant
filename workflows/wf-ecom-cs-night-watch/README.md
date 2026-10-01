# 夜间值守+次日汇总

> 自动应答→异常标记→晨报推送

工作流 `wf-ecom-cs-night-watch`　·　归属 智能客服+售后　·　触发 定时（22:00-8:00 + 8:30 晨报）　·　
复杂度 S　·　阶段 P0

## 调用链

- `文档问答（RAG）`（doc-qa-rag）
- `简报生成`（brief-generator）

## 文档

- [`WORKFLOW.md`](WORKFLOW.md) — 完整编排、闸门、降级与验收标准
- [`tests/cases.yaml`](tests/cases.yaml) — 端到端 / 闸门 / 降级用例

## 一句话试用

```text
帮我跑 智能客服+售后 的「夜间值守+次日汇总」：<你的输入>
```
