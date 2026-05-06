<div align="center">

# Leo Lin | 林中岳

**Interdisciplinary AI builder working across agent systems, knowledge workflows, and applied ML portfolios.**

[![GitHub](https://img.shields.io/badge/GitHub-LeoLin990405-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/LeoLin990405)
[![Blog](https://img.shields.io/badge/Blog-leolin990405.github.io-6C63FF?style=for-the-badge&logo=github&logoColor=white)](https://leolin990405.github.io/blog/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Zhongyue_Lin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/zhongyue-lin-327143207/)
[![Profile Views](https://komarev.com/ghpvc/?username=LeoLin990405&style=for-the-badge&color=6C63FF&label=PROFILE+VIEWS)](https://github.com/LeoLin990405)

</div>

---

## Current Focus | 当前主线

```yaml
name: "Zhongyue Lin (Leo) | 林中岳"
location: "China"
working_on:
  - "Codex / Claude Code skill ecosystems"
  - "Multi-model agent teams and AI workflow infrastructure"
  - "Knowledge Hub: Obsidian-based course notes, research notes, and WeChat archives"
  - "Applied ML and data-analysis portfolio projects"
research_bridge:
  - "History and institutional design -> multi-agent orchestration"
  - "Behavioral economics -> agent routing and evaluation"
  - "Knowledge management -> durable AI memory workflows"
languages: ["中文", "English"]
```

I build practical AI tooling around a simple question:

> How do we turn messy human workflows into reliable, inspectable, reusable agent systems?

我关注的是把真实工作流沉淀成可复用的智能体系统：能调度模型、能整理知识、能留下上下文，也能在需要时被人工审查。

---

## Maintained Project Map | 维护中的项目地图

| Area | Canonical Repository | Status | Notes |
|---|---|---:|---|
| Skills ecosystem | [claude-code-skills](https://github.com/LeoLin990405/claude-code-skills) | Active | Canonical public monorepo for installable Codex / Claude Code skills. `67` canonical installable units, `89` default install units. |
| Document parsing skill | [mineru-skill](https://github.com/LeoLin990405/mineru-skill) | Active | Standalone MinerU API skill with CLI helper, examples, and release surface. |
| R analytics skill | [r-analytics-skill](https://github.com/LeoLin990405/r-analytics-skill) | Active | R analytics pack with package-level data, stats, ML, spatial, NLP, and visualization workflows. |
| WeChat archive skill | `wechat-public-account-archive-skill` | Private active | Archives WeChat public account articles into Knowledge Hub while keeping auth material out of notes. |
| YouTube clipping skill | `youtube-clipper-skill` | Private active | Codex-ready video clipping workflow: download, semantic chaptering, bilingual subtitles, and summaries. |
| Knowledge base | [Knowledge-Hub](https://github.com/LeoLin990405/Knowledge-Hub) | Active | Obsidian-based CS self-study vault and long-term knowledge system. |
| Applied ML portfolio | [udacity-masters-ai-projects](https://github.com/LeoLin990405/udacity-masters-ai-projects) | Active index | Portfolio entry point for Udacity AI / ML / data analysis projects. |
| Landmark classifier | [landmark-classifier](https://github.com/LeoLin990405/landmark-classifier) | Completed | M5 retraining artifacts merged; transfer model passes rubric and scratch CNN now has a stronger trained baseline. |
| Multi-agent research | [civagent](https://github.com/LeoLin990405/civagent) | Active / public | Historical governance systems as agent orchestration patterns. |
| macOS usage monitor | [CodexBar](https://github.com/LeoLin990405/CodexBar) | Fork / contribution | Usage stats for Codex and Claude Code, plus provider experiments. |

---

## Skills Ecosystem | 技能生态

The skill ecosystem is being consolidated around one public canonical repository:

### [claude-code-skills](https://github.com/LeoLin990405/claude-code-skills)

```text
productivity        Obsidian, NotebookLM, Google Workspace, Knowledge Hub
development         MCP, frontend, repo design, D3, R analytics, SQL workflows
documents           PDF, DOCX, PPTX, XLSX, MinerU, document coauthoring
research            scientific skills, STEM modeling, history notes, macro research
ai-collaboration    multi-provider orchestration, agent teams, skill discovery
product-management  Lenny-inspired PM frameworks and playbooks
design              themes, CLI demos, visual assets
system              proxy, CDP, SVN, internal comms, OSS contribution
```

Recent consolidation work:

- Category toolkit routers now install correctly.
- Legacy wrappers such as `all-plan`, provider-specific shims, and `pm-*` aliases are separated from the canonical install surface.
- External nested submodule packs are documented without being flattened into the default install path.
- Older source repos are being treated as migration sources or standalone release surfaces, not as parallel canonical homes.

Standalone skills kept separate because they still have independent value:

| Repo | Why It Stays Separate |
|---|---|
| [mineru-skill](https://github.com/LeoLin990405/mineru-skill) | Has CLI helpers, examples, changelog, and an independent document parsing workflow. |
| [r-analytics-skill](https://github.com/LeoLin990405/r-analytics-skill) | Large package-level R workflow surface, useful as its own canonical pack. |
| `wechat-public-account-archive-skill` | Private local workflow with auth-sensitive operational scripts. |
| `youtube-clipper-skill` | Private media workflow with local configuration and output paths. |

---

## Agent Systems | 智能体系统

### Multi-model collaboration

I work on patterns for routing tasks across multiple model families and agent roles:

- role-based agent teams
- model/provider aliases
- smart task routing by skill, language, and intent
- inter-agent messaging and review loops
- durable context handoff between humans and models

Related repositories:

| Repository | Role |
|---|---|
| [mmteam-cc](https://github.com/LeoLin990405/mmteam-cc) | Multi-model agent team experiments for Claude Code-style workflows. |
| [civagent](https://github.com/LeoLin990405/civagent) | Governance systems as agent orchestration patterns. |
| [xiaotie](https://github.com/LeoLin990405/xiaotie) | Lightweight AI agent framework experiments. |
| [Hivemind](https://github.com/LeoLin990405/Hivemind) | Multi-AI routing and desktop collaboration prototype. |
| [blog](https://github.com/LeoLin990405/blog) | Essays connecting history, social science, and agent architecture. |

---

## Research Bridge | 跨学科研究

My favorite ideas come from treating old institutions as tested coordination systems.

| Discipline | Source Pattern | AI / Agent Application |
|---|---|---|
| History | Tang three-department review, Persian satrapies, Athenian councils | quality gates, federated delegation, distributed judgment |
| Political science | governance modes and institutional constraints | agent topologies, authority boundaries, escalation paths |
| Behavioral economics | fast/slow thinking, bounded rationality | model routing, evaluator design, failure-mode analysis |
| Knowledge management | notes, links, indexes, evidence trails | durable memory, research archives, retrieval-ready context |

Blog entry point: [leolin990405.github.io/blog](https://leolin990405.github.io/blog/)

---

## Applied ML Portfolio | 应用机器学习作品集

Main index: [udacity-masters-ai-projects](https://github.com/LeoLin990405/udacity-masters-ai-projects)

Selected projects:

| Project | Focus |
|---|---|
| [landmark-classifier](https://github.com/LeoLin990405/landmark-classifier) | PyTorch landmark classification, MPS retraining, transfer learning, full submission artifacts. |
| [teaching-llm-to-count](https://github.com/LeoLin990405/teaching-llm-to-count) | GRPO + LoRA experiments for teaching an LLM to count. |
| [agentsville-trip-planner](https://github.com/LeoLin990405/agentsville-trip-planner) | Agentic AI trip planning with ReACT-style workflows. |
| [face-generation](https://github.com/LeoLin990405/face-generation) | DCGAN face generation project. |
| [text-translation-sentiment](https://github.com/LeoLin990405/text-translation-sentiment) | Translation + sentiment pipeline using Hugging Face tooling. |
| [sentimentscope-imdb](https://github.com/LeoLin990405/sentimentscope-imdb) | Transformer-based IMDB sentiment analysis. |

Older course repositories remain useful as project records, while the portfolio index is the preferred entry point.

---

## Repo Governance | 仓库治理

I am gradually reducing repo sprawl:

| Keep Maintaining | Consolidate / Redirect | Archive When Safe |
|---|---|---|
| `claude-code-skills` | `claude-lenny-skills` -> product-management packs | old migrated skill source repos |
| `mineru-skill` | `claude-office-skills` -> documents packs | thin wrappers with no independent release surface |
| `r-analytics-skill` | `claude-design-skills` -> design packs | stale forks without active PRs |
| `Knowledge-Hub` | `claude-obsidian-skills` -> productivity packs | one-off course repos after portfolio indexing |
| `civagent` | `github-repo-design-skill` -> development pack | duplicate awesome lists after blog/Knowledge Hub import |

Principles:

- one canonical home per workflow
- no secrets or auth material in public repos
- private repos for operational scripts with local credentials
- public repos for reusable frameworks, skills, and portfolio artifacts
- README files should tell users where the maintained surface now lives

---

## Tech Stack | 技术栈

<div align="center">

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![R](https://img.shields.io/badge/R-276DC3?style=for-the-badge&logo=r&logoColor=white)
![Swift](https://img.shields.io/badge/Swift-F05138?style=for-the-badge&logo=swift&logoColor=white)
![Shell](https://img.shields.io/badge/Shell-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white)

![OpenAI](https://img.shields.io/badge/OpenAI_API-412991?style=for-the-badge&logo=openai&logoColor=white)
![Claude](https://img.shields.io/badge/Claude-191919?style=for-the-badge&logo=anthropic&logoColor=white)
![Gemini](https://img.shields.io/badge/Gemini-8E75B2?style=for-the-badge&logo=googlegemini&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-6C63FF?style=for-the-badge&logoColor=white)
![Obsidian](https://img.shields.io/badge/Obsidian-7C3AED?style=for-the-badge&logo=obsidian&logoColor=white)

</div>

---

## GitHub Stats | 数据统计

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
