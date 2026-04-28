<div align="center">

# 🧰 Khazix Skills

### 数字生命卡兹克的 AI 工具箱

*"把任何重复 3 遍的事 AI 化或自动化。"*

[![License](https://img.shields.io/badge/License-MIT-3B82F6?style=for-the-badge)](./LICENSE)
[![Skills](https://img.shields.io/badge/Skills-3-10B981?style=for-the-badge)](#-skills)
[![Prompts](https://img.shields.io/badge/Prompts-1-F59E0B?style=for-the-badge)](#-prompts)
[![AgentSkills](https://img.shields.io/badge/AgentSkills-Standard-8B5CF6?style=for-the-badge)](https://agentskills.io)

![Claude Code](https://img.shields.io/badge/Claude_Code-Skill-D97706?style=flat-square&logo=anthropic&logoColor=white)
![Codex](https://img.shields.io/badge/Codex-Skill-10B981?style=flat-square&logo=openai&logoColor=white)
![OpenCode](https://img.shields.io/badge/OpenCode-Skill-3B82F6?style=flat-square)
![OpenClaw](https://img.shields.io/badge/OpenClaw-Skill-8B5CF6?style=flat-square)

---

**这里是我自己每天在用的、迭代了几十轮的 Prompts 和 Skills，全部一字不改地开源出来。**

两种东西，一个目的：把我积累的方法论变成可复用的工具。

</div>

> **Prompts** — 轻量级，复制粘贴到任何 AI 对话或 Deep Research 里就能用
> **Skills** — 重量级，遵循 [Agent Skills](https://agentskills.io) 开放标准的结构化指令集，安装后 Agent 会自动加载

---

## 📦 安装方式

<details>
<summary><b>方式 1 · 通过 Agent 自然语言安装</b>（推荐）</summary>

在 Claude Code、Codex、OpenClaw 等支持 Skill 的 Agent 中，直接对话：

```
安装这个 skill：https://github.com/KKKKhazix/khazix-skills
```

</details>

<details>
<summary><b>方式 2 · 手动 git clone</b></summary>

```bash
git clone https://github.com/KKKKhazix/khazix-skills.git
cp -r khazix-skills/<skill-name> <你的 skills 目录>/
```

各工具的 skills 目录：

| 工具 | 路径 |
|---|---|
| Claude Code | `~/.claude/skills/` |
| Codex | `~/.codex/skills/` |
| OpenClaw | `~/.openclaw/skills/` |
| OpenCode | `.opencode/skills/`（项目级）/ `~/.config/opencode/skills/`（全局） |

例如装 neat-freak 到 Claude Code：

```bash
git clone https://github.com/KKKKhazix/khazix-skills.git
cp -r khazix-skills/neat-freak ~/.claude/skills/
```

</details>

<details>
<summary><b>方式 3 · 通过包管理器</b></summary>

```bash
# ClawHub
clawhub install neat-freak

# Tessl
tessl install khazix-skills/neat-freak
```

</details>

---

## ✨ Skills

<a id="-skills"></a>

<table>
<tr><td>

### 🧹 neat-freak（洁癖）

> *"如果不跑一遍 /neat，我就浑身难受，如坐针毡如芒刺背如鲠在喉。"*

会话结束时自动审查项目的**文档体系**、**根 CLAUDE.md / AGENTS.md**、**Agent 记忆系统**，把疏于维护的知识体系拉回到跟代码对齐的干净状态。最后给一份变更摘要。

**🩹 它解决的痛点**

- 文档脑腐：代码迭代了 7 轮，README 还停留在 1.0.0
- 记忆冲突：上一个会话定的事，下一个会话被推翻
- 跨项目漂移：上游 API 改了，下游集成文档没跟上
- 三层割裂：项目根 markdown、外部 docs、Agent 记忆，三份受众不同却经常顾此失彼

**⚡ 触发方式**

```
/neat            # 直接命令
整理一下          # 自然语言
同步一下          # 自然语言
sync up          # English
```

**🌐 跨平台**：Claude Code · Codex · OpenCode · OpenClaw

[![ClawHub](https://img.shields.io/badge/ClawHub-v1.0.1-EC4899?style=flat-square)](https://clawhub.ai)
[![Tessl](https://img.shields.io/badge/Tessl-0.1.1-3B82F6?style=flat-square)](https://tessl.io/registry/khazix-skills/neat-freak)

→ [SKILL.md](./neat-freak/SKILL.md) · 公众号讲解：*待发布*

</td></tr>
</table>

<table>
<tr><td>

### 🔭 hv-analysis（横纵分析法）

> *"纵向追时间深度，横向追同期广度，最终交汇出判断。"*

由卡兹克提出的通用深度研究方法论，融合了索绪尔的**历时-共时分析**、社会科学的**纵向-横截面研究设计**、商学院案例研究法、竞争战略分析。

自动联网收集信息、并行多 Agent 分头取证、最终输出一份**排版精美的 PDF 研究报告**（10,000–30,000 字）。

**🎯 适用对象**

- 产品 / 公司 / 概念 / 技术 / 人物的系统性深度研究
- 不适合纯名词解释 — 那种问题用普通对话即可

**🧠 双轴方法**

```
            ↑ 时间深度
            │
   纵轴 ────┼─────────  横轴
（叙事故事）│  当下截面
            │（竞品对比）
            ↓
       横纵交汇 → 独到洞察
```

**📄 产出**：自动生成封面 / 目录 / 多级标题彩色的 PDF，支持中英文混排

[![ClawHub](https://img.shields.io/badge/ClawHub-v1.0.0-EC4899?style=flat-square)](https://clawhub.ai)
[![Tessl](https://img.shields.io/badge/Tessl-published-3B82F6?style=flat-square)](https://tessl.io/registry/khazix-skills/hv-analysis)

→ [SKILL.md](./hv-analysis/SKILL.md) · [公众号讲解](https://mp.weixin.qq.com/s/Y_uRMYBmdLWUPnz_ac7jWA)

</td></tr>
</table>

<table>
<tr><td>

### ✍️ khazix-writer（卡兹克写作）

> *"有见识的普通人在认真聊一件打动他的事。"*

我自己公众号「数字生命卡兹克」的**长文写作 Skill**，把我三年内容创作的所有判断浓缩成结构化指令——内置完整的写作风格规则、四层自检体系、内容方法论和风格示例库。

装上之后，Agent 可以**用我的风格**写公众号长文。

**🎨 风格内核**

- 节奏感：句段长短交错，一句话自成一段制造重量
- 叙事驱动：不是参数罗列，是故事弧线
- 知识聊着聊着自然掏出，不"科普"不"赋能"
- 敢下判断、有事实支撑、明确"我觉得"
- 层层剥开：现象 → 表面 → 追问 → 洞察

**🚫 绝对禁区**

「首先...其次」「综上所述」「赋能 / 抓手 / 闭环」「在当今 AI 快速发展的时代」「说白了 / 本质上 / 换句话说」——这些 AI 味标记一律挡下。

[![ClawHub](https://img.shields.io/badge/ClawHub-v1.0.0-EC4899?style=flat-square)](https://clawhub.ai)
[![Tessl](https://img.shields.io/badge/Tessl-0.1.1-3B82F6?style=flat-square)](https://tessl.io/registry/khazix-skills/khazix-writer)

→ [SKILL.md](./khazix-writer/SKILL.md) · [公众号讲解](https://mp.weixin.qq.com/s/AtxGrii_K-nzkwUM9SNhEg)

</td></tr>
</table>

---

## 📝 Prompts

<a id="-prompts"></a>

<table>
<tr><td>

### 🔭 横纵分析法（Prompt 版）

hv-analysis Skill 的轻量化版本——**一段 prompt 复制粘贴到任何支持 Deep Research 的模型里就能用**（ChatGPT Deep Research、Gemini Deep Research、Grok Deep Search、Claude Research 都行），不需要安装任何东西。

半小时出一份万字级研究报告。

→ [横纵分析法.md](./prompts/横纵分析法.md) · [公众号讲解](https://mp.weixin.qq.com/s/Y_uRMYBmdLWUPnz_ac7jWA)

</td></tr>
</table>

---

## 🌟 关于卡兹克

数字生命卡兹克 · 虚实传媒（Virxact）创始人。视觉传达设计出身，做过用户研究和交互设计，**不是程序员**——做的事情是把 AI 翻译成普通人能理解、能用的东西。

公众号「数字生命卡兹克」，使命是「**激发大家对 AI 的好奇**」。

如果这些 skill 帮到你，欢迎给个 ⭐ Star，也欢迎在 Issues 或 Discussions 里聊。

---

<div align="center">

**License** · [MIT](./LICENSE) · 自由使用 / 修改 / 再分发

Made with ❤️ by [@KKKKhazix](https://github.com/KKKKhazix)

</div>
