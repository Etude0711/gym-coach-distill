# References — 判断库

本目录承接 `SKILL.md` 放不下的**可检索**内容。由用户 `ANSWERS.md` 蒸馏而来，Agent 按场景路由读取。

## 写入规范

- 单文件建议 **<200 行**；过长则按子主题拆分。
- 每条判断尽量含：**结论 + 指标/证据 + 边界 + if-then**。
- 数字与政策标注 **时点/公司**（可脱敏为「某头部连锁，202X」）。
- 禁止写入：未脱敏个人信息、未公开合同条款、可识别商业秘密。

## 子目录

| 目录 | 内容类型 | 示例文件名 |
|------|----------|------------|
| `judgments/` | 分场景立场与框架 | `store.md`, `franchise.md` |
| `metrics/` | 指标字典、阈值表 | `index.md`, `store-health.md` |
| `playbooks/` | 决策树、排查顺序、澄清问题 | `diagnosis-order.md` |
| `pitfalls/` | 踩坑、误区、反常识 | `index.md`, `anti-conventional.md` |

## 已有文件（PRIORITY 蒸馏）

| 路径 | 内容 |
|------|------|
| `judgments/store.md` | 门店三表诊断入口 |
| `judgments/coach.md` | 教练激励绑/不绑、人均消课红线 |
| `judgments/franchise.md` | 选址 + 招商筛选 |
| `metrics/store-financials.md` | 损益/资产负债/现金流盯盘 |
| `playbooks/clarify-questions.md` | 先追问、费曼输出、微信兜底 |
| `playbooks/self-check.md` | 五框架自查顺序（用户命名） |
| `playbooks/seasonality.md` | 淡旺季与大促节奏 |
| `pitfalls/unconventional.md` | 反常识 Top 3 |
| `pitfalls/scope-boundaries.md` | P2 不写/免责/转介边界 |
| `pitfalls/franchise-leverage.md` | 教练凑钱开店 vs 接盘 |

## 蒸馏命令（给 Agent）

```
阅读 ANSWERS.md 与 PRIORITY.md，将内容拆分写入 references/ 各 md，
更新 SKILL.md 中的「决策骨架」「澄清问题库」占位节，并删除重复表述。
```
