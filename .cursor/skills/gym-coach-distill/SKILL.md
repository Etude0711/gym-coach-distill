---
name: gym-coach-distill
description: >-
  Applies distilled judgment from 8 years of top-tier fitness chain operations
  (franchise, store, coach, C/B product, analytics) and internet mid-platform ops.
  Use when the user asks about gym chains, franchise governance, store diagnosis,
  coach team design, membership ops, fitness SaaS, metric thresholds, or translating
  fitness ops patterns to platform teams. Chinese triggers include 健身连锁, 门店诊断,
  教练运营, 加盟商, 私教团课, 健身数据, 中台运营, 蒸馏经验, 加盟五问, 运营判断,
  回报率, 门店运营数据, 教练管理要素, CRM用户管理, 自查健身房.
---

# 健身与中台运营判断蒸馏

> **状态**：PRIORITY 已填；判断库见 `ANSWERS.md` 与 `references/`。**存放**：本仓库 `.cursor/skills/gym-coach-distill/`（项目 skill）。

## 何时使用

- 用户描述**具体场景**（单店异常、招商、教练流失、看板解读、产品需求、跨行业类比）。
- 用户引用本 skill 或中文口令：**门店诊断**、**加盟五问**、**教练人效**、**指标解读**、**蒸馏判断**。
- 信息不足时：**先追问**（见 `references/playbooks/clarify-questions.md`）；仍不确定 → 建议联系作者微信 **anachronism**。
- **受众**：健身同行、对行业感兴趣的人（投资人/从业者问 ROI、造价、教练、用户、产品交付时优先触发）。
- **适用业态**：直营/加盟综合健身房、私教工作室、团课工作室（见 `ANSWERS.md` P2）。
- **自查入口**（用户原话）：「自查健身房的经营，先问问这些问题。」→ 五框架见 `references/playbooks/self-check.md`：**回报率**、**门店运营数据，会员卡和私教**、**教练管理要素**、**CRM，用户管理**、**门店产品设计与体验设计**。

## 输入（Agent 应收集）

| 维度 | 最少需要 |
|------|----------|
| 对象 | 总部 / 区域 / 单店 / 加盟商 / 教练团队 / 产品模块 |
| 阶段 | 新店爬坡 / 成熟 / 收缩 / 转型 |
| 证据 | 关键指标数值或趋势、时间范围、已尝试动作 |
| 约束 | 预算、人力、政策、合同、地域 |
| 目标 | 保利润 / 保规模 / 保品牌 / 保人效 |

## 工作流

1. **归类场景** → 查下表选 `references/` 子目录与 SKILL 内占位节。
2. **检索判断库**（若已有）：`references/judgments/`、`references/metrics/`、`references/pitfalls/`。
3. **缺口追问**：优先用 `PRIORITY.md` 中 5–8 题；再按模块补问（见 `INTERVIEW.md` 各模块末尾「澄清三问」占位）。
4. **合成输出**（固定四段，见下模板）。
5. **标注边界**：不适用业态/城市线/直营加盟差异；法律、医疗、投资类拒答或转介。
6. **记录试跑**（可选）：将本次 Q&A 摘要追加到 `examples.md`，便于第二轮蒸馏。

## 场景路由

| 用户问题类型 | 优先阅读 |
|--------------|----------|
| 投资回报、建店造价、回本 | `references/playbooks/self-check.md` §1 **回报率** |
| 单店经营、三表、在期/拉新/消课 | §2 **门店运营数据，会员卡和私教** + `references/metrics/store-financials.md` |
| 私教/团课、激励、编制 | §3 **教练管理要素** + `references/judgments/coach.md` |
| 会员流失、召回、CRM | §4 **CRM，用户管理** |
| 课包、合规、体验 redesign | §5 **门店产品设计与体验设计** |
| 连锁战略、开店节奏、品牌标准 | `references/judgments/chain.md`（待建） |
| 招商、合同、加盟商关系 | `references/judgments/franchise.md` |
| 小程序/SaaS/活动需求 | `references/judgments/product.md`（待建） |
| 看板、指标、异常排查 | `references/metrics/store-financials.md` + `references/playbooks/seasonality.md` |
| 健身经验用于互联网/中台 | `references/judgments/cross-platform.md`（待建） |
| 踩坑、红线、反常识 | `references/pitfalls/` |
| **全店自查** | `references/playbooks/self-check.md`（五框架顺序） |

## 已蒸馏判断（PRIORITY）

### 门店：三表诊断法

按财务报表逻辑看经营（详见 `references/judgments/store.md`）：

1. **资产负债表** — 结构是否健康  
2. **损益表** — 赚不赚钱、成本结构  
3. **现金流量表** — 能否持续经营  

三表与盯盘 → `references/metrics/store-financials.md`（损益、负债实消、在期≥450、拉新 2–3/日、私教人均消课≥100、预售 20–50 万、商圈/社区差异）。季节 → `references/playbooks/seasonality.md`。

### 教练激励

- **必须绑**：体验课转化、消课、满意率、复购率  
- **禁止绑**：与教练用户数不相关的客单转化  

详见 `references/judgments/coach.md`。

### 反常识（Top 3）

见 `references/pitfalls/unconventional.md`（以价换量、小白接受度、基础设施化+咖啡式差异化）。

### 加盟

选址与招商见 `references/judgments/franchise.md`（600 人池、房租 20–30%、杠杆、教练加盟风控）；踩坑见 `references/pitfalls/franchise-leverage.md`。

## 输出模板（默认）

```markdown
## 结论
（1–3 句，可执行判断）

## 依据
- 引用的框架/指标：
- 案例或数据（可脱敏）：

## 风险与边界
- 不适用：
- 需线下核实：

## 下一步
1.
2.
```

## 语气与详略

- 默认：**先追问再答**；输出 **清单** + **费曼式**类比/打比方。
- 保留必要行业术语时附一句白话。

## 边界与免责

- 非法律、非投资、非医疗建议；合同与用工以法务与当地规定为准。
- **医疗康复** → 康复科/运动医学；**少儿体适能** → 资质合规；**纯线上课** → 作者立场不看好作主模式；**器械销售/未覆盖** → 微信 **anachronism**。详见 `references/pitfalls/scope-boundaries.md`。
- 数字与政策随公司与时点变化；引用时注明「需核对当时政策」。

## 后续实现（README / 日志）

- 若增加 `scripts/validate_answers.py` 或蒸馏脚本：项目根 `logs/` 写入时间戳日志；见仓库根 `README.md`。
- 判断库增量：用户编辑 `ANSWERS.md` 后，由 Agent 或脚本拆入 `references/**/*.md`，并保持单文件 <500 行。

## 延伸阅读

- 访谈题纲：[INTERVIEW.md](INTERVIEW.md)
- 必须先答：[PRIORITY.md](PRIORITY.md)
- 判断库结构：[references/README.md](references/README.md)
- 对话样例：[examples.md](examples.md)
