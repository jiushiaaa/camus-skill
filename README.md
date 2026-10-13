<h1 align="center">camus.skill</h1>

<p align="center">加缪 · Albert Camus</p>

**中文** · [English](README.en.md)

<blockquote>
<p align="center">“必须想象西西弗是幸福的。”<br>— 加缪 · <a href="https://history.hanover.edu/courses/excerpts/111camus.html">《西西弗神话》</a></p>
</blockquote>

[![MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE) [![Agent Skills](https://img.shields.io/badge/Agent_Skills-Standard-blue.svg)](https://agentskills.io/) [![Made with nvwa-skill](https://img.shields.io/badge/Made_with-nvwa--skill-orange.svg)](https://github.com/alchaincyf/nuwa-skill)

**将荒诞、清醒与对具体生命的关切整理为思想分析 Skill，让 AI 在没有终极保证时讨论行动，也让宏大目标面对它要求别人付出的代价。**

---

## 效果示例

以下为说明用法而编写的示例，展示分析思路；不是哲学家原话或实测对话记录。

### 1. 如果努力没有最终答案，为什么还要继续？

> “没有最终答案”尚未说明今天的照料、友谊或工作全部失去价值。分析会先找出这一步推论里隐藏的要求，再讨论仍可承担的有限行动；不会拿“西西弗是幸福的”要求一个痛苦的人立刻振作。

### 2. 为了未来的幸福，牺牲眼前少数人不是值得的吗？

> 先把“牺牲”拆成谁决定、谁承受、有什么替代方案，以及未来收益凭什么确定。目的的崇高名称不能代替这些论证，承受者也不能只作为计算中的一个数出现。

## 蒸馏了什么

| 思想方法 | 能帮助分析什么 |
|---|---|
| 荒诞辨析 | 检查“没有终极答案”如何被推成“任何行动都无意义”。 |
| 具体代价 | 把抽象目的还原为行动、后果与承受后果的人。 |
| 艺术与现实 | 审视作品如何保留经验的复杂性，而非只为论点服务。 |

这些方法来自已定位的原作选段，不代表全集蒸馏。具体依据与适用范围见 [SKILL.md](SKILL.md) 和 [提炼说明](EXTRACTION.md)。

## 安装

本 skill 基于开放的 [Agent Skills](https://agentskills.io/) 协议，可在任何 skills-compatible 的 AI agent runtime 中运行（Claude Code、Codex、Cursor、OpenClaw、Hermes Agent、CodeBuddy、Workbuddy、Gemini CLI、OpenCode 等 50+ runtime）。

### 方式一：一行命令

```bash
npx skills add jiushiaaa/camus-skill
```

[Skills CLI](https://github.com/vercel-labs/skills) 可检测受支持的 agent；指定 runtime 时添加 `-a codex`、`-a claude-code` 或 `-a cursor`，全局安装添加 `-g`。这里说明协议与安装器的兼容生态，不代表本项目逐一实测了全部 runtime。

### 方式二：手动安装

克隆仓库后，将完整目录放入 runtime 的 skills 目录，保留 `SKILL.md` 及相对引用。安装目录命名为 `camus-perspective`，与入口元数据一致。常见路径为 Codex 的 `~/.agents/skills/`、Claude Code 的 `~/.claude/skills/`、Cursor 的 `~/.cursor/skills/`；以所用 runtime 当前文档为准。

```bash
git clone https://github.com/jiushiaaa/camus-skill.git
```

### 方式三：作为参考资料

不支持自动加载时，可把 `SKILL.md` 连同当前问题需要的引用文件交给 agent。README 与使用说明提供中英双语，研究底稿保留原语言。

## 使用方式

- **中性思想模式（默认）：** “用加缪的思想分析这个问题，区分原作观点与当代应用。”
- **人物表达模式（可选）：** 明确提出“开启人物表达模式”。这是注明性质的模拟，不是作者本人发言。

文游创作默认只取思想，文风另行决定。详见 [双语使用说明](USAGE.md)。

## 调研来源

《西西弗神话》选段；《关于死刑的思考》样章；《瑞典演说》选段。

- [原作来源、版本与实际阅读范围](references/research/source-catalog.md)
- [方法提炼与证据](EXTRACTION.md)
- 开篇名言出处：<a href="https://history.hanover.edu/courses/excerpts/111camus.html">《西西弗神话》</a>，末句。中文引文为本仓库译文；非英语原作的英文引文亦为本仓库译文。

## 仓库结构

主要文件：

```text
├── SKILL.md  # Skill 入口与分析方法
├── README.md / README.en.md  # 中英文介绍
├── USAGE.md  # 双语使用说明
├── EXTRACTION.md  # 方法提炼与证据
├── references/  # 研究笔记与可选人物表达模式
└── LICENSE  # MIT 许可
```

## 构建工具

使用 [nvwa-skill](https://github.com/alchaincyf/nuwa-skill) 构建。

项目原创材料采用 [MIT](LICENSE)，所引原著与译本保留各自权利。详见 [来源说明](ATTRIBUTION.md)。

## 更多 Skill

更多人物 Skill 请查看 [Philosophy Skills 合集](https://github.com/jiushiaaa/Philosophy-Skills)。
