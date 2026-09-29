# 毛选看世界 Skill

把地缘事件写成「毛选看世界」专栏。纲只有毛选，其他只当目，没有第二个纲。先抓多源通稿钉事实箱，再定文类：主角出手走**主篇**；盟友基地/内政走**侧翼·后勤反噬**；代理人次级战区走**侧翼·边缘燃烧**。两类侧翼禁止互套。不填格局层作业纸。收束的信号必须分叉成不同结果。

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

**侧翼·后勤反噬**（Fairford）：现场与资产 → 内政管道 → 接到主结构。

**侧翼·边缘燃烧**（塔伊兹）：事实箱与前线地理 → 边缘三特征 → 内战/清剿替代解释改归档 → 接到主结构（成本由平民承担）→ 三条路径三种结果。

动笔前应抓 Reuters/AFP/AP/DW/Al Jazeera/新华等公开通稿。禁止用棋手棋盘开篇，禁止把塔伊兹写成 Fairford。

完整规则：[`skills/mao-contradiction-analysis/SKILL.md`](skills/mao-contradiction-analysis/SKILL.md)  
正反示例：[`skills/mao-contradiction-analysis/examples.md`](skills/mao-contradiction-analysis/examples.md)  
系列成稿：[`columns/`](columns/)

## 仓库结构

```text
skills/mao-contradiction-analysis/
  SKILL.md       # 专栏章法 + 硬闸
  examples.md    # 正反示例
columns/                     # 系列成稿（校准用，不是通稿汇编）
.cursor/skills/mao-contradiction-analysis/  # 指向技能目录
```
