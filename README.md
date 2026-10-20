<div align="center">

# Leo Lin · 林中玥

[![GitHub](https://img.shields.io/badge/GitHub-LeoLin990405-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/LeoLin990405)
[![Blog](https://img.shields.io/badge/Blog-leolin990405.github.io-6C63FF?style=for-the-badge&logo=github&logoColor=white)](https://leolin990405.github.io/blog/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Zhongyue_Lin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/zhongyue-lin-327143207/)
[![Profile Views](https://komarev.com/ghpvc/?username=LeoLin990405&style=for-the-badge&color=6C63FF&label=PROFILE+VIEWS)](https://github.com/LeoLin990405)

### **English** &nbsp;·&nbsp; [中文](#chinese)

**Personal memory and personal data for AI agents, plus the infra and hardware they run on — local-first memory where a human-approved write comes before a model proposal, and an inference is never passed off as the user's own words.**

</div>

<a id="english"></a>

---

## The line

From collection, through structuring and judgment, to the memory layer and the device. Control order is **human > mechanism > model**. A conclusion ships with a rerunnable test, and a negative result stays in the record.

| Stage | Where | What |
|---|---|---|
| Collection | 华润万象生活 (Shanghai) | Daily reconciliation and paper receipts enter a pipeline a person can rerun |
| Structure & judgment | 小铁 | Scattered store data into one schema; the model judges, rules and a person release |
| Memory & device | BicaMind | Long-term memory for a voice agent, and the hardware it enters through |
| Forgetting & retention | memfw | Fixed rules forget and anchor; a model may propose, a person applies |

---

## Memory

**memfw** — a model-agnostic, local-first personal memory framework (Python, private). Five forgetting strategies (FIFO / LRU / decay / salience / consolidate-then-forget) are pure functions and give a reason per row. Human anchors are never evicted. The model may propose a merge; it applies only after a person approves. Markdown is the authority, a hash-chained JSONL log records every state change, and SQLite FTS5 is a disposable index. The framework does not call an LLM and does not send data out.

Full local LoCoMo, 2026-10-19, including the negative results: 10 conversations, 5,882 turns, 1,986 questions, 1,000 paired bootstrap samples with Holm correction, finished in 249 seconds. No pairwise difference is significant. At a 25% budget, salience has the highest point estimate, 14.5% against FIFO 13.0%, and that gap is not significant. On 200 synthetic items, none of the strategies cleared the collection bar. 396 tests and `mypy --strict` passed. A pilot import of 656 real memories on local MLX (Qwen2.5-7B 4-bit) is stuck on import: after 6+ hours only 498 rows landed, because each save rechecks the whole store. Model proposals are paused; batch writes are next. 38.4% of those records have only a file mtime as a timestamp.

**BicaMind** — my work on long-term memory for a voice agent. A spoken "remember this" has to actually land, and a model inference must not wear the user's voice. Explicit user memory is stored as such (replayed at confidence 0.95, recalled next session). Inferences are capped at 0.65, under the 0.7 bar of the always-on voice prompt, so they reach the live turn only through prefetch.

**[sayless](https://github.com/LeoLin990405/sayless)** — local-first dictation. A non-commercial learning project. Record → whisper.cpp on device (about 1 second for 8 seconds of speech; audio stays on the machine) → a deterministic dictionary → LLM polish → paste into the focused app. History and the lexicon stay local.

Day to day, the agents I use share one Markdown memory on my own NAS (user / feedback / project / reference / incident; credentials stay out). Snapshot 2026-10-17: about 600 memories, 1,400+ change events, 2,963 commits across several agent identities.

**Companion-model eval.** Whether a companion is good is not just factual accuracy. 150 scenarios (130 test / 20 dev, 17 subtypes) are frozen, blind-judged, turned into training data, then checked before/after. Real generations cover 9 providers: 1,168/1,170 outputs, 660 pairwise judgments. Still open: a synthetic set, a single judge, 13 rank reversals, an unfilled human-calibration pack, and a 500-step LoRA run.

**Flickfic** — a University of Hong Kong student startup initiated by REMi; I am the main engineer. Reader behavior (views, dwell, drop-off) drives regeneration of the weak states. Not linked here.

---

## Hardware & AI infra

- **On-device models.** MLX, GGUF, and whisper.cpp.
- **Home lab, on Tailscale.** Multi-GPU machines, Mac MLX for local inference, and k3s on three Lenovo Tiny machines, plus an Apple Silicon node and a NAS. A model farm swaps models as quota and quality change; task state stays in local SQLite.
- **Dev boards.** RK3566, RK3399, RK3568. Raspberry Pi Pico 2 W (ARM and RISC-V). ESP32.

---

## Supporting work

| Project | What it is |
|---|---|
| **[agos](https://github.com/LeoLin990405/agos)** | Honesty-first console and memory workbench. Every figure comes from a ledger on disk; a missing probe renders as not collected. Humans keep the decision; models propose. |
| **[civagent](https://github.com/LeoLin990405/civagent)** · ⭐ 41 | An orchestration and governance experiment: 57 historical governance systems compiled into multi-agent patterns, with a constitutional engine (`VETO` / `IMPEACH` / `EDICT`) and a tournament pipeline that tests whether the institution changes the outcome. |
| **[FuguNano](https://github.com/BicaMindLabs/FuguNano)** · ⭐ 28 | Training-free control plane (BicaMind Labs): plan, dispatch, review, repair, learn, with verifier-aware routing and a bounded repair loop. |

## Tools I keep sharp

Stars counted 2026-10-20.

- **[grimoire-skill](https://github.com/LeoLin990405/grimoire-skill)** · ⭐ 8 — parse a PDF once, forge two artifacts: typed reading notes for Obsidian and a reusable skill pack.
- **[oral-interview-transcription-skill](https://github.com/LeoLin990405/oral-interview-transcription-skill)** · ⭐ 16 — oral-history recordings → faithful edited transcripts, with an adversarial fidelity gate; data stays local.
- **[r-analytics-skill](https://github.com/LeoLin990405/r-analytics-skill)** · ⭐ 5 — 93 package-level R skills for Claude Code.
- **[skill-librarian](https://github.com/LeoLin990405/skill-librarian)** · ⭐ 1 — lint and index a large local `SKILL.md` library: duplicates, dead links, name collisions, weak descriptions.
- **[paper-reading-workflow-zh](https://github.com/LeoLin990405/paper-reading-workflow-zh)** · ⭐ 1 — evidence-grounded Chinese paper-reading workflow (PDF → MinerU → Obsidian).
- **[cn-cc](https://github.com/LeoLin990405/cn-cc)** · ⭐ 1 · **[mmteam-cc](https://github.com/LeoLin990405/mmteam-cc)** — route Claude Code work to Chinese model backends; multi-model agent teams with fan-out consensus.
- **[ScreenBar](https://github.com/LeoLin990405/ScreenBar)** — a SwiftUI menu-bar app that turns Macs on your tailnet into second screens.

Applied ML coursework: [udacity-masters-ai-projects](https://github.com/LeoLin990405/udacity-masters-ai-projects). Essays: [blog](https://leolin990405.github.io/blog/).

## Upstream

Merged pull requests in other people's repositories, coursework set aside. Counted 2026-10-20: **70 merged** across the 9 repositories below, **8 still open**. Star counts are exact.

| Repository | ⭐ | Merged | Highlights |
|---|---|---|---|
| [steipete/CodexBar](https://github.com/steipete/CodexBar) | 22,677 | 22 | LongCat provider ([#1697](https://github.com/steipete/CodexBar/pull/1697)) · empty Personal usage responses retry and keep the last good card ([#3128](https://github.com/steipete/CodexBar/pull/3128)) · live rollouts no longer starve cost updates ([#3314](https://github.com/steipete/CodexBar/pull/3314)) |
| [jackwener/OpenCLI](https://github.com/jackwener/OpenCLI) | 30,462 | 21 | Kimi web adapter, 21 commands ([#1804](https://github.com/jackwener/OpenCLI/pull/1804)) · Xiaohongshu risk-control cooldown retry ([#2207](https://github.com/jackwener/OpenCLI/pull/2207)) · X profile recovery ([#2193](https://github.com/jackwener/OpenCLI/pull/2193)) |
| [SeemSeam/claude_codex_bridge](https://github.com/SeemSeam/claude_codex_bridge) | 3,580 | 9 | Qwen Code CLI provider ([#124](https://github.com/SeemSeam/claude_codex_bridge/pull/124)) · GitHub Copilot CLI provider ([#122](https://github.com/SeemSeam/claude_codex_bridge/pull/122)) |
| [codewhale-hq/Codewhale](https://github.com/codewhale-hq/Codewhale) | 41,103 | 5 | session persists before stall recovery ([#3285](https://github.com/codewhale-hq/Codewhale/pull/3285)) · `@` completion file walk has a wall-clock budget ([#4367](https://github.com/codewhale-hq/Codewhale/pull/4367)) |
| [steipete/oracle](https://github.com/steipete/oracle) | 4,062 | 4 | completion proof for short captures ([#293](https://github.com/steipete/oracle/pull/293)) · hidden-window prompt submission ([#302](https://github.com/steipete/oracle/pull/302)) |
| [blueberrycongee/wuu](https://github.com/blueberrycongee/wuu) | 60 | 4 | background-command ownership ([#195](https://github.com/blueberrycongee/wuu/pull/195)) · stable tool prefix ([#194](https://github.com/blueberrycongee/wuu/pull/194)) |
| [BigPizzaV3/CodexPlusPlus](https://github.com/BigPizzaV3/CodexPlusPlus) | 32,404 | 2 | versioned base URL kept ([#1363](https://github.com/BigPizzaV3/CodexPlusPlus/pull/1363)) · graceful inject fallback ([#1360](https://github.com/BigPizzaV3/CodexPlusPlus/pull/1360)) |
| [steipete/RepoBar](https://github.com/steipete/RepoBar) | 2,215 | 2 | compact badges round to nearest ([#81](https://github.com/steipete/RepoBar/pull/81)) · opt-in release notifications ([#82](https://github.com/steipete/RepoBar/pull/82)) |
| [hoangsonww/Claude-Code-Agent-Monitor](https://github.com/hoangsonww/Claude-Code-Agent-Monitor) | 1,099 | 1 | non-negative subagent durations ([#171](https://github.com/hoangsonww/Claude-Code-Agent-Monitor/pull/171)) |

## Recently

- **2026-10** — [sayless](https://github.com/LeoLin990405/sayless) is public. memfw's full LoCoMo run is above, negative result included.
- **2026-09** — [agos](https://github.com/LeoLin990405/agos) opened: execution, approvals, and fleet state ([#1](https://github.com/LeoLin990405/agos/pull/1)); honest session, chat, and console slices ([#2](https://github.com/LeoLin990405/agos/pull/2)).

<div align="center">

[↑ back to top](#english) &nbsp;·&nbsp; [切换到中文 →](#chinese)

</div>

---
---

<a id="chinese"></a>

<div align="center">

# 林中玥 · Leo Lin

### [English](#english) &nbsp;·&nbsp; **中文**

**为 AI 智能体做个人记忆与个人数据，连同它们所依赖的基础设施与硬件：本地优先，人批准的写入先于模型提议，推断绝不冒充用户自己的话。**

</div>

---

## 这条线

从采集，经结构化与判断，到记忆层和设备入口。控制顺序是**人 > 机制 > 模型**。结论尽量配可复现的测试，负结果照实留下。

| 阶段 | 所在 | 做什么 |
|---|---|---|
| 采集 | 华润万象生活（上海） | 每日对账与纸质小票进入可以重跑的流程 |
| 结构化与判断 | 小铁 | 分散的门店数据收成一套 schema；模型负责判断，规则与人负责放行 |
| 记忆层与设备入口 | BicaMind | 语音 Agent 的长期记忆，以及它进入的硬件 |
| 遗忘与留存 | memfw | 固定规则负责遗忘与锚定；模型可以提议，人来批准 |

---

## 记忆

**memfw** — 模型无关、本地优先的个人记忆框架（Python，未公开）。五种遗忘策略（FIFO / LRU / 衰减 / 显著性 / 先整合后遗忘）是纯函数，逐条给出理由。人工锚定的记忆不被淘汰。模型可以提议合并，人批准后才应用。Markdown 是权威内容，带哈希链的 JSONL 记录每次状态变化，SQLite FTS5 只是可丢弃的索引。框架本身不调用 LLM，也不向外发送数据。

本地全量 LoCoMo（2026-10-19），含负结果：10 段对话、5,882 轮、1,986 题，1,000 次配对 bootstrap + Holm 校正，249 秒跑完。五种策略两两比较均无显著差异。25% 预算下显著性策略的点估计最高，14.5% 对 FIFO 的 13.0%，差异不显著。200 条合成数据上，没有策略达到采集门槛。396 项测试与 `mypy --strict` 通过。在本人 656 份真实记忆上，本地 MLX（Qwen2.5-7B 4-bit）试点卡在导入：6 小时余只写入 498 条，因为每次保存都重校验整库。模型提议阶段已暂停，下一步改为批量写入。其中 38.4% 的记录只有文件修改时间可作时间戳。

**BicaMind** — 我在做语音 Agent 的长期记忆。用户说「记住这个」，必须真的落库；模型的推断不能穿上用户的声音。用户显式记忆按显式来源入库（回放验证置信度 0.95，下次会话可召回）。推断的置信度上限 0.65，低于语音常驻 prompt 的 0.7 门槛，只能经预取进入当前轮。

**[sayless](https://github.com/LeoLin990405/sayless)** — 本地优先的语音听写，非商用的学习项目。录音 → 本机 whisper.cpp（8 秒语音约 1 秒转完，语音不出机器）→ 词语库确定性替换 → LLM 润色 → 粘贴进焦点应用。听写历史和词库都在本地。

日常使用的多个 Agent 共用一套放在自有 NAS 上的 Markdown 记忆（user / feedback / project / reference / incident；凭据不入库）。2026-10-17 快照：约 600 条记忆、1,400+ 条变更事件、来自多个 Agent 身份的 2,963 次提交。

**陪伴模型评测。** 陪伴好不好，不只看事实对不对。150 条场景（130 test / 20 dev，17 个子类）先冻结，再盲评，再变成训练数据，然后做 before/after 回归。真实生成覆盖 9 个 provider：1,168/1,170 条输出，660 条 pairwise 判断。尚未解决：合成测试集、单一 judge、13 处排序反转、人工校准包还空着、LoRA 只跑了 500 步。

**Flickfic** — 香港大学学生创业项目，由 REMi 发起，我是主力工程师。读者的浏览、停留和流失，用来决定哪一段重新生成。此处不放链接。

---

## 硬件与 AI 基础设施

- **端侧模型。** MLX、GGUF、whisper.cpp。
- **家庭实验室，Tailscale 组网。** 多 GPU 机器、Mac 上的 MLX 本地推理，以及三台联想 Tiny 上的 k3s，另有 Apple Silicon 节点和 NAS。模型农场按配额和质量替换模型；任务状态留在本机 SQLite。
- **开发板。** RK3566、RK3399、RK3568。Raspberry Pi Pico 2 W（ARM 与 RISC-V）。ESP32。

---

## 支撑工作

| 项目 | 是什么 |
|---|---|
| **[agos](https://github.com/LeoLin990405/agos)** | 诚实优先的控制台与记忆工作台。屏幕上的每个数字都来自磁盘账本；没有探针就显示「未采集」。人保留决定权，模型只提议。 |
| **[civagent](https://github.com/LeoLin990405/civagent)** · ⭐ 41 | 编排与治理实验：把 57 套历史治理制度编译成多智能体模式，带宪政引擎（`VETO` / `IMPEACH` / `EDICT`）和锦标赛管线，用来检验制度是否真的改变结果。 |
| **[FuguNano](https://github.com/BicaMindLabs/FuguNano)** · ⭐ 28 | 免训练的控制平面（BicaMind Labs）：规划、分派、审查、修复、学习，按验证器结果路由，修复循环有界。 |

## 常用工具

Star 数统计于 2026-10-20。

- **[grimoire-skill](https://github.com/LeoLin990405/grimoire-skill)** · ⭐ 8 — 一次解析 PDF，炼出两件器物：落进 Obsidian 的类型化阅读笔记，以及可复用的技能包。
- **[oral-interview-transcription-skill](https://github.com/LeoLin990405/oral-interview-transcription-skill)** · ⭐ 16 — 口述史录音 → 忠实整理稿，带对抗式忠实度质量门，数据全程本地。
- **[r-analytics-skill](https://github.com/LeoLin990405/r-analytics-skill)** · ⭐ 5 — 面向 Claude Code 的 93 个 R 包级技能。
- **[skill-librarian](https://github.com/LeoLin990405/skill-librarian)** · ⭐ 1 — 给大型本地 `SKILL.md` 技能库做体检与索引：重复、死链、重名、弱描述。
- **[paper-reading-workflow-zh](https://github.com/LeoLin990405/paper-reading-workflow-zh)** · ⭐ 1 — 证据落地的中文论文精读流程（PDF → MinerU → Obsidian）。
- **[cn-cc](https://github.com/LeoLin990405/cn-cc)** · ⭐ 1 · **[mmteam-cc](https://github.com/LeoLin990405/mmteam-cc)** — 把 Claude Code 任务路由到国产模型后端；多模型 agent 团队与扇出共识。
- **[ScreenBar](https://github.com/LeoLin990405/ScreenBar)** — SwiftUI 菜单栏应用，把 tailnet 里的 Mac 变成第二块屏幕。

应用 ML 课程作业：[udacity-masters-ai-projects](https://github.com/LeoLin990405/udacity-masters-ai-projects)。随笔在[博客](https://leolin990405.github.io/blog/)。

## 上游贡献

合进别人仓库的 pull request，课程作业除外。计数日期 2026-10-20：下表 9 个仓库共 **70 个已合并**，另有 **8 个仍开放**。Star 为精确值。

| 仓库 | ⭐ | 合并数 | 代表 PR |
|---|---|---|---|
| [steipete/CodexBar](https://github.com/steipete/CodexBar) | 22,677 | 22 | LongCat 用量源（[#1697](https://github.com/steipete/CodexBar/pull/1697)）· Personal 空用量响应会重试，并保留最近一张有效卡片（[#3128](https://github.com/steipete/CodexBar/pull/3128)）· 实时 rollout 不再饿死费用更新（[#3314](https://github.com/steipete/CodexBar/pull/3314)） |
| [jackwener/OpenCLI](https://github.com/jackwener/OpenCLI) | 30,462 | 21 | Kimi 网页端适配器，21 条命令（[#1804](https://github.com/jackwener/OpenCLI/pull/1804)）· 小红书风控冷却后重试（[#2207](https://github.com/jackwener/OpenCLI/pull/2207)）· X 主页数据恢复（[#2193](https://github.com/jackwener/OpenCLI/pull/2193)） |
| [SeemSeam/claude_codex_bridge](https://github.com/SeemSeam/claude_codex_bridge) | 3,580 | 9 | Qwen Code CLI 提供方（[#124](https://github.com/SeemSeam/claude_codex_bridge/pull/124)）· GitHub Copilot CLI 提供方（[#122](https://github.com/SeemSeam/claude_codex_bridge/pull/122)） |
| [codewhale-hq/Codewhale](https://github.com/codewhale-hq/Codewhale) | 41,103 | 5 | 卡死恢复前先持久化会话（[#3285](https://github.com/codewhale-hq/Codewhale/pull/3285)）· `@` 补全的文件遍历有墙钟预算（[#4367](https://github.com/codewhale-hq/Codewhale/pull/4367)） |
| [steipete/oracle](https://github.com/steipete/oracle) | 4,062 | 4 | 短捕获需完成证明（[#293](https://github.com/steipete/oracle/pull/293)）· 窗口隐藏时恢复提交（[#302](https://github.com/steipete/oracle/pull/302)） |
| [blueberrycongee/wuu](https://github.com/blueberrycongee/wuu) | 60 | 4 | 后台命令归属记录（[#195](https://github.com/blueberrycongee/wuu/pull/195)）· 稳定工具前缀（[#194](https://github.com/blueberrycongee/wuu/pull/194)） |
| [BigPizzaV3/CodexPlusPlus](https://github.com/BigPizzaV3/CodexPlusPlus) | 32,404 | 2 | 保留带版本号的 base URL（[#1363](https://github.com/BigPizzaV3/CodexPlusPlus/pull/1363)）· 注入模块缺失时优雅降级（[#1360](https://github.com/BigPizzaV3/CodexPlusPlus/pull/1360)） |
| [steipete/RepoBar](https://github.com/steipete/RepoBar) | 2,215 | 2 | 紧凑角标改为四舍五入（[#81](https://github.com/steipete/RepoBar/pull/81)）· 可为置顶仓库打开发布通知（[#82](https://github.com/steipete/RepoBar/pull/82)） |
| [hoangsonww/Claude-Code-Agent-Monitor](https://github.com/hoangsonww/Claude-Code-Agent-Monitor) | 1,099 | 1 | 子代理平均时长不再为负（[#171](https://github.com/hoangsonww/Claude-Code-Agent-Monitor/pull/171)） |

## 最近

- **2026-10** — [sayless](https://github.com/LeoLin990405/sayless) 公开。memfw 的全量 LoCoMo 见上，负结果一并记下。
- **2026-09** — [agos](https://github.com/LeoLin990405/agos) 公开：执行、审批与机群状态（[#1](https://github.com/LeoLin990405/agos/pull/1)）；会话、聊天与控制台的诚实切片（[#2](https://github.com/LeoLin990405/agos/pull/2)）。

<div align="center">

[English ↑](#english) &nbsp;·&nbsp; [回到顶部](#chinese)

</div>

---

## Stack | 技术栈

<div align="center">

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Go](https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white)
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
