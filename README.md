<div align="center">

# Leo Lin · 林中玥

[![GitHub](https://img.shields.io/badge/GitHub-LeoLin990405-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/LeoLin990405)
[![Blog](https://img.shields.io/badge/Blog-leolin990405.github.io-6C63FF?style=for-the-badge&logo=github&logoColor=white)](https://leolin990405.github.io/blog/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Zhongyue_Lin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/zhongyue-lin-327143207/)
[![Profile Views](https://komarev.com/ghpvc/?username=LeoLin990405&style=for-the-badge&color=6C63FF&label=PROFILE+VIEWS)](https://github.com/LeoLin990405)

### **English** &nbsp;·&nbsp; [中文](#chinese)

</div>

<a id="english"></a>

<div align="center">

**I read old institutions as tested coordination systems — and rebuild their patterns as AI agent systems.**

</div>

---

## The idea

A Tang-dynasty edict passed through three departments before it became law: one drafted it, one reviewed it, one carried it out. Persian empires ran on satrapies — federated delegation kept honest by a roving royal audit. Athenian councils rotated judgment across many hands so no single one could capture it.

These are not history trivia. They are **the original multi-agent systems** — battle-tested answers to the exact problems we hit when wiring up AI: how to delegate authority, gate quality, escalate failure, distribute judgment, and keep an inspectable record.

> So I work from one question: how do we turn messy human workflows into reliable, inspectable, reusable agent systems — and what can a thousand years of institutional design teach us about it?

---

## From institution to agent

This table is the spine. Everything below it is the same idea, expressed in code.

| Discipline | Tested pattern | What I build with it |
|---|---|---|
| History | Tang three-department review · Persian satrapies · Athenian rotation | quality gates · federated delegation · distributed judgment |
| Political science | governance modes & institutional constraints | agent topologies · authority boundaries · escalation paths |
| Behavioral economics | fast/slow thinking · bounded rationality | model routing · evaluator design · failure-mode analysis |
| Knowledge management | notes · links · indexes · evidence trails | durable memory · research archives · retrieval-ready context |

---

## Built on the idea

**[civagent](https://github.com/LeoLin990405/civagent) · ⭐ 38** — the thesis in its purest form: **57 historical governance systems turned into agent-orchestration patterns.** Pick a civilization, command an AI team that coordinates the way that civilization did.

**A governed skill ecosystem** — [claude-code-skills](https://github.com/LeoLin990405/claude-code-skills) is a 60+ skill monorepo, but the point is how it's *governed*. Two "mother skills" run it like a bureaucracy: `skills-master` (the strategist — classifies, merges, archives, audits) and a Grimoire forge engine that turns a PDF, repo, or vault into a draft skill. One canonical home per workflow, enforced quality gates, an archive you can roll back.

**Multi-model agent teams** — [mmteam-cc](https://github.com/LeoLin990405/mmteam-cc) and [Hivemind](https://github.com/LeoLin990405/Hivemind) make role-based delegation literal: model/provider aliases, smart routing by skill and language, inter-agent review loops, and durable context handoff between humans and models.

**The archive function** — [Knowledge-Hub](https://github.com/LeoLin990405/Knowledge-Hub) is record-keeping as infrastructure: 1300+ bilingual CS lecture notes, now public and published as a Quartz wiki with a frontmatter-validation CI guard. Notes → links → indexes → evidence trails, built to be retrieved.

**Good citizen upstream** — coordination also means contributing well inside other people's institutions. Fixes merged upstream into [steipete/CodexBar](https://github.com/steipete/CodexBar), [steipete/RepoBar](https://github.com/steipete/RepoBar), and [jackwener/OpenCLI](https://github.com/jackwener/OpenCLI).

---

## A product, too

**BicaMind** — a voice-first AI companion in an open ear-clip earphone, built around one promise: *you know everything*. It's where the same obsession — knowledge, on demand, made trustworthy — leaves the terminal and becomes something you actually wear.

---

## Recently

**2026-06-16** — RepoBar upstream fixes merged ([#81](https://github.com/steipete/RepoBar/pull/81), [#82](https://github.com/steipete/RepoBar/pull/82)); more OpenCLI fixes ([#1924](https://github.com/jackwener/OpenCLI/pull/1924) merged, [#1921](https://github.com/jackwener/OpenCLI/pull/1921) / [#1926](https://github.com/jackwener/OpenCLI/pull/1926) in review); new public skill `oral-interview-transcription-skill`; Knowledge-Hub now public as a Quartz wiki.

**2026-06-10** — three CodexBar fixes merged ([#1378](https://github.com/steipete/CodexBar/pull/1378), [#1383](https://github.com/steipete/CodexBar/pull/1383), [#1389](https://github.com/steipete/CodexBar/pull/1389)); an OpenCLI adapter wave (manus · kimi · qoder · trae-solo · antigravity · codex); chapter-level math-foundation notes; froze the `csdiy-deep-enhance` course-enhancement methodology into a reusable mother skill.

---

## Also

Applied ML and data work lives in [udacity-masters-ai-projects](https://github.com/LeoLin990405/udacity-masters-ai-projects) — a portfolio index of 12 projects across the AIPND, ML-with-PyTorch, Data Analyst, and Statistics nanodegrees. Essays connecting history, social science, and agent architecture are on the [blog](https://leolin990405.github.io/blog/).

<br>

<div align="center">

[↑ back to top](#english) &nbsp;·&nbsp; [切换到中文 →](#chinese)

</div>

---
---

<a id="chinese"></a>

<div align="center">

# 林中玥 · Leo Lin

### [English](#english) &nbsp;·&nbsp; **中文**

**把历史与制度当作被验证过的协调系统，重写成可调度、可审查、可复用的智能体。**

</div>

---

## 核心想法

一道唐代政令要经三省才成法：中书拟、门下审、尚书行。波斯帝国靠总督制运转——联邦式授权，再用巡回的「王之耳目」审计制衡。雅典议事会让判断在众人手中轮转，没有任何一只手能独揽。

这些不是历史冷知识。它们是**最早的多智能体系统**——对我们接 AI 时遇到的同一批问题，给出过被实战验证的答案：如何授权、如何把质量关、如何升级失败、如何分散判断、如何留下可审查的记录。

> 所以我做的事，就是把这套「制度智慧」翻译成代码：让模型像三省六部一样分工互审，让知识像档案制度一样留痕可查，让一个人也能指挥一支多模型的 agent 团队——能调度、能整理、能留下上下文，也能在需要时被人工审查。

---

## 从制度到智能体

这张表就是骨架，下面的一切都是同一个想法的代码化表达。

| 学科 | 被验证的模式 | 我用它造什么 |
|---|---|---|
| 历史 | 唐三省审核 · 波斯总督制 · 雅典轮值 | 质量门 · 联邦式授权 · 分散判断 |
| 政治学 | 治理模式与制度约束 | 智能体拓扑 · 权限边界 · 升级路径 |
| 行为经济学 | 快慢思考 · 有限理性 | 模型路由 · 评估器设计 · 失败模式分析 |
| 知识管理 | 笔记 · 链接 · 索引 · 证据链 | 持久记忆 · 研究档案 · 可检索上下文 |

---

## 把想法落成系统

**[civagent](https://github.com/LeoLin990405/civagent) · ⭐ 38** — 主线最纯粹的化身：**把 57 套历史治理制度变成 agent 编排模式**。选一个文明，指挥一支按那个文明方式协作的 AI 团队。

**一套受治理的技能生态** — [claude-code-skills](https://github.com/LeoLin990405/claude-code-skills) 是 60+ 技能的 monorepo，但重点在于它如何被「治理」。两个 mother skill 像官僚机构一样运转：`skills-master`（战略官——分类、合并、归档、审计）和把 PDF／仓库／知识库炼成草稿技能的 Grimoire 锻造引擎。每条工作流只有一个正本归宿、强制质量门、可回滚的归档。

**多模型 agent 团队** — [mmteam-cc](https://github.com/LeoLin990405/mmteam-cc) 和 [Hivemind](https://github.com/LeoLin990405/Hivemind) 把「按角色授权」做成实物：模型／供应商别名、按技能与语言智能路由、智能体之间的互审回路，以及人与模型之间的持久上下文交接。

**档案职能** — [Knowledge-Hub](https://github.com/LeoLin990405/Knowledge-Hub) 把「留痕」做成基础设施：1300+ 篇中英双语 CS 课程笔记，现已公开并发布为 Quartz wiki，配有 frontmatter 校验的 CI 护栏。笔记 → 链接 → 索引 → 证据链，为「可被检索」而建。

**做好上游的公民** — 协调也意味着在别人的「制度」里好好贡献。已向 [steipete/CodexBar](https://github.com/steipete/CodexBar)、[steipete/RepoBar](https://github.com/steipete/RepoBar)、[jackwener/OpenCLI](https://github.com/jackwener/OpenCLI) 合并多个上游修复。

---

## 也在做一款产品

**BicaMind** — 一款声音优先的 AI 伴侣，做成开放式耳夹耳机，围绕一句承诺：*you know everything*。它是同一种执念——让知识随取随用、且值得信赖——走出终端，变成一件真正戴在身上的产品。

---

## 最近

**2026-06-16** — RepoBar 上游修复合并（[#81](https://github.com/steipete/RepoBar/pull/81)、[#82](https://github.com/steipete/RepoBar/pull/82)）；更多 OpenCLI 修复（[#1924](https://github.com/jackwener/OpenCLI/pull/1924) 已合并，[#1921](https://github.com/jackwener/OpenCLI/pull/1921) / [#1926](https://github.com/jackwener/OpenCLI/pull/1926) 审查中）；新增公开技能 `oral-interview-transcription-skill`；Knowledge-Hub 转公开并上线 Quartz wiki。

**2026-06-10** — 三个 CodexBar 修复合并（[#1378](https://github.com/steipete/CodexBar/pull/1378)、[#1383](https://github.com/steipete/CodexBar/pull/1383)、[#1389](https://github.com/steipete/CodexBar/pull/1389)）；一波 OpenCLI 适配器（manus · kimi · qoder · trae-solo · antigravity · codex）；章节级数学基础笔记；把 `csdiy-deep-enhance` 课程增强方法论固化成可复用的 mother skill。

---

## 此外

应用 ML 与数据相关的作品收在 [udacity-masters-ai-projects](https://github.com/LeoLin990405/udacity-masters-ai-projects)——横跨 AIPND、ML-with-PyTorch、数据分析、统计四个 nanodegree 的 12 个项目索引。把历史、社会科学与 agent 架构连起来的随笔，在[博客](https://leolin990405.github.io/blog/)。

<div align="center">

[English ↑](#english) &nbsp;·&nbsp; [回到顶部](#chinese)

</div>

---

## Stack | 技术栈

<div align="center">

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![R](https://img.shields.io/badge/R-276DC3?style=for-the-badge&logo=r&logoColor=white)
![Swift](https://img.shields.io/badge/Swift-F05138?style=for-the-badge&logo=swift&logoColor=white)
![Shell](https://img.shields.io/badge/Shell-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white)

![Claude](https://img.shields.io/badge/Claude-191919?style=for-the-badge&logo=anthropic&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI_API-412991?style=for-the-badge&logo=openai&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-6C63FF?style=for-the-badge&logoColor=white)
![Obsidian](https://img.shields.io/badge/Obsidian-7C3AED?style=for-the-badge&logo=obsidian&logoColor=white)

</div>

---

## Stats | 数据统计

<div align="center">

<img width="49%" src="https://github-readme-stats.vercel.app/api?username=LeoLin990405&show_icons=true&theme=tokyonight&hide_border=true&count_private=true&include_all_commits=true&bg_color=0d1117&ring_color=6C63FF&icon_color=6C63FF" />
<img width="49%" src="https://github-readme-stats.vercel.app/api/top-langs/?username=LeoLin990405&layout=compact&theme=tokyonight&hide_border=true&langs_count=8&bg_color=0d1117" />

</div>

---

## Contact | 联系

- GitHub: [@LeoLin990405](https://github.com/LeoLin990405)
- Blog · 博客: [leolin990405.github.io/blog](https://leolin990405.github.io/blog/)
- LinkedIn: [Zhongyue Lin](https://www.linkedin.com/in/zhongyue-lin-327143207/)

If one of my projects is useful, a star is always appreciated. · 如果哪个项目帮到了你，欢迎点个 star。
