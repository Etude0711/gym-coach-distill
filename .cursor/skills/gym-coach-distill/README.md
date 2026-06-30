# gym-coach-distill

将 **8 年头部健身连锁运营**（加盟 / 门店 / 教练 / 产品 / 数据）与 **互联网中台运营** 中的判断，蒸馏为 Cursor Agent Skill。

## 文件一览

| 文件 | 用途 |
|------|------|
| `SKILL.md` | Agent 主指令（工作流、输入输出、路由） |
| `INTERVIEW.md` | 全量访谈题纲（8 模块 × 8–15 题） |
| `PRIORITY.md` | 下一轮必须先答的 8 题 |
| `ANSWERS.md` | **由你创建并填写**（从 INTERVIEW 模板复制） |
| `examples.md` | 试跑对话样例 |
| `references/` | 判断库（填答后迁入） |

## 推荐流程

1. ~~填写 `PRIORITY.md`~~ → 已写入 `ANSWERS.md`（PRIORITY 段）。
2. 优先补全：**P4 三表科目/阈值 → P5 加盟否决+案例 → P3 框架正式命名**。
3. 对 Agent 说：「根据 `ANSWERS.md` 蒸馏进 `references/` 并更新 `SKILL.md`」。
4. 用 2–3 个真实问题试跑，把 Q&A 记入 `examples.md`。

## 判断库目录（`references/`）

```
references/
├── README.md
├── judgments/          # 分场景判断短文（单文件建议 <200 行）
│   ├── chain.md      # 连锁
│   ├── store.md      # 门店
│   ├── coach.md      # 教练
│   ├── franchise.md  # 加盟
│   ├── product.md    # 产品
│   └── cross-platform.md
├── metrics/          # 指标定义、阈值、分层表
│   └── index.md
├── playbooks/        # 决策树、排查顺序、澄清问题
│   ├── clarify-questions.md
│   └── diagnosis-order.md
└── pitfalls/         # 踩坑、误区、反常识合集
    └── index.md
```

## 安装位置（已确认）

- **项目 skill — 本仓库**：`gym&coach/.cursor/skills/gym-coach-distill/`
- 随 git 分享给同行；在本仓库打开 Cursor 时可用 `@gym-coach-distill`
- **不**默认同步到 `~/.cursor/skills/`（若你个人其他项目也要用，再手动复制）

### 个人 skill vs 本仓库（备忘）

| | 本仓库（当前） | 个人 `~/.cursor/skills/` |
|---|---|---|
| 谁能用 | clone 仓库的人 | 仅你本机所有项目 |
| 分享 | push 即可 | 不随 git |
| 适合 | 教同行、共建判断库 | 私密备忘 |

## 日志（后续脚本）

校验/蒸馏脚本运行时，日志写入仓库根目录 `logs/`，文件名示例：`distill-20260604-143022.log`。本回合仅文档骨架，无脚本。

## 与 `gym-ops-distill` 的关系

同仓库下的 `gym-ops-distill` 为早期简版题纲；**以 `gym-coach-distill` 为准**。填答后勿维护两份 ANSWERS。
