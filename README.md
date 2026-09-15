<div align="center">

# Leo Lin · 林中玥

[![GitHub](https://img.shields.io/badge/GitHub-LeoLin990405-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/LeoLin990405)
[![Blog](https://img.shields.io/badge/Blog-leolin990405.github.io-6C63FF?style=for-the-badge&logo=github&logoColor=white)](https://leolin990405.github.io/blog/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Zhongyue_Lin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/zhongyue-lin-327143207/)
[![Profile Views](https://komarev.com/ghpvc/?username=LeoLin990405&style=for-the-badge&color=6C63FF&label=PROFILE+VIEWS)](https://github.com/LeoLin990405)

### **English** &nbsp;·&nbsp; [中文](#chinese)

**I read old institutions as tested coordination systems — and rebuild them as AI agent systems that are routable, reviewable, and honest about what they know.**

</div>

<a id="english"></a>

---

## The idea

A Tang-dynasty edict passed through three departments before it became law: one drafted, one reviewed, one executed. Persian satrapies ran on federated delegation kept honest by a roving audit. Athenian councils rotated judgment so no single hand could capture it.

These are **the original multi-agent systems** — battle-tested answers to the problems we hit when wiring up AI: delegating authority, gating quality, escalating failure, distributing judgment, and keeping an inspectable record.

| Discipline | Tested pattern | What I build with it |
|---|---|---|
| History | Tang three-department review · Persian satrapies · Athenian rotation | quality gates · federated delegation · distributed judgment |
| Political science | governance modes & institutional constraints | agent topologies · authority boundaries · escalation paths |
| Behavioral economics | fast/slow thinking · bounded rationality | model routing · evaluator design · failure-mode analysis |
| Knowledge management | notes · links · indexes · evidence trails | durable memory · research archives · retrieval-ready context |

---

## Building now

| Project | What it is |
|---|---|
| **[agos](https://github.com/LeoLin990405/agos)** | An honesty-first Agent OS deck: telemetry, shadow model routing, memory workbench, homelab fleet. The rule is enforced by tests — *the screen never says anything the data cannot prove.* Humans keep authority; models propose. |
| **[civagent](https://github.com/LeoLin990405/civagent)** · ⭐ 40 | The thesis in its purest form: **57 historical governance systems compiled into multi-agent orchestration patterns**. v6 adds a constitutional engine (`VETO` / `IMPEACH` / `EDICT`), regime-as-graph typing, and a tournament pipeline (Bradley–Terry ranking + bootstrap CI, ablations) to test whether institutions actually change outcomes. |
| **[FuguNano](https://github.com/BicaMindLabs/FuguNano)** · ⭐ 27 | An open, training-free reimplementation of Sakana Fugu: a control plane that makes the agents you already have run as one auditable loop — plan, dispatch, review, repair, learn — with a verifier-aware selector and a desktop Studio. |

## Tools I keep sharp

- **[grimoire-skill](https://github.com/LeoLin990405/grimoire-skill)** · ⭐ 8 — parse a PDF once, forge two artifacts: typed reading notes for Obsidian and a reusable skill pack.
- **[oral-interview-transcription-skill](https://github.com/LeoLin990405/oral-interview-transcription-skill)** · ⭐ 13 — oral-history recordings → faithful edited transcripts, with an adversarial fidelity gate; data stays local.
- **[skill-librarian](https://github.com/LeoLin990405/skill-librarian)** — lint and index a large local `SKILL.md` library: duplicates, dead links, name collisions, weak descriptions.
- **[paper-reading-workflow-zh](https://github.com/LeoLin990405/paper-reading-workflow-zh)** — evidence-grounded Chinese paper-reading workflow (PDF → MinerU → Obsidian).
- **[cn-cc](https://github.com/LeoLin990405/cn-cc)** · **[mmteam-cc](https://github.com/LeoLin990405/mmteam-cc)** — route Claude Code work to Chinese model backends; multi-model agent teams with fan-out consensus.
- **[ScreenBar](https://github.com/LeoLin990405/ScreenBar)** — a SwiftUI menu-bar app that turns Macs on your tailnet into second screens.

## Upstream

Coordination also means contributing well inside other people's institutions. Merged since mid-June 2026:

| Repository | ⭐ | Merged | Highlights |
|---|---|---|---|
| [steipete/CodexBar](https://github.com/steipete/CodexBar) | 21.4k | 11 | LongCat provider ([#1697](https://github.com/steipete/CodexBar/pull/1697)) · Doubao Agent Plan usage ([#2496](https://github.com/steipete/CodexBar/pull/2496)) · Safe Storage ACL reuse ([#2528](https://github.com/steipete/CodexBar/pull/2528)) · live rollouts no longer starve cost updates ([#3314](https://github.com/steipete/CodexBar/pull/3314)) |
| [jackwener/OpenCLI](https://github.com/jackwener/OpenCLI) | 29.3k | 8 | Xiaohongshu risk-control cooldown retry ([#2207](https://github.com/jackwener/OpenCLI/pull/2207)) · X profile recovery ([#2193](https://github.com/jackwener/OpenCLI/pull/2193)) · Eastmoney column fix ([#2131](https://github.com/jackwener/OpenCLI/pull/2131)) |
| [Hmbown/Codewhale](https://github.com/Hmbown/Codewhale) | 41.0k | 4 | session persists before stall recovery ([#3285](https://github.com/Hmbown/Codewhale/pull/3285)) · proxy-aware `fetch` ([#3577](https://github.com/Hmbown/Codewhale/pull/3577)) |
| [steipete/oracle](https://github.com/steipete/oracle) | 4.0k | 4 | completion proof for short captures ([#293](https://github.com/steipete/oracle/pull/293)) · hidden-window prompt submission ([#302](https://github.com/steipete/oracle/pull/302)) |
| [blueberrycongee/wuu](https://github.com/blueberrycongee/wuu) | 48 | 4 | background-command ownership ([#195](https://github.com/blueberrycongee/wuu/pull/195)) · stable tool prefix ([#194](https://github.com/blueberrycongee/wuu/pull/194)) |
| [BigPizzaV3/CodexPlusPlus](https://github.com/BigPizzaV3/CodexPlusPlus) | 30.9k | 2 | versioned base URL kept ([#1363](https://github.com/BigPizzaV3/CodexPlusPlus/pull/1363)) · graceful inject fallback ([#1360](https://github.com/BigPizzaV3/CodexPlusPlus/pull/1360)) |
| [hoangsonww/Claude-Code-Agent-Monitor](https://github.com/hoangsonww/Claude-Code-Agent-Monitor) | 998 | 1 | non-negative subagent durations ([#171](https://github.com/hoangsonww/Claude-Code-Agent-Monitor/pull/171)) |

## Recently

- **2026-09** — **agos** goes public: execution hardening, approvals and fleet state ([#1](https://github.com/LeoLin990405/agos/pull/1)), acceptance tree and honest session/chat/console slices ([#2](https://github.com/LeoLin990405/agos/pull/2)); CodexBar cost-update and titlebar fixes ([#3314](https://github.com/steipete/CodexBar/pull/3314), [#3315](https://github.com/steipete/CodexBar/pull/3315)); oral-interview skill adds a Word-style review pack and podcast genre ([#1](https://github.com/LeoLin990405/oral-interview-transcription-skill/pull/1)).
- **2026-08** — civagent R6–R14: regime editing API + online editor, an experimental-validity layer, runtime-graph diffs, CI with teeth ([#31](https://github.com/LeoLin990405/civagent/pull/31)–[#34](https://github.com/LeoLin990405/civagent/pull/34)); CodexBar Alibaba Personal plan support ([#3098](https://github.com/steipete/CodexBar/pull/3098), [#3128](https://github.com/steipete/CodexBar/pull/3128)) and z.ai 7/30-day ranges ([#2524](https://github.com/steipete/CodexBar/pull/2524)); OpenCLI Xiaohongshu cooldown ([#2207](https://github.com/jackwener/OpenCLI/pull/2207)).
- **2026-07** — civagent v6 hardening line: constitutional engine, Express API, tournament statistics, ablation generator, hill-climbing loop ([#17](https://github.com/LeoLin990405/civagent/pull/17)–[#30](https://github.com/LeoLin990405/civagent/pull/30)); FuguNano selector router, SWE-bench driver, and FuguNano Studio desktop GUI ([#6](https://github.com/BicaMindLabs/FuguNano/pull/6)–[#16](https://github.com/BicaMindLabs/FuguNano/pull/16)); four oracle browser fixes, four wuu PRs, CodexPlusPlus fixes; shipped skill-librarian and paper-reading-workflow-zh.
- **2026-06** — cn-cc `/cn:team` multi-model fan-out ([#5](https://github.com/LeoLin990405/cn-cc/pull/5)); Codewhale TUI fixes ([#3284](https://github.com/Hmbown/Codewhale/pull/3284), [#3285](https://github.com/Hmbown/Codewhale/pull/3285)); OpenCLI Gemini/SMZDM fixes ([#1967](https://github.com/jackwener/OpenCLI/pull/1967), [#1968](https://github.com/jackwener/OpenCLI/pull/1968)); ScreenBar released.

## Also

**BicaMind** — a voice-first AI companion in an open ear-clip earphone: the same obsession with trustworthy, on-demand knowledge, leaving the terminal. Applied ML work lives in [udacity-masters-ai-projects](https://github.com/LeoLin990405/udacity-masters-ai-projects); essays connecting history, social science and agent architecture are on the [blog](https://leolin990405.github.io/blog/).

<div align="center">

[↑ back to top](#english) &nbsp;·&nbsp; [切换到中文 →](#chinese)

</div>

---
---

<a id="chinese"></a>

<div align="center">

# 林中玥 · Leo Lin

### [English](#english) &nbsp;·&nbsp; **中文**

**把历史制度当作被验证过的协调系统，重写成可调度、可审查、只说数据能证明的话的智能体系统。**

</div>

---

## 核心想法

一道唐代政令要经三省才成法：中书拟、门下审、尚书行。波斯总督制靠联邦式授权，再用巡回审计制衡。雅典议事会让判断在众人手中轮转，没有任何一只手能独揽。

这些是**最早的多智能体系统**——对我们接 AI 时遇到的同一批问题给出过实战验证的答案：如何授权、如何把质量关、如何升级失败、如何分散判断、如何留下可审查的记录。

| 学科 | 被验证的模式 | 我用它造什么 |
|---|---|---|
| 历史 | 唐三省审核 · 波斯总督制 · 雅典轮值 | 质量门 · 联邦式授权 · 分散判断 |
| 政治学 | 治理模式与制度约束 | 智能体拓扑 · 权限边界 · 升级路径 |
| 行为经济学 | 快慢思考 · 有限理性 | 模型路由 · 评估器设计 · 失败模式分析 |
| 知识管理 | 笔记 · 链接 · 索引 · 证据链 | 持久记忆 · 研究档案 · 可检索上下文 |

---

## 正在做

| 项目 | 是什么 |
|---|---|
| **[agos](https://github.com/LeoLin990405/agos)** | 诚实优先的 Agent OS 控制台：遥测、影子模型路由、记忆工作台、homelab 机群。铁律由测试强制执行——*屏幕上不出现任何数据证明不了的话*。人保留决定权，模型只提议。 |
| **[civagent](https://github.com/LeoLin990405/civagent)** · ⭐ 40 | 主线最纯粹的化身：**把 57 套历史治理制度编译成多智能体编排模式**。v6 加入宪政引擎（`VETO` / `IMPEACH` / `EDICT`）、政体拓扑图类型化，以及锦标赛统计管线（Bradley–Terry 排名 + bootstrap 置信区间、消融实验），检验制度是否真的改变结果。 |
| **[FuguNano](https://github.com/BicaMindLabs/FuguNano)** · ⭐ 27 | Sakana Fugu 的开源、免训练复现：让你手上已有的 agent 跑成一个可审计的闭环——规划、分派、审查、修复、学习——配有验证感知的选择器与桌面端 Studio。 |

## 常用工具

- **[grimoire-skill](https://github.com/LeoLin990405/grimoire-skill)** · ⭐ 8 — 一次解析 PDF，炼出两件器物：落进 Obsidian 的类型化阅读笔记 + 可复用技能包。
- **[oral-interview-transcription-skill](https://github.com/LeoLin990405/oral-interview-transcription-skill)** · ⭐ 13 — 口述史录音 → 忠实整理稿，带对抗式忠实度质量门，数据全程本地。
- **[skill-librarian](https://github.com/LeoLin990405/skill-librarian)** — 给大型本地 `SKILL.md` 技能库做体检与索引：重复、死链、重名、弱描述。
- **[paper-reading-workflow-zh](https://github.com/LeoLin990405/paper-reading-workflow-zh)** — 证据落地的中文论文精读流程（PDF → MinerU → Obsidian）。
- **[cn-cc](https://github.com/LeoLin990405/cn-cc)** · **[mmteam-cc](https://github.com/LeoLin990405/mmteam-cc)** — 把 Claude Code 任务路由到国产模型后端；多模型 agent 团队与扇出共识。
- **[ScreenBar](https://github.com/LeoLin990405/ScreenBar)** — SwiftUI 菜单栏应用，把 tailnet 里的 Mac 变成第二块屏幕。

## 上游贡献

协调也意味着在别人的「制度」里好好贡献。2026 年 6 月中旬以来已合并：

| 仓库 | ⭐ | 合并数 | 代表 PR |
|---|---|---|---|
| [steipete/CodexBar](https://github.com/steipete/CodexBar) | 2.1万 | 11 | LongCat 用量源（[#1697](https://github.com/steipete/CodexBar/pull/1697)）· 豆包 Agent Plan 用量（[#2496](https://github.com/steipete/CodexBar/pull/2496)）· 复用已授权 Safe Storage ACL（[#2528](https://github.com/steipete/CodexBar/pull/2528)）· 实时 rollout 不再饿死费用更新（[#3314](https://github.com/steipete/CodexBar/pull/3314)） |
| [jackwener/OpenCLI](https://github.com/jackwener/OpenCLI) | 2.9万 | 8 | 小红书风控冷却重试（[#2207](https://github.com/jackwener/OpenCLI/pull/2207)）· X 主页数据恢复（[#2193](https://github.com/jackwener/OpenCLI/pull/2193)）· 东方财富列名修正（[#2131](https://github.com/jackwener/OpenCLI/pull/2131)） |
| [Hmbown/Codewhale](https://github.com/Hmbown/Codewhale) | 4.1万 | 4 | 卡死恢复前先持久化会话（[#3285](https://github.com/Hmbown/Codewhale/pull/3285)）· `fetch` 遵守代理环境变量（[#3577](https://github.com/Hmbown/Codewhale/pull/3577)） |
| [steipete/oracle](https://github.com/steipete/oracle) | 4.0k | 4 | 短捕获需完成证明（[#293](https://github.com/steipete/oracle/pull/293)）· 窗口隐藏时恢复提交（[#302](https://github.com/steipete/oracle/pull/302)） |
| [blueberrycongee/wuu](https://github.com/blueberrycongee/wuu) | 48 | 4 | 后台命令归属记录（[#195](https://github.com/blueberrycongee/wuu/pull/195)）· 稳定工具前缀（[#194](https://github.com/blueberrycongee/wuu/pull/194)） |
| [BigPizzaV3/CodexPlusPlus](https://github.com/BigPizzaV3/CodexPlusPlus) | 3.1万 | 2 | 保留带版本号的 base URL（[#1363](https://github.com/BigPizzaV3/CodexPlusPlus/pull/1363)）· 注入模块缺失时优雅降级（[#1360](https://github.com/BigPizzaV3/CodexPlusPlus/pull/1360)） |
| [hoangsonww/Claude-Code-Agent-Monitor](https://github.com/hoangsonww/Claude-Code-Agent-Monitor) | 998 | 1 | 子代理平均时长不再为负（[#171](https://github.com/hoangsonww/Claude-Code-Agent-Monitor/pull/171)） |

## 最近

- **2026-09** — **agos** 公开：执行加固、审批与机群状态（[#1](https://github.com/LeoLin990405/agos/pull/1)），验收树对齐并落地会话/聊天/控制台诚实片（[#2](https://github.com/LeoLin990405/agos/pull/2)）；CodexBar 费用更新与标题栏修复（[#3314](https://github.com/steipete/CodexBar/pull/3314)、[#3315](https://github.com/steipete/CodexBar/pull/3315)）；口述史技能新增逐段 Word 式审阅包与播客文类（[#1](https://github.com/LeoLin990405/oral-interview-transcription-skill/pull/1)）。
- **2026-08** — civagent R6–R14：政体编辑 API + 在线编辑器、实验效度层、运行时拓扑 diff、真正卡人的 CI（[#31](https://github.com/LeoLin990405/civagent/pull/31)–[#34](https://github.com/LeoLin990405/civagent/pull/34)）；CodexBar 支持阿里云个人版套餐（[#3098](https://github.com/steipete/CodexBar/pull/3098)、[#3128](https://github.com/steipete/CodexBar/pull/3128)）与 z.ai 7/30 天图表（[#2524](https://github.com/steipete/CodexBar/pull/2524)）；OpenCLI 小红书风控冷却（[#2207](https://github.com/jackwener/OpenCLI/pull/2207)）。
- **2026-07** — civagent v6 加固线：宪政引擎、Express API、锦标赛统计、消融生成器、爬山循环（[#17](https://github.com/LeoLin990405/civagent/pull/17)–[#30](https://github.com/LeoLin990405/civagent/pull/30)）；FuguNano 选择器路由、SWE-bench 驱动与 FuguNano Studio 桌面端（[#6](https://github.com/BicaMindLabs/FuguNano/pull/6)–[#16](https://github.com/BicaMindLabs/FuguNano/pull/16)）；oracle 四个浏览器修复、wuu 四个 PR、CodexPlusPlus 修复；发布 skill-librarian 与 paper-reading-workflow-zh。
- **2026-06** — cn-cc `/cn:team` 多模型扇出（[#5](https://github.com/LeoLin990405/cn-cc/pull/5)）；Codewhale TUI 修复（[#3284](https://github.com/Hmbown/Codewhale/pull/3284)、[#3285](https://github.com/Hmbown/Codewhale/pull/3285)）；OpenCLI Gemini/什么值得买修复（[#1967](https://github.com/jackwener/OpenCLI/pull/1967)、[#1968](https://github.com/jackwener/OpenCLI/pull/1968)）；发布 ScreenBar。

## 此外

**BicaMind** — 一款声音优先的 AI 伴侣，做成开放式耳夹耳机：同一种「让知识随取随用且值得信赖」的执念，走出终端。应用 ML 作品收在 [udacity-masters-ai-projects](https://github.com/LeoLin990405/udacity-masters-ai-projects)；连接历史、社会科学与 agent 架构的随笔在[博客](https://leolin990405.github.io/blog/)。

<div align="center">

[English ↑](#english) &nbsp;·&nbsp; [回到顶部](#chinese)

</div>

---

## Stack | 技术栈

<div align="center">

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Swift](https://img.shields.io/badge/Swift-F05138?style=for-the-badge&logo=swift&logoColor=white)
![Shell](https://img.shields.io/badge/Shell-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white)
![R](https://img.shields.io/badge/R-276DC3?style=for-the-badge&logo=r&logoColor=white)

![Claude](https://img.shields.io/badge/Claude-191919?style=for-the-badge&logo=anthropic&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI_API-412991?style=for-the-badge&logo=openai&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-6C63FF?style=for-the-badge&logoColor=white)
![Obsidian](https://img.shields.io/badge/Obsidian-7C3AED?style=for-the-badge&logo=obsidian&logoColor=white)

</div>

## Stats | 数据统计

<div align="center">

<a href="https://ghfind.com/u/leolin990405?ref=badge">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://ghfind.com/api/card/mini/leolin990405?lang=en&theme=dark" />
    <source media="(prefers-color-scheme: light)" srcset="https://ghfind.com/api/card/mini/leolin990405?lang=en&theme=light" />
    <img width="420" alt="GitHub Roast score card · ghfind" src="https://ghfind.com/api/card/mini/leolin990405?lang=en&theme=dark" />
  </picture>
</a>

<img width="49%" src="https://github-readme-stats.vercel.app/api?username=LeoLin990405&show_icons=true&theme=tokyonight&hide_border=true&count_private=true&include_all_commits=true&bg_color=0d1117&ring_color=6C63FF&icon_color=6C63FF" />
<img width="49%" src="https://github-readme-stats.vercel.app/api/top-langs/?username=LeoLin990405&layout=compact&theme=tokyonight&hide_border=true&langs_count=8&bg_color=0d1117" />

</div>

## Contact | 联系

- GitHub: [@LeoLin990405](https://github.com/LeoLin990405)
- Blog · 博客: [leolin990405.github.io/blog](https://leolin990405.github.io/blog/)
- LinkedIn: [Zhongyue Lin](https://www.linkedin.com/in/zhongyue-lin-327143207/)

If one of my projects is useful, a star is always appreciated. · 如果哪个项目帮到了你，欢迎点个 star。
