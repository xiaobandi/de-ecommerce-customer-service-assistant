# 能力与字段速查

技能：`handoff-to-human`（L1 原子技能）

## 元信息

| 字段 | 值 |
|---|---|
| 技能 ID | `skill_handoff_to_human` |
| 目录 | `skills/handoff-to-human` |
| 复杂度 | S |
| 阶段 | P0 |
| 可见性 | platform_shared |
| 版本 | v1.0.0 |
| 许可 | MIT |
| 验证等级 | A（自带脚本 `handoff_triage.py`，已用真实夹具执行并抓取 stdout/stderr/退出码） |

## 输入契约

- **必填**：会话内容
- **可选**：可自动应答范围定义
- **可选**：SLA 规则

## 脚本清单

| 脚本 | 用途 | 调用方式 |
|---|---|---|
| `scripts/handoff_triage.py` | 确定性执行逻辑 | `python3 scripts/handoff_triage.py` |

真实调用：

```bash
python3 scripts/handoff_triage.py --file examples/input/chat.txt
```

## 质量门

- 敏感项一律不自动应答
- 交接摘要含'已确认'与'未知'两栏

## 已知陷阱

- AI 承诺赔偿金额或时效是企业真实风险点，一律转人工
- 用户重复被转接是体验杀手，第二次转接必须带上下文

## 边界

- 不索要密码、验证码、身份证等凭据
