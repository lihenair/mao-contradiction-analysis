# 毛选矛盾分析 Skill

把地缘事件写成「毛选看世界」式分析时用的 Agent Skill：强制走格局层 → 区域层 → 事件层，并卡住四条纪律——行为≠结果、动机≠事实、方向≠幅度、变量≠预测。

本仓库就是这份 Skill。用 Cursor、Claude Code 或其他兼容 [Agent Skills](https://agentskills.io) 的工具加载即可。

## 在 Cursor 里用

**打开本仓库：** Skill 已放在 `.cursor/skills/mao-contradiction-analysis/`，项目打开后即可被发现。

**装进其他项目：**

```bash
mkdir -p .cursor/skills
cp -R skills/mao-contradiction-analysis .cursor/skills/
```

**装成个人 Skill（对所有项目生效）：**

```bash
mkdir -p ~/.cursor/skills
cp -R skills/mao-contradiction-analysis ~/.cursor/skills/
```

然后直接说「按毛选矛盾分析框架写这篇」或「用 mao-contradiction-analysis 看这件事」。

## 在 Claude Code / 其他 Agent 里用

把 `skills/mao-contradiction-analysis/` 整夹复制到该运行时的 skills 目录，例如：

```bash
cp -R skills/mao-contradiction-analysis ~/.claude/skills/
```

目录里必须保留 `SKILL.md`。需要对照写法时，模型应再读同目录的 `examples.md`。

## 分析时强制经过的环节

1. 格局层（百年未有之大变局）→ 区域层 → 事件层，不可乱跳
2. 现象识别 → 性质定性 → **替代解释检验（同等篇幅）** → 矛盾定位 → 当事人视角 → 条件推演 → 历史类比
3. 条件推演的每条路径必须对应**不同结果**；禁止「无论如何都会……」式收束
4. 文末用 `SKILL.md` 第七节清单过一遍

完整规则在 [`skills/mao-contradiction-analysis/SKILL.md`](skills/mao-contradiction-analysis/SKILL.md)。正反示例在 [`skills/mao-contradiction-analysis/examples.md`](skills/mao-contradiction-analysis/examples.md)。

## 框架边界

- 有明确理论偏好（矛盾辩证法），不追求价值中立
- 主要矛盾的选择是主观的，但选择过程必须透明
- 操作逻辑可推演，真实动机不可证伪
- 历史类比是参照系，不是因果证明
- 格局层只讲力量对比的方向与裂缝/生长点，不提前给终局

## 仓库结构

```text
skills/mao-contradiction-analysis/
  SKILL.md       # 正式规则（最高优先级）
  examples.md    # 正反示例
.cursor/skills/mao-contradiction-analysis/  # 指向上述目录，供本仓库在 Cursor 中直接加载
```

`pattern-layer.md`（格局层更细的模式库）按设计后置，本版未收录。
