<div align="center">

# Leo Lin · 林中岳

**I read old institutions as tested coordination systems — and rebuild their patterns as AI agent systems.**

把历史与制度当作被验证过的协调系统，重写成可调度、可审查、可复用的智能体。

[![GitHub](https://img.shields.io/badge/GitHub-LeoLin990405-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/LeoLin990405)
[![Blog](https://img.shields.io/badge/Blog-leolin990405.github.io-6C63FF?style=for-the-badge&logo=github&logoColor=white)](https://leolin990405.github.io/blog/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Zhongyue_Lin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/zhongyue-lin-327143207/)
[![Profile Views](https://komarev.com/ghpvc/?username=LeoLin990405&style=for-the-badge&color=6C63FF&label=PROFILE+VIEWS)](https://github.com/LeoLin990405)

</div>

---

## The idea | 核心想法

A Tang-dynasty edict passed through three departments before it became law: one drafted it, one reviewed it, one carried it out. Persian empires ran on satrapies — federated delegation kept honest by a roving royal audit. Athenian councils rotated judgment across many hands so no single one could capture it.

These are not history trivia. They are **the original multi-agent systems** — battle-tested answers to the exact problems we hit when wiring up AI: how to delegate authority, gate quality, escalate failure, distribute judgment, and keep an inspectable record.

> So I work from one question: how do we turn messy human workflows into reliable, inspectable, reusable agent systems — and what can a thousand years of institutional design teach us about it?

我做的事，就是把这套"制度智慧"翻译成代码：让模型像三省六部一样分工互审，让知识像档案制度一样留痕可查，让一个人也能指挥一支多模型的 agent 团队——能调度、能整理、能留下上下文，也能在需要时被人工审查。

---

## From institution to agent | 从制度到智能体

This table is the spine. Everything below it is the same idea, expressed in code.

| Discipline | Tested pattern | What I build with it |
|---|---|---|
| History | Tang three-department review · Persian satrapies · Athenian rotation | quality gates · federated delegation · distributed judgment |
| Political science | governance modes & institutional constraints | agent topologies · authority boundaries · escalation paths |
| Behavioral economics | fast/slow thinking · bounded rationality | model routing · evaluator design · failure-mode analysis |
| Knowledge management | notes · links · indexes · evidence trails | durable memory · research archives · retrieval-ready context |

---

## Built on the idea | 把想法落成系统

**[civagent](https://github.com/LeoLin990405/civagent) · ⭐ 38** — the thesis in its purest form: **57 historical governance systems turned into agent-orchestration patterns.** Pick a civilization, command an AI team that coordinates the way that civilization did.

**A governed skill ecosystem** — [claude-code-skills](https://github.com/LeoLin990405/claude-code-skills) is a 60+ skill monorepo, but the point is how it's *governed*. Two "mother skills" run it like a bureaucracy: `skills-master` (the strategist — classifies, merges, archives, audits) and a Grimoire forge engine that turns a PDF, repo, or vault into a draft skill. One canonical home per workflow, enforced quality gates, an archive you can roll back.

**Multi-model agent teams** — [mmteam-cc](https://github.com/LeoLin990405/mmteam-cc) and [Hivemind](https://github.com/LeoLin990405/Hivemind) make role-based delegation literal: model/provider aliases, smart routing by skill and language, inter-agent review loops, and durable context handoff between humans and models.

**The archive function** — [Knowledge-Hub](https://github.com/LeoLin990405/Knowledge-Hub) is record-keeping as infrastructure: 1300+ bilingual CS lecture notes, now public and published as a Quartz wiki with a frontmatter-validation CI guard. Notes → links → indexes → evidence trails, built to be retrieved.

**Good citizen upstream** — coordination also means contributing well inside other people's institutions. Fixes merged upstream into [steipete/CodexBar](https://github.com/steipete/CodexBar), [steipete/RepoBar](https://github.com/steipete/RepoBar), and [jackwener/OpenCLI](https://github.com/jackwener/OpenCLI).

---

## Recently | 最近

**2026-06-16** — RepoBar upstream fixes merged ([#81](https://github.com/steipete/RepoBar/pull/81), [#82](https://github.com/steipete/RepoBar/pull/82)); more OpenCLI fixes ([#1924](https://github.com/jackwener/OpenCLI/pull/1924) merged, [#1921](https://github.com/jackwener/OpenCLI/pull/1921) / [#1926](https://github.com/jackwener/OpenCLI/pull/1926) in review); new public skill `oral-interview-transcription-skill` (de-disfluency pass + adversarial fidelity gate, source data kept local); Knowledge-Hub now public as a Quartz wiki.

**2026-06-10** — three CodexBar fixes merged ([#1378](https://github.com/steipete/CodexBar/pull/1378), [#1383](https://github.com/steipete/CodexBar/pull/1383), [#1389](https://github.com/steipete/CodexBar/pull/1389)); an OpenCLI adapter wave (manus · gemini · kimi · qoder · trae-solo · antigravity · codex); chapter-level math-foundation notes; froze the `csdiy-deep-enhance` course-enhancement methodology into a reusable mother skill.

---

## Also | 此外

Applied ML and data work lives in [udacity-masters-ai-projects](https://github.com/LeoLin990405/udacity-masters-ai-projects) — a portfolio index of 12 projects across the AIPND, ML-with-PyTorch, Data Analyst, and Statistics nanodegrees. Essays connecting history, social science, and agent architecture are on the [blog](https://leolin990405.github.io/blog/).

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
- Blog: [leolin990405.github.io/blog](https://leolin990405.github.io/blog/)
- LinkedIn: [Zhongyue Lin](https://www.linkedin.com/in/zhongyue-lin-327143207/)

If one of my projects is useful, a star is always appreciated.
