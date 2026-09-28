# 毛选看世界 Skill

把地缘事件写成「毛选看世界」专栏。先定文类：主角自己出手走**主篇**；战火溢到盟友本土、基地、后勤走**侧翼/续篇**。不填「格局层 → 区域层 → 事件层」。纪律仍在：行为≠结果、功能≠动机、方向≠幅度、变量≠预测；收束必须带证伪条件或可观察信号。

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

然后直接说「写一篇毛选看世界」或「用 mao-contradiction-analysis」。

## 在 Claude Code / 其他 Agent 里用

```bash
cp -R skills/mao-contradiction-analysis ~/.claude/skills/
```

目录里必须保留 `SKILL.md`。对照写法读同目录 `examples.md`。

## 两种成稿

**主篇**（换岗、谈+打）：日期动作 → 为什么要做 → 火药桶 → 对手或选项 → 时间窗口 → 大国夹缝 → 数据黑箱 → 主要矛盾 + 证伪条件。

**侧翼/续篇**（Fairford 这一类）：现场与资产 → 外因贴上围栏 → 内政管道分层 → 接到主结构（主次不颠倒）→ 结构判断与个案定性分开 + 可观察信号。

禁止用棋手棋盘、目标函数集合开篇；禁止把侧翼硬套成 50 天闪电战或两套民调。

完整规则：[`skills/mao-contradiction-analysis/SKILL.md`](skills/mao-contradiction-analysis/SKILL.md)  
正反示例：[`skills/mao-contradiction-analysis/examples.md`](skills/mao-contradiction-analysis/examples.md)

## 仓库结构

```text
skills/mao-contradiction-analysis/
  SKILL.md       # 专栏章法 + 硬闸
  examples.md    # 正反示例
.cursor/skills/mao-contradiction-analysis/  # 指向上述目录
```
