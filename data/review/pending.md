# 待审核仓库 / Pending review

> 新增到 `dsh-plugin` Topic 下、带有简介、尚未经维护者核实的仓库。本文件由 `scripts/update.mjs` 每日刷新，仅供审核使用，不是用户可见页面。
>
> Repositories newly added to the `dsh-plugin` topic that the maintainer has not verified yet. Refreshed daily by `scripts/update.mjs`; review-only, not a user-facing page.

- 生成时间 / Generated: **2026-08-26**
- 快照日期 / Snapshot date: **2026-08-26 (UTC)**
- 待审核 / Pending: **1629**
- 从快照消失的已核准仓库 / Approved repositories missing from the snapshot: **353**

审核决定记到数据文件后运行 `node scripts/merge.mjs` 生效：

- 通过 → 加入 [data/approved.json](../approved.json)（`"owner/name": "YYYY-MM-DD"`）
- 剔除 → 加入 [data/curated.json](../curated.json) 的 `excluded_repos`，理由只写「不是 DSH 插件 + 它是什么」，并同步从 `approved.json` 移除
- 只进目录、不进榜单 → 加入 `approved.json` + `curated.json` 的 `leaderboard_exclusions`
- 非插件形态 / market 类（插件市场、商店、技能商城、内置市场的桌面端等）→ 加入 `curated.json` 的 `market_exclusions`（市场不能包含市场）
- 目录站 / awesome-list / 榜单站（如 `awesome-dsh-plugin*` 系列）→ `excluded_repos` 整体剔除，不留目录

完整约定见 [data/review/README.md](./README.md)。

Record decisions in the data files, then run `node scripts/merge.mjs`:

- Approve → add to [data/approved.json](../approved.json) (`"owner/name": "YYYY-MM-DD"`)
- Exclude → add to `excluded_repos` in [data/curated.json](../curated.json) — the reason just states "not a DSH plugin + what it is" — and remove it from `approved.json`
- Catalog-only (not in the board) → add to `approved.json` + `leaderboard_exclusions` in `curated.json`
- Non-plugin form / market class (plugin market, store, skill mall, desktop with a built-in market) → `market_exclusions` in `curated.json` (the market cannot include another market)
- Directory sites / awesome-lists / leaderboards (e.g. the `awesome-dsh-plugin*` family) → `excluded_repos` outright

See [data/review/README.md](./README.md) for the full convention.

| # | Project | Stars | Created | First seen | Description |
| ---: | --- | ---: | --- | --- | --- |
| 1 | [Molunerfinn/PicGo](https://github.com/Molunerfinn/PicGo) | 27052 | 2017-12-12 | 2026-08-22 | :rocket: The Ultimate Image Uploader for Efficient Creators. Supports Obsidian, Typora, VS Code etc. and 60+ image hosting services  (S3, GitHub, Cloudflare R2, Imgur, Aliyun OSS...). Paste, upload, done. |
| 2 | [titanwings/distilly](https://github.com/titanwings/distilly) | 24011 | 2026-03-30 | 2026-08-24 | Distilly — Distill how they think into reusable Skills for any Agent or Bot. Formerly Colleague Skill（原同事 Skill）. |
| 3 | [anywhere-labs/dsh-desktop](https://github.com/anywhere-labs/dsh-desktop) | 20657 | 2026-08-13 | 2026-08-24 | 为 DeepSeek Harness (DSH) 插件生态打造的现代化桌面端解决方案。万物皆「插件」，桌面本身也是「插件」。 |
| 4 | [yjh051108/dsh-routing-suite](https://github.com/yjh051108/dsh-routing-suite) | 6846 | 2026-08-14 | 2026-08-23 | dsh-routing-suite — injector + router-standard kit: install the runtime injector first, then the task-aware reasoning-mode router preset (measured P1-P23). |
| 5 | [zhu1090093659/dsh-web](https://github.com/zhu1090093659/dsh-web) | 6173 | 2026-08-12 | 2026-08-24 | DeepSeek Harness（DSH）Web 插件聚合生态包 · 一切皆插件，创意工坊分发 |
| 6 | [agentscope-ai/ReMe](https://github.com/agentscope-ai/ReMe) | 3356 | 2024-08-29 | 2026-08-24 | ReMe: Memory Management Kit for Agents - Remember Me, Refine Me. |
| 7 | [Tiger3807861189/J-Space-Cognition-Suite-V3.7](https://github.com/Tiger3807861189/J-Space-Cognition-Suite-V3.7) | 3017 | 2026-07-22 | 2026-08-23 | J-Space Cognition Suite V3.7 - AI cognitive-enhancement Skills based on Anthropic's J-space global workspace research. \| 哔哩哔哩：Tiger380 (UID 3494375382321675) — https://space.bilibili.com/3494375382321675 |
| 8 | [zilliztech/memsearch](https://github.com/zilliztech/memsearch) | 2515 | 2026-02-09 | 2026-08-24 | A persistent, unified memory layer for all your AI agents (e.g. Claude Code, Codex, DSH), backed by Markdown and Milvus. |
| 9 | [dsh-tauri-desk/deepseek-harness-desktop](https://github.com/dsh-tauri-desk/deepseek-harness-desktop) | 1231 | 2026-08-14 | 2026-08-23 | DeepSeek Harness Tauri 桌面版 \| Only 5mb installer, zero environment setup, preset plugins, Windows / macOS / Linux. |
| 10 | [vshulcz/deja-vu](https://github.com/vshulcz/deja-vu) | 728 | 2026-07-14 | 2026-08-23 | Search your past AI coding sessions — Claude Code, Codex, Cursor and 17 more. Indexes the session history they already wrote to disk, including months from before you installed it, and recalls it in any of them. No LLM, no embeddings, one local Go binary. |
| 11 | [vibeinging/dsh-desktop](https://github.com/vibeinging/dsh-desktop) | 632 | 2026-08-13 | 2026-08-23 | DeepSeek Harness Desktop App: a local AI desktop workspace for DSH Sessions, projects, files, web research, plugins, and Office artifacts. |
| 12 | [chainbase-labs/Agentkey](https://github.com/chainbase-labs/Agentkey) | 604 | 2026-04-23 | 2026-08-25 | Connect your AI agent to the world — Web search, Social media, Crypto & On-chain data. One plugin, zero extra config. |
| 13 | [Minglink/dsh-infinite-gen-2](https://github.com/Minglink/dsh-infinite-gen-2) | 484 | 2026-08-15 | 2026-08-25 | DeepSeek 专用破甲插件「无限二代」dsh-infinite-gen-2 — armor-breaking plugin for DeepSeek稳定化破甲提示词，求 Star 收藏 ⭐ |
| 14 | [yjh051108/dsh-router-standard](https://github.com/yjh051108/dsh-router-standard) | 371 | 2026-08-14 | 2026-08-23 | 已并入 dsh-routing-suite（单仓库化）；本仓库为历史镜像/归档 —— 注意力工程主线 v1.19.1/v34 研发线未发布。新代码见 github.com/yjh051108/dsh-routing-suite |
| 15 | [Unclecheng-li/DeepSec](https://github.com/Unclecheng-li/DeepSec) | 340 | 2026-07-09 | 2026-08-25 | DeepSec — AI Security Offense & Defense Platform. Shield audits AI-generated code for hallucinated packages, missing safeguards & AI pattern errors in real time. Spear automates authorized penetration testing with 40+ skill packs, from recon to PoC.  |
| 16 | [ericshang98/Perfect-Web-Clone](https://github.com/ericshang98/Perfect-Web-Clone) | 258 | 2026-01-06 | 2026-08-22 | Pixel-perfect clones of any webpage. Paste a URL, get a measured Vite + React replica. |
| 17 | [Aisland-SJL/dsh-worktable](https://github.com/Aisland-SJL/dsh-worktable) | 199 | 2026-08-16 | 2026-08-24 | 🖥️ Agent-project workbench for DeepSeek Harness — sidebar app drawer + dockable split workspace + a live control room watching every project. |
| 18 | [zenstory-ai/oh-story-dsh](https://github.com/zenstory-ai/oh-story-dsh) | 196 | 2026-08-19 | 2026-08-25 | A DSH plugin for novel writing and short-drama production, powered by Oh Story and Drama Skills. |
| 19 | [yjh051108/dsh-super-injector](https://github.com/yjh051108/dsh-super-injector) | 151 | 2026-08-13 | 2026-08-25 | 推荐组件（非必须）：DeepSeek Harness 运行时注入器；已随 dsh-routing-suite 单仓库化保留，本仓库继续维护/发布。 |
| 20 | [EthanYoQ/Invoice-Downloader](https://github.com/EthanYoQ/Invoice-Downloader) | 141 | 2026-03-02 | 2026-08-22 | 电子发票整理与报销准备工具：从邮箱批量收集 PDF/OFD/XML 发票，OCR 识别、分类归档并生成 Excel 汇总；提供 Windows/macOS 桌面版与 DSH 插件。 |
| 21 | [ZSeven-W/dsh-android](https://github.com/ZSeven-W/dsh-android) | 119 | 2026-08-21 | 2026-08-22 | DeepSeek Harness plugin for Android — build, run, and interact with a live emulator or USB device stream inside a conversation, driven entirely through adb. |
| 22 | [volcengine/ark-cli](https://github.com/volcengine/ark-cli) | 109 | 2026-06-15 | 2026-08-22 | The fastest way to put Volcengine Ark in your terminal and your AI agent — go from prompt to generated   media, multimodal answer, or deployed endpoint in a single command, no API glue code. |
| 23 | [1692775560/dsh-Mimir-Academic-research](https://github.com/1692775560/dsh-Mimir-Academic-research) | 81 | 2026-08-20 | 2026-08-24 | Mimir — 一站式科研工作台插件：LaTeX 论文边写边编译、arXiv 文献管理、实验追踪、指标图表、GPU 服务器 SSH 任务编排，管理科研全周期。An open-source research workbench plugin for the whole research cycle. |
| 24 | [Akimiya-z/codex-guard](https://github.com/Akimiya-z/codex-guard) | 63 | 2026-08-20 | 2026-08-23 | Quality gate for AI/Codex-generated pull requests: blocks TODO leftovers, leaked secrets, sloppy commits and red CI before they reach main. |
| 25 | [peiyuwang54/deepseek-harness-cli](https://github.com/peiyuwang54/deepseek-harness-cli) | 56 | 2026-08-14 | 2026-08-23 | DeepSeek CLI (UnOfficial) |
| 26 | [yuc16/PatentRadar](https://github.com/yuc16/PatentRadar) | 56 | 2026-05-05 | 2026-08-22 | 专利侵权分析系统 —— 输入专利公开号，产出竞品侵权分析报告；同时打包成 skill，可被任意 agent（codex，claude code 等） 调用。 |
| 27 | [yxxbc/dsh-balance-plugin](https://github.com/yxxbc/dsh-balance-plugin) | 56 | 2026-08-15 | 2026-08-23 | deepSeek 余额监控与用量统计（DSH 动态 Cordis 插件）：余额监控 · 官方充值入口 · 用量统计 · 三方插件管理 |
| 28 | [AgentDebugX/AgentDebugX](https://github.com/AgentDebugX/AgentDebugX) | 50 | 2026-07-10 | 2026-08-25 | A debugging framework for agentic AI systems: diagnose failures, attribute root causes, recover with evidence, and validate fixes through reruns. |
| 29 | [JingxuanC/causal-memory](https://github.com/JingxuanC/causal-memory) | 49 | 2026-07-26 | 2026-08-24 | Causal memory layer for AI agents — MCP server that records decision→outcome relationships. Survives compaction. |
| 30 | [lamost423/dsh-maze](https://github.com/lamost423/dsh-maze) | 49 | 2026-08-18 | 2026-08-26 | DeepSeek Harness 的执行迷宫——看 Agent 真实怎么干活：迷宫时间轴 · 数据轨道 · 确定性执行分析 · 多会话对比 \| The execution maze for DSH agents: maze timeline, per-step data tracks, deterministic execution analysis, multi-session comparison. Formerly dsh-trace-compare. |
| 31 | [xi-zhao/OpenQuantum](https://github.com/xi-zhao/OpenQuantum) | 47 | 2026-08-15 | 2026-08-23 | Open-source quantum Agent workspace with a desktop client, Web UI, messaging, Qiskit/MCP tools, and scientific validation |
| 32 | [T-Auto/dsh-ecosystem-spec](https://github.com/T-Auto/dsh-ecosystem-spec) | 42 | 2026-08-17 | 2026-08-22 | deepseek-harness TUI Plugin Access and Implementation Standards / deepseek-harness终端交互生态插件准入规范与实施标准 |
| 33 | [BeforeWave/dsh-with-chatgpt](https://github.com/BeforeWave/dsh-with-chatgpt) | 32 | 2026-08-21 | 2026-08-24 | Bring ChatGPT’s reasoning to your local codebase. Work directly, or delegate larger tasks to DSH. |
| 34 | [Rain-kl/dsh-preset-plus](https://github.com/Rain-kl/dsh-preset-plus) | 32 | 2026-08-24 | 2026-08-24 | DSH 预设编辑器插件, 支持一键破甲. |
| 35 | [HiWhaleW/dsh-toolbox](https://github.com/HiWhaleW/dsh-toolbox) | 29 | 2026-08-13 | 2026-08-25 | Local-first DeepSeek Harness plugins for product research, context routing, plugin preflight, and compatibility monitoring. |
| 36 | [ARFCON/dsh-hotplug-hub](https://github.com/ARFCON/dsh-hotplug-hub) | 26 | 2026-08-19 | 2026-08-22 | DSH - Dseam |
| 37 | [SLin-code/dsh-custom-skin](https://github.com/SLin-code/dsh-custom-skin) | 25 | 2026-08-24 | 2026-08-24 | DSH自定义壁纸/皮肤插件——Custom wallpapers and translucent skins for DeepSeek Harness Web |
| 38 | [fandc520/dsh-comfyui](https://github.com/fandc520/dsh-comfyui) | 24 | 2026-08-20 | 2026-08-22 | 一个基于DeepSeek-Harness的ComfyUI插件 |
| 39 | [10086ggqq/dsh_theme_terraria](https://github.com/10086ggqq/dsh_theme_terraria) | 23 | 2026-08-22 | 2026-08-23 | 把 DeepSeek Harness 的 AI 编码控制台变成泰拉瑞亚像素世界——向导陪你写代码，真实对话、工具审批、难度切换，单文件零依赖。 |
| 40 | [ZSeven-W/dsh-harbor](https://github.com/ZSeven-W/dsh-harbor) | 23 | 2026-08-22 | 2026-08-25 | DeepSeek Harness (DSH) plugin: a read-only ledger for the plugins you already have installed — a capability inventory with file:line evidence, declared-vs-detected reconciliation, cross-profile version drift, and a diff of what changed since the last scan. |
| 41 | [KelaoHu/dsh-lowtide](https://github.com/KelaoHu/dsh-lowtide) | 21 | 2026-08-23 | 2026-08-24 | Time-shifting task delegation for DeepSeek Harness (dsh): plan tasks at leisure, they run unattended off-peak, come back to a report. Human-adjudicated, desktop + web. |
| 42 | [baihejiangnan/deepseek-harness-desktop](https://github.com/baihejiangnan/deepseek-harness-desktop) | 19 | 2026-08-21 | 2026-08-23 | DeepSeek Harness 三端兼容桌面启动器：多实例完全隔离、并行协作，协作画布编排 Agent 工作流；便携版 Exe 一键启动、仅约 18M（不超过 20M）；双隔离机制让兼容性极强，无论 DSH 本体如何更新，兼容原生到野生狗奶。 |
| 43 | [Clarklevis1995/dsh-mobile](https://github.com/Clarklevis1995/dsh-mobile) | 19 | 2026-08-17 | 2026-08-23 | DeepSeek Harness Mobile 是一个面向 DeepSeek Harness 的原生 iOS 客户端。它通过 dsh-plugin-mobile-gateway 与 Harness 建立 WebSocket 连接，将工作区、会话、实时回复和 Agent 执行轨迹带到 iPhone，同时延续 DeepSeek WebUI 克制、清晰的视觉语言 |
| 44 | [cofy-x/dsh-console](https://github.com/cofy-x/dsh-console) | 19 | 2026-08-24 | 2026-08-24 | A TypeScript and React/Ink terminal frontend for DeepSeek Harness. |
| 45 | [plolpl789/dsh-raw-html](https://github.com/plolpl789/dsh-raw-html) | 19 | 2026-08-21 | 2026-08-24 | VCP visual-synesthesia protocol plugin for DeepSeek Harness: render agent HTML output as real UI (cards / KaTeX math / Mermaid diagrams / built-in calligraphy fonts / zero-JS interactions), plug-and-play on any DSH environment |
| 46 | [lizhiyao/oh-my-knowledge](https://github.com/lizhiyao/oh-my-knowledge) | 18 | 2026-03-24 | 2026-08-24 | OMK — Evidence-backed evaluation and observability for prompts, RAG, skills, agents, and workflows. Native Codex, Claude Code, and DeepSeek Harness support. |
| 47 | [omdsh-dev/stent](https://github.com/omdsh-dev/stent) | 18 | 2026-08-06 | 2026-08-22 | 灵感来源于MC Fabric的Cordis/DSH hook处理器 |
| 48 | [chumingjun/harness-one](https://github.com/chumingjun/harness-one) | 15 | 2026-08-20 | 2026-08-24 | Visual AI workflow orchestrator for DeepSeek Harness (dsh): multi-agent DAGs, live execution, recovery, and Feishu integration. |
| 49 | [klarkxy/zhihu-search](https://github.com/klarkxy/zhihu-search) | 15 | 2026-06-17 | 2026-08-23 | DeepSeek Harness plugin, Skill, CLI and MCP for Zhihu search, Zhida ask, and official open-platform APIs |
| 50 | [398894496-arch/runtime36](https://github.com/398894496-arch/runtime36) | 13 | 2026-08-21 | 2026-08-22 | Second brain for coding agents. Seal the day, distill into Obsidian, hit that page tomorrow. Cursor, Codex, Claude Code, DeepSeek Harness. |
| 51 | [TiantianFlow/dsh-one-gateway](https://github.com/TiantianFlow/dsh-one-gateway) | 13 | 2026-08-16 | 2026-08-22 | Private DSH One Gateway — loopback, identity-first ingress for DeepSeek Harness |
| 52 | [dsh-blue/blue](https://github.com/dsh-blue/blue) | 12 | 2026-08-18 | 2026-08-22 | Blue: a TUI is not a package, it is a Cordis plugin tree — a modern terminal UI for DeepSeek Harness with hot-swappable render, interaction, and command plugins. |
| 53 | [Minglink/DeepSeek-Harness-Hub](https://github.com/Minglink/DeepSeek-Harness-Hub) | 12 | 2026-08-24 | 2026-08-25 | 🌐 DeepSeek 官方与开源生态插件市场 (deepseek.stream) 使用指南与一键安装协议规范 |
| 54 | [NekroAI/nekro-nxt](https://github.com/NekroAI/nekro-nxt) | 12 | 2026-08-15 | 2026-08-26 | NekroNXT：基于 DeepSeek Harness（DSH）的多平台群聊智能体系统｜A DSH-powered multi-platform group-chat agent system |
| 55 | [havingautism/dsh-deepresearch](https://github.com/havingautism/dsh-deepresearch) | 11 | 2026-08-12 | 2026-08-22 | @deepseek-ai/dsh-deepresearch 把证据优先的 Codemini 研究工作区带到 DSH。它提供持久工作流状态、模型工具、生成的 deepResearch Remote namespace 和“深度研究”Web 工作区，同时组合宿主已有的 Web 与 subagent 能力。 |
| 56 | [sqs404/dsh-portable](https://github.com/sqs404/dsh-portable) | 11 | 2026-08-16 | 2026-08-23 | DeepSeek Harness 免安装便携版（Windows）：官方 npm 包 + 内置 Node.js，双击 exe 即用，拷贝到任意 64 位 Windows 电脑独立运行 |
| 57 | [TsFreddie/dsh-compaction-instant](https://github.com/TsFreddie/dsh-compaction-instant) | 11 | 2026-08-14 | 2026-08-22 | LLM-free lossless* compaction engine for DeepSeek Harness |
| 58 | [daha1216/dsh-adult-tension](https://github.com/daha1216/dsh-adult-tension) | 10 | 2026-08-19 | 2026-08-24 | DeepSeek Harness 成年人(18+/adult)互动叙事 Skill：NPC 活人感（有记忆/立场/底线）、自带破甲、数百项素材库、随机开局可预锁、时间推进、全维 YAML 存档。 |
| 59 | [daha1216/dsh-plugin-collection](https://github.com/daha1216/dsh-plugin-collection) | 10 | 2026-08-19 | 2026-08-22 | DeepSeek Harness（DSH）第三方插件精选目录：一键安装，条目均指向插件作者原仓库。 |
| 60 | [fishzjp/qa-skills](https://github.com/fishzjp/qa-skills) | 10 | 2026-06-24 | 2026-08-24 | 让 AI 像资深测试工程师一样工作：全生命周期 QA Agent Skills 框架——方法论 + 10 Skills + 可复现 Benchmark（Claude Code 等 Agent 可用） |
| 61 | [Leon0555/dsh-lan-access](https://github.com/Leon0555/dsh-lan-access) | 10 | 2026-08-14 | 2026-08-24 | 一个DSH局域网内访问插件：让 DeepSeek Harness 可在局域网内被其他设备访问的 DSH 插件。同一局域网下，手机/平板/电脑打开浏览器即可直接访问你某台设备上的 DSH——无需 SSH、无需内网穿透，npm 一键安装。 |
| 62 | [Physicolor/dsh-ui-harmonizer](https://github.com/Physicolor/dsh-ui-harmonizer) | 10 | 2026-08-15 | 2026-08-22 | Web UI polish layer for DeepSeek Harness: normalizes unfinished or self-contradictory official UI, reconciles style conflicts between installed plugins, and unifies the visual language via official design tokens. |
| 63 | [qkycir-123/dsh-run2skill](https://github.com/qkycir-123/dsh-run2skill) | 10 | 2026-08-19 | 2026-08-22 | Automatically turn successful DeepSeek Harness sessions into reusable, reviewable Agent Skills. |
| 64 | [Angel2518975237/deepseek-harness-hello-kitty-suite](https://github.com/Angel2518975237/deepseek-harness-hello-kitty-suite) | 9 | 2026-08-23 | 2026-08-23 | 💗 一套给 DeepSeek Harness 的粉色 Hello Kitty 主题皮肤 + 任务完成/提问提醒插件（Sweetheart Workspace Expressive skin & Hello Kitty Task-Done Notifier） |
| 65 | [dabaicai001/star-dsh-desktop](https://github.com/dabaicai001/star-dsh-desktop) | 9 | 2026-06-04 | 2026-08-25 | StarHub 是一款跨平台桌面应用（Tauri 2 + Rust 主进程 + DeepSeek Harness React 工作台 + Go Sidecar），把开发运维日常高频工具整合到同一个窗口 —— 数据库、SSH/SFTP、Docker 面板与 AI 助手。目标是减少在 Navicat、Xshell、Portainer、文件管理器和 AI 对话窗口之间来回切换的成本。  前端架构：基于 DeepSeek Harness 原生 React 工作台（/starhub-react 路由）。资产、设置、SSH 终端、SFTP、数据库 |
| 66 | [lna-lab/distill-kura](https://github.com/lna-lab/distill-kura) | 9 | 2026-08-21 | 2026-08-22 | 蒸留蔵 — distilled long-term memory for agents: recall by meaning, writing gated by evidence, one kura per agent mode. Ships as a DeepSeek Harness plugin and an MCP server. |
| 67 | [yinhcao/yinchao-ai-music-skill](https://github.com/yinhcao/yinchao-ai-music-skill) | 9 | 2026-08-20 | 2026-08-24 | AI 音乐生成 Agent Skill：支持文字/歌词生成歌曲、参考音频创作、BGM 与歌曲续写 |
| 68 | [AngelosZou/dsh-multi-folder](https://github.com/AngelosZou/dsh-multi-folder) | 8 | 2026-08-14 | 2026-08-25 | Secondary working directories for a DeepSeek Harness project — edit a source repo, a test repo, and a docs repo side by side without leaving the primary workspace. |
| 69 | [liustack/pptwise](https://github.com/liustack/pptwise) | 8 | 2026-07-16 | 2026-08-23 | A real PowerPoint, not a picture or HTML. Tell your AI what to cover and pptwise builds an editable deck on your own machine. Agent skill + DSH plugin, no account and no API key to render. \| 真正的 PPT，不是图片也不是 HTML。跟 AI 说要讲什么，pptwise 在你自己电脑上做出一份能改的 PPT。Agent skill + DSH 插件，不用注册，渲染不用 API key。 |
| 70 | [LoserFox/marisa-distro](https://github.com/LoserFox/marisa-distro) | 8 | 2026-08-13 | 2026-08-25 | 魔理沙 DSH 整合包发行：29 插件 + 一键安装 + profile 直装 |
| 71 | [AngelosZou/graphlint](https://github.com/AngelosZou/graphlint) | 7 | 2026-07-01 | 2026-08-26 | Dead-code detection for AI-generated codebases: graphlint builds a dependency graph, finds code unreachable from any entry point to enable codebase cleanup and functional‑effectiveness understanding. |
| 72 | [getpapi/papi](https://github.com/getpapi/papi) | 7 | 2026-06-12 | 2026-08-22 | Your AI starts every session from zero. Your project stays on course. Structured plan, build and review cycles for any MCP-capable AI coding tool. |
| 73 | [riesbri/dshline](https://github.com/riesbri/dshline) | 7 | 2026-08-17 | 2026-08-23 | The terminal-native frontend for the DeepSeek Harness plugin ecosystem. |
| 74 | [artec/clat](https://github.com/artec/clat) | 6 | 2025-12-07 | 2026-08-23 | Cmd-Line Agent, a Rust foundation compatible with the DeepSeek Harness framework. 命令行智能体，兼容深度探索驾具的 Rust 基座。 |
| 75 | [Chinesezjc/dsh-tool-todo-tree](https://github.com/Chinesezjc/dsh-tool-todo-tree) | 6 | 2026-08-13 | 2026-08-24 | Nested (tree-shaped) todo_write tool plugin for DeepSeek Harness (DSH) — the mutually-exclusive alternative to the flat dsh-tool-todo |
| 76 | [Elave-66/dsh-blue-sea-launcher](https://github.com/Elave-66/dsh-blue-sea-launcher) | 6 | 2026-08-21 | 2026-08-22 | Deepseek 二次元游戏/Galgame 风格启动图标。鲸鱼娘形象来源bilibili@上善无形 @ZipZipPipe，适合重度二次元使用，配合鲸鱼娘皮肤等二次元插件使用更佳！ |
| 77 | [hoyyang/dsh-mall](https://github.com/hoyyang/dsh-mall) | 6 | 2026-08-25 | 2026-08-25 | 全网最强 DeepSeek Harness 插件商场：全量收录 GitHub #dsh-plugin 生态插件，五维实用评分雷达图，智能搜索（AI 理解需求）、智能安装/更新/卸载（AI 装前审查+装后诊断）、一键批量更新、编辑精选与个性化推荐，自带 Skills 工具与 dsh-mall 技能，中英多语言界面。 |
| 78 | [IceApriler/dsh-remote-mobile](https://github.com/IceApriler/dsh-remote-mobile) | 6 | 2026-08-21 | 2026-08-23 | DeepSeek Harness 远程与移动端安全网关插件：零修改 DSH 底层代码安全开放局域网与 Tailscale 连接 \| DeepSeek Harness (DSH) Remote & Mobile Security Guard: safely opens Tailscale/LAN with zero core modifications, QR scan auth, RSA encryption & brute-force defense. |
| 79 | [liang-today/dsh-liangxiang](https://github.com/liang-today/dsh-liangxiang) | 6 | 2026-08-15 | 2026-08-23 | 众香成势，梁子显相。DeepSeek Harness 的 WebUI 插件，欢迎一起打梁。 |
| 80 | [sensedeal/cue-skills](https://github.com/sensedeal/cue-skills) | 6 | 2026-05-20 | 2026-08-24 | Cue Skills for Agents |
| 81 | [suntianc/dsh-antigravity-auth](https://github.com/suntianc/dsh-antigravity-auth) | 6 | 2026-08-21 | 2026-08-22 | DeepSeek Harness plugin for Antigravity OAuth login and native Antigravity Auth capability bundle |
| 82 | [tma1-ai/dsh-otel](https://github.com/tma1-ai/dsh-otel) | 6 | 2026-08-25 | 2026-08-25 | OpenTelemetry traces, metrics, and logs for DeepSeek Harness, written straight into GreptimeDB |
| 83 | [zzhang82/Agent-Memory-Bridge](https://github.com/zzhang82/Agent-Memory-Bridge) | 6 | 2026-04-05 | 2026-08-23 | Persistent engineering memory for coding agents over MCP. |
| 84 | [chenzheshushi-commits/dsh-evolve](https://github.com/chenzheshushi-commits/dsh-evolve) | 5 | 2026-08-23 | 2026-08-23 | Self-evolving memory + skill lifecycle for DeepSeek Harness — durable cross-session memory with zero-token deterministic recall, tiered approval, reinforcement learning from repetition, and anti-bloat convergence for both skills and memory. |
| 85 | [EachSheep/dsh-mario-pixel-skin](https://github.com/EachSheep/dsh-mario-pixel-skin) | 5 | 2026-08-16 | 2026-08-23 | Unofficial Mario-inspired pixel-adventure skin for DeepSeek Harness. |
| 86 | [fuzhengwei/walioffice-dsh-plugin](https://github.com/fuzhengwei/walioffice-dsh-plugin) | 5 | 2026-08-19 | 2026-08-22 | Deepseek Harness Walioffice 办公软件 插件 |
| 87 | [lo2589/deepseek-harness-media](https://github.com/lo2589/deepseek-harness-media) | 5 | 2026-08-14 | 2026-08-24 | use glm/minimax/openai/claude api in your deepseek harness |
| 88 | [monotykamary/dsh-factory](https://github.com/monotykamary/dsh-factory) | 5 | 2026-08-23 | 2026-08-24 | Durable dependency-graph task factory for DeepSeek Harness: recurring Agent work, safe checkout lanes, first-class queues, Triage, and artifacts. |
| 89 | [newborne/dsh-adb-ultimate](https://github.com/newborne/dsh-adb-ultimate) | 5 | 2026-08-19 | 2026-08-25 | Full-featured ADB device management plugin for DeepSeek Harness - control your Android device via AI |
| 90 | [PensiveFei/dsh-voice-scribe](https://github.com/PensiveFei/dsh-voice-scribe) | 5 | 2026-08-25 | 2026-08-25 | DSH voice input plugin: tap Alt to talk, get text in composer. Web Speech default (zero config), optional OpenAI-compatible ASR, polish via DSH LLM. |
| 91 | [Physicolor/dsh-widgets](https://github.com/Physicolor/dsh-widgets) | 5 | 2026-08-15 | 2026-08-22 | Right-hand widget rail for DeepSeek Harness Web UI: live session stats (turns, LLM/tool time, TTFT, speed, cache, tokens) plus OpenCode Go quota via a same-origin host proxy; extensible widget registry. |
| 92 | [sheep-programmer/dsh-web-search-free](https://github.com/sheep-programmer/dsh-web-search-free) | 5 | 2026-08-22 | 2026-08-22 | DSH 插件：免费网页搜索，双免费后端（Parallel 默认 + Exa 备用，均匿名免 key）+ 设置开关 + MCP server 双传输（stdio + HTTP/SSE 双端口），兼容 Claude Code / Codex \| Free web search for DeepSeek Harness: Parallel (default) + Exa (backup) free providers, settings toggle, and dual-transport MCP server (stdio + HTTP/SSE) for Claude Code / Codex |
| 93 | [Wenaixi/dsh-superpower](https://github.com/Wenaixi/dsh-superpower) | 5 | 2026-08-21 | 2026-08-22 | DSH port of obra/superpowers — 完整移植、中文化、DSH 原生 |
| 94 | [xinchen03/minta](https://github.com/xinchen03/minta) | 5 | 2026-05-31 | 2026-08-23 | The context quality layer for AI agents — memory that checks itself: lifecycle governance, calibrated confidence, and   staged claim gates. Local-first, MCP 19 tools, DeepSeek Harness plugin. |
| 95 | [yyyy231209/ai-company-framework](https://github.com/yyyy231209/ai-company-framework) | 5 | 2026-08-18 | 2026-08-24 | Company Is a Word. 一句话开一家AI公司 - open-source multi-agent orchestration framework for non-developers. 小白5分钟拥有自己的AI公司，可DIY任意行业、调教子Agent、无限家公司，支持飞书遥控。MIT |
| 96 | [zmh2000829/DSH-agent-bridge](https://github.com/zmh2000829/DSH-agent-bridge) | 5 | 2026-08-23 | 2026-08-23 | Use Grok Build inside DeepSeek Harness Web through ACP |
| 97 | [zrk222/code-factory](https://github.com/zrk222/code-factory) | 5 | 2026-07-08 | 2026-08-22 | Catch AI-generated tests that could never fail; wrap agent changes in local proof and evidence. Free core; proposed evidence-gated enterprise support SLA. |
| 98 | [azwosile/dsh-highres-vision](https://github.com/azwosile/dsh-highres-vision) | 4 | 2026-08-24 | 2026-08-25 | 专供 deepseek-v4-flash-vision-exp 的高清识图增强插件：放宽 DSH 图片限制 + highres_read 分块识图工具。 |
| 99 | [Cerbur/clutch-dsh](https://github.com/Cerbur/clutch-dsh) | 4 | 2026-08-19 | 2026-08-22 | Open-source DSH plugins for DeepSeek Harness, clutch-dsh-worktree. |
| 100 | [chipweaver/veripower](https://github.com/chipweaver/veripower) | 4 | 2026-06-11 | 2026-08-25 | An open-source agent flow from natural language spec through Verilog RTL and UVM verification to front-end signoff on commercial EDA tools |
| 101 | [Decrabbityyy/dsh-discovery](https://github.com/Decrabbityyy/dsh-discovery) | 4 | 2026-08-19 | 2026-08-23 | DeepSeek Harness model discovery plugins for local engines and API gateways |
| 102 | [Hilbert-beinghappy/dsh-plugin-clarify](https://github.com/Hilbert-beinghappy/dsh-plugin-clarify) | 4 | 2026-08-20 | 2026-08-22 | Off-transcript clarification Host plugin for DeepSeek Harness |
| 103 | [IcyCreamDAS/shidi-skill](https://github.com/IcyCreamDAS/shidi-skill) | 4 | 2026-08-03 | 2026-08-23 | AI4S 科研 Agent 技能 \| AI-for-Science research workflow skill for coding agents: literature review · experiment design · figures · paper reading — files out, cross-verified, zero deps \| 文献调研/实验方案/作图/精读，交付文件+交叉验证，零依赖，MIT |
| 104 | [Innocent-children/dev-flow](https://github.com/Innocent-children/dev-flow) | 4 | 2026-08-14 | 2026-08-22 | Local process control and recovery for Codex and DeepSeek Harness: explicit scope, verification budgets, and durable task state. |
| 105 | [JasonWei04/dsh-computer-use](https://github.com/JasonWei04/dsh-computer-use) | 4 | 2026-08-18 | 2026-08-22 | computer-use in dsh |
| 106 | [louke6572/dsh-whale-widget-plus](https://github.com/louke6572/dsh-whale-widget-plus) | 4 | 2026-08-25 | 2026-08-25 | 基于DeepSeek-Balance-Whale-Widget开发，新增了两版不同的表情，需要那个版本的表情可以自己让agent帮你换，增加了火山coding plan额度查询，新增加台词自定义切换增加，增加了表情与台词手动切换 |
| 107 | [lxfu1/dsh-plugin-chart](https://github.com/lxfu1/dsh-plugin-chart) | 4 | 2026-08-21 | 2026-08-24 | DeepSeek Harness plugin that bundles the AntV chart visualization skill and a native chart-generation tool. |
| 108 | [Max-Null/dsh-chinese-thinking](https://github.com/Max-Null/dsh-chinese-thinking) | 4 | 2026-08-15 | 2026-08-25 | One-line fix: inject a fixed system-prompt section so the agent always thinks and replies in Chinese, whatever the user's language · 中文思考：注入固定提示词，让 agent 始终用中文思考与回复（无论用户语言） |
| 109 | [nisconder/npm-safe-forDSH](https://github.com/nisconder/npm-safe-forDSH) | 4 | 2026-08-19 | 2026-08-23 | 本地优先的 npm 包供应链安全扫描引擎，deepseek harness 插件版本 |
| 110 | [NOirBRight/dsh-mobile](https://github.com/NOirBRight/dsh-mobile) | 4 | 2026-08-15 | 2026-08-24 | Android client and Host pairing plugin for DeepSeek Harness |
| 111 | [Nono-neko/dsh-browser](https://github.com/Nono-neko/dsh-browser) | 4 | 2026-08-21 | 2026-08-23 | Cordis bundle plugin for DeepSeek Harness(DSH). Built‑in multi‑tab browser powered by Puppeteer, provides browser_open/browser_read agent tools & workspace file preview inside DSH Web GUI. |
| 112 | [Ottohere-Mourn/TeachReplay](https://github.com/Ottohere-Mourn/TeachReplay) | 4 | 2026-08-22 | 2026-08-22 | Teach once, replay anywhere — harness-agnostic Teach-by-Demonstration engine (Record → Compile → Replay → Verify) with OpenMausBot and DeepSeek Harness integrations. |
| 113 | [Shrbuz/dsh-session-buddy](https://github.com/Shrbuz/dsh-session-buddy) | 4 | 2026-08-23 | 2026-08-23 | DeepSeek Harness 插件：回复/提问/审批三类会话通知（系统原生 toast）+ 会话内梯子目录导航。DeepSeek Harness plugin: session notifications (reply/ask/approval) with native OS toasts + an in-conversation ladder outline. |
| 114 | [staff-os/dsh-workbench](https://github.com/staff-os/dsh-workbench) | 4 | 2026-08-22 | 2026-08-25 | An enterprise workbench for the DeepSeek Harness: AI employees, knowledge bases, skills, MCP servers and DSH plugins, all manageable from a running session. |
| 115 | [tdyangbo/PianpianUI](https://github.com/tdyangbo/PianpianUI) | 4 | 2026-08-23 | 2026-08-23 | 用于DeepSeek Harness的林翩翩主题UI插件。使用《哀鸿：城破十日记》的角色林翩翩作为页面半透明背景，并支持透明度和深度调节。 |
| 116 | [Tianbuyu-wwx/DSH-FormatForge](https://github.com/Tianbuyu-wwx/DSH-FormatForge) | 4 | 2026-06-10 | 2026-08-25 | FormatForge — DeepSeek Harness plugin: drag any file (PDF/DOCX/XLSX/EML…, 30+ formats) into dsh and it becomes AI-readable structured data. npm: @tianbuyu-wwx/dsh-formatforge |
| 117 | [Wenaixi/dsh-ponytail](https://github.com/Wenaixi/dsh-ponytail) | 4 | 2026-08-21 | 2026-08-22 | DSH 完整移植版 DietrichGebert/ponytail — 懒惰 senior 模式，hook注入 |
| 118 | [wuliLiuyue/wxpilot](https://github.com/wuliLiuyue/wxpilot) | 4 | 2026-03-24 | 2026-08-22 | wxpilot — A CLI for automating WeChat Mini Programs, built for AI Agents. Lets an Agent drive the WeChat DevTools like a browser — page navigation, element interaction, state reading, network capture & mocking.  面向 AI Agent 的微信小程序自动化 CLI 让 Agent 像操作浏览器一样操作微信开发者工具——页面导航、元素交互、状态读取、网络抓包与 mock。 |
| 119 | [xxccdl/deepseek-harness-desktop](https://github.com/xxccdl/deepseek-harness-desktop) | 4 | 2026-08-15 | 2026-08-22 | DeepSeek Harness 桌面版 — Electron 壳层封装 dsh web，集成记忆查看、电脑控制、桌面设置、定时任务、快捷对话、预算血条等桌面插件。DeepSeek Harness Desktop — Electron shell wrapping dsh web with desktop-only plugins: memory viewer, computer use, desktop settings, scheduler, quick chat, and usage bar. |
| 120 | [z-col/dsh-workspace-groups](https://github.com/z-col/dsh-workspace-groups) | 4 | 2026-08-21 | 2026-08-22 | DeepSeek Harness web client plugin: group sidebar workspaces into a configurable three-level tree (分类→项目→会话). Sidecar YAML rules. dsh-plugin. |
| 121 | [zhouzhencheng07/dsh-kit](https://github.com/zhouzhencheng07/dsh-kit) | 4 | 2026-08-13 | 2026-08-23 | Free keyless Tavily web search tool for DeepSeek Harness (dsh) |
| 122 | [zp-home/dsh-weixin-clawbot](https://github.com/zp-home/dsh-weixin-clawbot) | 4 | 2026-08-21 | 2026-08-22 | Phone-to-DSH control through Tencent's official Weixin ClawBot/iLink channel \| 基于腾讯官方微信 ClawBot/iLink 的 DSH 手机远程控制插件 |
| 123 | [1014029855/dsh-context-lens](https://github.com/1014029855/dsh-context-lens) | 3 | 2026-08-23 | 2026-08-23 | Inspect, measure, search, and compare the exact provider-neutral context assembled by DeepSeek Harness. |
| 124 | [aa2246740/dsh-watcher](https://github.com/aa2246740/dsh-watcher) | 3 | 2026-08-20 | 2026-08-25 | Read-only Agent work-path observer for DeepSeek Harness |
| 125 | [AgentsDanceAI/deepseek-harness-cloud](https://github.com/AgentsDanceAI/deepseek-harness-cloud) | 3 | 2026-08-21 | 2026-08-22 | Accounts, credits and cloud agent workspaces for DeepSeek Harness — run it as a hosted product, or self-host in 5 minutes. |
| 126 | [ai4paper/apaper-plugin](https://github.com/ai4paper/apaper-plugin) | 3 | 2026-05-15 | 2026-08-24 | Claude Code plugin for academic paper authoring: bundles writing/figure/PDF skills with the apaper-mcp server. |
| 127 | [AlexKaiqi/dsh-multi-model-provider](https://github.com/AlexKaiqi/dsh-multi-model-provider) | 3 | 2026-08-17 | 2026-08-24 | Model catalog, portraits, Agent selection, and multimodal runtimes for DeepSeek Harness |
| 128 | [AlexPeng07/dsh-custom-plugin](https://github.com/AlexPeng07/dsh-custom-plugin) | 3 | 2026-08-22 | 2026-08-23 | dsh-custom-plugin是一个为 DeepSeek Harness (DSH) Web GUI 打造的增强插件。提供：背景天气特效/玻璃拟态、时间线轨道、项目文件夹、提示词库、对话导出、Mermaid 图表渲染、引用回复、余额查询与每日 Token 用量面板等多种便利功能 |
| 129 | [AngelosZou/dsh-python-env](https://github.com/AngelosZou/dsh-python-env) | 3 | 2026-08-16 | 2026-08-25 | Workspace-scoped Python virtual environment management for a DeepSeek Harness project — discover, create, install into, and remove virtual environments without sandbox, network, or subprocess pitfalls. |
| 130 | [AQian0/dsh-desktop](https://github.com/AQian0/dsh-desktop) | 3 | 2026-08-14 | 2026-08-23 | 基于Tauri的简易dsh桌面端套壳 \| A simple Tauri-based desktop wrapper for dsh |
| 131 | [Azzygoatcoder/agent-useful-skills](https://github.com/Azzygoatcoder/agent-useful-skills) | 3 | 2026-06-17 | 2026-08-24 | 模块化 AI 科研/工程技能 monorepo（DeepSeek Harness / Claude Code 通用）— plugins/ + skills/ + bin 脚本 + LaTeX 模板，验证环驱动 |
| 132 | [baihui-ai/a2ui-render-in-dsh](https://github.com/baihui-ai/a2ui-render-in-dsh) | 3 | 2026-08-24 | 2026-08-25 | Interactive A2UI cards for the dsh web UI — quizzes, forms, charts and diagrams rendered inline in the conversation, with a full action loop back to the agent. |
| 133 | [CaiZongyuan/dsh-ag-ui](https://github.com/CaiZongyuan/dsh-ag-ui) | 3 | 2026-08-23 | 2026-08-23 | AG-UI protocol gateway plugin for DeepSeek Harness |
| 134 | [chidaic/dsh-light-memory](https://github.com/chidaic/dsh-light-memory) | 3 | 2026-08-23 | 2026-08-23 | 轻量记忆系统插件：四个 Markdown 文件（USER/PROJECT/WORKLOG/CONVENTION）+ append/distill 两个动作，零外部部件，prefix-cache 友好 |
| 135 | [clclyzybzjsq/deepseek-harness-yunoseek](https://github.com/clclyzybzjsq/deepseek-harness-yunoseek) | 3 | 2026-08-23 | 2026-08-23 | 一个基于tv动画yumemita中的人物千石由乃，使用剧照素材，应用于deepseek-harness的自定义配色插件；A custom color scheme plugin for deepseek-harness, based on the character Yuno Sengoku from the TV anime "Yumemita" |
| 136 | [CREAIT-nl/dsh-plugins](https://github.com/CREAIT-nl/dsh-plugins) | 3 | 2026-08-22 | 2026-08-23 | Plugins for DeepSeek Harness: deep research as an agent preset, per-model generation limits, Claude Code hook compatibility, and web fetch/search tools. |
| 137 | [CWNU-Open-Source-Community/dsh-webgate](https://github.com/CWNU-Open-Source-Community/dsh-webgate) | 3 | 2026-08-16 | 2026-08-22 | DSH 远程访问插件：内网二维码 / cloudflared 隧道 / frp+自有服务器（含登录门户） |
| 138 | [ddtcorex/maestro-skills](https://github.com/ddtcorex/maestro-skills) | 3 | 2026-05-25 | 2026-08-22 | Universal AI Agent Development Skills Hub & Cordis Plugin for Govard, Magento 2, Laravel. Works with Claude Code, Codex CLI, OpenCode, GitHub Copilot, DeepSeek Harness. |
| 139 | [dushaobindoudou/dsh-freeroute](https://github.com/dushaobindoudou/dsh-freeroute) | 3 | 2026-08-21 | 2026-08-26 | dsh free token route |
| 140 | [EasyTZ/Deepseek-Harness-Desktop](https://github.com/EasyTZ/Deepseek-Harness-Desktop) | 3 | 2026-08-20 | 2026-08-24 | Deepseek-Harness-Desktop |
| 141 | [edge-sky/dsh-oauth-adapter](https://github.com/edge-sky/dsh-oauth-adapter) | 3 | 2026-08-22 | 2026-08-24 | A OAuth adapter for DSH |
| 142 | [f20880479-lab/dsh-peak-gate](https://github.com/f20880479-lab/dsh-peak-gate) | 3 | 2026-08-25 | 2026-08-25 | DeepSeek Harness 峰谷计费插件：高峰时段发送前确认（可勾选本次高峰段内不再提示），支持将消息排队到空闲时段（半价）自动发送；可拖拽悬浮队列窗口、调整发送顺序与时间。 |
| 143 | [fashionmascherine-svg/dsh-polymarket-knowhow](https://github.com/fashionmascherine-svg/dsh-polymarket-knowhow) | 3 | 2026-08-22 | 2026-08-23 | DeepSeek Harness plugin (dsh-plugin): complete Polymarket superpowers — 31 verified tools across Gamma/CLOB/Data-API/Perps/RFQ/Bridge, embedded knowhow skill, live WebSocket stream. Read-only by default. |
| 144 | [FuqiangCraft/dsh-desktop](https://github.com/FuqiangCraft/dsh-desktop) | 3 | 2026-08-24 | 2026-08-24 | Desktop companion plugin and native shell for DeepSeek Harness (DSH) |
| 145 | [fxylabs/superself](https://github.com/fxylabs/superself) | 3 | 2026-07-23 | 2026-08-23 | The open Company State Runtime — version control for your project's state. Goals, decisions, work, and evidence outlive every chat, context window, and agent session. Ships the self CLI. |
| 146 | [hanxuanliang/dsh-chaos](https://github.com/hanxuanliang/dsh-chaos) | 3 | 2026-08-15 | 2026-08-23 | Durable multi-agent collaboration for DeepSeek Harness: channels, threads, tasks, and resumable agent sessions. |
| 147 | [Hilbert-beinghappy/dsh-plugin-auxiliary-runtime](https://github.com/Hilbert-beinghappy/dsh-plugin-auxiliary-runtime) | 3 | 2026-08-21 | 2026-08-22 | Auxiliary inference usage, limits, and cancellation runtime for official DeepSeek Harness plugins |
| 148 | [huyang218/dsh-desktop](https://github.com/huyang218/dsh-desktop) | 3 | 2026-08-17 | 2026-08-23 | Unofficial macOS/Windows desktop app for DeepSeek Harness (dsh): manages the runtime, supervises the server, and puts the web UI in a real window. |
| 149 | [Jarad-z/dsh-goalmesh](https://github.com/Jarad-z/dsh-goalmesh) | 3 | 2026-08-23 | 2026-08-24 | Goal-driven multi-agent orchestration for DeepSeek Harness — bounded DAG scheduling, nested delegation, typed evidence, and durable trajectory UI. |
| 150 | [Jason-skd/dsh-session-fork](https://github.com/Jason-skd/dsh-session-fork) | 3 | 2026-08-20 | 2026-08-22 | Makes the branch the building block of AI conversation management — parallel workflows, continuous and mergeable conversation memory |
| 151 | [KannaKuron/dsh-gitbash-shell](https://github.com/KannaKuron/dsh-gitbash-shell) | 3 | 2026-08-23 | 2026-08-23 | DSH plugin: Git Bash shell for all agent modes on Windows (replaces pwsh executor) |
| 152 | [Lukeknow0/dsh-side-chat](https://github.com/Lukeknow0/dsh-side-chat) | 3 | 2026-08-21 | 2026-08-24 | Read-only side chat plugin for DeepSeek Harness (DSH) — ask temporary questions with inherited context while the parent agent keeps running. |
| 153 | [mantonlove/dsh-prism-plugin](https://github.com/mantonlove/dsh-prism-plugin) | 3 | 2026-08-18 | 2026-08-26 | Prism · 棱镜 — a deeply customizable glassmorphism theme plugin for the DeepSeek Harness Web GUI |
| 154 | [Max-Null/dsh-memory](https://github.com/Max-Null/dsh-memory) | 3 | 2026-08-15 | 2026-08-25 | Cross-session plaintext memory for DeepSeek Harness: suggested → human-approved, searchable, human owns the data · 跨会话明文记忆：模型写入待审核、人工确认生效，明文可审计 |
| 155 | [maxwell-feng/dsh-searxng-web](https://github.com/maxwell-feng/dsh-searxng-web) | 3 | 2026-08-22 | 2026-08-23 | DeepSeek Harness plugin: back the native web_search / web_fetch tools with your self-hosted SearXNG instance — keyless, private, no third-party search vendor. |
| 156 | [megatronyy/dsh-tradingagents](https://github.com/megatronyy/dsh-tradingagents) | 3 | 2026-08-22 | 2026-08-22 | TradingAgents for DeepSeek Harness: the 14-role A-share multi-agent analysis pipeline behind /trading-agent |
| 157 | [MengYuil/dsh-ponytail](https://github.com/MengYuil/dsh-ponytail) | 3 | 2026-08-23 | 2026-08-23 | Lazy senior dev mode for DeepSeek Harness — ponytail port (always-on minimal-code ruleset, /ponytail-review/audit/debt/gain/help) |
| 158 | [modelbus/deepseek-harness-pro](https://github.com/modelbus/deepseek-harness-pro) | 3 | 2026-08-21 | 2026-08-23 | deepseek-harness-pro 是基于 deepseek-harness 的 Web+Electron 客户端，兼容已有的deepseek-harness环境，并支持一键部署最新版deepseek-harness。相比原web功能做出增强：新增实时任务看板、电脑管家（清理/调优/进程管理）、独立插件中心等功能。界面友好，跨平台，开源免费，让 deepseek-harness 更强大易用。 |
| 159 | [ParticleLight/dsh-browser-plus](https://github.com/ParticleLight/dsh-browser-plus) | 3 | 2026-08-21 | 2026-08-22 | Enhanced shared browser for DeepSeek Harness: visible + AI-driven WebContentsView, ego-style page chrome, operation trail, JS dialog auto-accept, per-task windows & spaces, Electron 42.x pinned |
| 160 | [PenguinAndy/dsh-ezcommit-plugin](https://github.com/PenguinAndy/dsh-ezcommit-plugin) | 3 | 2026-08-22 | 2026-08-22 | One-click Git commit plugin for DSH: the session model splits workspace changes into reviewed Conventional Commits batches, with built-in sensitive-file filtering. |
| 161 | [peterwangze/dsh-novel-writing](https://github.com/peterwangze/dsh-novel-writing) | 3 | 2026-08-21 | 2026-08-22 | DSH (DeepSeek Harness) 自动化小说写作发布流水线插件：claude-writing-workflow 迁移版 agent 预设 + 小说工作台（可视化/实时渲染/章节编辑）+ 多平台发布配置与数据驱动优化闭环 |
| 162 | [rayafriandion/dsh-oc-tui](https://github.com/rayafriandion/dsh-oc-tui) | 3 | 2026-08-15 | 2026-08-24 | The plugin can use terminal UI like opencode/claude code and other CLI/TUI agents. |
| 163 | [skymecode/dsh-deep-diving](https://github.com/skymecode/dsh-deep-diving) | 3 | 2026-08-20 | 2026-08-22 | plugin for dsh deep diving  |
| 164 | [SoMarkAI/dsh-tool-somark](https://github.com/SoMarkAI/dsh-tool-somark) | 3 | 2026-08-14 | 2026-08-24 | SoMark document parser tool (somark_parse) plugin for DeepSeek Harness |
| 165 | [soyoungzsy/soya-workflows](https://github.com/soyoungzsy/soya-workflows) | 3 | 2026-08-20 | 2026-08-21 | 🏭 SOYA Workflows — enterprise workflow skills for DeepSeek Harness: notify (webhook), docs (Yuque API), intel (RSS), report (daily/weekly/monthly).  企业工作流四件套 AI 技能。 |
| 166 | [SpookySandwich/dsh-plugin-message-edit](https://github.com/SpookySandwich/dsh-plugin-message-edit) | 3 | 2026-08-21 | 2026-08-22 | DSH 消息编辑插件：编辑已发送的消息并从该处分叉对话，气泡下方带版本计数与树状视图。Edit a sent message and branch from that point — version counter, tree view, placement presets. |
| 167 | [sqfcyily/dsh-workspace-files](https://github.com/sqfcyily/dsh-workspace-files) | 3 | 2026-08-25 | 2026-08-25 | 在DeepSeek Harness Web GUI 中浏览工作区的目录/文件，并结合 Git 显示文件改动。 |
| 168 | [ssheleg/task-pipeline](https://github.com/ssheleg/task-pipeline) | 3 | 2026-07-18 | 2026-08-26 | Full-cycle delivery orchestrator for AI coding agents: a mandatory intake grill that front-loads every decision, then ten gated stages — docs, brainstorm, decompose, spec, plan, build, tests, deploy, post-deploy, acceptance — with a loop guard that breaks churn. Loads in DeepSeek Harness (dsh). |
| 169 | [SSShooter/dsh-mindmap-live](https://github.com/SSShooter/dsh-mindmap-live) | 3 | 2026-08-23 | 2026-08-23 | DSH 实时思维导图插件：Agent 与你共编同一棵树，改动即时互相同步，支持停靠分屏与全屏专注两种视图 |
| 170 | [sunzhentao/dsh--prompt--enhance](https://github.com/sunzhentao/dsh--prompt--enhance) | 3 | 2026-08-24 | 2026-08-24 | DeepSeek Harness提示词增强插件 |
| 171 | [Tannnnhauser/pivot-web-search](https://github.com/Tannnnhauser/pivot-web-search) | 3 | 2026-05-02 | 2026-08-24 | Resilient multi-provider web search & content extraction for Claude Code, DeepSeek Harness, and any MCP host — quota-aware failover, JS rendering, and a CLI. |
| 172 | [Vesna-Strivozha/DSH-LLM-wiki-plugin](https://github.com/Vesna-Strivozha/DSH-LLM-wiki-plugin) | 3 | 2026-08-23 | 2026-08-23 | 基于Karpathy的wiki方法论搭建的插件，让你的DSH直接变身成LLM wiki，不需要Obsidian+Claudian插件，国内网络友好 |
| 173 | [vonweller/dsh-skillhub](https://github.com/vonweller/dsh-skillhub) | 3 | 2026-08-24 | 2026-08-24 | Browse skillhub.cn skills and install selected ones into ~/.dsh/skills |
| 174 | [whisperflo/dsh-deepseek-console](https://github.com/whisperflo/dsh-deepseek-console) | 3 | 2026-08-22 | 2026-08-22 | DeepSeek 账户控制台：实时余额监控 / 用量与成本统计 / 消费额度管理 / 全局悬浮 HUD（官方 API 直连，Key 仅存本机） |
| 175 | [Wike-CHI/dsh-mobile](https://github.com/Wike-CHI/dsh-mobile) | 3 | 2026-08-24 | 2026-08-24 | Mobile device capability plugin for DeepSeek Harness: MobileService seam, mock/mobile-mcp providers, agent tools (observe/open_app/tap/type/back), tiered execution policy |
| 176 | [WSL043/dsh-native-session-manager](https://github.com/WSL043/dsh-native-session-manager) | 3 | 2026-08-15 | 2026-08-22 | DSH Native Session Manager for DeepSeek Harness: search archived conversations, restore sessions, and safely delete chat history. |
| 177 | [xiangrui979/foresight](https://github.com/xiangrui979/foresight) | 3 | 2026-08-22 | 2026-08-22 | ForeSight: a temporal-aspect long-term memory plugin for DeepSeek Harness (dsh) |
| 178 | [xiaoksio/dsh-solution-explorer](https://github.com/xiaoksio/dsh-solution-explorer) | 3 | 2026-08-23 | 2026-08-23 | DSH Web GUI right sidebar: VS Code-style file explorer plus source control (git status, stage/unstage/discard, commit, diff, commit graph, sync fetch/pull/push, branch/remote management, git init, multi-repo, color-coded file status, file-type icons, image preview) with editable diff view, syntax-highlighted editor, and file operations. |
| 179 | [xxccdl/DeepSeek-Harness-Mobile](https://github.com/xxccdl/DeepSeek-Harness-Mobile) | 3 | 2026-08-21 | 2026-08-23 | 在 Android 手机上运行 DeepSeek Harness AI 助手的 React Native 应用，内置 Termux + proot-distro 完整 Linux 环境，无需 root，支持手机控制 |
| 180 | [yxy050208/multisim-mcp](https://github.com/yxy050208/multisim-mcp) | 3 | 2026-08-08 | 2026-08-23 | Unofficial MCP server for AI-driven NI Multisim circuit generation, simulation, data export, and reports |
| 181 | [ZekaiShi/evo-subagent](https://github.com/ZekaiShi/evo-subagent) | 3 | 2026-08-22 | 2026-08-24 | Unified DeepSeek Harness plugin: role-based subagent routing + per-agent evolution (prefercmd/memory as knowledge allow/deny lists), so repeated tasks start from proven commands and save tokens. Unified subagent routing and evolution: prefercmd/memory serve as knowledge allow/deny lists, saving tokens. |
| 182 | [zilliztech/dsh-milvus](https://github.com/zilliztech/dsh-milvus) | 3 | 2026-08-18 | 2026-08-24 | DeepSeek Harness(DSH) plugin for Milvus |
| 183 | [zyh20041227/improved_vision_for_deepseek](https://github.com/zyh20041227/improved_vision_for_deepseek) | 3 | 2026-08-22 | 2026-08-23 | Full-coverage image tiling for DeepSeek Harness vision models, dense-text OCR, and document AI |
| 184 | [0neKbyte/dsh-approval-assistant_0neKbyte](https://github.com/0neKbyte/dsh-approval-assistant_0neKbyte) | 2 | 2026-08-23 | 2026-08-24 | deepseek 审批+问答+完成时添加提醒，可设置浏览器、系统通知、弹窗通知，可自拟音效 |
| 185 | [0xRabit/dsh-crypto-portfolio](https://github.com/0xRabit/dsh-crypto-portfolio) | 2 | 2026-08-22 | 2026-08-22 | A free, 100% self-hosted DeepSeek Harness plugin that unifies your on-chain and CEX assets. |
| 186 | [1Lyn-en/dsh-whale](https://github.com/1Lyn-en/dsh-whale) | 2 | 2026-08-15 | 2026-08-24 | DeepSeek Harness 极简回复插件，提供六档精简模式与 CyberUI 主题，可节省 60–75% 输出 Token｜A DSH plugin with six brevity modes and a CyberUI theme. |
| 187 | [88514205-oss/dsh-ryoshu-slash](https://github.com/88514205-oss/dsh-ryoshu-slash) | 2 | 2026-08-16 | 2026-08-25 | DSH plugin: 天殺拔刀斬——带斩击特效的文件删除工具，强制审查防误删；official bundle, install via `dsh plugin --profile web add` github:88514205-oss/dsh-ryoshu-slash |
| 188 | [AbelKeithsun/dsh-question-nav](https://github.com/AbelKeithsun/dsh-question-nav) | 2 | 2026-08-21 | 2026-08-25 | In-session question minimap for the DeepSeek Harness Web GUI: a vertical column of round dots overlaid on the left edge of the conversation column, one dot per user question — hover enlarges and shows full text, click jumps to that message. |
| 189 | [afoxsss/dsh-conversation-map](https://github.com/afoxsss/dsh-conversation-map) | 2 | 2026-08-24 | 2026-08-24 | 会话地图（Conversation Minimap）—— DeepSeek Harness (dsh) Web 客户端插件。 |
| 190 | [AI-Scarlett/DSH-Store](https://github.com/AI-Scarlett/DSH-Store) | 2 | 2026-08-16 | 2026-08-25 | DSH STORE — third-party plugin marketplace and guarded lifecycle manager for DeepSeek Harness. |
| 191 | [ai-yukin/dsh-0-tools](https://github.com/ai-yukin/dsh-0-tools) | 2 | 2026-08-20 | 2026-08-25 | Zero-cost, zero-hassle toolkit for DeepSeek Harness (DSH): one-click free model setup (Zhipu GLM-4-Flash + OpenRouter Ox-Alpha) for complete beginners. 小白零门槛零费用套件。 |
| 192 | [Alain-Prot0s5/dsh-screenshot](https://github.com/Alain-Prot0s5/dsh-screenshot) | 2 | 2026-08-21 | 2026-08-22 | DeepSeek Harness Desktop 截图自动粘贴插件（需安装 DSH Desktop 版，仅 Win10/11，纯 AI 生成）：相机按钮 / 全局热键 Alt+A → 系统截图 → 自动粘贴进输入框 \| Screenshot-to-input plugin for DeepSeek Harness Desktop (DSH Desktop app required; Windows 10/11 only; AI-generated): camera button & global hotkey Alt+A -> snip -> auto-paste into composer |
| 193 | [AlexKaiqi/dsh-session-assistant](https://github.com/AlexKaiqi/dsh-session-assistant) | 2 | 2026-08-20 | 2026-08-24 | Session-scoped full-duplex voice assistant for DeepSeek Harness with safe drafting, explicit Agent submission, and optional knowledge curation. |
| 194 | [alextangson/dsh-dispatch](https://github.com/alextangson/dsh-dispatch) | 2 | 2026-08-23 | 2026-08-24 | 📱 Dispatch tasks to DeepSeek Harness (dsh) from your phone — approvals on your lock screen, isolated git worktrees, E2E encrypted, self-hostable. Like Claude Code Dispatch, for dsh. |
| 195 | [AndrasSama/dsh-omp-advisor](https://github.com/AndrasSama/dsh-omp-advisor) | 2 | 2026-08-24 | 2026-08-25 | Ward concil is oh-my-pi advisor subsystem ported to DeepSeek Harness — independent reviewer models watch your agent and advise it (nit injects, concern/blocker steer) it also include an auto resume and git checkpoints |
| 196 | [anonRTtty/dsh-api-balance-displayer-plugin](https://github.com/anonRTtty/dsh-api-balance-displayer-plugin) | 2 | 2026-08-24 | 2026-08-24 | DeepSeek API 余额显示插件 / DeepSeek API balance display for DeepSeek Harness |
| 197 | [aorucshiea/dsh-plugin-toggle](https://github.com/aorucshiea/dsh-plugin-toggle) | 2 | 2026-08-24 | 2026-08-25 | Hot-plug enable/disable switches for installed DSH plugins |
| 198 | [aorucshiea/dsh-preset-switch](https://github.com/aorucshiea/dsh-preset-switch) | 2 | 2026-08-24 | 2026-08-25 | Optional mid-session agent-preset switching for DeepSeek Harness |
| 199 | [aorucshiea/dsh-safe-tui](https://github.com/aorucshiea/dsh-safe-tui) | 2 | 2026-08-24 | 2026-08-25 | DeepSeek Harness safe-mode recovery console: minimal TUI, history, repair, model/provider management |
| 200 | [AxelGoal/Deepharn](https://github.com/AxelGoal/Deepharn) | 2 | 2026-08-23 | 2026-08-24 | Un escritorio propio para DeepSeek Harness en macOS: frontend nuevo sobre su API, concha nativa en Swift y dos plugins. |
| 201 | [backrooms-yrc/dsh-openai-gateway](https://github.com/backrooms-yrc/dsh-openai-gateway) | 2 | 2026-08-23 | 2026-08-23 | Expose DeepSeek Harness (dsh) as an OpenAI-compatible API server — /v1/chat/completions + /v1/models, backed by real agent sessions with tools and workspaces. 把 DeepSeek Harness 暴露为 OpenAI 兼容 API 服务端。 |
| 202 | [BaronCyrus/dsh-harness-ally](https://github.com/BaronCyrus/dsh-harness-ally) | 2 | 2026-08-22 | 2026-08-22 | DeepSeek Harness 联盟模式：自由组合 DSH、Claude Code、Codex 与全部已配置模型，保留原生 Agent 生命周期与实时执行过程。 |
| 203 | [BenjaminSHI4008/deepseek-pet-Seeki](https://github.com/BenjaminSHI4008/deepseek-pet-Seeki) | 2 | 2026-08-17 | 2026-08-23 | DeepSeek Harness 桌宠插件：透明置顶的桌面精灵（2D 像素风状态机） |
| 204 | [bettermen/dsh-course-writer](https://github.com/bettermen/dsh-course-writer) | 2 | 2026-08-23 | 2026-08-23 | 虾说教材写作 · dsh-course-writer — AI course-authoring workspace plugin for DeepSeek Harness (DSH). 三栏式工作台 · 九阶段门禁 · 课程/章节/资料库/知识图谱 · 导出 TXT/Word · 分享协作。Three-pane workspace, nine-phase gated workflow, lorebook, export & share. |
| 205 | [BigBlueBaby/codex2dsh](https://github.com/BigBlueBaby/codex2dsh) | 2 | 2026-08-24 | 2026-08-25 | 把 Codex（OpenAI Codex CLI / Desktop）的 MCP 服务器、技能、全局指令、记忆与会话历史一键迁移进 DeepSeek Harness（DSH）——可视化面板 + CLI，源码只读、dry-run 预览、密钥按原样迁移。 |
| 206 | [bluechips-zhao/dsh-receipt](https://github.com/bluechips-zhao/dsh-receipt) | 2 | 2026-08-24 | 2026-08-24 | DeepSeek Harness 对话使用情况记录超市小票插件：按模型统计的令牌使用量、调用次数、耗时和成本 \| Conversation usage receipt plugin for DeepSeek Harness: per-model token usage, calls, time and cost |
| 207 | [c-ling/dsh-plugin-request-retry](https://github.com/c-ling/dsh-plugin-request-retry) | 2 | 2026-08-23 | 2026-08-23 | DeepSeek Harness 请求重试插件：模型请求失败且错误信息命中关键词时，在内置重试策略耗尽后继续自动追加重试；设置面板可管理关键词与退避参数。 |
| 208 | [caob23/dsh-browser-control](https://github.com/caob23/dsh-browser-control) | 2 | 2026-08-22 | 2026-08-23 | Chrome 浏览器扩展 + DeepSeek Harness 插件，让 AI Agent 直接操控你的真实浏览器。 |
| 209 | [cdxDNRF/dsh-wishadel-theme](https://github.com/cdxDNRF/dsh-wishadel-theme) | 2 | 2026-08-14 | 2026-08-24 | dsh主题维什戴尔风格 |
| 210 | [chenjie1129/deepseek-harness-reliability-governor](https://github.com/chenjie1129/deepseek-harness-reliability-governor) | 2 | 2026-08-23 | 2026-08-24 | Evidence-gated completion and trusted code verification for DeepSeek Harness agents |
| 211 | [chensl139-ok/dsh-archived-panel](https://github.com/chensl139-ok/dsh-archived-panel) | 2 | 2026-08-23 | 2026-08-23 | DeepSeek Harness 插件:侧边栏「已归档」面板,可查看/打开/取消归档会话 A side panel that lists, opens, and unarchives archived sessions. |
| 212 | [chidaic/dsh-agent-notify](https://github.com/chidaic/dsh-agent-notify) | 2 | 2026-08-22 | 2026-08-22 | DSH Web GUI task-completion notifications: Windows system-level alerts (browser Notification API) when the agent finishes a task or needs your input - click-to-open session, background-only mode, settings page in Settings  |
| 213 | [Chu-m/dsh-chat-continue](https://github.com/Chu-m/dsh-chat-continue) | 2 | 2026-08-22 | 2026-08-22 | Auto-retry failed API requests to keep DSH conversations going. Supports configurable status codes and error codes.  自动重试失败的 API 请求，让 DSH 对话不中断。支持自定义状态码和错误码。 |
| 214 | [chunfenxiazhi-collab/dsh-stability-audit](https://github.com/chunfenxiazhi-collab/dsh-stability-audit) | 2 | 2026-08-24 | 2026-08-25 | Scan installed dsh plugins and grade stability risk (hook surface, startup work, preflight, deps) with optional isolated install verification |
| 215 | [chuxumilk/dsh-404-panic-lock](https://github.com/chuxumilk/dsh-404-panic-lock) | 2 | 2026-08-23 | 2026-08-23 | 用DSH 开发的轻量化插件:按 Ctrl+Shift+L 一键把页面伪装成静态 404 截图,暂时锁死鼠标键盘,防止别人乱动电脑 |
| 216 | [crazy-L118/dsh-deepseek-balance-widget](https://github.com/crazy-L118/dsh-deepseek-balance-widget) | 2 | 2026-08-19 | 2026-08-24 | DeepSeek balance widget for the dsh web sidebar |
| 217 | [Cyning12/dsh-coding-kit](https://github.com/Cyning12/dsh-coding-kit) | 2 | 2026-08-16 | 2026-08-24 | DSH plugin + gate CLI for ICVO coding standards. Load ≠ inject: call apply_coding_standards. CLI: npx dsh-coding-kit |
| 218 | [d3cker/dsh-open-terminal](https://github.com/d3cker/dsh-open-terminal) | 2 | 2026-08-23 | 2026-08-23 | OpenTerminal support for DeepSeek Harness |
| 219 | [DaiYuhangSustc/dsh-cae-plugin](https://github.com/DaiYuhangSustc/dsh-cae-plugin) | 2 | 2026-08-24 | 2026-08-24 | Mochi 🐶 — natural-language CAE plugin for DeepSeek Harness: one sentence in, a full CAD → mesh → solve → post-process pipeline out (CalculiX FEA + OpenFOAM CFD). \| 自然语言驱动的 CAE插件：一句话跑通 CAD → 网格 → 求解 → 后处理全链路（CalculiX 结构 + OpenFOAM CFD）。 |
| 220 | [DamonBao/dsh-dungeon-party](https://github.com/DamonBao/dsh-dungeon-party) | 2 | 2026-08-22 | 2026-08-22 | Safety-first five-agent orchestration plugin for DeepSeek Harness (DSH), with leases, scopes, checkpoints, validation, and recovery. |
| 221 | [dat-lequoc/dsh-kiro](https://github.com/dat-lequoc/dsh-kiro) | 2 | 2026-08-24 | 2026-08-25 | Kiro provider for DeepSeek Harness with Builder ID login, live model discovery, and reasoning effort controls |
| 222 | [ddtcorex/dsh-maestro-memory](https://github.com/ddtcorex/dsh-maestro-memory) | 2 | 2026-08-24 | 2026-08-25 | DSH plugin for durable, cross-session memory & todos — five tracks (global/user/project/key/daily), confirmation-gated writes, Git-backed sync, in-place adoption of ~/.dsh/memories. |
| 223 | [dingminhua/dsh-subagent-default-model](https://github.com/dingminhua/dsh-subagent-default-model) | 2 | 2026-08-16 | 2026-08-25 | Configurable default model for subagent delegations via settings.yaml, with single-model and multi-model round-robin/random strategies. |
| 224 | [DM010727/dsh-cline](https://github.com/DM010727/dsh-cline) | 2 | 2026-08-25 | 2026-08-25 | Deepseek harness 开源插件 — DSH (DeepSeek Harness) + Cline VS Code ecosystem fusion |
| 225 | [dong3434/dsh-auto-maintenance](https://github.com/dong3434/dsh-auto-maintenance) | 2 | 2026-08-24 | 2026-08-24 | DSH Auto Maintenance System - Diagnosis, Fix, Backup, Monitor |
| 226 | [drscrewdriver/dsh-session-search-toggle](https://github.com/drscrewdriver/dsh-session-search-toggle) | 2 | 2026-08-19 | 2026-08-22 | 给 DeepSeek Harness 侧边栏加一个会话内容检索——标题/内容一键切换，还能按用户/回复/工具筛选 |
| 227 | [elviass/dsh-cost-insights](https://github.com/elviass/dsh-cost-insights) | 2 | 2026-08-22 | 2026-08-22 | DeepSeek Harness 的用量、费用、Token、缓存、余额与模型价格分析插件。 |
| 228 | [enterhalf/dsh-web-network-optimizer](https://github.com/enterhalf/dsh-web-network-optimizer) | 2 | 2026-08-21 | 2026-08-22 | dsh网页端网络优化：通过缓存与压缩技术降低传输，从而大幅提升网页加载速度；同时提供网络断连指示与自动断网重连功能。非常适合追求极致性能或网络不稳定用户使用。Network optimization for the DSH web UI: reduces transfer size with caching and compression to greatly speed up page loading, plus a connection-drop indicator and automatic reconnection. Ideal for users pursuing peak performance or using unstable networks. |
| 229 | [Entity-Him/dsh-hiboard-push](https://github.com/Entity-Him/dsh-hiboard-push) | 2 | 2026-08-23 | 2026-08-23 | Push task-completion messages to the Huawei HarmonyOS assistant-today (负一屏) card feed from DeepSeek Harness — wire-compatible with the OpenClaw today-task skill. |
| 230 | [Entity-Him/dsh-sky-skin](https://github.com/Entity-Him/dsh-sky-skin) | 2 | 2026-08-25 | 2026-08-25 | Sky: Children of the Light themed skin for DeepSeek Harness web UI - light children on a glowing star map, candlelight gold and starry night. 光遇·遇境主题皮肤。 |
| 231 | [ericw0315/dsh-usage-lite](https://github.com/ericw0315/dsh-usage-lite) | 2 | 2026-08-21 | 2026-08-22 | 为 DeepSeek Harness Web 界面提供简洁、优雅的余额与 Token 用量面板。  Compact provider balances and local token-usage analytics for the DeepSeek Harness Web UI. |
| 232 | [ErrorLst/dsh-code-pipeline](https://github.com/ErrorLst/dsh-code-pipeline) | 2 | 2026-08-23 | 2026-08-24 | DSH bundle plugin: 为 code-pipeline 预设（PTC 流水线）动态注入阶段子代理工具（subagent_plan / subagent_impl / subagent_review），各阶段 provider/model/思考等级可在设置页实时配置 |
| 233 | [EternalNight996/dsh-theme](https://github.com/EternalNight996/dsh-theme) | 2 | 2026-08-22 | 2026-08-23 | DeepSeek Harness theme skin plugin - built-in themes / static image / dynamic 360-follow video. |
| 234 | [etony668/dsh-task-board](https://github.com/etony668/dsh-task-board) | 2 | 2026-08-23 | 2026-08-24 | DSH 项目任务看板插件：会话「任务看板」视图 + 父子任务树工具与技能 + 本地 JSON 存储（CodexFF 移植） |
| 235 | [faith1688/dsh-usage-meter-harness](https://github.com/faith1688/dsh-usage-meter-harness) | 2 | 2026-08-17 | 2026-08-25 | 专为 DeepSeek API 打造的实时用量 / 费用 / 余额计量插件 —— 在聊天输入框旁直接看到 tokens、花费与真实余额。 |
| 236 | [FAVKTOXIC/dsh-theme-liquid-glass](https://github.com/FAVKTOXIC/dsh-theme-liquid-glass) | 2 | 2026-08-23 | 2026-08-24 | Apple Liquid Glass theme for DeepSeek Harness |
| 237 | [FloatingLifeTL/dsh-plugin_session-manager-custom](https://github.com/FloatingLifeTL/dsh-plugin_session-manager-custom) | 2 | 2026-08-22 | 2026-08-24 | DeepSeek Harness Web plugin for local session data management |
| 238 | [Flycat43/liang-desktop-pet](https://github.com/Flycat43/liang-desktop-pet) | 2 | 2026-08-23 | 2026-08-24 | An unofficial desktop companion UI for DeepSeek Harness.梁圣 |
| 239 | [gameswu/dsh-human-coding](https://github.com/gameswu/dsh-human-coding) | 2 | 2026-08-26 | 2026-08-26 | DeepSeek Harness 增加古法编程模式，让模型监督你写代码！ |
| 240 | [GM-HZ/dsh-dag-workflow](https://github.com/GM-HZ/dsh-dag-workflow) | 2 | 2026-08-23 | 2026-08-24 | Durable DAG workflows for DeepSeek Harness: Agent-guided templates, SQLite recovery, plugin nodes, and XYFlow Canvas. |
| 241 | [Guard42/dsh-humanize](https://github.com/Guard42/dsh-humanize) | 2 | 2026-08-24 | 2026-08-24 | Humanize 模式 — humanfia 流理念 × DeepSeek Harness 的 agent 预设：Flow 编排 · SHA-256 流锁 · HMAC 评审门禁 · 事件回放恢复 · 一行命令安装 · 可定制领域变体 |
| 242 | [guyuefangyuanl/dsh-memory](https://github.com/guyuefangyuanl/dsh-memory) | 2 | 2026-08-21 | 2026-08-22 | Cross-session persistent memory for the DeepSeek Harness: a model-facing memory tool, an always-on index section, and a bundled maintenance skill. |
| 243 | [hanshanyike/dsh-yolo](https://github.com/hanshanyike/dsh-yolo) | 2 | 2026-08-20 | 2026-08-25 | 把对话里说过的重要事情，变成持续可跟进的计划。  为 deepseek-harness 打造的个人助手：从对话中整理事项、跟踪变化，并在需要时提醒你。 |
| 244 | [hatanokokosa/dsh-colorschemes](https://github.com/hatanokokosa/dsh-colorschemes) | 2 | 2026-08-22 | 2026-08-22 | A DSH ColorScheme Plugin |
| 245 | [HeyBobChan/canon-deepseek-harness-plugin](https://github.com/HeyBobChan/canon-deepseek-harness-plugin) | 2 | 2026-08-23 | 2026-08-24 | Canon integration plugin for DeepSeek Harness |
| 246 | [HIT-HTML/dsh-ENHANCED](https://github.com/HIT-HTML/dsh-ENHANCED) | 2 | 2026-08-24 | 2026-08-25 | One plugin, every upgrade DeepSeek Harness lacks out of the box: multi-engine web search, skills & MCP managers, per-profile plugin toggles, session cleanup with hover-delete, one-click restart/shutdown, themes. Single tool surface, no telemetry. |
| 247 | [Howe829/dsh-insider](https://github.com/Howe829/dsh-insider) | 2 | 2026-08-20 | 2026-08-22 | Runtime observability and relationship graph for DeepSeek Harness and Cordis |
| 248 | [huang-chunc/dsh-user-message-timeline](https://github.com/huang-chunc/dsh-user-message-timeline) | 2 | 2026-08-22 | 2026-08-26 | dsh Web 悬浮药丸导轨：预览·跳转·分页，设置-插件-插件配置可切换左右贴边 |
| 249 | [huyang218/dsh-plugins](https://github.com/huyang218/dsh-plugins) | 2 | 2026-08-18 | 2026-08-24 | Plugins for DeepSeek Harness (dsh) — 18 build-free ESM bundles: model-facing tools, runtime wrappers and web UI extensions. Installable by name, URL or local path from the dsh CLI, dsh Desktop or dsh Android. |
| 250 | [hw-cola/dsh-dynamic-agents](https://github.com/hw-cola/dsh-dynamic-agents) | 2 | 2026-08-25 | 2026-08-25 | DSH插件，动态AGENTS.md |
| 251 | [hyperion2144/dsh-subagent-pro](https://github.com/hyperion2144/dsh-subagent-pro) | 2 | 2026-08-20 | 2026-08-22 | DSH Web extension: live subagent monitor + role-based subagent routing + Claude Code style .dsh/agents/*.md persona injection |
| 252 | [hyrinx/dsh-plugin-open-with](https://github.com/hyrinx/dsh-plugin-open-with) | 2 | 2026-08-22 | 2026-08-25 | 在DeepSeek Harness Web 会话头部添加胶囊拆分按钮，一键在当前工作区打开VS Code、终端（CMD / PowerShell）和文件资源管理器。 |
| 253 | [imkelt/DSH-RAG](https://github.com/imkelt/DSH-RAG) | 2 | 2026-08-22 | 2026-08-24 | Local knowledge bases with explicit, source-backed retrieval for DeepSeek Harness Web. |
| 254 | [imkingjh999/dsh-deepsea](https://github.com/imkingjh999/dsh-deepsea) | 2 | 2026-08-23 | 2026-08-23 | DSH plugin: 深海摸鱼 —— context 越深潜得越深，答完摸鱼集镭射生物卡 \| Deep-sea slacking holo cards |
| 255 | [imroc/dsh-project-prompt](https://github.com/imroc/dsh-project-prompt) | 2 | 2026-08-26 | 2026-08-26 | Private, per-project prompt rules for DeepSeek Harness — matched by git remote/repo/path, worktree-aware, never committed to the repo |
| 256 | [inmny/dsh-continue](https://github.com/inmny/dsh-continue) | 2 | 2026-08-24 | 2026-08-25 | 为 DeepSeek Harness 增加一个直接续跑按钮。当会话异常结束时，可以从现有上下文继续执行，不会引入其他提示词。 |
| 257 | [iskshadow195563/DeepSeek_Harness_Balance_Banner](https://github.com/iskshadow195563/DeepSeek_Harness_Balance_Banner) | 2 | 2026-08-22 | 2026-08-23 | 💵 DeepSeek 余额横幅(dsh 插件):页面顶部右侧(主题切换按钮左侧)同时显示 USD/CNY 余额,负值高亮,60s 自动刷新,一条命令安装 |
| 258 | [iskshadow195563/DeepSeek_Harness_Files_Panel](https://github.com/iskshadow195563/DeepSeek_Harness_Files_Panel) | 2 | 2026-08-22 | 2026-08-23 | 📁 右侧可折叠的 DeepSeek 上传文件管理面板(dsh 插件):列出/复制/清理 DeepSeek Files API 上传的图片,密钥零暴露,一条命令安装 |
| 259 | [J0ss077/dsh-always-require-tools-approval](https://github.com/J0ss077/dsh-always-require-tools-approval) | 2 | 2026-08-24 | 2026-08-24 | Stop. Confirm. Run. A DeepSeek Harness plugin that pauses selected tools and waits for your explicit approval before every execution. |
| 260 | [JimChen-g/dsh-action-outbox](https://github.com/JimChen-g/dsh-action-outbox) | 2 | 2026-08-16 | 2026-08-26 | Batch Review Inbox for DeepSeek Harness — stage, inspect, edit, approve, and commit exact tool side effects safely. |
| 261 | [joekytc/dsh-swarm](https://github.com/joekytc/dsh-swarm) | 2 | 2026-08-20 | 2026-08-24 | Run multi-agent task pipelines on DSH like a team — plan, execute, review, and deliver code through a visual kanban with provable completion. |
| 262 | [JohnnyTing/dsh-official-homepage-theme](https://github.com/JohnnyTing/dsh-official-homepage-theme) | 2 | 2026-08-24 | 2026-08-24 | 复刻 DeepSeek Harness 官方首页主题插件 |
| 263 | [joshryandavis/dsh-llm-aws-kiro](https://github.com/joshryandavis/dsh-llm-aws-kiro) | 2 | 2026-08-21 | 2026-08-24 | deeepseek-harness kiro provider |
| 264 | [k-ying/dsh-vsceditor](https://github.com/k-ying/dsh-vsceditor) | 2 | 2026-08-25 | 2026-08-25 | DeepSeek Harness 内嵌 VSCode 编辑器插件：嵌入完整 code-server，agent 写文件时自动弹出红绿 diff 跟随（edit sync / file locking / follow mode） |
| 265 | [LCYLYM/dsh-plugin-compat-guardian](https://github.com/LCYLYM/dsh-plugin-compat-guardian) | 2 | 2026-08-22 | 2026-08-22 | Repository-installed CI repair bot that keeps DeepSeek Harness plugins compatible with new DSH releases |
| 266 | [leonardwwq/dsh-cultivation](https://github.com/leonardwwq/dsh-cultivation) | 2 | 2026-08-20 | 2026-08-26 | A DSH plugin that gives AI characters persistent relationships and evolving user models through long-term interaction. |
| 267 | [Letter2025/dsh-task-worktree](https://github.com/Letter2025/dsh-task-worktree) | 2 | 2026-08-18 | 2026-08-25 | Complete Git worktree support for DeepSeek Harness: task-scoped isolated checkouts on their own branches, recorded in a per-repo manifest that survives sessions and restarts |
| 268 | [lifeopsgo/dsh-capability-toggle-plugin](https://github.com/lifeopsgo/dsh-capability-toggle-plugin) | 2 | 2026-08-22 | 2026-08-22 | Toggle individual agent capabilities (skills, MCP, tools, prompt, approval, guards) from the DSH WebUI composer — session / project / global. DSH 各种能力（mcp/skill/tool等）多层级开关灵活控制 |
| 269 | [LingYuYue1/dsh-workbench](https://github.com/LingYuYue1/dsh-workbench) | 2 | 2026-08-23 | 2026-08-23 | VSCode 风格工作台侧边栏：文件树 / 多标签预览 / CodeMirror 编辑 / 终端 / Git / 全库搜索 / 变更审查 \| Workbench sidebar panel for DeepSeek Harness |
| 270 | [LINinLIN-0079/godot-asset-planner-public](https://github.com/LINinLIN-0079/godot-asset-planner-public) | 2 | 2026-08-21 | 2026-08-24 | Godot asset & project-goal management for DeepSeek Harness: godot_* model tools, /gap REST API, and a better-sidebar UI with asset manager, scene-tree viewer and Git panel. / DeepSeek Harness 的 Godot 资产与项目目标统一管理插件：godot_* 模型工具 + /gap REST 路由 + better-sidebar 界面（资产管理器 / 场景树查看器 / Git 版本控制）。 |
| 271 | [Linux-System-0/peaklow](https://github.com/Linux-System-0/peaklow) | 2 | 2026-08-23 | 2026-08-23 | DeepSeek Harness (Cordis) 高峰/低峰自动调度插件：宿主 + 浏览器端 client 状态卡。dsh-plugin |
| 272 | [linxuhao/AItelier](https://github.com/linxuhao/AItelier) | 2 | 2026-04-04 | 2026-08-25 | AI-Atelier, the all in one personal "atelier" (means handcraft studio in french) that can adapt to your need. |
| 273 | [lishLRF/dsh-plugin-onekey](https://github.com/lishLRF/dsh-plugin-onekey) | 2 | 2026-08-22 | 2026-08-23 | 适配插件中心的一键安装/卸载 |
| 274 | [lispking/dsh-auto-evolve](https://github.com/lispking/dsh-auto-evolve) | 2 | 2026-08-22 | 2026-08-22 | A self-evolving plugin for DeepSeek Harness (dsh). It observes how the agent runs, proposes improvements to its own assets via the LLM, validates each proposal inside a sandboxed trial agent, and applies only verified mutations — with a versioned ledger and automatic rollback on regression. |
| 275 | [liustack/summono](https://github.com/liustack/summono) | 2 | 2026-08-17 | 2026-08-24 | One click and DeepSeek Harness is running — the free launcher & installer for AI harnesses. 一键安装启动 DeepSeek Harness。 |
| 276 | [liznee/dsh-file-resource](https://github.com/liznee/dsh-file-resource) | 2 | 2026-08-22 | 2026-08-22 | DeepSeek Harness Web 的本地文件输入插件。在输入框原有的 + 菜单顶部增加 attach，并用分隔线与 Harness 原生命令区分；不会再增加一个单独按钮。Private local file attachments for DeepSeek Harness with native images and bounded document reading. |
| 277 | [loadingvx/deepseeh-harness-ultra-slash](https://github.com/loadingvx/deepseeh-harness-ultra-slash) | 2 | 2026-08-17 | 2026-08-23 | /steer commands for deepseek-harness |
| 278 | [loeanxi/dsh-injection-guard](https://github.com/loeanxi/dsh-injection-guard) | 2 | 2026-08-19 | 2026-08-22 | Source-aware prompt injection protection for DeepSeek Harness |
| 279 | [log-li/dsh-automode](https://github.com/log-li/dsh-automode) | 2 | 2026-08-21 | 2026-08-22 | CC-style auto approval layer for DeepSeek Harness: deterministic rules + two-stage classifier, circuit breaker, fail-to-human. Shadow mode day one. |
| 280 | [ltxlong/dsh-session-kit](https://github.com/ltxlong/dsh-session-kit) | 2 | 2026-08-22 | 2026-08-23 | 会话管理菜单、归档管理、轮次级删除、重新生成，话题快捷导航。Add a management menu for conversations, archive conversation management, delete by round, regenerate, and a quick topic navigation on the right. |
| 281 | [lunaship/dsh-links](https://github.com/lunaship/dsh-links) | 2 | 2026-08-18 | 2026-08-22 | Android companion for DeepSeek Harness: trusted-LAN pairing, mobile sessions, SSE approvals, experimental tunnels, and a planned DSH Links Relay. |
| 282 | [lutrodev/dsh-roleplay](https://github.com/lutrodev/dsh-roleplay) | 2 | 2026-08-25 | 2026-08-26 | Roleplay plugin suite for DeepSeek Harness: character cards, lorebooks, personas, presets, state, and conversation tools. |
| 283 | [luxueliu/luxueliu-usage-command](https://github.com/luxueliu/luxueliu-usage-command) | 2 | 2026-08-20 | 2026-08-22 | 内置DSH指令，一键展示今日全局付费模型总消耗账单（人民币版）！按模型×分小时查当日¥消费，缓存命中/未命中/输出三档单价，官方/中转/套餐全覆盖 — DeepSeek Harness 插件 |
| 284 | [Lxd-Ashe/dsh-codex-theme](https://github.com/Lxd-Ashe/dsh-codex-theme) | 2 | 2026-08-24 | 2026-08-24 | Codex 主题外观插件 for DeepSeek Harness（DSH）：把 Codex 主题配置（codex-theme-v1，80 款浅/深色主题）做成可在 DSH 中直接切换、可自定义的外观插件。 |
| 285 | [lywusichen/dsh-sidebar-buttons](https://github.com/lywusichen/dsh-sidebar-buttons) | 2 | 2026-08-23 | 2026-08-23 | 管理 DeepSeek Harness 左下侧栏按钮的插件：拖拽排序、显隐控制，隐藏按钮收进"更多"菜单，可统一按钮高度。 |
| 286 | [margbug01/dsh-ma-plugins](https://github.com/margbug01/dsh-ma-plugins) | 2 | 2026-08-15 | 2026-08-22 | DeepSeek Harness (DSH) plugins: Tavily+Exa web search, Oracle second opinion, GitHub Librarian, /handoff, session manager, and file drop. |
| 287 | [Max-Null/dsh-draft-polish](https://github.com/Max-Null/dsh-draft-polish) | 2 | 2026-08-21 | 2026-08-25 | Draft polish for DeepSeek Harness: one-click LLM polish of your draft in the composer, rewrites it in place with session context · 草稿润色：发送前一键调用 LLM 润色草稿，结果回填输入框 |
| 288 | [Max-Null/dsh-skill-mcp-center](https://github.com/Max-Null/dsh-skill-mcp-center) | 2 | 2026-08-17 | 2026-08-25 | Skill & MCP center for DeepSeek Harness: manage skills and MCP servers in Settings, live MCP status in the sidebar · Skill 与 MCP 管理中心：设置里管理技能与 MCP 服务器，侧边栏实时状态 |
| 289 | [maxmilian/dsh-sonarqube](https://github.com/maxmilian/dsh-sonarqube) | 2 | 2026-08-24 | 2026-08-24 | Read-only SonarQube Community Build tools for DeepSeek Harness |
| 290 | [menotbobbybrown/dsh-plugin-mcp](https://github.com/menotbobbybrown/dsh-plugin-mcp) | 2 | 2026-08-21 | 2026-08-22 | Universal Model Context Protocol (MCP) Bridge Plugin for DeepSeek Harness (dsh) — Everything is a Plugin |
| 291 | [mhwww/DSH-Wallpaper-Engine](https://github.com/mhwww/DSH-Wallpaper-Engine) | 2 | 2026-08-23 | 2026-08-24 | DeepSeek Harness (dsh) 背景图片插件：内置默认图 / 自定义上传 / Wallpaper Engine 创意工坊一键应用 / 视频壁纸 ffmpeg 高清抽帧 |
| 292 | [Moon-shiyue/dsh-github-connect](https://github.com/Moon-shiyue/dsh-github-connect) | 2 | 2026-08-22 | 2026-08-23 | 便携式 GitHub 连接插件 for DeepSeek Harness (DSH)：composer 左下角一键授权，AI 可通过 github_api 工具操作你的 GitHub。Portable GitHub connection plugin: OAuth device flow / PAT, proxy & system-CA aware. |
| 293 | [MoonlitDropOfBlood/dsh-archive-manager](https://github.com/MoonlitDropOfBlood/dsh-archive-manager) | 2 | 2026-08-18 | 2026-08-23 | DSH的归档管理插件 |
| 294 | [MoonlitDropOfBlood/dsh-token-stats](https://github.com/MoonlitDropOfBlood/dsh-token-stats) | 2 | 2026-08-18 | 2026-08-23 | dsh的token消耗的统计插件 |
| 295 | [mqhe2007/dsh-pm](https://github.com/mqhe2007/dsh-pm) | 2 | 2026-08-21 | 2026-08-22 | dsh-pm is the ChunSun × DeepSeek Harness reference plugin: an AI-native project-delivery loop driven by ChunSun. Requirements / Runs / Steps / acceptance scenarios & cases / work-memory, a session delivery panel, and 28 chunsun_* model tools — with the platform as the single source of truth. MIT. |
| 296 | [MrElysium/convoport](https://github.com/MrElysium/convoport) | 2 | 2026-08-23 | 2026-08-24 | Capture AI conversations from any web chat, keep them 100% local, and port them into any agent as live sessions — not dead exports. |
| 297 | [MrmoLabs/dsh-mermaid](https://github.com/MrmoLabs/dsh-mermaid) | 2 | 2026-08-23 | 2026-08-23 | Render Mermaid code blocks as SVG diagrams in DeepSeek Harness Web, with diagram/code switching, streaming support, dark mode, strict security, and npm/GitHub installation. |
| 298 | [NaNQiQ/deepseek-harness-remote-ssh](https://github.com/NaNQiQ/deepseek-harness-remote-ssh) | 2 | 2026-08-24 | 2026-08-24 | 让 DeepSeek Harness（DSH） 使用原生工具直接操作远程 Linux 服务器，自由切换服务器 |
| 299 | [necokeine/dsh-codex-relay](https://github.com/necokeine/dsh-codex-relay) | 2 | 2026-08-22 | 2026-08-23 | Selectable Codex model provider for DeepSeek Harness over the local Codex app-server |
| 300 | [nicecx/dsh-relay](https://github.com/nicecx/dsh-relay) | 2 | 2026-08-18 | 2026-08-24 | DSH plugin: relay approval & question requests to any chat channel — iMessage, Email, WeChat built-in; Telegram/DingTalk/Feishu/Slack via a common adapter contract (src/channels/types.js) |
| 301 | [niushuanan/xiaozhuang-dsh](https://github.com/niushuanan/xiaozhuang-dsh) | 2 | 2026-08-23 | 2026-08-24 | Plugin-enhanced DeepSeek Harness distribution with Computer Use, Teamwork, model usage, and multi-worktree development. |
| 302 | [nxz1026/dsh-tray](https://github.com/nxz1026/dsh-tray) | 2 | 2026-08-19 | 2026-08-22 | DeepSeek Harness — Custom Windows Tray Launcher |
| 303 | [Nzssm1/dsh-a-stock-five-dimension](https://github.com/Nzssm1/dsh-a-stock-five-dimension) | 2 | 2026-08-21 | 2026-08-22 | A DeepSeek Harness (DSH) community agent preset for rigorous A-share five-dimension (technical/valuation/fundamental/capital-flow/news) standardized analysis: persona, skill knowledge base, hard risk gate, deterministic Python scoring core, Tencent-first collectors. Not an investment recommendation. |
| 304 | [oxgbl/dsh-no-cmd-launcher](https://github.com/oxgbl/dsh-no-cmd-launcher) | 2 | 2026-08-22 | 2026-08-22 | DSH background launcher: double-click icon to run dsh web without any cmd window, plus desktop start/stop shortcuts (npm/CLI installs, no DSH Desktop dependency) |
| 305 | [PetCT/dsh-Bio-image-dup-check](https://github.com/PetCT/dsh-Bio-image-dup-check) | 2 | 2026-08-25 | 2026-08-25 | 科研图片查重 DSH 插件 · 本地离线检测整图重复/翻转/旋转/缩放、copy-move、跨图区域复用与 PDF 稿件图片。A local-offline integrity checker for life-science figures (DeepSeek Harness plugin). |
| 306 | [pg527322814/dsh-bayes-predict](https://github.com/pg527322814/dsh-bayes-predict) | 2 | 2026-08-21 | 2026-08-22 | dsh-贝叶斯个股预测插件：多指标信号融合的上涨概率估计、趋势状态识别与持仓风险度量（A 股 + 美股） |
| 307 | [Phant0Meow/dsh-meow-cachebilling](https://github.com/Phant0Meow/dsh-meow-cachebilling) | 2 | 2026-08-22 | 2026-08-23 | 一个能帮你省钱的插件！缓存其实比你想象的贵！换窗口可以省缓存钱，但换窗口有顾虑，或许你懒得重新描述项目和规则，或者你还需要那个上下文。所以这个插件，就是为了告诉你，当前轮，纯粹上下文缓存的部分，到底花了你多少钱。这样你才心里有个底，判断什么时候该换窗口。 在dsh-plugin标签里全网找了，那么多计费插件，并没有人写这一项……真奇怪，难道只有我有这个需求吗？ |
| 308 | [picoaide/picoaide-harness](https://github.com/picoaide/picoaide-harness) | 2 | 2026-08-16 | 2026-08-23 | PicoAide Harness：企业级 DeepSeek Harness 一体化平台。桌面客户端 + 本地智能体引擎 + 管理后台，支持私有化部署。 |
| 309 | [purezhi/dsh-plugin-whale3](https://github.com/purezhi/dsh-plugin-whale3) | 2 | 2026-08-22 | 2026-08-23 | 鲸鱼 for DeepSeek Harness |
| 310 | [qinyre/dsh-plugin-atlas](https://github.com/qinyre/dsh-plugin-atlas) | 2 | 2026-08-18 | 2026-08-23 | Archive manager (browse / unarchive / auto-rules) plus a Codex-style fisheye conversation rail for dsh.·归档管理与对话刻度尺插件 |
| 311 | [qinyuehuan/dsh-whale-status](https://github.com/qinyuehuan/dsh-whale-status) | 2 | 2026-08-22 | 2026-08-23 | 把鲸鱼娘思考时的 deep diving 状态文案换成任意多句随机播放，蓝青水流动画，颜色/流速可自定义（DeepSeek Harness plugin） |
| 312 | [qishuilalala/dsh-voice-mode](https://github.com/qishuilalala/dsh-voice-mode) | 2 | 2026-08-22 | 2026-08-23 | DSH 语音双工对话模式：流式 zipformer2 识别入可编辑草稿，可选唤醒词，Edge TTS 按句朗读 + 实时字幕，开口即打断（barge-in），无需 API Key。Full-duplex voice mode for DeepSeek Harness, no API key. |
| 313 | [qwert702/dsh-commander](https://github.com/qwert702/dsh-commander) | 2 | 2026-08-22 | 2026-08-23 | Commander for the DeepSeek Harness Web GUI: one conversation orchestrates others via <dsh-dispatch> protocol blocks, with automatic result receipts. |
| 314 | [qwert702/dsh-memory](https://github.com/qwert702/dsh-memory) | 2 | 2026-08-22 | 2026-08-23 | Long-term memory plugin for the DeepSeek Harness Web GUI: project+global stores, auto extraction/injection, small-model consolidation, Obsidian-style link graph. |
| 315 | [rebron1900/dsh-mnemosyne](https://github.com/rebron1900/dsh-mnemosyne) | 2 | 2026-08-22 | 2026-08-23 | Mnemosyne 记忆层在 DeepSeek Harness 中的插件 — 本地优先、SQLite 支持的跨会话记忆。 |
| 316 | [rickyfu0625-cell/dsh-billing-dashboard](https://github.com/rickyfu0625-cell/dsh-billing-dashboard) | 2 | 2026-08-24 | 2026-08-24 | DeepSeek Harness 用量看板插件：余额 / 消费 / token / 7 日趋势 / 一键充值 |
| 317 | [robbywang25/dsh-codex-pins](https://github.com/robbywang25/dsh-codex-pins) | 2 | 2026-08-22 | 2026-08-25 | Codex-style pinned sessions for DeepSeek Harness — always visible above the sidebar list |
| 318 | [Ruiming-cn/dsh-better-at](https://github.com/Ruiming-cn/dsh-better-at) | 2 | 2026-08-21 | 2026-08-22 | Fast @ file/session reference caching for DeepSeek Harness Web / DSH @ 引用菜单加速插件 |
| 319 | [Ruiming-cn/dsh-more-session-operations](https://github.com/Ruiming-cn/dsh-more-session-operations) | 2 | 2026-08-21 | 2026-08-22 | DeepSeek Harness Web sidebar session-row menu enhancements: mark unread via the official completed-reminder dot, copy session ID, delete session with confirmation, archive confirmation, and recursive subagent-session deletion. |
| 320 | [ruisenbai/dsh-annotation](https://github.com/ruisenbai/dsh-annotation) | 2 | 2026-08-17 | 2026-08-23 | Inline, batchable comments for DeepSeek Harness assistant replies |
| 321 | [sakthiveltofficial/dsh-git-plugins](https://github.com/sakthiveltofficial/dsh-git-plugins) | 2 | 2026-08-22 | 2026-08-22 | dsh-git: Git & source-control plugin suite for DeepSeek Harness — local git + GitHub/GitLab/Bitbucket/Azure DevOps/Gitea + self-evolving memory |
| 322 | [SeerableOfficial/dsh-web-search-toggle](https://github.com/SeerableOfficial/dsh-web-search-toggle) | 2 | 2026-08-22 | 2026-08-22 | DSH plugin: a per-session "Web Search" toggle that forces the agent to search the web before answering. |
| 323 | [shangjian2023/dsh-rss-daily](https://github.com/shangjian2023/dsh-rss-daily) | 2 | 2026-08-22 | 2026-08-22 | dsh plugin: 46-source daily RSS digest, LLM-edited, delivered via webhook (ServerChan/PushDeer/WxWork/TG/Bark/gotify) |
| 324 | [shenjackyuanjie/dsh-sfw](https://github.com/shenjackyuanjie/dsh-sfw) | 2 | 2026-08-05 | 2026-08-23 | 为了防止你的好bro/同事看到内测dsh然后：？这是什么 |
| 325 | [Shizuku-keop/dsh-micro-inversion-standard](https://github.com/Shizuku-keop/dsh-micro-inversion-standard) | 2 | 2026-08-24 | 2026-08-24 | 一个可复用的 DSH Agent Preset：双阶段、Token 精益的编码智能体模式。  核心目标：把模型思维链的起手习惯从 "let me" 翻转为 "we need"，同时把上下文占用与 Token 消耗压到最低，并保持供应商 KV Cache 对未变前缀持续命中。 |
| 326 | [Shizuku-keop/dsh-plugin-brainstorm-visualizer](https://github.com/Shizuku-keop/dsh-plugin-brainstorm-visualizer) | 2 | 2026-08-24 | 2026-08-24 | DeepSeek Harness Brainstorming Visualization Plugin Seamlessly combining AI divergent reasoning with visual interaction, built specifically for solving complex problems |
| 327 | [SKzrui/DSH-CLI](https://github.com/SKzrui/DSH-CLI) | 2 | 2026-08-14 | 2026-08-22 | DSH‑CLI：轻量命令行，流式输出、工具调用、按目录恢复会话，密钥与模型灵活配置，一条命令对话 DeepSeek Harness。 \|  Lightweight CLI for DeepSeek Harness – streaming, tool calling, per‑dir session recovery, flexible config. Start with one command. |
| 328 | [soarGuo/dsh-auto-vision](https://github.com/soarGuo/dsh-auto-vision) | 2 | 2026-08-24 | 2026-08-24 | Bridges images into text for non-vision DeepSeek Harness models — your message stays untouched, zero manual setup. |
| 329 | [SoberReport-AI/DeepGuard](https://github.com/SoberReport-AI/DeepGuard) | 2 | 2026-08-22 | 2026-08-23 | A dsh plugin security audit agents team can trigger a security audit and provide a security audit report by submitting an issue |
| 330 | [ssheleg/sshlg-skills](https://github.com/ssheleg/sshlg-skills) | 2 | 2026-07-24 | 2026-08-26 | Eight agent skills, one command, every agent. Umbrella installer for the ssheleg family — super-ux, task-pipeline, agent-sync, make-skill, sheleg-design, seo-aeo-audit, sheleg-dev, agent-stack — across Claude Code, Cursor, Codex and 70+ more agents. Loads in DeepSeek Harness (dsh). |
| 331 | [Star-Guest/dsh-plugin-tavern](https://github.com/Star-Guest/dsh-plugin-tavern) | 2 | 2026-08-22 | 2026-08-22 | 酒馆（SillyTavern 精简版）DSH 插件：角色卡解析管理员 card-analyst + 角色扮演讲述者 roleplay |
| 332 | [stas130286-blip/dsh-brainagent](https://github.com/stas130286-blip/dsh-brainagent) | 2 | 2026-08-22 | 2026-08-23 | BrainAgent — brain-inspired plugin for DeepSeek Harness (dsh): a pipeline of heuristic filters, statistical memory stores and context injections; reward-ledger + UCB1 bandit learning loop (RL-lite). 676 tests. Free noncommercial use. |
| 333 | [T-MKT/dsh-customization-settings](https://github.com/T-MKT/dsh-customization-settings) | 2 | 2026-08-19 | 2026-08-22 | Provide generic UI customization settings for DeepSeek Harness, like wallpaper, theme color, etc.  |
| 334 | [TaoruiLiu19/dsh-gsv](https://github.com/TaoruiLiu19/dsh-gsv) | 2 | 2026-08-25 | 2026-08-25 | dsh-gsv-tts 是一个为 DeepSeek Harness (DSH) 开发的语音合成插件，将本地高性能 TTS 引擎 GSV-TTS-Lite 无缝接入 DSH 智能体生态。 |
| 335 | [the-thinker0/dsh-memory-search-plus](https://github.com/the-thinker0/dsh-memory-search-plus) | 2 | 2026-08-25 | 2026-08-26 | A local-first full-text memory search plugin for DeepSeek Harness, enabling fast cross-conversation search, message-level navigation, and intelligent retrieval of your AI coding history. |
| 336 | [Tianbuyu-wwx/dsh-hermes-link](https://github.com/Tianbuyu-wwx/dsh-hermes-link) | 2 | 2026-08-23 | 2026-08-24 | Bidirectional bridge between Hermes Agent and DeepSeek Harness (DSH). v0.2.4 — single-bundle Cordis plugin replacing the archived hermes-foundation/-oneshot-arbitrate/-dispatch-bridge triad. |
| 337 | [tingfeng347/dsh-vscode-workbench](https://github.com/tingfeng347/dsh-vscode-workbench) | 2 | 2026-08-23 | 2026-08-24 | 在 DeepSeek Harness 中叠加 VS Code 风格的本地开发工作台。 |
| 338 | [treers2/qq-operations](https://github.com/treers2/qq-operations) | 2 | 2026-08-25 | 2026-08-25 | QQ NT desktop automation for DeepSeek Harness (DSH) skill - dynamic UI Automation locate, dual mode, self-check; 操控 QQ NT 桌面版的 DSH skill（UIA 类名定位/双模式/自检） |
| 339 | [tristan-mcinnis/dsh-browser-vision](https://github.com/tristan-mcinnis/dsh-browser-vision) | 2 | 2026-08-22 | 2026-08-22 | Browser tool for DeepSeek Harness that can SEE the page: browser-use over CDP driven by deepseek-v4-flash-vision-exp. Reads canvas text, text inside images and rendered charts, returns schema-validated JSON, and reports per-run cost. |
| 340 | [try-works/dsh-browser-agent](https://github.com/try-works/dsh-browser-agent) | 2 | 2026-08-23 | 2026-08-23 | DeepSeek Harness bundle: a Chrome browser for agents (browser_goto / browser_evaluate / browser_screenshot tools) with a live two-way pane inside the DSH Web GUI. The browser engine is a fork of zenbu-labs/terminal-browser with the React Ink terminal UI replaced by a DSH tool surface and web pane. |
| 341 | [tuojc/dsh-browser-firefox](https://github.com/tuojc/dsh-browser-firefox) | 2 | 2026-08-22 | 2026-08-22 | Firefox browser-control plugin for DeepSeek Harness: one DSH plugin + one Firefox extension, driving your own Firefox over a token-authenticated WebSocket. Text-first toolset (snapshot/click/type/navigate/tab-stack) with screenshot as visual fallback. Firefox add-on available on AMO. Ported from Lum1104/dsh-browser (MIT). |
| 342 | [TuringCorp-net/mosaic-memory-compress](https://github.com/TuringCorp-net/mosaic-memory-compress) | 2 | 2026-06-08 | 2026-08-23 | Stateless dialogue compression that mimics human memory. LLM conversations stay bounded forever — no session management, no context overflow. |
| 343 | [TYEclipse/dsh-musictheory](https://github.com/TYEclipse/dsh-musictheory) | 2 | 2026-08-24 | 2026-08-25 | Music theory math toolbox for DeepSeek Harness (dsh): note parsing, frequency/MIDI conversion, correctly spelled chords (26 qualities) and scales (17 types) — zero runtime dependencies |
| 344 | [UncleK/dsh-think-translate](https://github.com/UncleK/dsh-think-translate) | 2 | 2026-08-24 | 2026-08-26 | Thinking-chain UI translation for DeepSeek Harness: 8 target languages, local Ollama model primary with in-panel download, Google/Bing fallback |
| 345 | [vcxmug/dsh-evo](https://github.com/vcxmug/dsh-evo) | 2 | 2026-08-13 | 2026-08-23 | Native Firecrawl tools for DeepSeek Harness agents via MCP — one composition row, zero custom code |
| 346 | [vibeinging/dsh-red-alert](https://github.com/vibeinging/dsh-red-alert) | 2 | 2026-08-23 | 2026-08-23 | A real Red Alert 2 AI battlefield plugin for DeepSeek Harness with fog-safe control, live DSH Chat, and post-match learning. |
| 347 | [wackyju2-beep/dsh-better](https://github.com/wackyju2-beep/dsh-better) | 2 | 2026-08-22 | 2026-08-23 | 更好的 DSH \| Unofficial dsh plugin: archived sessions & task notifications / 已归档会话管理 · 任务系统通知 |
| 348 | [Wanbinyu/dsh-concurrency-meter](https://github.com/Wanbinyu/dsh-concurrency-meter) | 2 | 2026-08-19 | 2026-08-25 | Read-only model request concurrency monitoring for DeepSeek Harness |
| 349 | [wang-junjian/dsh-artifact-viewer](https://github.com/wang-junjian/dsh-artifact-viewer) | 2 | 2026-08-24 | 2026-08-25 | DeepSeek Harness 插件：产物浏览器 |
| 350 | [wangyuanchuan2022/dsh-prompt-optimizer](https://github.com/wangyuanchuan2022/dsh-prompt-optimizer) | 2 | 2026-08-23 | 2026-08-23 | 一键优化提示词：在输入框工具行（发送按钮左侧）新增「优化」按钮。 点击后读取当前草稿把草稿重写为结构更清晰的提示词，并直接写回输入框。 长文本支持（输入框架构修复）： 修复 composer 的长文本缺陷 |
| 351 | [wenbobodley/dsh-guandan](https://github.com/wenbobodley/dsh-guandan) | 2 | 2026-08-23 | 2026-08-24 | 掼蛋 Guandan card game plugin for DeepSeek Harness (DSH) - 掼蛋-中联储卫 / GUANDAN-中联储卫 |
| 352 | [Whale-Zhang/dsh-complete-chime](https://github.com/Whale-Zhang/dsh-complete-chime) | 2 | 2026-08-23 | 2026-08-23 | DSH plugin: play a chime when a conversation turn finishes. Built-in tones plus custom upload in Settings → Plugins. |
| 353 | [Whale-Zhang/dsh-cron-tasks](https://github.com/Whale-Zhang/dsh-cron-tasks) | 2 | 2026-08-24 | 2026-08-24 | Scheduled tasks for DeepSeek Harness: sidebar jobs, isolated run history, cron/at schedules. |
| 354 | [win4r/dsh-pi-review](https://github.com/win4r/dsh-pi-review) | 2 | 2026-08-23 | 2026-08-23 | Read-only Pi Agent code review plugin for DeepSeek Harness |
| 355 | [wowyuarm/dsh-agent-team](https://github.com/wowyuarm/dsh-agent-team) | 2 | 2026-08-23 | 2026-08-24 | Help humans organize tasks and let agents collaborate: durable Workspaces, Channels, Tasks, and managed Agent members for DeepSeek Harness |
| 356 | [x1shang/dsh-koin-lily-news](https://github.com/x1shang/dsh-koin-lily-news) | 2 | 2026-08-21 | 2026-08-26 | 菲奖得主强推的百合新闻订阅DSH插件 |
| 357 | [Xinyi21yf/deepseek-harness-plugins](https://github.com/Xinyi21yf/deepseek-harness-plugins) | 2 | 2026-08-23 | 2026-08-24 | Personal DeepSeek Harness plugins, designs, and learning notes |
| 358 | [XuXcode/dsh-loghud](https://github.com/XuXcode/dsh-loghud) | 2 | 2026-08-23 | 2026-08-23 | Live Spring Boot error HUD with opt-in AI diagnosis for DeepSeek Harness |
| 359 | [yamingmou/dsh-retrace](https://github.com/yamingmou/dsh-retrace) | 2 | 2026-08-19 | 2026-08-25 | Recall (撤回), edit-and-resend (编辑重发) and regenerate (重新生成) for DeepSeek Harness conversation messages — Web and Desktop plugin |
| 360 | [yangdongzhen590/dsh-knj-scheduler](https://github.com/yangdongzhen590/dsh-knj-scheduler) | 2 | 2026-08-23 | 2026-08-24 | Cron task scheduler for DeepSeek Harness: scheduled sessions with your prompt, workspace-aware placement, paginated execution history, open-session from the panel. |
| 361 | [yhfgyyf/dsh-guardian-mode](https://github.com/yhfgyyf/dsh-guardian-mode) | 2 | 2026-08-23 | 2026-08-23 | Guardian preset for DeepSeek Harness with independent persistent Codex auditing |
| 362 | [YiMlT/dsh-notify-yimit](https://github.com/YiMlT/dsh-notify-yimit) | 2 | 2026-08-22 | 2026-08-22 | DeepSeek Harness 通知插件:在 **任务完成 / 任务出错 / 运行中 / 等待审批 / 等待回答** 时提醒用户。 通知标题为对话标题;系统通知与自定义通知均支持**点击跳转到对应会话**。 |
| 363 | [yingzaicc/dsh-editor-selection](https://github.com/yingzaicc/dsh-editor-selection) | 2 | 2026-08-23 | 2026-08-23 | 让 DSH 理解"用户此刻在编辑器里看着什么"。当你在编辑器中选中某个文件或行区间,后续对话自动聚焦于它——通过 @path:10-25 的环境知会行注入,而不是把文件内容塞进上下文。 |
| 364 | [yishengjun8/dsh-workspace-studio](https://github.com/yishengjun8/dsh-workspace-studio) | 2 | 2026-08-17 | 2026-08-26 | 允许显示工作区的文件树、浏览文件内容、并且允许对话中嵌入引用的文件内容、自由切换思维分支视图，目标是和VSCode相类似的开发体验 |
| 365 | [Young4ever33/dsh-token-attention](https://github.com/Young4ever33/dsh-token-attention) | 2 | 2026-08-22 | 2026-08-22 | Token Check · 词元管理：DeepSeek Harness (DSH) 的 token 注意力管理面板——按任务/日/周/月记录 token 消耗与费用（命中/未命中/输出/推理），支持 DeepSeek 峰谷计价，并给出换对话、写 hand-off 的执行时机建议。 |
| 366 | [yu502950715yang/dsh-use-wallpaper](https://github.com/yu502950715yang/dsh-use-wallpaper) | 2 | 2026-08-17 | 2026-08-24 | DSH Web GUI 壁纸背景插件：从本机 Wallpaper Engine 壁纸库加载背景，wasm 渲染 scene 壁纸 |
| 367 | [zaimokuza-yoshiteru/dsh-acp-adapter](https://github.com/zaimokuza-yoshiteru/dsh-acp-adapter) | 2 | 2026-08-24 | 2026-08-24 | Use AI agents from the DSH session UI. |
| 368 | [zeropointnine/dsh-compact-and-branch](https://github.com/zeropointnine/dsh-compact-and-branch) | 2 | 2026-08-23 | 2026-08-24 | Compact a session and continue the work in a new one |
| 369 | [zhangdong456/dsh-prompt-presets](https://github.com/zhangdong456/dsh-prompt-presets) | 2 | 2026-08-21 | 2026-08-22 | Prompt Presets to manage your library  |
| 370 | [zhaoan2308184882-spec/deepseek-harness-plugins](https://github.com/zhaoan2308184882-spec/deepseek-harness-plugins) | 2 | 2026-08-24 | 2026-08-24 | Unofficial community plugins for DeepSeek Harness: Codex provider and role model router |
| 371 | [zhiyaoli0221/dsh-finance-db](https://github.com/zhiyaoli0221/dsh-finance-db) | 2 | 2026-08-22 | 2026-08-23 | Read-only market data for DeepSeek Harness. Ask about a stock, and let DSH call the data tools directly. \| 为 DeepSeek Harness 提供只读金融市场数据。让 DSH 直接调用工具查询行情。 |
| 372 | [zmm863-commits/dsh-paperclip](https://github.com/zmm863-commits/dsh-paperclip) | 2 | 2026-08-16 | 2026-08-25 | DSH Web GUI paperclip button: a single 📎 button in the composer that opens a file picker (drag & drop supported) and inserts file contents into the textarea. 在 DSH Web 输入框右侧添加回形针按钮，点击选择/拖拽文件，内容自动插入输入框。 |
| 373 | [Zn-Dk/dsh-session-repair](https://github.com/Zn-Dk/dsh-session-repair) | 2 | 2026-08-22 | 2026-08-22 | DSH Web 会话诊断、可信备份与一键安全修复插件。 |
| 374 | [ztmajor/DSCoder](https://github.com/ztmajor/DSCoder) | 2 | 2026-08-20 | 2026-08-24 | 这是我给自己写的一个小工具——现在有太多 dsh-desktop 类项目，插件越装越多，越来越重，我就想要个干净的 AI 编码壳，里面有我需要的最基本的功能。于是有了 DSCoder。主要供我自己日常使用，如果你也有类似的需求，也欢迎取用。 |
| 375 | [0QwQ0/dsh-discord-richpresence](https://github.com/0QwQ0/dsh-discord-richpresence) | 1 | 2026-08-22 | 2026-08-24 | dsh-plugin: push vague, user-configurable DSH interaction states to local Discord as Rich Presence |
| 376 | [1024483906-pixel/dsh-novel-reader](https://github.com/1024483906-pixel/dsh-novel-reader) | 1 | 2026-08-25 | 2026-08-25 | DSH休闲阅读文本插件 |
| 377 | [2327644800/dsh-usage-analytics](https://github.com/2327644800/dsh-usage-analytics) | 1 | 2026-08-22 | 2026-08-22 | Personal usage analytics & activity dashboard for the DeepSeek Harness (dsh) web GUI: token totals, contribution heatmap, model share, insights. Local-only, metadata only. |
| 378 | [240xu/dsh-websearch](https://github.com/240xu/dsh-websearch) | 1 | 2026-08-20 | 2026-08-22 | Unified web search provider for DSH |
| 379 | [2522669008-zcy/dsh-time-prefix](https://github.com/2522669008-zcy/dsh-time-prefix) | 1 | 2026-08-24 | 2026-08-25 | 在每条用户消息前自动插入 【2026/08/23，22:36】 这样的时间文本 |
| 380 | [6HOLLIS/DSH-Hiyuki-Frost-Sakura](https://github.com/6HOLLIS/DSH-Hiyuki-Frost-Sakura) | 1 | 2026-08-24 | 2026-08-25 | Immersive Hiyuki dual-form skin for DeepSeek Harness Web, with frost/sakura transitions, themed controls, and native DSH layout. |
| 381 | [937862061/dsh-project-workbench](https://github.com/937862061/dsh-project-workbench) | 1 | 2026-08-22 | 2026-08-23 | DeepSeek Harness Web 本地项目工作台：按项目、需求组和会话管理原生对话，并以渐进式共享记忆自动衔接组内上下文。  Local DeepSeek Harness Web plugin that organizes native conversations by project and requirement group, with progressive shared memory automatically carried into each group conversation. |
| 382 | [988hj7tczd-oss/dsh-a11y-scan](https://github.com/988hj7tczd-oss/dsh-a11y-scan) | 1 | 2026-08-24 | 2026-08-24 | DSH native accessibility (WCAG) scanner: runs axe-core over local HTML files / build output / URLs and reports violations as Markdown/HTML/JSON |
| 383 | [988hj7tczd-oss/dsh-asciinema](https://github.com/988hj7tczd-oss/dsh-asciinema) | 1 | 2026-08-24 | 2026-08-24 | DSH plugin: record terminal/tool output as asciinema v2 (.cast), replay with an offline embedded player, and export HTML |
| 384 | [988hj7tczd-oss/dsh-dep-vuln-scan](https://github.com/988hj7tczd-oss/dsh-dep-vuln-scan) | 1 | 2026-08-24 | 2026-08-24 | Scan project lockfiles (npm/pnpm/yarn/pip/go/cargo/maven/gradle) against the free OSV API and report confirmed dependency vulnerabilities with fix versions |
| 385 | [988hj7tczd-oss/dsh-invoice-tools](https://github.com/988hj7tczd-oss/dsh-invoice-tools) | 1 | 2026-08-24 | 2026-08-24 | DSH native tools: parse Chinese e-invoice PDFs into structured JSON with amount cross-check, and generate expense reports (Markdown / xlsx) |
| 386 | [988hj7tczd-oss/dsh-lsp-packs](https://github.com/988hj7tczd-oss/dsh-lsp-packs) | 1 | 2026-08-24 | 2026-08-24 | Out-of-the-box per-language LSP configuration packs for DeepSeek Harness: 12 Cordis plugins (one per language) reusing the shared @deepseek-ai/dsh-lsp-stdio + @deepseek-ai/dsh-tool-lsp base |
| 387 | [988hj7tczd-oss/dsh-mcp-tunnel](https://github.com/988hj7tczd-oss/dsh-mcp-tunnel) | 1 | 2026-08-24 | 2026-08-24 | DSH plugin: expose a local MCP server to remote agents via outbound-only tunnel (mcp-proxy + cloudflared Quick Tunnel) and register the public URL into dsh-mcp-client |
| 388 | [988hj7tczd-oss/dsh-modernize-code](https://github.com/988hj7tczd-oss/dsh-modernize-code) | 1 | 2026-08-24 | 2026-08-24 | DSH skill pack: legacy code modernization workflow (preflight -> assess -> map -> transform) with Cordis mount plugin, offline Python scripts and smoke tests |
| 389 | [988hj7tczd-oss/dsh-pr-description](https://github.com/988hj7tczd-oss/dsh-pr-description) | 1 | 2026-08-24 | 2026-08-24 | DSH native tool: analyze the current branch diff and generate a Conventional Commits PR title, description and self-review checklist |
| 390 | [988hj7tczd-oss/dsh-receipts](https://github.com/988hj7tczd-oss/dsh-receipts) | 1 | 2026-08-24 | 2026-08-24 | Mine local DSH session logs (JSONL) into personal usage & impact receipts: Markdown day/week/month reports plus a self-contained HTML receipt |
| 391 | [988hj7tczd-oss/dsh-workflow-templates](https://github.com/988hj7tczd-oss/dsh-workflow-templates) | 1 | 2026-08-24 | 2026-08-24 | DSH preset workflow template library: 12 reusable orchestration script templates with list/search/run/validate tools |
| 392 | [aa2246740/dsh-auto-review](https://github.com/aa2246740/dsh-auto-review) | 1 | 2026-08-20 | 2026-08-25 | Codex-style Auto-review and Approve for me mode for DeepSeek Harness |
| 393 | [aa2246740/dsh-creator-mode-plus](https://github.com/aa2246740/dsh-creator-mode-plus) | 1 | 2026-08-20 | 2026-08-25 | Fail-closed Creator Mode+ bridge for DeepSeek Harness, supervised externally by DSHX. |
| 394 | [aa2246740/dsh-gateway](https://github.com/aa2246740/dsh-gateway) | 1 | 2026-08-25 | 2026-08-25 | One DSH Host, one messaging Gateway. Bring your own Slack and Feishu apps. |
| 395 | [aa2246740/dsh-oauth-login](https://github.com/aa2246740/dsh-oauth-login) | 1 | 2026-08-15 | 2026-08-25 | Pi-native multi-provider OAuth login for DeepSeek Harness. Independent store — never touches official CLI auth files. |
| 396 | [ABccgh/dsh-agent-studio](https://github.com/ABccgh/dsh-agent-studio) | 1 | 2026-08-23 | 2026-08-23 | DSH 智能体与插件开发预设：为 DeepSeek Harness 构建 agent preset 与预设本地插件的开发智能体，含 preset_* 工具集、插件/技能脚手架、静态审查与挂载校验。 |
| 397 | [Abel-86/task-chime](https://github.com/Abel-86/task-chime) | 1 | 2026-08-22 | 2026-08-23 | DSH task chime: play local sounds for approval/permission requests and task completion, configurable from the Web GUI. DSH 任务提示音插件 |
| 398 | [ac0033/dsh-ctm](https://github.com/ac0033/dsh-ctm) | 1 | 2026-08-16 | 2026-08-25 | dsh 插件：CTM 上下文/终端管理，把模型上下文变成可见、可编辑、可评分的一等对象 |
| 399 | [ADDD1118/dsh-balance](https://github.com/ADDD1118/dsh-balance) | 1 | 2026-08-23 | 2026-08-23 | DeepSeek Harness (dsh) balance card — floating glass card (estimated days, balance, conversation usage/cost) + adjustable-size settings card |
| 400 | [AGSQ11/dsh-completion-gate](https://github.com/AGSQ11/dsh-completion-gate) | 1 | 2026-08-22 | 2026-08-22 | Evidence-backed production-readiness barrier for DeepSeek Harness. |
| 401 | [ai-yucheng/dsh-composer-image-tools](https://github.com/ai-yucheng/dsh-composer-image-tools) | 1 | 2026-08-21 | 2026-08-22 | DSH 聊天输入框图片工具(自研):上传图片 + 区域截图,注入草稿图片轨。零依赖,纯客户端+Electron desktopCapturer 截屏。 |
| 402 | [aiworkskills/deepseek-harness-server](https://github.com/aiworkskills/deepseek-harness-server) | 1 | 2026-08-18 | 2026-08-26 | 一个可以接入应用系统的deepseek harness插件，让原有的应用系统快速接入智能体能力 |
| 403 | [ajuwm/dsh-roleplay-plugin](https://github.com/ajuwm/dsh-roleplay-plugin) | 1 | 2026-08-23 | 2026-08-23 | 以角色扮演为主体、桌宠为附加功能的 DeepSeek Harness 插件 |
| 404 | [AKS1st/dock-media](https://github.com/AKS1st/dock-media) | 1 | 2026-08-21 | 2026-08-22 | Media player for the DSH dock: plays audio (music player) and video (fullscreen) files, streamed over HTTP Range. |
| 405 | [alanpaul1969/dsh-agent-sticky-note](https://github.com/alanpaul1969/dsh-agent-sticky-note) | 1 | 2026-08-23 | 2026-08-23 | 📌 Sticky-note plugin for DeepSeek Harness — agent notices & pending decisions visible in the Web GUI (Tailscale-friendly) |
| 406 | [AlexKaiqi/dsh-realtime-voice](https://github.com/AlexKaiqi/dsh-realtime-voice) | 1 | 2026-08-20 | 2026-08-24 | Full-duplex realtime voice-agent plugin for DeepSeek Harness, with OpenAI Realtime (WebRTC) and Doubao Duplex (WebSocket) adapters. |
| 407 | [AlexZhou19871030/dsh-cron-scheduler](https://github.com/AlexZhou19871030/dsh-cron-scheduler) | 1 | 2026-08-22 | 2026-08-23 | dsh-cron-scheduler |
| 408 | [Alphainfix/wechat-clawbot](https://github.com/Alphainfix/wechat-clawbot) | 1 | 2026-08-24 | 2026-08-24 | 💬 A DeepSeek Harness plugin that brings your DSH agent into WeChat — chat with it from anywhere: native photo understanding, two-way file transfer, long-term memory, scheduled reminders, and permission approvals answered right in the chat. |
| 409 | [andyfan1094/dsh-codebase-memory](https://github.com/andyfan1094/dsh-codebase-memory) | 1 | 2026-08-21 | 2026-08-22 | DSH bundle that bridges the Codebase Memory MCP code knowledge graph into DSH via the official @deepseek-ai/dsh-mcp-client. |
| 410 | [andyfan1094/dsh-feishu](https://github.com/andyfan1094/dsh-feishu) | 1 | 2026-08-21 | 2026-08-22 | DSH Feishu self-built app integration: WebSocket inbound messages, OK-reaction acknowledgement, and turn replies on the original chat. |
| 411 | [andyfan1094/dsh-github](https://github.com/andyfan1094/dsh-github) | 1 | 2026-08-21 | 2026-08-22 | GitHub authentication and local Git workflow plugin for the dsh web GUI: accounts, repository browsing, clone, pull, push, status, commit, and a settings panel. |
| 412 | [andyfan1094/dsh-winrm](https://github.com/andyfan1094/dsh-winrm) | 1 | 2026-08-21 | 2026-08-22 | Remote Windows administration for the dsh web GUI: WinRM/PowerShell Remoting host config, PowerShell exec, streaming console, service and process management, base64-chunked file transfer, cluster execution, plus agent tools (winrm_list, winrm_exec, winrm_service, winrm_process, winrm_upload, winrm_download, winrm_cluster). Standalone Cordis plugin. |
| 413 | [anonRTtty/DSH-mobile-remote-mode-plugin](https://github.com/anonRTtty/DSH-mobile-remote-mode-plugin) | 1 | 2026-08-25 | 2026-08-25 | DSH (DeepSeek Harness) mobile remote mode plugin - LAN discovery, QR pairing, Level-1 observer and Level-2 remote prompt from Android/iOS phones and any browser. Multi-platform, early development (Dev0.1). |
| 414 | [anweat/dsh-context-console](https://github.com/anweat/dsh-context-console) | 1 | 2026-08-22 | 2026-08-22 | Complete context workbench for DeepSeek Harness: trajectory, inventory, cache history, message forge, and session-log recovery |
| 415 | [Anyway-one/dsh-image-gen](https://github.com/Anyway-one/dsh-image-gen) | 1 | 2026-08-25 | 2026-08-25 | DeepSeek Harness Image2 生图插件，通过第三方 OpenAI Images 兼容接口调用 gpt-image-2，只需配置  API Key 和 baseURL。 |
| 416 | [aorucshiea/dsh-easy-start](https://github.com/aorucshiea/dsh-easy-start) | 1 | 2026-08-25 | 2026-08-26 | DSH Web browser lifecycle: ask/close/keep service on browser close, one-click restart with auto refresh |
| 417 | [aorucshiea/dsh-omnipotent-preset](https://github.com/aorucshiea/dsh-omnipotent-preset) | 1 | 2026-08-24 | 2026-08-25 | Omnipotent agent preset for DeepSeek Harness: Standard/PTC/Minimal + routing modes |
| 418 | [Ardig24/dsh-trajectory-ablation](https://github.com/Ardig24/dsh-trajectory-ablation) | 1 | 2026-08-25 | 2026-08-26 | Finds the actual cause of an agent failure by reconstructing, diffing, and ablating its context - a DeepSeek Harness plugin. |
| 419 | [Ares-song-RD/dsh-desktop-pet](https://github.com/Ares-song-RD/dsh-desktop-pet) | 1 | 2026-08-25 | 2026-08-25 | 桌宠插件：在 DeepSeek Harness Web 界面右下角悬浮一只可拖拽、会眨眼摇尾的小猫。A cute desktop pet plugin for the DeepSeek Harness Web GUI. |
| 420 | [ArmyWas/dsh-plugin-reducer](https://github.com/ArmyWas/dsh-plugin-reducer) | 1 | 2026-08-18 | 2026-08-26 | External CLI that finds a 1-minimal DeepSeek Harness plugin set reproducing a profile failure. |
| 421 | [artwar2020/dsh-model-center](https://github.com/artwar2020/dsh-model-center) | 1 | 2026-08-25 | 2026-08-25 | DSH 模型中心插件：免费模型目录 / 真免费实测 / 价格余额 / 一键切换 / 用量统计 — Model center plugin for DeepSeek Harness |
| 422 | [ateen18/dsh-plugin-security-review](https://github.com/ateen18/dsh-plugin-security-review) | 1 | 2026-08-18 | 2026-08-24 | Security review gate for DeepSeek Harness (dsh) plugins: static pre-install vetting of malicious code, vulnerabilities and supply-chain risks (with deobfuscation decoding), runtime audit, optional tool-call guard, and a one-click web review/install/uninstall panel. |
| 423 | [B1lli/dsh-plugin-bench](https://github.com/B1lli/dsh-plugin-bench) | 1 | 2026-08-22 | 2026-08-23 | Evidence-backed, type-aware quality scorecards for DeepSeek Harness plugins. |
| 424 | [bailynlove/web-search-opencode-responses](https://github.com/bailynlove/web-search-opencode-responses) | 1 | 2026-08-21 | 2026-08-22 | dsh WebSearchProvider over the OpenCode Zen Go Responses API server-side web_search tool |
| 425 | [Baisbt/dsh-GreaterClarity-plugin](https://github.com/Baisbt/dsh-GreaterClarity-plugin) | 1 | 2026-08-23 | 2026-08-23 | 对话快速定位，AI头像，支持导出对话流内容 |
| 426 | [banttethai-ops/dsh-right-editor](https://github.com/banttethai-ops/dsh-right-editor) | 1 | 2026-08-21 | 2026-08-22 | Right-docked file panel for DSH Web: browse any directory and view/edit text, images, Office (docx/xlsx/pptx) and PDF documents. Uses local Python for parsing. |
| 427 | [bao-hp/dsh-check-update](https://github.com/bao-hp/dsh-check-update) | 1 | 2026-08-24 | 2026-08-24 | Check for DSH updates with changelog and backup. |
| 428 | [baosfeng/my-dsh-plugins](https://github.com/baosfeng/my-dsh-plugins) | 1 | 2026-08-22 | 2026-08-22 | DSH（DeepSeek Harness）插件集合仓库：文件活动、思考增强、Mermaid 渲染、通知提醒、插件守护、Skill 管理、任务可靠性、插件开发模式等 8 个插件，独立版本、GitHub Release 发布 |
| 429 | [beartackler/dsh-bridge](https://github.com/beartackler/dsh-bridge) | 1 | 2026-08-25 | 2026-08-26 | Your harness muscle memory, verified and installed into DeepSeek Harness - familiar commands, connectors flow, and a trust-verified plugin catalog |
| 430 | [better-er/dsh-live-token-stats](https://github.com/better-er/dsh-live-token-stats) | 1 | 2026-08-21 | 2026-08-26 | dsh·实时 Token 统计·溺水检测插件 |
| 431 | [BharathBillawa/dsh-tool-ddgs](https://github.com/BharathBillawa/dsh-tool-ddgs) | 1 | 2026-08-22 | 2026-08-22 | DuckDuckGo web search and URL fetch tools for DeepSeek Harness, no API key required. Provides web_search (via ddgs) and   web_fetch (via trafilatura) as a drop-in bundle |
| 432 | [bingfengaaaaa/dsh-jj-vcs](https://github.com/bingfengaaaaa/dsh-jj-vcs) | 1 | 2026-08-22 | 2026-08-22 | Jujutsu version-control plugin and skill for DeepSeek Harness multi-agent teams |
| 433 | [bitterSmilezzz/dsh-plugins](https://github.com/bitterSmilezzz/dsh-plugins) | 1 | 2026-08-18 | 2026-08-25 | DSH 插件伞仓库（DSH Plugin Umbrella）— 所有新增插件的共同遵循仓库：承载插件契约（Pi / DSH 官方 / DSH-Store 准入 / dsh-std 协议）+ 按契约自动校验自有插件（GitHub Actions），经验档案按主题归档。 |
| 434 | [blackdm666/dsh-plugin-88api-image](https://github.com/blackdm666/dsh-plugin-88api-image) | 1 | 2026-08-22 | 2026-08-22 | 统一接入 Image2 与 Nano Banana 四款模型，覆盖文生图、多参考图编辑、2K/4K 输出、顺序批量任务、默认模型持久化和脱敏 Key 配置。 |
| 435 | [botaochen840-lgtm/fatfish-pet-smart-companion](https://github.com/botaochen840-lgtm/fatfish-pet-smart-companion) | 1 | 2026-08-22 | 2026-08-22 | FatFish Pet Smart Companion - 自包含智能桌面桌宠（改编自 whale-girl），下载即用，可选真连 DeepSeek Harness |
| 436 | [bowang-lab/dsh-medomni](https://github.com/bowang-lab/dsh-medomni) | 1 | 2026-08-19 | 2026-08-22 | deepseek harness plugin for medical image analysis |
| 437 | [Boy-Grid/dsh-multi-folder-workspace](https://github.com/Boy-Grid/dsh-multi-folder-workspace) | 1 | 2026-08-22 | 2026-08-23 | Multi-folder workspaces for DeepSeek Harness: one workspace spanning several folders, with sessions able to read and write every member. Core patch set + plugin + a one-command npx launcher. |
| 438 | [buguoshixc/dsh-user-message-navigator](https://github.com/buguoshixc/dsh-user-message-navigator) | 1 | 2026-08-23 | 2026-08-23 | Codex-style user-message navigation sidebar for DeepSeek Harness Web |
| 439 | [Carrick-K7/dsh-ai-quota](https://github.com/Carrick-K7/dsh-ai-quota) | 1 | 2026-08-24 | 2026-08-24 | DeepSeek Harness plugin: AI subscription quotas & balances (Codex, Kimi, DeepSeek, OpenCode Go) — model tool, Settings page, composer chip |
| 440 | [caseyyy/dsh-goal-planner](https://github.com/caseyyy/dsh-goal-planner) | 1 | 2026-08-25 | 2026-08-25 | 目标驱动的每日任务计划器：多目标任务数据 + Web 每日预览面板，与微信提醒推送共享数据 · Goal-driven daily task planner for DSH: multi-goal tasks + daily preview panel, one data file with the WeChat reminder pipeline. |
| 441 | [Castor6/BrowserRig](https://github.com/Castor6/BrowserRig) | 1 | 2026-08-21 | 2026-08-26 | Open-source local driver for trusted agents to control your existing signed-in Chromium browser without browser-wide remote-debugging approval. |
| 442 | [cczzyy-cn/c-vision](https://github.com/cczzyy-cn/c-vision) | 1 | 2026-08-22 | 2026-08-23 | DeepSeek Harness (DSH) 视觉插件 —— 给智能体屏幕/窗口视觉 + 电脑使用能力（see/ocr/list_windows + 鼠标键盘操作），跨语言调用捆绑的 Python cvision，Windows / macOS 可用。 |
| 443 | [chenbin-dev/dsh-scan-mcp](https://github.com/chenbin-dev/dsh-scan-mcp) | 1 | 2026-08-23 | 2026-08-23 | 能够扫描本地claudecode、codex、codebuddy等Agent配置过的mcp工具的插件 |
| 444 | [chengdb/dsh-plugin-capability-panel](https://github.com/chengdb/dsh-plugin-capability-panel) | 1 | 2026-08-21 | 2026-08-26 | 在 Web GUI 里可视化管理项目的全部能力——Skills、MCP 服务器、快捷消息， 全部支持项目级 / 全局级双作用域，全部可以不离开浏览器完成安装、启停与分发 |
| 445 | [chenpengye/dsh-balance-local](https://github.com/chenpengye/dsh-balance-local) | 1 | 2026-08-21 | 2026-08-22 | DeepSeek API balance plugin for DeepSeek Harness (dsh): Settings-page panel + composer badge. Key stays on the Host; browser gets sanitized balance only. |
| 446 | [chenpengye/dsh-balance-whale](https://github.com/chenpengye/dsh-balance-whale) | 1 | 2026-08-21 | 2026-08-22 | 🐳 Floating DeepSeek API balance widget for DeepSeek Harness (dsh) with a whale-girl icon. Key stays on the Host; browser gets sanitized balance only. |
| 447 | [ChenSiyun1234/dsh-tray-windows](https://github.com/ChenSiyun1234/dsh-tray-windows) | 1 | 2026-08-22 | 2026-08-22 | 把 DeepSeek Harness (dsh web) 变成真正的 Windows 桌面应用：托盘控制、独立应用窗口、退出即彻底停止后端（无残留进程）。非官方项目。 |
| 448 | [chenzhi-clude/dsh-hooks-pack](https://github.com/chenzhi-clude/dsh-hooks-pack) | 1 | 2026-08-21 | 2026-08-22 | One-click Claude Code and Codex hooks for DeepSeek Harness: auto-discovers your existing hooks config and runs it on the official bridge plugins. |
| 449 | [cherrchen/dsh-client-ui-details-host](https://github.com/cherrchen/dsh-client-ui-details-host) | 1 | 2026-08-24 | 2026-08-25 | 可移植 DSH Client Details 栏基础设施，在 AppFrame 详情列承载活动 surface；DeepSeek Harness Desktop 内置。 / Portable DSH Client details-column infrastructure for one active AppFrame surface; built into DeepSeek Harness Desktop. |
| 450 | [cherrchen/dsh-plugin-git](https://github.com/cherrchen/dsh-plugin-git) | 1 | 2026-08-23 | 2026-08-25 | DSH Git 仓库服务与 Client UI 插件，依赖 Details Host；DeepSeek Harness Desktop 预装。 / DSH Git repository service and client UI; requires Details Host; pre-installed in DeepSeek Harness Desktop. |
| 451 | [cherrchen/dsh-theme-studio](https://github.com/cherrchen/dsh-theme-studio) | 1 | 2026-08-26 | 2026-08-26 | 可移植的 DSH/Cordis 主题插件：内置配色浏览、预览、应用与持久化；DeepSeek Harness Desktop 预装。 / Portable DSH/Cordis theme overlay plugin with builtin palettes, preview, apply, and persistence; pre-installed in DeepSeek Harness Desktop. |
| 452 | [Chillizu/mop-plugins](https://github.com/Chillizu/mop-plugins) | 1 | 2026-08-15 | 2026-08-26 | MiOpIIk：DeepSeek Harness 单职责插件集 + 四层 agent 工作流 preset（npm: dsh-miopiik） |
| 453 | [chinazkk/dsh-task-panel](https://github.com/chinazkk/dsh-task-panel) | 1 | 2026-08-14 | 2026-08-26 | DSH Web task panel for queued sub-agent execution, scheduled runs, auto review, acceptance, rework, and historical session context. |
| 454 | [Chinesezjc/dsh-tool-owned-render](https://github.com/Chinesezjc/dsh-tool-owned-render) | 1 | 2026-08-14 | 2026-08-24 | Design note and interactive prototype for tool-owned render: each tool owns its own result presentation, composing shared layout primitives instead of a central render-kind union. |
| 455 | [CJL-1995/dsh-session-health](https://github.com/CJL-1995/dsh-session-health) | 1 | 2026-08-23 | 2026-08-24 | a plugin that can judge your Agent session is healthy or not |
| 456 | [cking000bigdemon/dsh-acp-interactive](https://github.com/cking000bigdemon/dsh-acp-interactive) | 1 | 2026-08-25 | 2026-08-25 | 面向 Zed 等编辑器的 DeepSeek Harness 交互式 ACP 插件。 |
| 457 | [Cloud-J/dsh-chat-jumper](https://github.com/Cloud-J/dsh-chat-jumper) | 1 | 2026-08-24 | 2026-08-24 | dsh对话导航 |
| 458 | [cn-zhangpeng/dsh-shanhai-stats](https://github.com/cn-zhangpeng/dsh-shanhai-stats) | 1 | 2026-08-22 | 2026-08-23 | 山海系列 DeepSeek Harness 用量统计插件：总量徽章、每日走势、GitHub 风格热力图、按模型/提供商分组明细 |
| 459 | [CochraneK/dsh-gate-game-plugin](https://github.com/CochraneK/dsh-gate-game-plugin) | 1 | 2026-08-24 | 2026-08-24 | Logo-eating mini-game + one-click lock button for DeepSeek Harness web UI |
| 460 | [code4lala/dsh-plugin-workspace-path](https://github.com/code4lala/dsh-plugin-workspace-path) | 1 | 2026-08-25 | 2026-08-26 | 可用于在 DSH Web 侧边栏快速查看每个工作区的完整目录路径，减少同名工作区混淆。它作为 DSH 客户端插件安装到 Web profile，在标题下方注入路径副标题并自动换行，支持热加载、位置匹配和重命名或排序后实时同步。 |
| 461 | [coeasy/dsh-go](https://github.com/coeasy/dsh-go) | 1 | 2026-08-23 | 2026-08-24 | DeepSeek Harness 插件市场导航站 |
| 462 | [coldfish486/dsh-anime25d-pets](https://github.com/coldfish486/dsh-anime25d-pets) | 1 | 2026-08-23 | 2026-08-22 | Anime2.5DRig × DSH 桌宠：借助see-through，只凭一张干净背景的图像，即可获得带自动装配、发丝物理、表情动画和状态镜像的桌宠 |
| 463 | [crazy-L118/dsh-desktop-notify](https://github.com/crazy-L118/dsh-desktop-notify) | 1 | 2026-08-25 | 2026-08-26 | Desktop notification plugin for dsh: get a native OS toast when the AI finishes its reply. Toggle lives in dsh Settings → General. |
| 464 | [czx1111/dsh-plugin-manager](https://github.com/czx1111/dsh-plugin-manager) | 1 | 2026-08-22 | 2026-08-25 | dsh-plugin-manager |
| 465 | [daizihan233/dsh-my-go](https://github.com/daizihan233/dsh-my-go) | 1 | 2026-08-20 | 2026-08-22 | My tasks, where to GO????? |
| 466 | [danhcng3822f/dsh-mcp-kimicodeandmgr](https://github.com/danhcng3822f/dsh-mcp-kimicodeandmgr) | 1 | 2026-08-21 | 2026-08-22 | MCP engine and manager for DeepSeek Harness. Fork of yangfch3/dsh-mcp-mgr, MCP layer rebuilt on kimi-code's architecture: self-contained engine, three config layers, transport-driven status. |
| 467 | [DaoCaoRenH/dsh-openai-responses-bridge](https://github.com/DaoCaoRenH/dsh-openai-responses-bridge) | 1 | 2026-08-19 | 2026-08-22 | DeepSeek Harness plugin for third-party OpenAI Responses and native Gemini APIs, with custom providers, model discovery, and hosted web search. |
| 468 | [dat-lequoc/dsh-supervisor](https://github.com/dat-lequoc/dsh-supervisor) | 1 | 2026-08-22 | 2026-08-22 | Always-on supervisor agent bundle for DeepSeek Harness: main-agent preset + schedule overlay, one dsh plugin add away |
| 469 | [DaXiGua732/start-dsh](https://github.com/DaXiGua732/start-dsh) | 1 | 2026-08-22 | 2026-08-22 | 一个能够直接快速启动DSH的ps脚本，具备高峰时段检测功能，高峰时段启动时不会直接进入DSH，反之直接进入，帮助个人开发者省钱省力 |
| 470 | [ddtcorex/dsh-maestro-config](https://github.com/ddtcorex/dsh-maestro-config) | 1 | 2026-08-25 | 2026-08-26 | Maestro Config — shared settings service for the dsh-maestro-* suite over the single namespaced store (~/.dsh/maestro/settings.json) |
| 471 | [ddtcorex/dsh-maestro-govard](https://github.com/ddtcorex/dsh-maestro-govard) | 1 | 2026-08-25 | 2026-08-26 | Thin bridge exposing the Govard CLI to DeepSeek Harness agents as tools. |
| 472 | [ddtcorex/dsh-maestro-guard](https://github.com/ddtcorex/dsh-maestro-guard) | 1 | 2026-08-25 | 2026-08-26 | Host-only safety gate for DeepSeek Harness: approval store, secret redaction, permission policy, waterfall pre-execute integration. |
| 473 | [ddtcorex/dsh-maestro-meta](https://github.com/ddtcorex/dsh-maestro-meta) | 1 | 2026-08-24 | 2026-08-26 | Maestro Harness meta-bundle: one plugin to install the whole Govard + DSH harness |
| 474 | [ddtcorex/dsh-maestro-mobile](https://github.com/ddtcorex/dsh-maestro-mobile) | 1 | 2026-08-24 | 2026-08-25 | Portrait & mobile adaptation for the DeepSeek Harness Web UI — overlay drawer, full-width conversation, sheet dialogs, safe-area handling. Below 1024px it adapts; at ≥1024px it is a no-op. |
| 475 | [ddtcorex/dsh-maestro-notifier](https://github.com/ddtcorex/dsh-maestro-notifier) | 1 | 2026-08-25 | 2026-08-26 | Maestro Notifier — pluggable notifier service for DeepSeek Harness (Telegram first; registry open to further providers) |
| 476 | [ddtcorex/dsh-maestro-observe](https://github.com/ddtcorex/dsh-maestro-observe) | 1 | 2026-08-25 | 2026-08-26 | Observability / debug tooling for DeepSeek Harness: trace, cost, and health capture + client dashboard. |
| 477 | [ddtcorex/dsh-maestro-remote](https://github.com/ddtcorex/dsh-maestro-remote) | 1 | 2026-08-25 | 2026-08-26 | Remote access for DeepSeek Harness via cloudflared tunnel + proxy, with PIN auth and Telegram notifications. |
| 478 | [ddtcorex/dsh-maestro-review](https://github.com/ddtcorex/dsh-maestro-review) | 1 | 2026-08-25 | 2026-08-26 | Pluggable merge-request review pipeline for DeepSeek Harness (webhook → orchestrator → findings) with GitLab + GitHub providers. |
| 479 | [DecarbonizedGlucose/dsh-memory-note](https://github.com/DecarbonizedGlucose/dsh-memory-note) | 1 | 2026-08-17 | 2026-08-23 | Lightweight local cross-session memory for DeepSeek Harness |
| 480 | [deluo/dsh-usage-display](https://github.com/deluo/dsh-usage-display) | 1 | 2026-08-22 | 2026-08-23 | 在 dsh（DeepSeek Harness）会话头部展示模型厂商余额/用量徽标的插件：内置 DeepSeek 余额、MiniMax Token Plan 与智谱 GLM Coding Plan 配额，适配器架构支持接入更多厂商；host 侧按轮次取数，经 SSE 同步到浏览器。 |
| 481 | [demo007x/dsh-web-mermaid](https://github.com/demo007x/dsh-web-mermaid) | 1 | 2026-08-21 | 2026-08-22 | Deepseek harness mermaid流程图渲染插件 |
| 482 | [DevViking-Persike/dsh-cliproxy](https://github.com/DevViking-Persike/dsh-cliproxy) | 1 | 2026-08-22 | 2026-08-22 | DeepSeek Harness plugin: routes cliproxy-claude and cliproxy-openai through a local CLIProxyAPI, so the agent reaches your own CLI subscriptions |
| 483 | [DevViking-Persike/dsh-subscriptions](https://github.com/DevViking-Persike/dsh-subscriptions) | 1 | 2026-08-23 | 2026-08-24 | DeepSeek Harness plugin: use your own Claude and ChatGPT/Codex subscriptions as model providers, over each vendor's OAuth sign-in |
| 484 | [dfzjb/whalemaid-desktop-pet](https://github.com/dfzjb/whalemaid-desktop-pet) | 1 | 2026-08-24 | 2026-08-25 | 像素风蓝发鲸鱼女仆桌面宠物 · DSH Agent 桌面入口 · Electron + TypeScript |
| 485 | [dHR-P/dsh-safe-launch](https://github.com/dHR-P/dsh-safe-launch) | 1 | 2026-08-23 | 2026-08-23 | DSH (DeepSeek Harness) plugin: dsh-safe-launch - desktop safe-start launcher with last-good boot config, consent-gated canary updates for dsh & plugins, compatibility-checked plugin installation. DeepSeek Harness safe launcher plugin |
| 486 | [DiligenceLai/dsh-memory-ga](https://github.com/DiligenceLai/dsh-memory-ga) | 1 | 2026-08-22 | 2026-08-22 | Gated GA-style layered memory for DeepSeek Harness: hard-injected L1 index + RULES, session working checkpoint, settlement ritual to Skills/L1/L2 - no silent auto-retain. |
| 487 | [Diluka/dsh-persona](https://github.com/Diluka/dsh-persona) | 1 | 2026-08-25 | 2026-08-26 | Configurable coding collaboration style prompts and settings UI for DeepSeek Harness. |
| 488 | [Dingpenghui-good/dsh-plugin-manager](https://github.com/Dingpenghui-good/dsh-plugin-manager) | 1 | 2026-08-16 | 2026-08-23 | Writable plugin management tab for DeepSeek Harness - toggle, enable/disable, and uninstall user-installed Cordis plugins from Settings |
| 489 | [DK-Zhu/dsh-consult](https://github.com/DK-Zhu/dsh-consult) | 1 | 2026-08-21 | 2026-08-24 | Evidence-first multi-model consultation for DeepSeek Harness: 2–5 independently configured models review the same evidence, and the main agent synthesizes their anonymous opinions. |
| 490 | [dlssjdyka0019/dsh-launcher](https://github.com/dlssjdyka0019/dsh-launcher) | 1 | 2026-08-24 | 2026-08-24 | 管理多个隔离的 DeepSeek Harness (DSH) 实例的 Windows 桌面工具 |
| 491 | [dsh-ai-org/top-dsh-plugins](https://github.com/dsh-ai-org/top-dsh-plugins) | 1 | 2026-08-22 | 2026-08-22 | 📈 Daily-updated DeepSeek Harness plugin rankings · 每日更新的 DSH 插件榜单 — powered by dsh-ai.org |
| 492 | [duyanta123/dsh-refactor-insight](https://github.com/duyanta123/dsh-refactor-insight) | 1 | 2026-08-22 | 2026-08-23 | Turn codebase smells into an executable, priority-ordered refactoring plan (file-length / deep-nesting / TODO-density). |
| 493 | [dygin/dsh-recover-context](https://github.com/dygin/dsh-recover-context) | 1 | 2026-08-19 | 2026-08-23 | hsd agent context make recover or reedit |
| 494 | [EarzuChan/DshVibeLearning](https://github.com/EarzuChan/DshVibeLearning) | 1 | 2026-08-22 | 2026-08-23 | A Vibe Learning Plugin made for DeepSeek Harness |
| 495 | [Elave-66/dsh-blue-sea-player](https://github.com/Elave-66/dsh-blue-sea-player) | 1 | 2026-08-23 | 2026-08-23 | 蓝海之约鲸鱼娘 DSH 播放器插件：12 套皮肤 · 5 首默认音乐 · CD 旋转封面 · 收纳小球 |
| 496 | [elmaxid/dsh-manage](https://github.com/elmaxid/dsh-manage) | 1 | 2026-08-21 | 2026-08-22 | Instalacion y administracion de DeepSeek Harness (dsh): install/start/stop/update/status para puestos dev |
| 497 | [enoughpower/dsh-harmony](https://github.com/enoughpower/dsh-harmony) | 1 | 2026-08-22 | 2026-08-23 | DSH Harmony 客户端 搭配 dsh-pocket 使用 |
| 498 | [Entity-Him/dsh-doc-quick](https://github.com/Entity-Him/dsh-doc-quick) | 1 | 2026-08-25 | 2026-08-25 | Drag documents into the dsh web chat for direct local-file processing; a right sidebar lists outputs and file paths. 拖拽文档进 Web 对话框快速处理，右侧侧栏展示产出。 |
| 499 | [Entity-Him/dsh-harmonyos-market](https://github.com/Entity-Him/dsh-harmonyos-market) | 1 | 2026-08-24 | 2026-08-25 | HarmonyOS-exclusive plugin market for DeepSeek Harness — only plugins that actually run on HarmonyOS |
| 500 | [eomis/packhub-workbench-assistant](https://github.com/eomis/packhub-workbench-assistant) | 1 | 2026-08-23 | 2026-08-23 | DSH Desktop workbench installer, switcher, and updater |
| 501 | [esonx/dsh-project-j4agent](https://github.com/esonx/dsh-project-j4agent) | 1 | 2026-08-24 | 2026-08-24 | Jira-like Agent-native Project Management for DSH |
| 502 | [Evan1u/deepseek-harness-desktop](https://github.com/Evan1u/deepseek-harness-desktop) | 1 | 2026-08-22 | 2026-08-23 | Light-weight Desktop App for Deepseek Harness |
| 503 | [eversko/dsh-blackbox](https://github.com/eversko/dsh-blackbox) | 1 | 2026-08-24 | 2026-08-25 | Privacy-safe flight recorder and incident reports for DeepSeek Harness. |
| 504 | [Evhye38496/dsh-perfscope](https://github.com/Evhye38496/dsh-perfscope) | 1 | 2026-08-23 | 2026-08-24 | One-click health check & score for your DeepSeek Harness plugins. Scan -> Score -> Fix -> Share. PerfScope for dsh. |
| 505 | [exoticknight/dsh-labnana](https://github.com/exoticknight/dsh-labnana) | 1 | 2026-08-22 | 2026-08-22 | Labnana image generation for DeepSeek Harness: text-to-image / image-to-image / precise editing — chat image cards, credentials-domain API key, settingsScope UI |
| 506 | [falling-ts/dsh-force-compact](https://github.com/falling-ts/dsh-force-compact) | 1 | 2026-08-23 | 2026-08-26 | Aggressive context compaction for local-first agents. Runs Qwen3.8‑27B on self‑hosted llama.cpp at low context, shrinking history so the live prompt stays small, fast, and private—delivering a big‑window experience without API cost or data egress. 面向本地的激进上下文压缩插件。自托管 llama.cpp 低上下文运行 Qwen3.8‑27B,不断收缩历史、保持常驻 prompt 小而快,兼顾隐私与大窗口体验,零 API 成本、数据不出本机。 |
| 507 | [fatatalia/dsh-dreaming](https://github.com/fatatalia/dsh-dreaming) | 1 | 2026-08-18 | 2026-08-25 | dsh 梦境记忆整合插件：凌晨随机窗口把记忆梦境化（裸上下文 narrative 纯梦写作）+ 信号驱动洞察晋升 + MEMORY.md 预算管理，随 dsh web 启停 |
| 508 | [FeatherHunter/dsh-plugin-ui-debug](https://github.com/FeatherHunter/dsh-plugin-ui-debug) | 1 | 2026-08-18 | 2026-08-22 | DSH 插件 UI 调试神器：让 AI 在真实 Chrome 中帮你看界面、点按钮、拖组件，一键安装零配置 |
| 509 | [fenglin-ai/dsh-funasr-voice](https://github.com/fenglin-ai/dsh-funasr-voice) | 1 | 2026-08-22 | 2026-08-23 | DeepSeek Harness 本地离线语音输入插件：麦克风 → FunASR(SenseVoice) → 输入框，全离线识别。 |
| 510 | [fengyungithub/dsh-short-video-studio](https://github.com/fengyungithub/dsh-short-video-studio) | 1 | 2026-08-25 | 2026-08-25 | 基于deepseek harness的类MiniMax-Design的AI视频创作工作台 |
| 511 | [Fisfzy/dsh-cae-agent](https://github.com/Fisfzy/dsh-cae-agent) | 1 | 2026-08-21 | 2026-08-23 | 让 DeepSeek Harness (DSH) 通过原生工具直接操控本机 Abaqus/CAE 的 Cordis 插件。21 个 DSH 原生工具覆盖完整建模链（几何/材料/网格/接触/分析步/载荷/边界/作业/ODB），TypeScript 编写，socket bridge 直连本机（不走 MCP）。 |
| 512 | [fjzzwxp/dsh-mnemosyne-memory](https://github.com/fjzzwxp/dsh-mnemosyne-memory) | 1 | 2026-08-24 | 2026-08-25 | Mnemosyne 永久记忆插件 - 为 DSH 提供长期记忆、向量搜索和 LLM 反思功能，对标 Hindsight Coding Agents |
| 513 | [flg1217/dsh-quick-commands](https://github.com/flg1217/dsh-quick-commands) | 1 | 2026-08-24 | 2026-08-24 | User-defined slash commands for DeepSeek Harness: configure quick commands (name + prompt) in the settings panel; /name inserts a chip that expands to the prompt on send. |
| 514 | [Freakz2z/dsh-evidence-ledger](https://github.com/Freakz2z/dsh-evidence-ledger) | 1 | 2026-08-24 | 2026-08-24 | Local append-only evidence ledger for DeepSeek Harness |
| 515 | [Frog755/dsh-hybrid-memory](https://github.com/Frog755/dsh-hybrid-memory) | 1 | 2026-08-24 | 2026-08-24 | Hybrid memory plugin for DeepSeek Harness (DSH): L1 frozen-snapshot memory (MEMORY.md/USER.md, prefix-cache friendly) + L2 searchable knowledge base (facts + SQLite FTS5) + L3 multi-tool import (Hermes/Claude/Codex/WorkBuddy). 混合记忆插件：L1 冻结快照 + L2 可检索知识库 + L3 多工具导入。数据本地存储。 |
| 516 | [Frog755/dsh-prompt-vault](https://github.com/Frog755/dsh-prompt-vault) | 1 | 2026-08-22 | 2026-08-22 | Prompt Vault: 输入框上方的提示词库（DSH 插件）— 📚 按钮展开面板，点条目一键填入 prompt。DeepSeek Harness prompt library plugin. |
| 517 | [fsrmqi/dsh-promptkit](https://github.com/fsrmqi/dsh-promptkit) | 1 | 2026-08-26 | 2026-08-26 | Prompt building & enhancement toolkit for DeepSeek Harness: Studio + QuickEnhancer. 开源的 Prompt 构建与增强工具包。 |
| 518 | [Fz2hOpenSource/firmware-forge](https://github.com/Fz2hOpenSource/firmware-forge) | 1 | 2026-08-24 | 2026-08-25 | 基于 DSH 的 AI 嵌入式固件工程工作台，覆盖固件设计、协议设计、测试验证、编译、烧录与调试闭环。 |
| 519 | [Gaines-cz/dsh-a-share-screener](https://github.com/Gaines-cz/dsh-a-share-screener) | 1 | 2026-08-21 | 2026-08-22 | A-share stock screening plugin for DeepSeek Harness (dsh): pluggable strategies, Tushare token via credentials ref, free Eastmoney/Tencent fallback. |
| 520 | [genesis-agents/dsh-plugins](https://github.com/genesis-agents/dsh-plugins) | 1 | 2026-08-22 | 2026-08-24 | Plugins for DeepSeek Harness: a source library that reads 72 feeds and publishes podcasts, digests and reports, plus web search over Serper, Tavily and Brave |
| 521 | [GooDAnDReaDY/dsh-russian-lang](https://github.com/GooDAnDReaDY/dsh-russian-lang) | 1 | 2026-08-23 | 2026-08-23 | Russian localization for the DeepSeek Harness web UI: ru dictionaries for core namespaces and a third option in the native language list (Settings - General - Language). |
| 522 | [goodie1972/prompt-optimizer](https://github.com/goodie1972/prompt-optimizer) | 1 | 2026-08-24 | 2026-08-25 | 🔮 Multi-tool AI prompt optimizer plugin for ZCode, Claude Code, Codex CLI, Reasonix, DSH, MimoCode, OpenCode — 中文提示词优化插件 \| AI prompt optimizer plugin with /optimize command and optimize_prompt MCP tool |
| 523 | [graceen2331-prog/find-plugin](https://github.com/graceen2331-prog/find-plugin) | 1 | 2026-08-23 | 2026-08-23 | DeepSeek Harness tool for finding and verifying community DSH plugins on GitHub |
| 524 | [GreenLv/dsh-session-insights](https://github.com/GreenLv/dsh-session-insights) | 1 | 2026-08-21 | 2026-08-22 | Local-first, evidence-backed workflow retrospectives for DeepSeek Harness |
| 525 | [gtbwpkwjnb-alt/learn-skill](https://github.com/gtbwpkwjnb-alt/learn-skill) | 1 | 2026-06-21 | 2026-08-23 | 学习+链接 → 全自动采集·AI总结·亮点·术语·评分·图谱·深度OCR·入库 \| One link → AI analysis+highlights+glossary+rating+knowledge graph → KB import (v3.5) |
| 526 | [gtbwpkwjnb-alt/skills-summarize-audit-skill](https://github.com/gtbwpkwjnb-alt/skills-summarize-audit-skill) | 1 | 2026-06-18 | 2026-08-23 | Skills Audit — 技能审查·画像·评分·优化 / Universal agent tool auditor — profile, score, optimize |
| 527 | [gtbwpkwjnb-alt/summarize-skill](https://github.com/gtbwpkwjnb-alt/summarize-skill) | 1 | 2026-06-17 | 2026-08-23 | 会话级全维总结 — 项目·进度·建议·错误，一个命令全清 \| Session-level summary for project/progress/suggestion/error |
| 528 | [guhanfei-ai/dsh-mindmap](https://github.com/guhanfei-ai/dsh-mindmap) | 1 | 2026-08-22 | 2026-08-23 | 让DSH帮你快速制作思维脑图 |
| 529 | [Gyanano/dsh-grok-auth](https://github.com/Gyanano/dsh-grok-auth) | 1 | 2026-08-22 | 2026-08-23 | DeepSeek Harness plugin that reuses the official Grok CLI login (SuperGrok / X Premium OAuth) for an xai LLM route |
| 530 | [Hades03/dsh-model-quota-usage](https://github.com/Hades03/dsh-model-quota-usage) | 1 | 2026-08-22 | 2026-08-22 | DeepSeek Harness plugin: DeepSeek balance and per-provider/model token usage in a draggable overlay. |
| 531 | [Hanmiao33/dsh-bubble-explain](https://github.com/Hanmiao33/dsh-bubble-explain) | 1 | 2026-08-23 | 2026-08-24 | bubble-explain |
| 532 | [HaoyueQin/dsh-deepseek-monitor](https://github.com/HaoyueQin/dsh-deepseek-monitor) | 1 | 2026-08-22 | 2026-08-22 | DeepSeek Harness web plugin: DeepSeek balance & platform usage monitoring inside the official Settings-Models-DeepSeek card, plus a live balance chip left of the model name in the composer tool row. Ported from DeepSeekMonitorWindows. |
| 533 | [HaoyueQin/dsh-diff-stat](https://github.com/HaoyueQin/dsh-diff-stat) | 1 | 2026-08-24 | 2026-08-25 | DeepSeek Harness web plugin: inline +N −M diff badges on edit/write tool rows and a per-turn file change summary card. Scroll-windowed diffs, PTC/code-dispatch fallback, undo — no git required. |
| 534 | [Harvey-Will/dsh-vision-analysis](https://github.com/Harvey-Will/dsh-vision-analysis) | 1 | 2026-08-21 | 2026-08-22 | Vision tools for DeepSeek Harness: OCR, chart extraction, UI review, comparison & image-to-code via OpenAI- or Anthropic-compatible endpoints, with a built-in FREE anonymous vision source and automatic rate-limit failover. 支持 OpenAI/Anthropic 兼容视觉端点。 |
| 535 | [Harzva/dsh-agent-project-sync](https://github.com/Harzva/dsh-agent-project-sync) | 1 | 2026-08-23 | 2026-08-23 | Synchronize Codex and Claude project directories into native DeepSeek Harness workspaces. |
| 536 | [having5548/dsh-notify](https://github.com/having5548/dsh-notify) | 1 | 2026-08-23 | 2026-08-24 | Universal notification plugin for DeepSeek Harness: in-app toasts, native Windows toasts, one-click approval from the action center |
| 537 | [helibeiqi/dsh-csp-runtime](https://github.com/helibeiqi/dsh-csp-runtime) | 1 | 2026-08-23 | 2026-08-24 | Cognitive State Protocol (CSP) v0.1 — the cross-framework interop layer that makes AI thinking state serializable, persistable, and transferable. Host-side Cordis plugin for the DSH ecosystem. |
| 538 | [Hjay1101/dsh-plugin-token-usage](https://github.com/Hjay1101/dsh-plugin-token-usage) | 1 | 2026-08-22 | 2026-08-23 | GitHub-style token usage heat map for DeepSeek Harness — day/week/month granularity, per-model breakdown, hover-today badge. Read-only, fully local. |
| 539 | [honyKing/dsh-session-archive-plugin](https://github.com/honyKing/dsh-session-archive-plugin) | 1 | 2026-08-23 | 2026-08-23 | DSH 上下文存档与历史检索插件：自动压缩前把会话完整存档（zstd 解码为可读 jsonl + 摘要），压缩后按需全文检索历史对话。内置 archive_session / search_archive 工具与打包技能，dsh plugin add 一键安装。 |
| 540 | [Hou-DL/dsh-token-heatmap](https://github.com/Hou-DL/dsh-token-heatmap) | 1 | 2026-08-24 | 2026-08-24 | Local Token heatmap plugin for DSH Web — GitHub-style calendar views, per-hour/week/month/quarter/year, fully local, zero billing. |
| 541 | [HOWILLMAKEIT/football-mcp](https://github.com/HOWILLMAKEIT/football-mcp) | 1 | 2026-08-24 | 2026-08-25 | 面向 Claude、Codex、Cursor 和 DeepSeek Harness 的足球数据 MCP Server，支持 18 个欧洲联赛、8 个杯赛，以及比赛、积分榜、交锋、赔率和近期状态查询。 |
| 542 | [HuanLinOTO/dsh-plugin-better-locale](https://github.com/HuanLinOTO/dsh-plugin-better-locale) | 1 | 2026-08-23 | 2026-08-23 | DSH web 插件：通过运行时 monkey-patch LocaleRuntime.lookup 注入第三语言（ja/ko/...）覆盖，保持 dsh active locale 不变；通过 DSH 设置页通用分区暴露切换 UI。 \| DSH web plugin: injects third-language (ja/ko/...) overrides via a runtime monkey-patch of LocaleRuntime.lookup, leaving the dsh active locale unchanged; exposes a switcher UI through the DSH settings page (General section). |
| 543 | [Huasecc/dsh-usage](https://github.com/Huasecc/dsh-usage) | 1 | 2026-08-15 | 2026-08-24 | DeepSeek 用量面板—DSHWeb GUI 余额与Token用量仪表盘 |
| 544 | [hufang360/dsh-sticky-notes](https://github.com/hufang360/dsh-sticky-notes) | 1 | 2026-08-16 | 2026-08-22 | 记下想法，让agent落盘！ |
| 545 | [hw-cola/dsh-message-enhancer](https://github.com/hw-cola/dsh-message-enhancer) | 1 | 2026-08-24 | 2026-08-24 | DSH插件，消息功能增强 |
| 546 | [hw-cola/dsh-remote-control](https://github.com/hw-cola/dsh-remote-control) | 1 | 2026-08-25 | 2026-08-25 | DSH插件，手机远程控制 |
| 547 | [hzthzt/dsh-skill-switch](https://github.com/hzthzt/dsh-skill-switch) | 1 | 2026-08-22 | 2026-08-23 | Windows Junction-based global Skill switcher for DeepSeek Harness Web. |
| 548 | [icyaaaww/dsh-adaptive-model-router](https://github.com/icyaaaww/dsh-adaptive-model-router) | 1 | 2026-08-24 | 2026-08-24 | Deterministic per-turn adaptive model routing for DeepSeek Harness |
| 549 | [iguowz/dsh-cortex](https://github.com/iguowz/dsh-cortex) | 1 | 2026-08-23 | 2026-08-23 | 低成本多模型编排插件（Cortex）：大模型规划验收，子agent小模型执行，降本保质 |
| 550 | [ImCabbage/dsh-plugin-mindmap](https://github.com/ImCabbage/dsh-plugin-mindmap) | 1 | 2026-08-20 | 2026-08-23 | MindMap: a DeepSeek Harness plugin that distills conversations into persistent storylines with an interactive map tab. |
| 551 | [imsai-sh/dsh-1024store](https://github.com/imsai-sh/dsh-1024store) | 1 | 2026-08-24 | 2026-08-26 | DeepSeek Harness plugin store, marketplace and hub — 11,000+ dsh plugins with search, rankings, install commands and a free public API. DeepSeek Harness 插件市场 / 插件商店：自动收集与格式校验，免费搜索 API。deepseek1024.com |
| 552 | [IP050/dsh-video-player](https://github.com/IP050/dsh-video-player) | 1 | 2026-08-25 | 2026-08-26 | A floating, draggable, resizable **video player** for DeepSeek Harness (DSH). |
| 553 | [iyam-x/iyam-dsh-desktop](https://github.com/iyam-x/iyam-dsh-desktop) | 1 | 2026-08-24 | 2026-08-22 | a deepseek harness desktop |
| 554 | [jackuh105/dsh-message-edit](https://github.com/jackuh105/dsh-message-edit) | 1 | 2026-08-23 | 2026-08-23 | Edit or undo your sent messages in DeepSeek Harness's Web GUI — hides everything after from chat view and model context. |
| 555 | [Jaeger0624/dsh-conversation-nav](https://github.com/Jaeger0624/dsh-conversation-nav) | 1 | 2026-08-23 | 2026-08-23 | Codex-style conversation turn navigation for DeepSeek Harness Web GUI: piano-key rail, hover preview with send time, click-to-jump, per-turn marks |
| 556 | [jarvisluk/dsh-projectless-session](https://github.com/jarvisluk/dsh-projectless-session) | 1 | 2026-08-18 | 2026-08-26 | Projectless sessions for DeepSeek Harness with isolated date-organized working directories |
| 557 | [JasonFreeLab/dsh-command-code-review](https://github.com/JasonFreeLab/dsh-command-code-review) | 1 | 2026-08-25 | 2026-08-25 | /code-review slash command for DeepSeek Harness — five parallel review lenses, per-finding confidence scoring, then a gh reply back on the pull request. |
| 558 | [jasonliu119/find-image-prompt-skill](https://github.com/jasonliu119/find-image-prompt-skill) | 1 | 2026-08-23 | 2026-08-23 | Open AI-agent skill and DeepSeek function-calling adapter for turning ideas and public reference images into production-ready image prompts. |
| 559 | [JasonQQ/dsh-btw-plugin](https://github.com/JasonQQ/dsh-btw-plugin) | 1 | 2026-08-24 | 2026-08-25 | Codex-style /btw command for DeepSeek Harness: side questions answered in a conversation-seeded subagent context, without polluting the main context |
| 560 | [JimChen-g/dsh-frontier-repro](https://github.com/JimChen-g/dsh-frontier-repro) | 1 | 2026-08-16 | 2026-08-26 | Evidence-first frontier AI radar and reproducibility gate for DeepSeek Harness |
| 561 | [Jimmyzwang-cloud/dsh-inkscreen-theme](https://github.com/Jimmyzwang-cloud/dsh-inkscreen-theme) | 1 | 2026-08-22 | 2026-08-23 | Ink-and-paper Apple-glass theme for DeepSeek Harness (dsh) web client, with a handwritten jimmy sidebar brand |
| 562 | [jinsiyu/dsh-code-server-app](https://github.com/jinsiyu/dsh-code-server-app) | 1 | 2026-08-25 | 2026-08-26 | 将code-server（VSCode网页版）打包安装到dsh内的插件，快速实现专业的文件编辑。Package and install code-server (the web version of VSCode) as a plugin within dsh to quickly achieve professional file editing. |
| 563 | [jinzheng8115/dsh-Minesweeper](https://github.com/jinzheng8115/dsh-Minesweeper) | 1 | 2026-08-24 | 2026-08-24 | DeepSeek Harness minesweeper plugin — agent tool set + human panel sharing one board. 扫雷插件：agent 工具集与人类面板共享同一棋盘。 |
| 564 | [jisi71/dsh-memories](https://github.com/jisi71/dsh-memories) | 1 | 2026-08-21 | 2026-08-22 | Dual-ledger cross-session memory for DeepSeek Harness: auto-extracted long-term facts (MEMORY.md) + living project progress ledger (PROGRESS.md), recalled into every new session. Inspired by OpenAI Codex's memory pipeline. |
| 565 | [jkamkk/dsh-liquid-glass-input](https://github.com/jkamkk/dsh-liquid-glass-input) | 1 | 2026-08-25 | 2026-08-25 | Liquid Glass input card for the DSH web GUI: kube.io SVG refraction with coupled-spring press animation |
| 566 | [jli658942-web/dsh-market-skill](https://github.com/jli658942-web/dsh-market-skill) | 1 | 2026-08-22 | 2026-08-22 | DSH Market 全局 skill：教 Agent 发现、评估、安装 DeepSeek Harness 插件/技能。Global skill teaching agents to use DSH Market (dsh.market) to discover, evaluate and install DSH plugins and skills. |
| 567 | [JMweitao/dsh-local-plugin-installer](https://github.com/JMweitao/dsh-local-plugin-installer) | 1 | 2026-08-21 | 2026-08-22 | 从 DSH Web 设置页安装并构建本地插件 / Install and build local DeepSeek Harness plugins from the Web settings page. |
| 568 | [joao-paulo-santos/dsh-event-relay](https://github.com/joao-paulo-santos/dsh-event-relay) | 1 | 2026-08-24 | 2026-08-25 | Event relay: one SSE channel pushing host-side notifications to subscribed browser surfaces (server-side topic-prefix filtering, __relay/open reconnect signal) |
| 569 | [JohnXu22786/auditrail](https://github.com/JohnXu22786/auditrail) | 1 | 2026-08-23 | 2026-08-23 | Security auditing and session forensics for DeepSeek Harness (dsh): full tool-invocation-chain recording (who/what/files/status/duration) fr |
| 570 | [JohnXu22786/calendar](https://github.com/JohnXu22786/calendar) | 1 | 2026-08-23 | 2026-08-23 | CalDAV + iCalendar + RRULE calendar integration bundle for DeepSeek Harness (dsh), with Chinese-bias (lunar calendar / holidays / Asia/Shang |
| 571 | [JohnXu22786/ci-runner](https://github.com/JohnXu22786/ci-runner) | 1 | 2026-08-23 | 2026-08-23 | Trigger GitHub Actions workflow runs and local test pipelines, stream their logs back, and on failure hand the tail of the log to DeepSeek f |
| 572 | [JohnXu22786/dsh-web-submit](https://github.com/JohnXu22786/dsh-web-submit) | 1 | 2026-08-23 | 2026-08-23 | DeepSeek Harness plugin: run headless-style tasks through the live dsh web process — CLI-invoked sessions appear in the Web UI in real time (POST /x/headless, GET status, SSE live events). |
| 573 | [Jokasa7/dsh-product-subagent-console](https://github.com/Jokasa7/dsh-product-subagent-console) | 1 | 2026-08-22 | 2026-08-22 | Plan, run, and compare multi-Agent work inside DeepSeek Harness conversations |
| 574 | [jony5933/codex-dsh-bridge](https://github.com/jony5933/codex-dsh-bridge) | 1 | 2026-08-24 | 2026-08-24 | A visible, workspace-aware Codex to DeepSeek Harness Web Host bridge. |
| 575 | [JovanHE/ds-balance](https://github.com/JovanHE/ds-balance) | 1 | 2026-08-22 | 2026-08-23 | A minimal DeepSeek account balance widget for the DeepSeek Harness web GUI |
| 576 | [jsoncode/dsh-balance-by-token](https://github.com/jsoncode/dsh-balance-by-token) | 1 | 2026-08-21 | 2026-08-22 | DeepSeek Harness（dsh）双面插件（宿主 + 浏览器半边）：查看 DeepSeek 账户余额， 按 token 用量估算费用，价格按模型 × 高峰/空闲时段在线配置。所有能力收敛在 统一弹框中（侧边栏底部「余额」入口），另在会话头部提供实时 「当前会话 ≈xx CNY \| 余额 xx CNY」按钮。界面中英双语（跟随宿主 UI 语言）。 |
| 577 | [Jstn-1g/dsh-guarded-live-voice](https://github.com/Jstn-1g/dsh-guarded-live-voice) | 1 | 2026-08-25 | 2026-08-26 | Safety-first DSH realtime voice foundation: exact session binding, consent protocol, and proposal-only authority. |
| 578 | [JuwanXu/dsh-camel](https://github.com/JuwanXu/dsh-camel) | 1 | 2026-08-25 | 2026-08-25 | DeepSeek Harness plugin for provider/model-aware adaptive rate-limit pacing, visible retries, and free-model recovery. |
| 579 | [JuwanXu/dsh-continue](https://github.com/JuwanXu/dsh-continue) | 1 | 2026-08-25 | 2026-08-25 | DeepSeek Harness plugin for fail-closed network recovery, recommended answers, decision learning, and unattended continuation. |
| 580 | [jypjypjypjyp/dsh-guardrail](https://github.com/jypjypjypjyp/dsh-guardrail) | 1 | 2026-08-25 | 2026-08-25 | DSH 插件：工具调用规范守卫（deny/warn 拦截 + 规则管理面板） |
| 581 | [KaichenCurry/dsh-design-mode](https://github.com/KaichenCurry/dsh-design-mode) | 1 | 2026-08-22 | 2026-08-23 | Agentic image Design Mode for DeepSeek Harness: infinite canvas, ask_user clarification, image tools, comments, and provider routing. |
| 582 | [kaijia323/dsh-sidebar](https://github.com/kaijia323/dsh-sidebar) | 1 | 2026-08-19 | 2026-08-26 | DSH Web Client 的 VSCode 风格文件树侧栏插件：虚拟化懒加载文件树，支持文本 / Markdown / 图片预览。 |
| 583 | [KakaruHayate/dsh-degen-heal](https://github.com/KakaruHayate/dsh-degen-heal) | 1 | 2026-08-25 | 2026-08-25 | Detect and self-heal LLM output degeneration loops inside a DeepSeek Harness agent session. |
| 584 | [kanchengw/dsh-assembly.resume](https://github.com/kanchengw/dsh-assembly.resume) | 1 | 2026-08-25 | 2026-08-25 | Import local Codex and Claude sessions into DeepSeek Harness. |
| 585 | [kedoupi/xiaotaozi-dsh](https://github.com/kedoupi/xiaotaozi-dsh) | 1 | 2026-08-21 | 2026-08-22 | xiaotaozi-dsh：小桃子 DeepSeek Harness 插件与 Mac 客户端 |
| 586 | [kfirsch/dsh-hebrew-rtl](https://github.com/kfirsch/dsh-hebrew-rtl) | 1 | 2026-08-24 | 2026-08-25 | Hebrew RTL support for the DeepSeek Harness web UI: dominant-script block direction, bidi-safe input fields, and RTL-aware line navigation. |
| 587 | [Kian-Oraish/dsh-prompt-enchant](https://github.com/Kian-Oraish/dsh-prompt-enchant) | 1 | 2026-08-23 | 2026-08-25 | 增强提示词魔法棒:DSH Web 对话输入框的灵活自适应提示词增强插件 |
| 588 | [kittimzhe/dsh-session-export](https://github.com/kittimzhe/dsh-session-export) | 1 | 2026-08-22 | 2026-08-22 | Human-readable session transcript export for DeepSeek Harness — /transcript writes Markdown/JSON to a host path via ctx.sessionQuery (dsh-plugin) |
| 589 | [komoai2026/dsh-zpdf](https://github.com/komoai2026/dsh-zpdf) | 1 | 2026-08-22 | 2026-08-23 | Zpdf tools for DeepSeek Harness with durable API-key settings and CLI configuration. |
| 590 | [L1ttleBad/dsh-multi-task](https://github.com/L1ttleBad/dsh-multi-task) | 1 | 2026-08-25 | 2026-08-25 | A prototype Multi-task Agent Preset for DeepSeek Harness. |
| 591 | [L3n3L/dsh-resume](https://github.com/L3n3L/dsh-resume) | 1 | 2026-08-21 | 2026-08-22 | AI 写简历容易，但写完总会遇到模板难看、排版溢出、页面留白、改一处全局变形等问题。dsh-resume 专注解决“内容生成后的视觉复核”：让 AI 和用户一起把简历调到真正适合投递的刚好一页。AI can write a resume, but the result often looks unbalanced, overflows the page, leaves large blank areas, or breaks after a small edit. dsh-resume focuses on visual review after generation, helping AI and users refine the resume into a polished. |
| 592 | [lansi-ai/dsh-desktop](https://github.com/lansi-ai/dsh-desktop) | 1 | 2026-08-25 | 2026-08-26 | 把 DeepSeek Harness 做成一个真正的桌面应用：Electron 主进程内嵌 Cordis Host（与官方 Web 版同内核、零移植）， 渲染进程加载官方 Web UI 发行物（file:///自定义协议 + IPC 桥接，不开放 HTTP 端口）， 所有桌面原生能力（托盘、全局热键、系统通知、剪贴板、开机自启、协议唤起、多窗口）以 host 插件 形态注入运行时， 与官方「一切皆插件」的架构同构——不是给网页套壳，而是把桌面能力变成可装配、可卸载、可审查的插件树。  AI 驱动开发声明 |
| 593 | [lansi-ai/dsh-fetch-url](https://github.com/lansi-ai/dsh-fetch-url) | 1 | 2026-08-24 | 2026-08-25 | DeepSeek Harness (DSH) 抓取工具插件 — 注册模型可调用的 fetch_url 工具，抓取任意 URL（境内直连 / 境外走代理），返回有界摘要。 |
| 594 | [lansi-ai/dsh-plugin-starter](https://github.com/lansi-ai/dsh-plugin-starter) | 1 | 2026-08-24 | 2026-08-25 | DSH plugin development starter: a loadable skill (SKILL.md) plus copy-paste templates for building dual-face (Host + Client) DSH plugins |
| 595 | [Laplace-bit/dsh-pianist](https://github.com/Laplace-bit/dsh-pianist) | 1 | 2026-08-17 | 2026-08-25 | 🎹 A DeepSeek Harness piano plugin — deterministic musical timeline, Canvas2D grand piano, sample-based audio. 让 AI 弹一曲，也是模型的本事。 |
| 596 | [lasdrder0705/dsh-pro-vision](https://github.com/lasdrder0705/dsh-pro-vision) | 1 | 2026-08-21 | 2026-08-22 | DSH plugin: let DeepSeek-V4-Pro use V4-Flash-Vision-Exp for attached images. Install: dsh plugin --profile web add github:lasdrder0705/dsh-pro-vision |
| 597 | [launchmaniac/dsh-media-tools](https://github.com/launchmaniac/dsh-media-tools) | 1 | 2026-08-23 | 2026-08-24 | OpenRouter image, video, and speech generation as deepseek-harness tools — an out-of-tree profile bundle, no fork required |
| 598 | [Lbunc/dsh-local-llm-controller](https://github.com/Lbunc/dsh-local-llm-controller) | 1 | 2026-08-21 | 2026-08-22 | 为DSH接入本地大模型能力：在「设置→插件」页一键启停本地 llama.cpp 大模型（35B/9B，视觉×文本×快速/长上下文），卡片内配置、一条命令安装、自动注册，装完即用。 \| start/stop a local llama.cpp llama-server right from Settings → Plugins, with Qwen3.6-35B / Qwen3.5-9B (vision × text, fast × long-context) as session models — card config, one-command install, auto-registered. |
| 599 | [lc23313/dsh-autoupdate](https://github.com/lc23313/dsh-autoupdate) | 1 | 2026-08-23 | 2026-08-23 | dsh 内置自动更新插件 — Auto-update for DeepSeek Harness: safe version detection, exit-time apply, health check, auto-rollback & circuit breaker. |
| 600 | [lcohvne-tomorin/dsh-background](https://github.com/lcohvne-tomorin/dsh-background) | 1 | 2026-08-23 | 2026-08-24 | Custom background wallpaper plugin for DeepSeek Harness chat page — upload local image or image link, tune opacity and dark overlay, scope to chat area or full screen. |
| 601 | [lengquan88/dsh-dual-auto](https://github.com/lengquan88/dsh-dual-auto) | 1 | 2026-08-21 | 2026-08-22 | Dual-model auto-routing plugin for DeepSeek Harness: low-cost direct / high-cost upgrade + escape-learning closed loop |
| 602 | [lengzhanbao/dsh-raiden-theme](https://github.com/lengzhanbao/dsh-raiden-theme) | 1 | 2026-08-26 | 2026-08-26 | Raiden Inazuma Atelier / 稻妻雷电工房 — DSH Web 紫金亚克力主题（独立于 Taffy） |
| 603 | [leolee9086/zhihu-tools](https://github.com/leolee9086/zhihu-tools) | 1 | 2026-08-22 | 2026-08-26 | 知乎数据开放平台 DSH 静态双面插件:17工具+精美卡片+串行化限流。QQ群1017854502 https://qm.qq.com/q/RAHJuyhQQ |
| 604 | [leonardoxr/dsh-auto-chat-titles](https://github.com/leonardoxr/dsh-auto-chat-titles) | 1 | 2026-08-22 | 2026-08-24 | Semantic, configurable chat titles for DeepSeek Harness |
| 605 | [leonardoxr/dsh-claude-usage](https://github.com/leonardoxr/dsh-claude-usage) | 1 | 2026-08-24 | 2026-08-24 | Anthropic Claude plan usage indicator for DeepSeek Harness |
| 606 | [leonardoxr/dsh-companion](https://github.com/leonardoxr/dsh-companion) | 1 | 2026-08-22 | 2026-08-24 | Read-only workspace and session JSON API plugin for DeepSeek Harness native clients. |
| 607 | [leonardoxr/dsh-harness-updater](https://github.com/leonardoxr/dsh-harness-updater) | 1 | 2026-08-24 | 2026-08-24 | Claude Code / Codex CLI update detection, prompting, and one-click channel updates for DeepSeek Harness |
| 608 | [leonardoxr/dsh-native](https://github.com/leonardoxr/dsh-native) | 1 | 2026-08-22 | 2026-08-24 | Native desktop and iOS shell for trusted HTTPS web apps, with saved servers and first-class DeepSeek Harness support. |
| 609 | [leonardoxr/dsh-plugin-manager](https://github.com/leonardoxr/dsh-plugin-manager) | 1 | 2026-08-24 | 2026-08-24 | Safe loopback-only Web UI for managing DeepSeek Harness profile plugins |
| 610 | [leonardoxr/dsh-routed-subagent](https://github.com/leonardoxr/dsh-routed-subagent) | 1 | 2026-08-22 | 2026-08-22 | Complexity-routed subagent delegation for DeepSeek Harness: the model picks the runtime tier per task. |
| 611 | [lhbsaa/dsh-visibridge](https://github.com/lhbsaa/dsh-visibridge) | 1 | 2026-08-17 | 2026-08-23 | DeepSeek Harness vision plugin: analyze_image (structured OCR evidence) + capture_image (USB camera visual loop). 摄像头视觉闭环 + 结构化证据，支持 Ollama / DeepSeek / Xiaomi 三后端。 |
| 612 | [libiwolve/dsh-experience-library](https://github.com/libiwolve/dsh-experience-library) | 1 | 2026-08-24 | 2026-08-24 | dsh-experience-library: 更有经验的 DeepSeek - 经验验证固化层(实时采集/加工/三层检验/技能书/benchmark验证) |
| 613 | [lindog114514/dsh-dglab](https://github.com/lindog114514/dsh-dglab) | 1 | 2026-08-23 | 2026-08-23 | Deepseek harness的DG-LAB 控制插件为 AI 提供 dglab-kit 工具集 |
| 614 | [lispking/dsh-qq-skin](https://github.com/lispking/dsh-qq-skin) | 1 | 2026-08-22 | 2026-08-22 | A QQ NT messenger skin for DeepSeek Harness (dsh). Light and dark share one QQ NT language. |
| 615 | [litianshuo110/dsh-ds-vision-auto-route](https://github.com/litianshuo110/dsh-ds-vision-auto-route) | 1 | 2026-08-22 | 2026-08-22 | Route image-bearing turns to a configurable image-capable model for DeepSeek Harness |
| 616 | [liyu34/dsh-wsl-tray](https://github.com/liyu34/dsh-wsl-tray) | 1 | 2026-08-22 | 2026-08-22 | 为运行在 WSL 里的 DeepSeek Harness（DSH）提供 Windows 桌面快捷方式与系统托盘启动器。 |
| 617 | [lmong11/dsh-game-center](https://github.com/lmong11/dsh-game-center) | 1 | 2026-08-21 | 2026-08-22 | AI-powered Game Center plugin for DeepSeek Harness, featuring Texas Holdem with 1–7 agent players. |
| 618 | [longnb47/dsh-agent-gateway](https://github.com/longnb47/dsh-agent-gateway) | 1 | 2026-08-23 | 2026-08-25 | MCP stdio gateway for exposing local AGY, Codex, and OpenCode CLI agents to DeepSeek Harness (DSH). |
| 619 | [LongSir0419/dsh-git-branch-manage](https://github.com/LongSir0419/dsh-git-branch-manage) | 1 | 2026-08-24 | 2026-08-24 | DSH bundle: 当前 Git 分支徽标。在会话 header 与新会话欢迎页显示当前分支，支持切换、新建、更新、拉取、推送、删除（仅本地分支，IDEA 风格目录树）。 |
| 620 | [Loopiplusplus/dsh-plugin-toggle-manager](https://github.com/Loopiplusplus/dsh-plugin-toggle-manager) | 1 | 2026-08-20 | 2026-08-22 | Visual plugin manager for DSH Web. |
| 621 | [looput/dsh-finance-lab](https://github.com/looput/dsh-finance-lab) | 1 | 2026-08-18 | 2026-08-26 | DeepSeek Harness finance plugin: direct market HTTP APIs, portfolio settings, model tools |
| 622 | [lory69060/cn-intel-mcp-dsh](https://github.com/lory69060/cn-intel-mcp-dsh) | 1 | 2026-08-24 | 2026-08-24 | DeepSeek Harness plugin: China hard-tech supply chain intelligence (MCP: signal board / track record / Q&A) |
| 623 | [Lottle7/dsh-quota](https://github.com/Lottle7/dsh-quota) | 1 | 2026-08-25 | 2026-08-25 | Multi-provider quota, balance and Token-cost dashboard for DeepSeek Harness Web. |
| 624 | [loyalchiiina/dsh-chat-image-lightbox](https://github.com/loyalchiiina/dsh-chat-image-lightbox) | 1 | 2026-08-23 | 2026-08-23 | DSH plugin: display images inline in chat with lightbox zoom, download (save-as), and prev/next navigation |
| 625 | [ls-cool-123/dsh-account-balance](https://github.com/ls-cool-123/dsh-account-balance) | 1 | 2026-08-22 | 2026-08-22 | DeepSeek account balance dashboard plugin for dsh web — shows your DeepSeek API balance above the chat window. |
| 626 | [lsh2002/dsh-custom-fonts](https://github.com/lsh2002/dsh-custom-fonts) | 1 | 2026-08-24 | 2026-08-24 | deepseek-harness的修改字体插件 |
| 627 | [Lucasli2018/totoro-pet](https://github.com/Lucasli2018/totoro-pet) | 1 | 2026-08-24 | 2026-08-25 | DSH Web GUI 桌宠插件（悬浮 Q 版龙猫 · 喂食/抚摸/玩耍/睡觉互动养成） |
| 628 | [luckybilly/dsh-split-view](https://github.com/luckybilly/dsh-split-view) | 1 | 2026-08-25 | 2026-08-25 | 一个插件把 DeepSeek Harness 主窗口变成多个分屏，同时查看多个会话的状态。再也不用在会话列表里切来切去了。 |
| 629 | [luxueliu/luxueliu-reasoning-efforts](https://github.com/luxueliu/luxueliu-reasoning-efforts) | 1 | 2026-08-21 | 2026-08-22 | DSH里只有ds能选推理强度？20个常用模型推理强度按钮已就位！涵盖grok/Gemini / Kimi/glm……20个模型仅预设，实际槽位无上限！可以任意添加你的本地网关模型！（非 ds 系网关模型推理强度档位插件 + 路由级 llm-pi-ai 补丁） |
| 630 | [LVSUGARS/dsh-web-launcher](https://github.com/LVSUGARS/dsh-web-launcher) | 1 | 2026-08-21 | 2026-08-22 | Windows desktop launcher for DeepSeek Harness (DSH) Web: install the official CLI, manage local workspaces, and safely start, stop, and update DSH. |
| 631 | [lxxz1918/dsh-theme-customizer](https://github.com/lxxz1918/dsh-theme-customizer) | 1 | 2026-08-22 | 2026-08-22 | DeepSeek Harness（DSH）Web 界面自定义主题插件：背景/文字/框线/细节全可视化调整，可导入导出预设，持久化保存。 |
| 632 | [ly028716/dsh-memory-plugin](https://github.com/ly028716/dsh-memory-plugin) | 1 | 2026-08-20 | 2026-08-22 | Intelligent memory system for DSH - Track user preferences, tool usage, and project context to provide personalized recommendations |
| 633 | [M1ssbe4r/PocketCode](https://github.com/M1ssbe4r/PocketCode) | 1 | 2026-08-26 | 2026-08-26 | An AI agent that can code, build, and run apps locally on your phone.一个能在手机本地完成编码、编译和运行应用的AI Agent。。 |
| 634 | [Machine-126/dsh-alert-sound](https://github.com/Machine-126/dsh-alert-sound) | 1 | 2026-08-23 | 2026-08-23 | Notification sound + Chinese voice alerts for the DeepSeek Harness web GUI (approval / answer / completion / error), with a settings page. |
| 635 | [Malenia12/seedance-video-generator](https://github.com/Malenia12/seedance-video-generator) | 1 | 2026-08-22 | 2026-08-22 | Seedance 2.5 video generator: DSH agent plugin + local web workbench |
| 636 | [MaRi23333/dsh-subagent-library](https://github.com/MaRi23333/dsh-subagent-library) | 1 | 2026-08-22 | 2026-08-23 | DeepSeek Harness 具名子代理库插件：settings 驱动的角色名册，list_subagents / delegate 工具与设置页。Named subagent roster plugin for DeepSeek Harness. |
| 637 | [mario03690/dsh-lines](https://github.com/mario03690/dsh-lines) | 1 | 2026-08-22 | 2026-08-22 | Freeze a working sequence into a hosted production line. Turn a sequence of tool calls that alr |
| 638 | [Max-Null/dsh-plugin-center](https://github.com/Max-Null/dsh-plugin-center) | 1 | 2026-08-16 | 2026-08-25 | Plugin center for DeepSeek Harness: browse, install and update community plugins from inside the Web UI · DSH 插件管理中心：在 Web 界面浏览社区市场、一键安装与更新插件 |
| 639 | [Max-Null/seek-soul-in-darkness](https://github.com/Max-Null/seek-soul-in-darkness) | 1 | 2026-08-15 | 2026-08-23 | Seek Soul in Darkness (SSiD) — DSH-based desktop AI: finding the soul of silicon life in darkness · 暗夜寻魂（思灵）：基于 DSH 的桌面 AI，寻找硅基生命的灵魂 |
| 640 | [maxmilian/dsh-forge](https://github.com/maxmilian/dsh-forge) | 1 | 2026-08-24 | 2026-08-24 | DeepSeek Harness tools for self-hosted Gitea and Forgejo instances |
| 641 | [maxmilian/dsh-grafana-query](https://github.com/maxmilian/dsh-grafana-query) | 1 | 2026-08-26 | 2026-08-26 | Read-only Grafana metrics and alert tools for DeepSeek Harness (PromQL via datasource proxy). |
| 642 | [maxmilian/dsh-odoo](https://github.com/maxmilian/dsh-odoo) | 1 | 2026-08-26 | 2026-08-26 | Read-only Odoo tools for DeepSeek Harness, with an opt-in restricted draft-create tool. |
| 643 | [maxmilian/dsh-sentry](https://github.com/maxmilian/dsh-sentry) | 1 | 2026-08-26 | 2026-08-26 | Read-only Sentry issue and event tools for DeepSeek Harness. |
| 644 | [mba1398/dsh-done](https://github.com/mba1398/dsh-done) | 1 | 2026-08-23 | 2026-08-23 | One plugin that don't consume tokens. |
| 645 | [Melosic/dsh-invoke](https://github.com/Melosic/dsh-invoke) | 1 | 2026-08-14 | 2026-08-26 | Prompt Vault & Invoker for DeepSeek Harness — 管理、分类、快速调用提示词，支持侧边栏 GUI 与复制粘贴 |
| 646 | [meng-114/dsh-image-tiler](https://github.com/meng-114/dsh-image-tiler) | 1 | 2026-08-21 | 2026-08-22 | DSH插件：将大图像分割成带标签的800像素图块，并保留概览图，同时保留视觉模型所需的细节。包含设置卡。DSH plugin: slice large images into labeled 800px tiles + overview, preserving detail for vision models. Settings card included. |
| 647 | [mengzhangj/dsh-wallpaper](https://github.com/mengzhangj/dsh-wallpaper) | 1 | 2026-08-25 | 2026-08-26 | DSH-Wallpaper background wallpaper and system font picker plugin for DSH Desktop. Plugin source only, no DSH core. |
| 648 | [menotbobbybrown/create-dsh-app](https://github.com/menotbobbybrown/create-dsh-app) | 1 | 2026-08-22 | 2026-08-22 | 1-Line AI Agent Scaffolding Generator for DeepSeek Harness (dsh) — Everything is a Plugin |
| 649 | [menotbobbybrown/dsh-plugin-browser](https://github.com/menotbobbybrown/dsh-plugin-browser) | 1 | 2026-08-22 | 2026-08-22 | Native Web Browser Automation Agent Plugin for DeepSeek Harness (dsh) — Everything is a Plugin |
| 650 | [menotbobbybrown/dsh-plugin-memory](https://github.com/menotbobbybrown/dsh-plugin-memory) | 1 | 2026-08-22 | 2026-08-22 | Persistent Knowledge Graph & Long-Term Memory Plugin for DeepSeek Harness (dsh) — Everything is a Plugin |
| 651 | [messiahyl/dsh-plugins](https://github.com/messiahyl/dsh-plugins) | 1 | 2026-08-21 | 2026-08-22 | DSH 插件总仓库：monorepo 开发 + 安装源（本地归档/npm/GitHub/索引）+ 第三方目录。国内网络友好，归档 sha256 校验。 |
| 652 | [MichaelShii/dsh-plugin-teamflow](https://github.com/MichaelShii/dsh-plugin-teamflow) | 1 | 2026-08-17 | 2026-08-26 | dsh plugin teamflow |
| 653 | [Mikuzjc/dsh-office-for-mso](https://github.com/Mikuzjc/dsh-office-for-mso) | 1 | 2026-08-23 | 2026-08-23 | DeepSeek Harness (DSH) plugin/skill: control open Word/Excel/PowerPoint via Office add-in (33 actions, AI-orchestrated, near-Copilot workflows) \| DSH 的 Office 技能：操控打开的 Word/Excel/PPT |
| 654 | [MingYU-kalo/dsh-https-fix](https://github.com/MingYU-kalo/dsh-https-fix) | 1 | 2026-08-21 | 2026-08-22 | DeepSeek Harness plugin: built-in HTTPS reverse proxy with configurable settings (设置→插件配置→Https Fix) |
| 655 | [minyang2020/dsh-migrate-on-429](https://github.com/minyang2020/dsh-migrate-on-429) | 1 | 2026-08-22 | 2026-08-22 | DeepSeek Harness (dsh) plugin: automatic session handoff when a session keeps hitting 429 TPM rate limits — cancel old, summarize handover, continue in a fresh session. True handoff, never parallel. |
| 656 | [Missher12/dsh-missher-memory](https://github.com/Missher12/dsh-missher-memory) | 1 | 2026-08-23 | 2026-08-24 | Project-scoped reviewed long-project memory for DeepSeek Harness |
| 657 | [mjn96/dsh-rhine-theme](https://github.com/mjn96/dsh-rhine-theme) | 1 | 2026-08-24 | 2026-08-24 | 明日方舟莱茵生命美术风格的deepseek harness皮肤主题 |
| 658 | [mjw-git/dsh-pet](https://github.com/mjw-git/dsh-pet) | 1 | 2026-08-24 | 2026-08-24 | Desktop pet plugin for DeepSeek Harness (dsh) — grows with your agent token usage; XP economy, custom spritesheets, SSE status push, one-command install |
| 659 | [ML-QSeek/SurvX](https://github.com/ML-QSeek/SurvX) | 1 | 2026-06-24 | 2026-08-24 | SurvX — A paradigm for building intelligent systems where behavior is driven by data change. It unifies capability units (F), structured entities (Matter), and self-evolving entities (Ego) under one architecture that works with or without AI. A prototype exploring XGI (Xenogenic General Intelligence) and the future of development. |
| 660 | [mokuyoaxis/agent-guard](https://github.com/mokuyoaxis/agent-guard) | 1 | 2026-08-22 | 2026-08-23 | Make destructive AI-agent actions reversible by default — quarantine + audit + human escalation for rm/git destructive operations. Reliability infrastructure, not a sandbox. |
| 661 | [monotykamary/dsh-multiprovider](https://github.com/monotykamary/dsh-multiprovider) | 1 | 2026-08-24 | 2026-08-25 | Provider-neutral multi-account scheduling, affinity, health, and Settings UI for DeepSeek Harness |
| 662 | [MoonlitDropOfBlood/dsh-agent-approval](https://github.com/MoonlitDropOfBlood/dsh-agent-approval) | 1 | 2026-08-18 | 2026-08-23 | DSH 的自动审批权限插件 |
| 663 | [MoonlitDropOfBlood/dsh-memory-manager](https://github.com/MoonlitDropOfBlood/dsh-memory-manager) | 1 | 2026-08-18 | 2026-08-23 | DSH基本的记忆功能 |
| 664 | [MS666666/dsh-archive-manager](https://github.com/MS666666/dsh-archive-manager) | 1 | 2026-08-22 | 2026-08-22 | DeepSeek Harness归档管理器 |
| 665 | [mycyg/memory-palace](https://github.com/mycyg/memory-palace) | 1 | 2026-08-25 | 2026-08-25 | Event-based long-term memory for LLM agents — associative surfacing over query RAG. Closed-loop episodic events, budgeted injection, tiered forgetting. Claude Code hooks + DeepSeek Harness plugin, one shared .memory/ format. |
| 666 | [Nasbaye/dsh-launcher](https://github.com/Nasbaye/dsh-launcher) | 1 | 2026-08-24 | 2026-08-25 | DeepSeek Harness one-click restart plugin: status dot, reliable worker (pre-flight + health check), resume-after-restart and auto-continue on token truncation |
| 667 | [NattoCB/dsh-plugin-pin-session](https://github.com/NattoCB/dsh-plugin-pin-session) | 1 | 2026-08-23 | 2026-08-24 | Pin sessions in the DeepSeek Harness web GUI: Pinned Sessions group above the sidebar list + Pin/Unpin in the session row menu. |
| 668 | [NattoCB/dsh-web-search-session-follow](https://github.com/NattoCB/dsh-web-search-session-follow) | 1 | 2026-08-23 | 2026-08-23 | DSH web_search provider that follows the conversation's routed model provider — per-provider endpoint/credential/dialect table with built-in official fallback |
| 669 | [NEVSTOP-LAB/dsh-version-inspector](https://github.com/NEVSTOP-LAB/dsh-version-inspector) | 1 | 2026-08-23 | 2026-08-24 | DSH 版本信息插件，在 DSH 设置面板新增「版本信息」页，以紧凑多列树展示 DeepSeek Harness、插件与依赖的版本，支持按包名/版本过滤与 day/dark |
| 670 | [NexusAgentX/dsh-reasoning-effort](https://github.com/NexusAgentX/dsh-reasoning-effort) | 1 | 2026-08-15 | 2026-08-26 | Host-side dsh plugin that adds seven reasoning-effort levels to third-party llm-pi-ai models in the web composer. |
| 671 | [nicecx/dsh-macos-calendar](https://github.com/nicecx/dsh-macos-calendar) | 1 | 2026-08-24 | 2026-08-24 | DSH host-side plugin: real macOS Calendar integration (create/list/query/delete events via AppleScript) for DeepSeek Harness agents |
| 672 | [nicecx/dsh-matrix-skin](https://github.com/nicecx/dsh-matrix-skin) | 1 | 2026-08-24 | 2026-08-24 | Night-friendly Matrix dark-green skin for the DeepSeek Harness web GUI (standalone mirror of upstream dsh-web-ui packages/skins/matrix) |
| 673 | [Nigel211/dsh-text2img-compress](https://github.com/Nigel211/dsh-text2img-compress) | 1 | 2026-08-22 | 2026-08-22 | 把长文本渲染成图片发送，利用每图 384 token 封顶压缩 LLM 输入 token，专为DeepSeek Harness设计的插件；Pack long text into images to cut LLM input tokens (384/image cap) — a DeepSeek Harness plugin. |
| 674 | [nikoart-liu/dsh-open-in-x](https://github.com/nikoart-liu/dsh-open-in-x) | 1 | 2026-08-24 | 2026-08-24 | 在 DeepSeek Harness Web 界面中，把当前会话的工作目录直接交给本机外部应用打开。 |
| 675 | [njuptlzf/dsh-dynamic-background](https://github.com/njuptlzf/dsh-dynamic-background) | 1 | 2026-08-22 | 2026-08-23 | DeepSeek Harness (DSH) 动态背景切换插件：上传 GIF/静态图与内置 12 色纯色调色板，定时丝滑交叉淡入淡出切换页面背景，聊天区自动叠加主题色保护层。安装：dsh plugin add github:njuptlzf/dsh-dynamic-background |
| 676 | [NokorinNishikino/kidai-plugin-remote](https://github.com/NokorinNishikino/kidai-plugin-remote) | 1 | 2026-08-21 | 2026-08-22 | KPR 纪代管理：DSH的外部管理器，启停插件、隔离运行、手动回滚、预检诊断、变砖救急！配合KSG（Kidai-snapshot-guard）使用，自动快照、备份回滚！  |
| 677 | [NokorinNishikino/kidai-plugin-remote-client](https://github.com/NokorinNishikino/kidai-plugin-remote-client) | 1 | 2026-08-21 | 2026-08-22 | KPR‘C 纪代管理（Client）：零依赖的桌面客户端，DSH的外部管理器，启停插件、隔离运行、手动回滚、预检诊断、变砖救急！配合KSG（Kidai-snapshot-guard）使用，保存自动快照、备份回滚！ |
| 678 | [NokorinNishikino/kidai-snapshot-guard](https://github.com/NokorinNishikino/kidai-snapshot-guard) | 1 | 2026-08-21 | 2026-08-22 | KSG 纪代备份：DSH 内部备份插件，关闭自动保存快照、开机确认、单 zip 备份导出导入恢复、隔离自动恢复、多主流备份插件文件兼容 |
| 679 | [NONAME-2121237/dsh-timeline](https://github.com/NONAME-2121237/dsh-timeline) | 1 | 2026-08-24 | 2026-08-24 | DSH web plugin: interaction timeline rail for long conversations (fork-independent successor of dsh-history) |
| 680 | [NonchalantLudens/dsh-skin-collection](https://github.com/NonchalantLudens/dsh-skin-collection) | 1 | 2026-08-23 | 2026-08-23 | Multi-style skin collection for DeepSeek Harness (dsh) web GUI — 9 themes with scoped decoration CSS and a sidebar skin manager |
| 681 | [notload/dsh-session-toc](https://github.com/notload/dsh-session-toc) | 1 | 2026-08-23 | 2026-08-23 | 为 DeepSeek Harness Web UI 每个会话页右侧加一个类似deepseek网页端的常驻、可折叠的目录栏：每条用户提问对应一个条目，点击即可滚动定位到对应消息并高亮当前条目。 |
| 682 | [omdsh-dev/dsh-accessibility](https://github.com/omdsh-dev/dsh-accessibility) | 1 | 2026-08-25 | 2026-08-26 | Screen-reader guidance and in-app accessibility diagnostics for DeepSeek Harness |
| 683 | [OneCat2015/Remote-My-DSH](https://github.com/OneCat2015/Remote-My-DSH) | 1 | 2026-08-21 | 2026-08-23 | 一个Deepseek Harness远程插件（AI Coding注意） |
| 684 | [oneinitAI/dsh-thunderforge](https://github.com/oneinitAI/dsh-thunderforge) | 1 | 2026-08-22 | 2026-08-23 | ⚡ ThunderForge · 宇宙无敌雷霆霹雳炫光 — 励志做 0 元以内最 nb 的 DSH 插件（产品目标）：一站式 DSH 插件开发套件 |
| 685 | [open-dsh-plugins/dsh-open-in-app](https://github.com/open-dsh-plugins/dsh-open-in-app) | 1 | 2026-08-20 | 2026-08-24 | dsh web-UI plugin: open the current session's workspace folder with an installed app (Finder, Terminal, VS Code, Ghostty, Zed, ...) — icons included |
| 686 | [OpenCnid/recursus](https://github.com/OpenCnid/recursus) | 1 | 2026-08-22 | 2026-08-22 | A durable, full-access runtime agent built on DeepSeek Harness |
| 687 | [orpheus0829/dsh-identity-control](https://github.com/orpheus0829/dsh-identity-control) | 1 | 2026-08-21 | 2026-08-22 | 为 DeepSeek Harness (DSH) 打造的自定义人设控制插件。 在对话输入栏旁自由填写你的人设文本，一键开关，所有新对话自动生效、免重启。 人设纯粹是你设定的风格，不覆盖 DSH 安全护栏，安装即用、状态持久化。 |
| 688 | [oxlyn/dsh-model-health](https://github.com/oxlyn/dsh-model-health) | 1 | 2026-08-22 | 2026-08-22 | dsh model health status check |
| 689 | [oxlyn/dsh-plugin-mgr](https://github.com/oxlyn/dsh-plugin-mgr) | 1 | 2026-08-22 | 2026-08-22 | deepseek harness plugin manager |
| 690 | [pan17/dsh-minimax-usage](https://github.com/pan17/dsh-minimax-usage) | 1 | 2026-08-24 | 2026-08-24 | DSH plugin: floating MiniMax Token Plan usage bubble in the Web UI |
| 691 | [papachong/deepseek-harness-tui](https://github.com/papachong/deepseek-harness-tui) | 1 | 2026-08-21 | 2026-08-25 | This is a standalone terminal for deepseek-harness (designed based on a plug-in approach), updated in sync with the official deepseek-harness repository, and inherits the capabilities of the official product. |
| 692 | [paulalesius/dsh-hindsight-advanced](https://github.com/paulalesius/dsh-hindsight-advanced) | 1 | 2026-08-23 | 2026-08-23 | Long-term memory for DeepSeek Harness agents: automatic recall each turn, a retain/recall/reflect tool, standing rules, and visibility you scope to the whole bank, a preset, or a session. |
| 693 | [pc439527/dsh-model-provider](https://github.com/pc439527/dsh-model-provider) | 1 | 2026-08-24 | 2026-08-24 | DeepSeek Harness Model Selector UX Enhancement Plugin: show each model's provider (providerId:modelId identity, provider-grouped catalog, shadowed composer model seat) |
| 694 | [pengls/dsh-quick-view](https://github.com/pengls/dsh-quick-view) | 1 | 2026-08-23 | 2026-08-23 | dsh quick view plugin |
| 695 | [PetCT/dsh-plugin-marketplace](https://github.com/PetCT/dsh-plugin-marketplace) | 1 | 2026-08-23 | 2026-08-23 | DSH 插件市场 · A plugin marketplace inside DeepSeek Harness — browse, search, favorite, one-click download community plugins |
| 696 | [pharaohnie/dsh-context-mode](https://github.com/pharaohnie/dsh-context-mode) | 1 | 2026-08-23 | 2026-08-24 | DSH 原生 Cordis 插件：知识库(FTS5)、路由强制、会话记忆、沙箱执行(Think-in-Code)——context-window 减负 |
| 697 | [philmingdao/anno](https://github.com/philmingdao/anno) | 1 | 2026-08-16 | 2026-08-22 | Local-first HTML review and annotation for AI coding agents |
| 698 | [pmorgan3/deep-tui](https://github.com/pmorgan3/deep-tui) | 1 | 2026-08-21 | 2026-08-22 | deep-tui is a plugin-first coding-agent harness built on Cordis. Providers, tools, prompts, permissions, storage, themes, commands, renderers, and the agent loop are all replaceable plugins. |
| 699 | [ppjun2026/dsh-client-ui-lingxi](https://github.com/ppjun2026/dsh-client-ui-lingxi) | 1 | 2026-08-23 | 2026-08-23 | 灵犀（Lingxi）— DSH Web GUI 灵感工作台插件：想法池录入/孵化/计划/立项管理 + AI 解析评分与关联图谱，单文件 JSON 存储，零构建工具链，MIT。 |
| 700 | [Practice019/dsh-kun-pet](https://github.com/Practice019/dsh-kun-pet) | 1 | 2026-08-15 | 2026-08-25 | Kun Like 桌宠 - DSH 桌面宠物插件 |
| 701 | [puesite/dsh-telegram-notify](https://github.com/puesite/dsh-telegram-notify) | 1 | 2026-08-23 | 2026-08-24 | DSH/EAC Telegram 通知 + 聊天 + 远程批准插件 |
| 702 | [purezhi/dsh-plugin-confirmo](https://github.com/purezhi/dsh-plugin-confirmo) | 1 | 2026-08-22 | 2026-08-23 | 复刻 confirmo for DeepSeek Harness |
| 703 | [pwping/moyu_games](https://github.com/pwping/moyu_games) | 1 | 2026-08-25 | 2026-08-25 | 一款Deepseek Harness Web UI 的摸鱼游戏插件，执行任务时,在右下角位置弹窗游戏窗口，任务执行时间玩玩益智游戏 |
| 704 | [qinglang8609/deepseek_herdr](https://github.com/qinglang8609/deepseek_herdr) | 1 | 2026-08-21 | 2026-08-23 | 多智能体总指挥插件（DeepSeek Harness 原生版） ——让 DeepSeek 高效打开并指挥一个 claude / opencode / codex 智能体团队，实时看到每个智能体在做什么，通过共享记忆与任务看板编排多人协作。 |
| 705 | [QinXi-ai/dsh-codex-import](https://github.com/QinXi-ai/dsh-codex-import) | 1 | 2026-08-13 | 2026-08-23 | Read-only Codex setup compatibility scanner for DeepSeek Harness |
| 706 | [quaner1234-cmd/dsh-subagent-watchdog](https://github.com/quaner1234-cmd/dsh-subagent-watchdog) | 1 | 2026-08-23 | 2026-08-23 | DSH plugin that auto-continues a native continuable subagent once when it ends with explicit max-tokens termination — then stops. No loops, no timers, official seams only. |
| 707 | [qwert702/dsh-continue-on-limit](https://github.com/qwert702/dsh-continue-on-limit) | 1 | 2026-08-20 | 2026-08-23 | Auto-continue for DeepSeek Harness: when a local model hits its output-token cap, automatically send "continue" so the reply keeps flowing |
| 708 | [Qx002/dsh-group-chat](https://github.com/Qx002/dsh-group-chat) | 1 | 2026-08-21 | 2026-08-22 | DeepSeek Harness插件，多AI群聊插件 |
| 709 | [ramen-ai-dev/ramen-ai-integrations](https://github.com/ramen-ai-dev/ramen-ai-integrations) | 1 | 2026-06-26 | 2026-08-25 | Pre-execution semantic firewall for AI agents. Signed policy verdicts, BYOK, zero-trust receipts. |
| 710 | [rangrongg/SearchSieve](https://github.com/rangrongg/SearchSieve) | 1 | 2026-08-26 | 2026-08-26 | DeepSeek Harness 插件：逐页判断搜索结果的语义相关度，智能过滤无关噪音，量化信息覆盖度，让每一次AI检索都透明可信。 |
| 711 | [Rannist/balance-dsh](https://github.com/Rannist/balance-dsh) | 1 | 2026-08-23 | 2026-08-24 | DSH 插件：显示 DeepSeek 账户余额 + 会话 token/费用，含高峰/空闲计费 |
| 712 | [rayadesune/DeepSeek-Harness-chat-billing](https://github.com/rayadesune/DeepSeek-Harness-chat-billing) | 1 | 2026-08-17 | 2026-08-24 | 类原生计费插件 |
| 713 | [rayzhu1109/dsh-balance](https://github.com/rayzhu1109/dsh-balance) | 1 | 2026-08-22 | 2026-08-23 | balance record & usage tracking |
| 714 | [re-ITRT/dsh-keyring](https://github.com/re-ITRT/dsh-keyring) | 1 | 2026-08-22 | 2026-08-22 | DeepSeek Harness 密钥保险箱插件：自动捕获与脱敏密钥/凭据，settings 界面管理，支持会话级与全局级存储。 |
| 715 | [reatcat/l123-harness](https://github.com/reatcat/l123-harness) | 1 | 2026-08-22 | 2026-08-22 | L1-L2-L3 三级记忆 agent 底座：门禁、事件日志、周审提炼、TDD 执行流。Claude Code 插件。 |
| 716 | [red000000/dsh-cross-session-bridge](https://github.com/red000000/dsh-cross-session-bridge) | 1 | 2026-08-22 | 2026-08-23 | 适用于deepseek harness的根会话桥插件，可令根会话间双向通信 |
| 717 | [Rock-ql/dsh-relay-fast](https://github.com/Rock-ql/dsh-relay-fast) | 1 | 2026-08-25 | 2026-08-25 | DSH relay plugin: reasoning-effort autofill, /models sync, capability-aware Fast toggle \| DSH 中转站思考等级与 Fast 开关插件 |
| 718 | [Ruiming-cn/dsh-ask-in-sidebar](https://github.com/Ruiming-cn/dsh-ask-in-sidebar) | 1 | 2026-08-25 | 2026-08-25 | Ask a sidebar assistant about selected assistant text using the current DeepSeek Harness conversation context, without touching the main conversation. |
| 719 | [runfali/dsh-config-center](https://github.com/runfali/dsh-config-center) | 1 | 2026-08-24 | 2026-08-24 | dsh 扩展管理中心：WebUI 内统一管理 插件 / Skill / MCP -- bundle 安装移除、cordis.patch.yml 行增删改、SKILL.md 编辑、MCP 动态挂载即时生效。零侵入 bundle 插件，不改 dsh 源码。 |
| 720 | [runfali/dsh-export-kit](https://github.com/runfali/dsh-export-kit) | 1 | 2026-08-24 | 2026-08-24 | dsh 对话导出套件：一键将对话导出为 Markdown / TXT / JSON / CSV / PNG 长图 / PDF，附公式复制（LaTeX / MathML / Word 兼容）、设置备份与全会话归档。零侵入 bundle 插件，不改 Harness 源码。 |
| 721 | [runfali/dsh-mem0-plugins](https://github.com/runfali/dsh-mem0-plugins) | 1 | 2026-08-24 | 2026-08-24 | dsh 持久化记忆插件 - 依托自建的 mem0‑graph 服务器实现自动回忆与回写。 |
| 722 | [Ruszero01/dsh-tang-governance](https://github.com/Ruszero01/dsh-tang-governance) | 1 | 2026-08-23 | 2026-08-26 | Three Departments and Six Ministries governance mode plugin for DeepSeek Harness \| dsh 三省六部模式插件 |
| 723 | [S2P2/dsh-lab](https://github.com/S2P2/dsh-lab) | 1 | 2026-08-21 | 2026-08-23 | My DeepSeek Harness (DSH) plugin lab — workflow extensions, grilling UI experiments, quota widgets, and other things skills alone can't do. pnpm monorepo, one package per plugin. |
| 724 | [sakthiveltofficial/dsh-gmail-plugins](https://github.com/sakthiveltofficial/dsh-gmail-plugins) | 1 | 2026-08-25 | 2026-08-25 | dsh-gmail: Gmail plugin suite for DeepSeek Harness — 61 model-facing tools + 2 polling triggers over the Gmail & People APIs (OAuth2) |
| 725 | [sakthiveltofficial/dsh-shopify-plugins](https://github.com/sakthiveltofficial/dsh-shopify-plugins) | 1 | 2026-08-26 | 2026-08-26 | Shopify plugin for DeepSeek Harness: 213 model-facing shopify_* tools over the Shopify Admin REST + GraphQL APIs (products, orders, customers, inventory, fulfillments, discounts, content, webhooks, themes, billing, bulk operations) with Admin API access-token auth. |
| 726 | [sarfarazstark/dsh-material-file-icons](https://github.com/sarfarazstark/dsh-material-file-icons) | 1 | 2026-08-23 | 2026-08-23 | Material Icon Theme file & folder icons for the DeepSeek Harness web GUI (dsh-better-sidebar) - 349 authentic SVGs, named folders with open variants, zero patching required |
| 727 | [sch246/dsh-warm-minimal](https://github.com/sch246/dsh-warm-minimal) | 1 | 2026-08-24 | 2026-08-24 | DSH 温暖极简模式：会话创建即写入一条高质量首轮轨迹（we/let's 风格），真实输入从第二轮开始，AGENTS.md 与技能目录自然注入 |
| 728 | [scientisbo/dsh-codex-usage](https://github.com/scientisbo/dsh-codex-usage) | 1 | 2026-08-23 | 2026-08-24 | Codex 用量 · 订阅配额 + DeepSeek 余额聚合（DeepSeek Harness host 插件） \| Codex subscription quota & DeepSeek balance aggregator for DeepSeek Harness |
| 729 | [scientisbo/dsh-deepseek-usage](https://github.com/scientisbo/dsh-deepseek-usage) | 1 | 2026-08-23 | 2026-08-24 | DeepSeek 用量 · 余额面板（DeepSeek Harness Web 客户端插件） \| A clean DeepSeek usage & balance panel for DeepSeek Harness |
| 730 | [Sddft97/dsh-client-ui-skin-verdandi](https://github.com/Sddft97/dsh-client-ui-skin-verdandi) | 1 | 2026-08-22 | 2026-08-22 | Aether Gazer Verdandi-inspired skin for the DeepSeek Harness Web UI |
| 731 | [Seetraum/harness-session-delete](https://github.com/Seetraum/harness-session-delete) | 1 | 2026-08-25 | 2026-08-25 | Deepseek Harness 删除会话 |
| 732 | [SeireiA/dsh-plugin-rtk](https://github.com/SeireiA/dsh-plugin-rtk) | 1 | 2026-08-21 | 2026-08-21 | DeepSeek Harness plugin for RTK-powered shell output compaction |
| 733 | [sg88/dsh-proxy-switch](https://github.com/sg88/dsh-proxy-switch) | 1 | 2026-08-22 | 2026-08-22 | DSH 网络代理开关：直连失败自动回退到 HTTP/SOCKS5 代理，设置面板可配置代理地址 |
| 734 | [shangshuo1/DSH-Virtual](https://github.com/shangshuo1/DSH-Virtual) | 1 | 2026-08-24 | 2026-08-24 | Manage multiple isolated DeepSeek Harness (dsh) instances like virtual machines. Rust/egui native desktop app. |
| 735 | [shaomingbo/dsh-attention](https://github.com/shaomingbo/dsh-attention) | 1 | 2026-08-23 | 2026-08-24 | Desktop attention alerts for DeepSeek Harness Web: tab title, favicon, sound, and native OS notifications. |
| 736 | [Sharl210/dsh-strip-sandbox-permissions](https://github.com/Sharl210/dsh-strip-sandbox-permissions) | 1 | 2026-08-21 | 2026-08-22 | Strip sandbox_permissions/justification from model tool-call arguments to avoid false sandbox escalation errors |
| 737 | [Shhaaawwww/vibe-intent-compiler](https://github.com/Shhaaawwww/vibe-intent-compiler) | 1 | 2026-08-25 | 2026-08-25 | A one-click DeepSeek Harness plugin that compiles messy Vibe Coder drafts into concise, faithful, actionable instructions without inventing details. |
| 738 | [ShinonomeAya/dsh-git-chain](https://github.com/ShinonomeAya/dsh-git-chain) | 1 | 2026-08-26 | 2026-08-26 | DeepSeek Harness plugin: Cursor-style Git commit-chain graph with SVG lanes, commit details, diff, filtering, and guarded branch switching. |
| 739 | [shixiong0529/dsh-schedule-enable](https://github.com/shixiong0529/dsh-schedule-enable) | 1 | 2026-08-26 | 2026-08-26 | 为deepseek harness创建自动化任务 |
| 740 | [Shizuku-keop/dsh-compat-guard](https://github.com/Shizuku-keop/dsh-compat-guard) | 1 | 2026-08-25 | 2026-08-25 | Compatibility governance for DeepSeek Harness: upgrade pre-flight gate, storage-format fingerprint,  backup, session migration, per-profile lockfile, plugin x DSH compat matrix. |
| 741 | [Shizuku-keop/dsh-health](https://github.com/Shizuku-keop/dsh-health) | 1 | 2026-08-26 | 2026-08-26 | Session loop-health diagnostics for DeepSeek Harness: oscillation/stall/near-repeat/per-tool/token/compaction profiles + auditable 0-100 score. CLI + live watch bundle. |
| 742 | [shuaihaoV/dsh-TheWanderingEarthII](https://github.com/shuaihaoV/dsh-TheWanderingEarthII) | 1 | 2026-08-25 | 2026-08-25 | The Wandering Earth II · 流浪地球2 — DSH Web GUI 电影风格主题：发动机点火联动、MOSS 化发送按钮、星场 HUD |
| 743 | [shyuan-hub/dsh-compact-button](https://github.com/shyuan-hub/dsh-compact-button) | 1 | 2026-08-23 | 2026-08-23 | one-click Compact context button for the DSH Web context meter panel. |
| 744 | [Simon-yyy/dsh-theme-escook](https://github.com/Simon-yyy/dsh-theme-escook) | 1 | 2026-08-23 | 2026-08-23 | 为DeepSeek Harness桌面端打造的一款主题 |
| 745 | [sjlgg/dsh-free-web-search](https://github.com/sjlgg/dsh-free-web-search) | 1 | 2026-08-23 | 2026-08-23 | a deepseek plugin for free web search |
| 746 | [SkuraSshly/dsh-done-badge](https://github.com/SkuraSshly/dsh-done-badge) | 1 | 2026-08-24 | 2026-08-24 | DeepSeek Harness (DSH) task completion badge: native Windows taskbar counter (ITaskbarList3) while the window is away, auto-clears on return. Subagent sessions excluded. |
| 747 | [Slymaster/dsh-theme-lab](https://github.com/Slymaster/dsh-theme-lab) | 1 | 2026-08-24 | 2026-08-24 | Unofficial modular themes and starter kit for DeepSeek Harness. |
| 748 | [Smith-yue/harness-plugin](https://github.com/Smith-yue/harness-plugin) | 1 | 2026-08-23 | 2026-08-23 | harness-plugin |
| 749 | [SnowRikka/dsh-llama-responses](https://github.com/SnowRikka/dsh-llama-responses) | 1 | 2026-08-22 | 2026-08-23 | DeepSeek Harness plugin: run subagents on a local llama.cpp model via the OpenAI Responses (/v1/responses) protocol — LLM adapter + delegation skill |
| 750 | [spirits001/dsh-user-message-rail](https://github.com/spirits001/dsh-user-message-rail) | 1 | 2026-08-23 | 2026-08-23 | A dsh client plugin: a tick rail on the window left edge marking every message you sent, with hover preview and jump-to-message. |
| 751 | [SpookySandwich/dsh-plugin-no-workspace](https://github.com/SpookySandwich/dsh-plugin-no-workspace) | 1 | 2026-08-22 | 2026-08-23 | DSH 免工作区插件：不选工作区也能直接开始对话，独立会话在侧边栏平铺显示，原生工作区界面保持不变。Start chatting without picking a workspace; standalone conversations list flat in the sidebar. |
| 752 | [sryimnoob123/dsh-global-prompt](https://github.com/sryimnoob123/dsh-global-prompt) | 1 | 2026-08-25 | 2026-08-25 | DSH settings plugin for global and project AGENTS.md, identity/persona injection, and result notifications. |
| 753 | [sryimnoob123/dsh-tool-pwsh-safe](https://github.com/sryimnoob123/dsh-tool-pwsh-safe) | 1 | 2026-08-20 | 2026-08-26 | Elbow-proof PowerShell for DeepSeek Harness: pwsh_safe tool runs scripts via base64 -EncodedCommand, immune to quoting/escaping pain, sandbox-seam based |
| 754 | [sryimnoob123/dsh-web-search-ollama](https://github.com/sryimnoob123/dsh-web-search-ollama) | 1 | 2026-08-20 | 2026-08-25 | Ollama-backed web search provider for DeepSeek Harness (ctx.web) |
| 755 | [ssheleg/agent-sync](https://github.com/ssheleg/agent-sync) | 1 | 2026-07-29 | 2026-08-26 | Several coding agents, one repository, no collisions — leases with a TTL, race-free id reservation, a run journal and a generated board over a pluggable knowledge cloud. Ships in the sshlg-skills bundle. Loads in DeepSeek Harness (dsh). |
| 756 | [ssheleg/make-skill](https://github.com/ssheleg/make-skill) | 1 | 2026-07-24 | 2026-08-26 | A skill that builds skills: create, audit and ship Agent Skills and Claude Code plugins — conformance to the open standard, a validator that can fail, every distribution channel, and the MCP/A2A boundary. Loads in DeepSeek Harness (dsh). |
| 757 | [ssheleg/seo-aeo-audit](https://github.com/ssheleg/seo-aeo-audit) | 1 | 2026-07-27 | 2026-08-26 | Evidence-first website audit for search AND answer engines. Ten tracks from crawl access to AI citation mechanics; every finding carries an observation, every recommendation an evidence tier. Output is a prioritized change plan plus a link-building brief with keyword CSV — not a score. Loads in DeepSeek Harness (dsh). |
| 758 | [ssheleg/sheleg-design-skill](https://github.com/ssheleg/sheleg-design-skill) | 1 | 2026-06-11 | 2026-08-26 | The taste layer for AI coding agents: cinematic scroll-driven landing pages (one scroll clock, motion that degrades to calm, WebGL particle formations), product-UI style packs each shipping a ready token layer, and the Figma border — tokens as variables, design to code without hand-copied values. Loads in DeepSeek Harness (dsh). |
| 759 | [ssheleg/super-ux](https://github.com/ssheleg/super-ux) | 1 | 2026-07-19 | 2026-08-26 | Scenario-driven UI development for AI coding agents: a versioned design chain in docs/ux/ — personas and jobs → user flows → a screens-and-states map with Figma frames → traced scenarios → evidence-backed audits → fix plans. One /ux entry point, a linter that fails when the docs drift from the code. Loads in DeepSeek Harness (dsh). |
| 760 | [SsTtone1/dsh-message-cleaner](https://github.com/SsTtone1/dsh-message-cleaner) | 1 | 2026-08-25 | 2026-08-25 | DSH Web GUI 插件：在会话输入框上方提供历史消息记录面板，支持按条删除、原位恢复与内置节点导航条，让长会话的管理像编辑文档一样简单。 |
| 761 | [StabCut/dsh-edit-regenerate](https://github.com/StabCut/dsh-edit-regenerate) | 1 | 2026-08-18 | 2026-08-24 | DSH plugin: edit a user message in conversation history and regenerate from the revised prompt in a forked session. |
| 762 | [Stellight/dsh-imggen](https://github.com/Stellight/dsh-imggen) | 1 | 2026-08-22 | 2026-08-22 | DeepSeek Harness plugin: text-to-image output with in-chat image cards, download button, history gallery, and provider selection tabs (Pollinations / OpenAI DALL-E 3). |
| 763 | [steve-magne/dsh-plugins](https://github.com/steve-magne/dsh-plugins) | 1 | 2026-08-24 | 2026-08-25 | DeepSeek Harness plugins — dual-face cordis packages extending the DSH web surface: command deck, git worktrees, one-click PRs, cron-scheduled tasks |
| 764 | [SUJIElearning/dsh-trashbin](https://github.com/SUJIElearning/dsh-trashbin) | 1 | 2026-08-23 | 2026-08-23 | DSH 回收站（删除冷静区）：归档的对话进入回收站，支持恢复、立即移除、7 天自动清理 |
| 765 | [SUJIElearning/zhaoyu-restart](https://github.com/SUJIElearning/zhaoyu-restart) | 1 | 2026-08-23 | 2026-08-23 | One-click silent DSH restart button for DeepSeek Harness (dsh-plugin) |
| 766 | [sumarilkkxx/dsh-atlas](https://github.com/sumarilkkxx/dsh-atlas) | 1 | 2026-08-21 | 2026-08-22 | Visual conversation canvas for DeepSeek Harness. |
| 767 | [sumomok/dsh-plugins](https://github.com/sumomok/dsh-plugins) | 1 | 2026-08-23 | 2026-08-23 | DeepSeek Harness plugins by sumomok: quote earlier messages, edit & rerun a prompt, account balance & spend |
| 768 | [sunkeycn/dsh-desktop](https://github.com/sunkeycn/dsh-desktop) | 1 | 2026-08-25 | 2026-08-25 | Native macOS desktop wrapper for DeepSeek Harness with plugin management and FRP remote access |
| 769 | [SunNull/dsh-relay](https://github.com/SunNull/dsh-relay) | 1 | 2026-08-16 | 2026-08-24 | Cloud relay for DeepSeek Harness: expose your home dsh instance to any device with full real-time sync (out-of-tree plugin + wire-trunk architecture) |
| 770 | [T-Markus-Liang/dsh-game-studio](https://github.com/T-Markus-Liang/dsh-game-studio) | 1 | 2026-08-21 | 2026-08-22 | DSH Game Studio: AI-native Game Development Runtime for DeepSeek Harness — 可安装/卸载/升级的游戏开发插件（/game 子命令、动态 Agent Pool、引擎适配器、Verifier + Quality Gate） |
| 771 | [TalkingRainTuT/dsh-VoiceChat](https://github.com/TalkingRainTuT/dsh-VoiceChat) | 1 | 2026-08-23 | 2026-08-23 | 一个DSH的语音聊天插件 \| Realtime voice chat plugin for DeepSeek Harness: configurable translate + multi-TTS + auto-start local servers. |
| 772 | [Tangtang232/dsh-recovery](https://github.com/Tangtang232/dsh-recovery) | 1 | 2026-08-25 | 2026-08-25 | Recovery: Web first aid for DeepSeek Harness |
| 773 | [tanle-mtr/dsh-plogin-plugin-recommender](https://github.com/tanle-mtr/dsh-plogin-plugin-recommender) | 1 | 2026-08-22 | 2026-08-23 | The most comprehensive AI-curated list of DeepSeek Harness (DSH) plugins - 190+ plugins, 12 categories, updated hourly by AI. |
| 774 | [TaoruiLiu19/DSHwork](https://github.com/TaoruiLiu19/DSHwork) | 1 | 2026-08-15 | 2026-08-24 | DeepSeek Harness Desktop Client |
| 775 | [taskschd1145/deepseek-harness-clean](https://github.com/taskschd1145/deepseek-harness-clean) | 1 | 2026-08-22 | 2026-08-22 | 一个"三无"DSH桌面子端：打开它，就等于在浏览器里打DSH， 只不过它是一个带托盘图标、全原生的 Windows 窗口。 |
| 776 | [taxueseek/dsh-healthcheck](https://github.com/taxueseek/dsh-healthcheck) | 1 | 2026-08-15 | 2026-08-22 | DeepSeek Harness 环境体检插件：磁盘/内存/延迟/~/.dsh 膨胀/插件版本落后检测，历史基线趋势，只读不删。 |
| 777 | [taxueseek/dsh-snippets](https://github.com/taxueseek/dsh-snippets) | 1 | 2026-08-15 | 2026-08-22 | DeepSeek Harness 极简常用片段/命令工具箱：JSONL 存储，5 个工具，零依赖。AI 的收藏夹。 |
| 778 | [taxueseek/taxue-dsh-artisan](https://github.com/taxueseek/taxue-dsh-artisan) | 1 | 2026-08-19 | 2026-08-22 | taxue 画师：DeepSeek Harness 一体化视觉创作工具链（提示词反推/优化 + 多供应商生图，支持异步后台出图） |
| 779 | [thedeveloper256/dsh-model-router](https://github.com/thedeveloper256/dsh-model-router) | 1 | 2026-08-21 | 2026-08-22 | DeepSeek Harness plugin: role-based model routing — planner (root agent) on deepseek-v4-pro, delegated executor subagents on deepseek-v4-flash; ships a prompt section and a pro-flash-routing skill. |
| 780 | [TheHeartFickle/dsh-one-dark-pro](https://github.com/TheHeartFickle/dsh-one-dark-pro) | 1 | 2026-08-22 | 2026-08-23 | DSH（DeepSeek Harness）主题插件：注册 One Dark Pro 配色，并把「外观」设置里的主题添加 One Dark Pro。 |
| 781 | [TheHeartFickle/dsh-session-manager](https://github.com/TheHeartFickle/dsh-session-manager) | 1 | 2026-08-21 | 2026-08-22 | DSH 会话管理插件 —— 对话回退 + 归档会话，长会话可回滚、可整理。 |
| 782 | [TianyiTwT/dsh-image-zoom](https://github.com/TianyiTwT/dsh-image-zoom) | 1 | 2026-08-23 | 2026-08-24 | **Smart image splitting and zooming for Vision-Language Models (VLMs) inside [DeepSeek Harness (dsh)](https://github.com/deepseek-ai/deepseek-harness).** |
| 783 | [tieveto666-code/dsh-data-mode](https://github.com/tieveto666-code/dsh-data-mode) | 1 | 2026-08-23 | 2026-08-23 | DSH 数据模式插件：在原版 DeepSeek Harness 上增加只读问数。连接数据库或上传 CSV/Excel，用自然语言查数，并支持按数据源管理业务知识。 |
| 784 | [tieveto666-code/dsh-memory-migration](https://github.com/tieveto666-code/dsh-memory-migration) | 1 | 2026-08-26 | 2026-08-26 | 为原版 DeepSeek Harness 提供长期记忆：用键值对保存身份、偏好、方法论和约束，并在后续对话中按提问召回。可手动增删改查；也可选「记忆迁移」，从 ChatGPT / Claude / Gemini / DeepSeek 官方导出包提取少量核心记忆。独立插件，不修改 DSH 源码。 |
| 785 | [TNTsama11/dsh-tool-vision](https://github.com/TNTsama11/dsh-tool-vision) | 1 | 2026-08-21 | 2026-08-22 | DeepSeek Harness (DSH) plugin that lets a text-only agent call DeepSeek-V4-Flash-Vision-Exp to see images on demand, without manually switching models. |
| 786 | [tobysunsun/dsh-code-reading-coach](https://github.com/tobysunsun/dsh-code-reading-coach) | 1 | 2026-08-22 | 2026-08-22 | 代码研读教练：交互式引导研读论文对应的开源代码，五段研读法 |
| 787 | [Triple3h/dsh-usage-stats](https://github.com/Triple3h/dsh-usage-stats) | 1 | 2026-08-19 | 2026-08-23 | DSH Web plugin: usage statistics — daily/model tokens, sessions, messages, activity heatmap in a zcode-style panel. DSH Web 插件：侧边栏使用统计面板（按天/按模型 tokens、会话、消息、活跃热力图）。 |
| 788 | [trrrrrryg/dsh-ssh-forge](https://github.com/trrrrrryg/dsh-ssh-forge) | 1 | 2026-08-24 | 2026-08-26 | DSH SSH Forge：为 DeepSeek Harness（DSH）提供 SSH 远程工作区能力：已核验的服务器身份、失败关闭的 Agent 执行路由、远端文件与命令操作；提供 Windows 离线一键安装包，无需 Node.js 或构建工具。 |
| 789 | [TT-Wang/dsh-cron](https://github.com/TT-Wang/dsh-cron) | 1 | 2026-08-26 | 2026-08-26 | Scheduled work for DeepSeek Harness that survives session end, host restart and machine sleep — it schedules an outcome (completion window + effect check + catch-up), not a moment. |
| 790 | [TwilightSpirit/dsh-message-edit](https://github.com/TwilightSpirit/dsh-message-edit) | 1 | 2026-08-22 | 2026-08-23 | 在消息气泡上加修改按钮，通过 DSH surface replace 机制改写模型上下文，fork 继承、支持 markdown、可审计 |
| 791 | [tyx6661234/dsh-community-listening](https://github.com/tyx6661234/dsh-community-listening) | 1 | 2026-08-26 | 2026-08-26 | 面向 DeepSeek Harness (DSH) 的社交评论研究插件 |
| 792 | [uckkk/dsh-valley-meter](https://github.com/uckkk/dsh-valley-meter) | 1 | 2026-08-22 | 2026-08-22 | Minimal peak/valley electricity-price countdown widget for DeepSeek Harness: live off-peak countdown & period, official account balance, today's spend, configurable colors, minimal/detailed styles. |
| 793 | [Unintendedz/dsh-attention-notify](https://github.com/Unintendedz/dsh-attention-notify) | 1 | 2026-08-23 | 2026-08-23 | Browser notifications for every DSH event that needs user attention |
| 794 | [Unintendedz/dsh-conversation-tree](https://github.com/Unintendedz/dsh-conversation-tree) | 1 | 2026-08-23 | 2026-08-23 | ChatGPT-style immutable reply branches, inline branch switching, and whole-tree browsing for DeepSeek Harness. |
| 795 | [Unintendedz/dsh-response-meta](https://github.com/Unintendedz/dsh-response-meta) | 1 | 2026-08-23 | 2026-08-23 | Always-visible model, reasoning, throughput, timestamp, runtime, and TTFT metadata for DeepSeek Harness replies. |
| 796 | [Unintendedz/dsh-session-tools](https://github.com/Unintendedz/dsh-session-tools) | 1 | 2026-08-23 | 2026-08-23 | Archive, cross-session read, and copy-ID tools for DeepSeek Harness conversations. |
| 797 | [unStone/dsh-plugin-web-ppt](https://github.com/unStone/dsh-plugin-web-ppt) | 1 | 2026-08-22 | 2026-08-22 | DeepSeek Harness plugin: let your agent read and export .pptx / .ppt — pure JS, no PowerPoint, no conversion, no network. |
| 798 | [v587d/dsh-LLM-quotes](https://github.com/v587d/dsh-LLM-quotes) | 1 | 2026-08-25 | 2026-08-25 | Latest LLM provider API prices, right inside DeepSeek Harness (dsh) → Settings → Models.最新的大模型（LLM）厂商 API 价格，直接显示在 DeepSeek Harness（dsh） 的 设置 → 模型 页面中。 |
| 799 | [vanhungbui-11/dsh-wallpaper-bridge](https://github.com/vanhungbui-11/dsh-wallpaper-bridge) | 1 | 2026-08-25 | 2026-08-25 | Wallpaper Engine bridge for DeepSeek Harness (DSH) on Windows |
| 800 | [viethoang35/dsh-chat-bridge](https://github.com/viethoang35/dsh-chat-bridge) | 1 | 2026-08-22 | 2026-08-24 | Chat bridge that connects Telegram (WhatsApp, Zalo, Viber, ... ) to DeepSeek Harness via its headless CLI |
| 801 | [vikasranax/dsh-plugin-cats](https://github.com/vikasranax/dsh-plugin-cats) | 1 | 2026-08-23 | 2026-08-24 | A DeepSeek Harness plugin that fetches random cat facts from a public API. |
| 802 | [viplocco/dsh-delete-message](https://github.com/viplocco/dsh-delete-message) | 1 | 2026-08-22 | 2026-08-24 | DeepSeek Harness 消息级删除插件，用于避免用户误发或错误的助手消息污染会话上下文。 |
| 803 | [Wanbinyu/dsh-companion](https://github.com/Wanbinyu/dsh-companion) | 1 | 2026-08-21 | 2026-08-25 | Local state-aware desktop companion and task-status overlay for DeepSeek Harness Web |
| 804 | [wang-kaopu/dsh-cordis-devtools](https://github.com/wang-kaopu/dsh-cordis-devtools) | 1 | 2026-08-23 | 2026-08-26 | Give coding Agents runtime evidence for debugging and verifying DSH / Cordis plugins. 让 Coding Agent 获得用于调试和验证 DSH / Cordis 插件的运行时证据。 |
| 805 | [wangbobo-coder/gitee-ai-employee](https://github.com/wangbobo-coder/gitee-ai-employee) | 1 | 2026-08-24 | 2026-08-24 | Gitee AI 员工：在 issue 里 @ 机器人并指定目标分支，它自动克隆仓库开发、提交 PR，可自动合并并关闭 issue。Issue-driven Gitee AI developer for DeepSeek Harness. |
| 806 | [wangzhanchao883/dsh-plugin](https://github.com/wangzhanchao883/dsh-plugin) | 1 | 2026-08-22 | 2026-08-22 | DeepSeek Harness plugin collection: self-developed DSH plugins (screenshot capture, OCR, Obsidian). ?? DSH ?????? |
| 807 | [wanyexin1998/dsh-workbench](https://github.com/wanyexin1998/dsh-workbench) | 1 | 2026-08-26 | 2026-08-26 | Community-maintained source preview for two-Pane DeepSeek Harness Web workflows |
| 808 | [Washington5533/guarftrain](https://github.com/Washington5533/guarftrain) | 1 | 2026-08-09 | 2026-08-26 | 🛡️ 一行命令，训练脚本零行改动，获得完整守护能力。GPU 监控 · 崩溃恢复 · OOM 自救 · Agent 决策 · MCP 35 工具 · Web Dashboard。 |
| 809 | [weshopai/weshop-skill-package](https://github.com/weshopai/weshop-skill-package) | 1 | 2026-08-20 | 2026-08-25 | Creative AI Skills for Codex, Claude Code, Cursor, Deepseek harness and any Agent Skills-compatible runtime. |
| 810 | [whoisjiahao/dsh-feishu-channel](https://github.com/whoisjiahao/dsh-feishu-channel) | 1 | 2026-08-16 | 2026-08-22 | 飞书 × DeepSeek Harness 遥控器：在飞书聊天里驱动 DSH agent——流式富卡片、一键审批、按模型能力传图、费用与峰谷计量 |
| 811 | [wilburli/onlyMemory-plugin](https://github.com/wilburli/onlyMemory-plugin) | 1 | 2026-08-25 | 2026-08-25 | 零外部依赖的 LLM 长期记忆插件，专为 [DeepSeek Harness] 设计。 |
| 812 | [woosh2010/dsh-usage-dashboard](https://github.com/woosh2010/dsh-usage-dashboard) | 1 | 2026-08-21 | 2026-08-22 | DeepSeek Harness (dsh) usage analytics plugin: peak/valley billing dock, token/cost/model dashboard, cross-session history, global filters \| 用量分析插件：峰谷计费坞 + 用量仪表盘 |
| 813 | [wozoulesky/dsh-obsidian](https://github.com/wozoulesky/dsh-obsidian) | 1 | 2026-08-14 | 2026-08-23 | DSH（DeepSeek Harness）嵌入 Obsidian 的 AI 协作者插件：聊天侧边栏、内联编辑、@提及与计划模式（连接本地 http://127.0.0.1:3080） |
| 814 | [WSL043/dsh-native-deepseek-balance](https://github.com/WSL043/dsh-native-deepseek-balance) | 1 | 2026-08-24 | 2026-08-24 | DeepSeek API cash balance and private DSH-local request, token, cache, daily, and per-model usage charts for DeepSeek Harness. |
| 815 | [WSL043/dsh-native-reasoning-slider](https://github.com/WSL043/dsh-native-reasoning-slider) | 1 | 2026-08-23 | 2026-08-23 | Model-aware reasoning effort slider for DeepSeek Harness, with a Claude-inspired WebGL energy field, native themes, and a live demo. |
| 816 | [wuzhigouno-collab/dsh-rp-composer](https://github.com/wuzhigouno-collab/dsh-rp-composer) | 1 | 2026-08-23 | 2026-08-24 | TriComposer · DSH web 端 RP 结构化输入插件：台词/动作/心理分框填空、模板组装发送，从输入层消除 AI 对玩家言行的成分误识别。Structured tri-channel input composer for LLM roleplay on DeepSeek Harness. |
| 817 | [wyouwd1/dsh-opencode-models](https://github.com/wyouwd1/dsh-opencode-models) | 1 | 2026-08-24 | 2026-08-24 | Manage OpenCode Zen free-tier and Go-tier models in DeepSeek Harness: live listings from opencode.ai, drift per route, four agent tools plus an OpenCode Models settings section. |
| 818 | [xianrui69/dsh-quick-phrases](https://github.com/xianrui69/dsh-quick-phrases) | 1 | 2026-08-26 | 2026-08-26 | DeepSeek Harness client plugin: quick-phrase chip bar above the composer + /-triggered phrase menu |
| 819 | [xiaochaZ/dsh-session-title-summary](https://github.com/xiaochaZ/dsh-session-title-summary) | 1 | 2026-08-25 | 2026-08-26 | DSH plugin: rolling session summary + current-task title (@xiaochaz) |
| 820 | [XIAOke8698/dsh-memory-forget](https://github.com/XIAOke8698/dsh-memory-forget) | 1 | 2026-08-23 | 2026-08-23 | Forgetting engine for AI agents — memory TTL, decay, eviction, audit. The opposite of memory programming. DSH plugin + local skill + CLI. |
| 821 | [XiaoluoFoxington/dsh-theme-hacker-terminal](https://github.com/XiaoluoFoxington/dsh-theme-hacker-terminal) | 1 | 2026-08-24 | 2026-08-24 | Hacker-terminal skin for the dsh web GUI: pure black, high-contrast green, right-angle geometry, monospace font, full-width conversation, OLED-safe, scrollbars on Gecko/Blink/WebKit. |
| 822 | [xiaoshi7915/dsh-memory-manager](https://github.com/xiaoshi7915/dsh-memory-manager) | 1 | 2026-08-25 | 2026-08-26 | A unified memory management layer |
| 823 | [xiaoso456/dsh-run-config](https://github.com/xiaoso456/dsh-run-config) | 1 | 2026-08-23 | 2026-08-24 | Run configuration management for DeepSeek Harness (DSH) — IDEA-style run control for the web GUI: reusable LLM prompts and background commands, one click to launch. |
| 824 | [XiaoWind/dsh-cron](https://github.com/XiaoWind/dsh-cron) | 1 | 2026-08-21 | 2026-08-22 | DeepSeek Harness plugin: a /cron slash command for cron-scheduled recurring agent loops |
| 825 | [xie-tj/dsh-easy-exit](https://github.com/xie-tj/dsh-easy-exit) | 1 | 2026-08-21 | 2026-08-23 | Optional DeepSeek Harness plugin for editing and resending the latest direct-human message |
| 826 | [Xingkong42/dsh-zh-labels](https://github.com/Xingkong42/dsh-zh-labels) | 1 | 2026-08-21 | 2026-08-22 | DSH 界面中文标签持久化插件 - Persistent Chinese UI labels for DeepSeek Harness |
| 827 | [Xinlong-Wu/dsh-auto-review](https://github.com/Xinlong-Wu/dsh-auto-review) | 1 | 2026-08-20 | 2026-08-24 | adds an auto-review permission preset to DeepSeek Harness. Same Codex auto review |
| 828 | [xiuyuan18/dsh-engram-session](https://github.com/xiuyuan18/dsh-engram-session) | 1 | 2026-08-23 | 2026-08-23 | Unofficial community plugin: per-session Engram memory for DeepSeek Harness — spawns an engram MCP child per agent session rooted at the session workspace, registers mem_* tools per agent scope, and injects the Memory Protocol as a system-prompt section. |
| 829 | [XMoon/dsh-profile-settings](https://github.com/XMoon/dsh-profile-settings) | 1 | 2026-08-23 | 2026-08-23 | Per-profile settings overlay for DeepSeek Harness: global settings.yaml plus profiles/<name>/settings.patch.yml, transparently layered under ctx.settings |
| 830 | [xswt442-cmd/dsh-instance-manager](https://github.com/xswt442-cmd/dsh-instance-manager) | 1 | 2026-08-23 | 2026-08-24 | DSH 常驻插件：侧边栏面板统一查看并停止本机 3080–3129 端口的 dsh 实例 \| Sidebar panel to list and gracefully stop local dsh web instances (ports 3080-3129) |
| 831 | [xuan666-lab/dsh-openrouter-provider-advisor](https://github.com/xuan666-lab/dsh-openrouter-provider-advisor) | 1 | 2026-08-24 | 2026-08-24 | DSH plugin that ranks OpenRouter providers by cost, speed, context, and reliability, then switches the active route. |
| 832 | [xuanyuanluoxue/computer-use-vision](https://github.com/xuanyuanluoxue/computer-use-vision) | 1 | 2026-08-22 | 2026-08-22 | Windows computer-use capability for DSH: screenshot, vision, simulated input, self-evolving knowledge base. Plugin + skill dual-mode. |
| 833 | [xuc865/dsh-librarian](https://github.com/xuc865/dsh-librarian) | 1 | 2026-08-23 | 2026-08-24 | a dsh plugin that helps you to automatically generate, evolve and manage your dsh plugins |
| 834 | [yafangwang9/dsh-voice-plugin](https://github.com/yafangwang9/dsh-voice-plugin) | 1 | 2026-08-24 | 2026-08-24 | Voice input plugin for DeepSeek Harness |
| 835 | [yangbobo2021/relay-dsh-plugin-claude](https://github.com/yangbobo2021/relay-dsh-plugin-claude) | 1 | 2026-08-23 | 2026-08-26 | Claude Code integration plugin for DeepSeek Harness, providing native Claude conversations powered by the Claude Agent SDK, with approvals, session continuity, and DSH tool support. |
| 836 | [yangbobo2021/relay-dsh-plugin-codex](https://github.com/yangbobo2021/relay-dsh-plugin-codex) | 1 | 2026-08-23 | 2026-08-26 | Codex integration plugin for DeepSeek Harness, providing native Codex conversations powered by the Codex App Server, with workspace, terminal, approval, and DSH tool support. |
| 837 | [yangdongzhen590/dsh-knj-workflow](https://github.com/yangdongzhen590/dsh-knj-workflow) | 1 | 2026-08-23 | 2026-08-24 | Config-driven development-task orchestration plugin for DeepSeek Harness: workflows + task management + stage progress UI. |
| 838 | [yanglingrise/dsh-erii-boot-splash](https://github.com/yanglingrise/dsh-erii-boot-splash) | 1 | 2026-08-22 | 2026-08-22 | Erii (Sakura) themed boot splash animation for the DeepSeek Harness Web UI: falling sakura petals, a mint monster mascot, and the line "Sakura, walk slower." Auto fades out; pure client-side. |
| 839 | [yangwuan55/dsh-feishu-integration](https://github.com/yangwuan55/dsh-feishu-integration) | 1 | 2026-08-24 | 2026-08-24 | Bidirectional Feishu/Lark integration for DeepSeek Harness: summaries, reply routing, binding UI, and QR provisioning. |
| 840 | [yaways/dsh-subagent-claude-code-wrapper](https://github.com/yaways/dsh-subagent-claude-code-wrapper) | 1 | 2026-08-22 | 2026-08-22 | Let DSH subagents call any Claude-compatible CLI, not just the SDK-bundled one. Fork of @deepseek-ai/dsh-subagent-claude-code. |
| 841 | [Ycet/dsh-fun-turn-status](https://github.com/Ycet/dsh-fun-turn-status) | 1 | 2026-08-22 | 2026-08-23 | 替换 DSH 任务运行中的 Deep diving... 状态文案：30 秒随机轮换幽默文案，设置-插件-插件配置页可增删改（最多 50 条），与其他同类插件共存时优先级最高。 |
| 842 | [yhyfhgs/dsh-model-hub](https://github.com/yhyfhgs/dsh-model-hub) | 1 | 2026-08-25 | 2026-08-25 | DeepSeek Harness plugin: provider sign-in, model catalog, and selection routing over a loopback-only /model-hub channel |
| 843 | [YINGCHAO-98/dsh-private-plugins](https://github.com/YINGCHAO-98/dsh-private-plugins) | 1 | 2026-08-25 | 2026-08-26 | 在 DeepSeek Harness Web 设置中统一导入、启用、更新和管理本地及云端私有插件。 |
| 844 | [yingzaicc/dsh-editor-selection-vscode](https://github.com/yingzaicc/dsh-editor-selection-vscode) | 1 | 2026-08-23 | 2026-08-23 | DSH 编辑器选区桥接扩展:把 VS Code 的主选区(路径+行区间,不含任何文件内容)推送给本地 DeepSeek Harness,使对话自动聚焦你正在看的代码。 |
| 845 | [yingzaicc/dsh-gitland](https://github.com/yingzaicc/dsh-gitland) | 1 | 2026-08-23 | 2026-08-23 | DeepSeek Harness（DSH）的 Git 面板插件：在 Web GUI 中呈现 GoLand 风格的 Git 工具窗口 —— 提交日志时间线（彩色泳道图）、分支管理、worktree 管理，以及工作区状态摘要，并支持简单的 分支/worktree 操作。 |
| 846 | [yishengdaxiaonengjihui/dsh-poor-router](https://github.com/yishengdaxiaonengjihui/dsh-poor-router) | 1 | 2026-08-26 | 2026-08-26 | Budget-LLM pool router for DeepSeek Harness: ledger, health tracking, Thompson-sampling failover across free-tier models. 穷鬼路由器 |
| 847 | [YJLTF/dsh-plugin-offline-packager](https://github.com/YJLTF/dsh-plugin-offline-packager) | 1 | 2026-08-25 | 2026-08-25 | DeepSeek Harness 离线打包插件 — 在联网环境下将 DSH 插件打包为离线安装包（.tgz），传输到离线 DSH 环境中加载安装。 |
| 848 | [ynnmuraii/dsh-sandbox](https://github.com/ynnmuraii/dsh-sandbox) | 1 | 2026-08-22 | 2026-08-26 | dsh-lab meta-repo: plugin laboratory for DeepSeek Harness (workbench, template, catalog) |
| 849 | [yongshuai0314/dsh-readcache](https://github.com/yongshuai0314/dsh-readcache) | 1 | 2026-08-23 | 2026-08-24 | 为 DSH read 工具提供版本令牌校验的进程内结果缓存 \| Version-token-validated in-process result cache for the DSH read tool |
| 850 | [yth1120/deepseek-harness](https://github.com/yth1120/deepseek-harness) | 1 | 2026-08-23 | 2026-08-23 | DeepSeek Harness source with the dsh-web-workbench plugin suite (right workbench, terminal, timeline, review, files and browser preview). |
| 851 | [yu-wenchao/dsh-free-models-hub](https://github.com/yu-wenchao/dsh-free-models-hub) | 1 | 2026-08-26 | 2026-08-26 | 免费模型排行榜 · DeepSeek Harness 社区插件，在 DeepSeek Harness (DSH) Web UI 左侧边栏提供「免费模型榜」：分页浏览（每页 10 条、页码窗口、首页/末页）、 点击标题展开 API 调用地址 / 模型名称 / 【点击这里申请免费密钥key】按钮， 并支持一键配置到 设置 → 模型 → 自定义提供方 —— 用户只需自行粘贴免费 API Key |
| 852 | [YunlongL-byte/dsh-launcher](https://github.com/YunlongL-byte/dsh-launcher) | 1 | 2026-08-22 | 2026-08-22 | macOS 程序坞一键启动 DeepSeek Harness (DSH) 的快捷启动器 / One-click DSH launcher for macOS Dock |
| 853 | [Yurzi/dsh-pdf-mineru](https://github.com/Yurzi/dsh-pdf-mineru) | 1 | 2026-08-24 | 2026-08-24 | Provider-independent DSH PDF parsing tools powered by MinerU. |
| 854 | [yushuosun/dsh-cost-governor](https://github.com/yushuosun/dsh-cost-governor) | 1 | 2026-08-22 | 2026-08-22 | Cost governance & budget enforcement for DeepSeek Harness: per-model token-cost accounting, multi-provider pricing, budget warn thresholds, and a usage dashboard. |
| 855 | [yxie2/dsh-petrinet](https://github.com/yxie2/dsh-petrinet) | 1 | 2026-08-24 | 2026-08-24 | Workflow-net runtime for DeepSeek Harness: resource-aware concurrency, native loops and fan-out, static soundness checking before a plan becomes durable, and process mining over its own event log. |
| 856 | [yyyq0325-ai/dsh-webgate](https://github.com/yyyq0325-ai/dsh-webgate) | 1 | 2026-08-22 | 2026-08-26 | 为 DeepSeek Harness 的 Web GUI 加一道账号密码门：每次打开 DSH Web 都必须先登录；登录令牌有效期 12 小时；令牌过期被登出时，后台正在运行的任务完全不受影响，重新登录后一切还在。 |
| 857 | [zclDragon/dsh-side-chat](https://github.com/zclDragon/dsh-side-chat) | 1 | 2026-08-22 | 2026-08-23 | DSH web plugin: Codex-style /side side conversations — a temporary fork of the current chat in a floating panel, without interrupting the main task. |
| 858 | [zergtant/dsh-remote-access](https://github.com/zergtant/dsh-remote-access) | 1 | 2026-08-23 | 2026-08-24 | DeepSeek Harness (dsh) 远程访问插件：提供 TLS、登录认证、会话保护和 HTTP/WebSocket 透明反代，支持局域网及 FRP ，cloudflare隧道等远程访问。 |
| 859 | [Zh1rV/dsh-web-search-tavily](https://github.com/Zh1rV/dsh-web-search-tavily) | 1 | 2026-08-24 | 2026-08-25 | DeepSeek Harness 的 Tavily 搜索插件 |
| 860 | [zhaimingyou/dsh.plus](https://github.com/zhaimingyou/dsh.plus) | 1 | 2026-08-25 | 2026-08-25 | DSH plugin that shows the dsh.plus curated plugin catalog inside DeepSeek Harness |
| 861 | [zheng16965/dsh-deliverables-toggle](https://github.com/zheng16965/dsh-deliverables-toggle) | 1 | 2026-08-24 | 2026-08-24 | 为 DeepSeek Harness 对话产物列表增加主动展开与收起功能的 Web UI 插件。 |
| 862 | [zhengjy01/dsh-cubox](https://github.com/zhengjy01/dsh-cubox) | 1 | 2026-08-23 | 2026-08-23 | Cubox sync plugin for DeepSeek Harness: scheduled sync, AI daily brief from your prompt template into Obsidian, per-card markdown export — via the /c/api/cli endpoints |
| 863 | [zhengjy01/dsh-skill-studio](https://github.com/zhengjy01/dsh-skill-studio) | 1 | 2026-08-23 | 2026-08-23 | Skill studio for DeepSeek Harness: visualize, edit and enable/disable agent skills from the web settings panel and via skillmgr_* tools |
| 864 | [zhengjy01/weread-export](https://github.com/zhengjy01/weread-export) | 1 | 2026-08-23 | 2026-08-23 | 微信读书 (WeChat Reading) integration for DeepSeek Harness: official Skills API gateway — bookshelf, highlights/thoughts, reading stats, flomo export |
| 865 | [ZHOUcourier/dsh-theme-whalegirl](https://github.com/ZHOUcourier/dsh-theme-whalegirl) | 1 | 2026-08-22 | 2026-08-23 | DeepSeek-鲸鱼娘 (Whale Girl) theme for the DeepSeek Harness Web UI — ported from DreamSkin ver_cb557ececaa5de3f3dbe: full --dsw-* token remap + ambient wallpaper. |
| 866 | [zhubaohi/dsh-qwen38-compaction-fix](https://github.com/zhubaohi/dsh-qwen38-compaction-fix) | 1 | 2026-08-25 | 2026-08-25 | DSH plugin: stop qwen3.8-27b from burning its output budget on thinking during context compaction |
| 867 | [zhuifengqug/pixel-skin](https://github.com/zhuifengqug/pixel-skin) | 1 | 2026-08-23 | 2026-08-23 | dsh像素风皮肤 |
| 868 | [ZhuoSir/dsh-cron](https://github.com/ZhuoSir/dsh-cron) | 1 | 2026-08-22 | 2026-08-22 | DeepSeek Harness 定时任务插件：对话中自然语言创建，到点自动执行并在会话中回复，支持 cron 表达式与 Web 管理面板 |
| 869 | [zhuzhujunandy/dsh-model-router](https://github.com/zhuzhujunandy/dsh-model-router) | 1 | 2026-08-23 | 2026-08-23 | Tiered model routing plugin for DeepSeek Harness (DSH): route delegated work to fast/medium/heavy model tiers with DoD verification, cross-provider fallback, background delegation, and per-conversation budget modes. |
| 870 | [ZnFr60/dsh-lan-access-for-rpi-os-or-debian](https://github.com/ZnFr60/dsh-lan-access-for-rpi-os-or-debian) | 1 | 2026-08-26 | 2026-08-26 | Raspberry Pi 64-bit (aarch64) LAN access + boot auto-start installer for the DeepSeek Harness (dsh) Web UI: phone/LAN devices control dsh from a browser (0.0.0.0 bind, /api trust fence, crypto.randomUUID polyfill, privileged-API fix, systemd auto-start). |
| 871 | [ZnFr60/dsh-lan-access-for-windows](https://github.com/ZnFr60/dsh-lan-access-for-windows) | 1 | 2026-08-25 | 2026-08-26 | DeepSeek Harness LAN-access bundle plugin: bind dsh web to 0.0.0.0 + crypto.randomUUID secure-context shim for phone browsers. |
| 872 | [zoumutou/dsh-attachment-downscale](https://github.com/zoumutou/dsh-attachment-downscale) | 1 | 2026-08-22 | 2026-08-22 | DSH 插件：图片附件超限自动降级（2000px / 3.5MB / 4000万像素） |
| 873 | [zslzxy/aitoubiaoling-bid-review](https://github.com/zslzxy/aitoubiaoling-bid-review) | 1 | 2026-08-23 | 2026-08-24 | AI投标灵标书审核 Skill：稳定审核非扫描 PDF/DOCX 的商务标、技术标与通用文档风险 |
| 874 | [zzj8442-blip/dsh-mobile-remote](https://github.com/zzj8442-blip/dsh-mobile-remote) | 1 | 2026-08-24 | 2026-08-24 | 📡 手机远程遥控 DeepSeek Harness：实时进度 / 审批 / 对话（PWA + PIN 配对 + Tailscale 外网支持） |
| 875 | [01men/ybkk-AIOS](https://github.com/01men/ybkk-AIOS) | 0 | 2026-08-21 | 2026-08-24 | 企业 AI 资源统一管理平台 —— 13 个 dsh/cordis 插件（IAM/OIDC/MCP/Skill 市场/Agent/审计/计费/插件市场），dsh plugin add 可直接安装 |
| 876 | [0231071/llm-as-a-verifier](https://github.com/0231071/llm-as-a-verifier) | 0 | 2026-08-25 | 2026-08-25 | LLM-as-a-Verifier plugin for DeepSeek Harness (DSH): best-of-N 候选并行生成 + 概率枢轴锦标赛(PPT)验证器择优, 官方样式设置卡片, lav_status/lav_set 会话工具 \| DSH 插件: 让 AI 回答经过多候选验证器选优 |
| 877 | [0N3-0/dsh-tui-mcp-manager](https://github.com/0N3-0/dsh-tui-mcp-manager) | 0 | 2026-08-25 | 2026-08-25 |   面向 dsh-TUI 的原生 MCP Server 管理插件：通过 /mcp-manager 浮窗完成 MCP CRUD、启停、Sets、复制、Inspector、Tool schema、Doctor Lite 和凭据引用管理，并将配   置原子写入当前 profile，支持 Cordis HMR 热重载。 |
| 878 | [0QwQ0/dsh-ui-auth](https://github.com/0QwQ0/dsh-ui-auth) | 0 | 2026-08-23 | 2026-08-23 | DeepSeek Harness Web UI 认证网关插件：登录门禁、用户管理、管理员专属模型/Key 配置、数据隔离 · Authentication gate for the DeepSeek Harness Web UI: login gate, user management, admin-only model/API-key config, data isolation |
| 879 | [0w0miki/dsh-question-rail](https://github.com/0w0miki/dsh-question-rail) | 0 | 2026-08-23 | 2026-08-24 | 给Deepseek Harness滚动条加上提问节点 |
| 880 | [0xrushmoon/dsh-plugin](https://github.com/0xrushmoon/dsh-plugin) | 0 | 2026-08-24 | 2026-08-24 | dsh-plugin |
| 881 | [1-CellBio/dsh-okf](https://github.com/1-CellBio/dsh-okf) | 0 | 2026-08-19 | 2026-08-22 | DeepSeek Harness plugin: turn research PDFs into a citable OKF markdown library, with full-text & semantic search, knowledge graph, and survey writing. |
| 882 | [12398k/dsh-opencode-go-dashboard](https://github.com/12398k/dsh-opencode-go-dashboard) | 0 | 2026-08-24 | 2026-08-24 | dsh-opencode-go-dashboard |
| 883 | [142gg-GZX/unity-dsh-bridge](https://github.com/142gg-GZX/unity-dsh-bridge) | 0 | 2026-08-25 | 2026-08-25 | DSH plugin: control Unity / Tuanjie editor over a local HTTP bridge — build scenes, write C#, compile, play, screenshot, simulate input. |
| 884 | [18126295767-cell/dsh-mac-control](https://github.com/18126295767-cell/dsh-mac-control) | 0 | 2026-08-19 | 2026-08-22 | Give DeepSeek Harness hands on your Mac: native browser and desktop control tools for macOS. |
| 885 | [1clickreport/dsh-1clickreport](https://github.com/1clickreport/dsh-1clickreport) | 0 | 2026-08-22 | 2026-08-23 | Connect your marketing data (Google Ads, Meta, GA4, Search Console, Shopify, Stripe) to DeepSeek Harness via MCP |
| 886 | [2017java/dsh-md-overlay](https://github.com/2017java/dsh-md-overlay) | 0 | 2026-08-24 | 2026-08-26 | DSH web 插件：可悬浮 / 可停靠的多标签 Markdown 预览面板 + md_preview 模型工具，会话里一键预览报告。 |
| 887 | [2017java/dsh-md-viewer](https://github.com/2017java/dsh-md-viewer) | 0 | 2026-08-24 | 2026-08-26 | DSH web 插件：在 dsh-better-sidebar 侧边栏内把 Markdown 富渲染为预览（代码高亮 / 目录 / 一键复制）。 |
| 888 | [240xu/tech-lead-skill](https://github.com/240xu/tech-lead-skill) | 0 | 2026-08-24 | 2026-08-26 | Evidence-driven planning and safe change-control skill for OpenCode |
| 889 | [452926826/dsh-at-skill](https://github.com/452926826/dsh-at-skill) | 0 | 2026-08-25 | 2026-08-26 | Invoke DeepSeek Harness skills with @name and composer suggestions |
| 890 | [452926826/dsh-feishu-bot](https://github.com/452926826/dsh-feishu-bot) | 0 | 2026-08-25 | 2026-08-26 | Connect a Feishu bot to DeepSeek Harness projects and conversations |
| 891 | [452926826/dsh-ssh-logs](https://github.com/452926826/dsh-ssh-logs) | 0 | 2026-08-25 | 2026-08-26 | Read allowlisted remote logs over SSH from DeepSeek Harness conversations |
| 892 | [988hj7tczd-oss/dsh-math-olympiad](https://github.com/988hj7tczd-oss/dsh-math-olympiad) | 0 | 2026-08-24 | 2026-08-24 | DSH skill bundle: competition math (IMO/Putnam/USAMO/AIME) solved with pure reasoning, adversarial verification in a fresh subagent, and calibrated confidence |
| 893 | [988hj7tczd-oss/dsh-skill-creator](https://github.com/988hj7tczd-oss/dsh-skill-creator) | 0 | 2026-08-24 | 2026-08-24 | One-shot DSH skill (SKILL.md) generator: capture intent, draft, validate, package and distribute skills from inside a DeepSeek Harness session |
| 894 | [988hj7tczd-oss/harness-github](https://github.com/988hj7tczd-oss/harness-github) | 0 | 2026-08-23 | 2026-08-26 | DeepSeek Harness GitHub plugin: review PRs, triage issues, debug Actions CI, handle incoming GitHub events (webhooks + polling) via dsh-native tools. |
| 895 | [a805026135/dsh-constellation](https://github.com/a805026135/dsh-constellation) | 0 | 2026-08-25 | 2026-08-25 | A live, self-organizing constellation map of your DeepSeek Harness plugin universe — AI-balanced taxonomy, bilingual labels, instant search, health diagnostics, and one-click plugin operations. |
| 896 | [aa2246740/dsh-cuadrive-mac](https://github.com/aa2246740/dsh-cuadrive-mac) | 0 | 2026-08-20 | 2026-08-25 | macOS-only DeepSeek Harness plugin: private cua-driver computer-use for DSH |
| 897 | [aa2246740/dsh-dragndrop-attachments](https://github.com/aa2246740/dsh-dragndrop-attachments) | 0 | 2026-08-24 | 2026-08-25 | Codex-style drag-and-drop files, folders, ZIP and Office attachments for DeepSeek Harness |
| 898 | [aa2246740/dsh-files-panel](https://github.com/aa2246740/dsh-files-panel) | 0 | 2026-08-18 | 2026-08-25 | Community DeepSeek Harness plugin: right-side workspace file tree. Does not patch DSH core. |
| 899 | [aa2246740/dsh-grok-plan-mode](https://github.com/aa2246740/dsh-grok-plan-mode) | 0 | 2026-08-21 | 2026-08-25 | Full Grok Build Plan Mode port for DeepSeek Harness. Replaces official DSH Plan with Grok's state machine, plan.md edit gate, enter/exit tools, and review surface. |
| 900 | [aa2246740/dsh-image-conatiner](https://github.com/aa2246740/dsh-image-conatiner) | 0 | 2026-08-19 | 2026-08-25 | Codex-style generated-image gallery and lightbox for DeepSeek Harness |
| 901 | [aa2246740/dsh-resume](https://github.com/aa2246740/dsh-resume) | 0 | 2026-08-20 | 2026-08-25 | Continue Codex, Claude Code, and Cursor work in DeepSeek Harness |
| 902 | [aa2246740/pstack-dsh](https://github.com/aa2246740/pstack-dsh) | 0 | 2026-08-25 | 2026-08-25 | DeepSeek Harness port of official pstack. Playbooks and principles are poteto's; only the harness call layer is rewritten. |
| 903 | [ABccgh/dsh-github-plugin-tools](https://github.com/ABccgh/dsh-github-plugin-tools) | 0 | 2026-08-23 | 2026-08-23 | GitHub ↔ DSH plugin management: install / upload / uninstall tools |
| 904 | [ABccgh/dsh-ima-plugin](https://github.com/ABccgh/dsh-ima-plugin) | 0 | 2026-08-23 | 2026-08-23 | DeepSeek Harness dynamic Cordis plugin: ima_kb tool for Tencent IMA knowledge base, notes and experimental RAG qa |
| 905 | [ABccgh/dsh-plugin-dev](https://github.com/ABccgh/dsh-plugin-dev) | 0 | 2026-08-23 | 2026-08-23 | DSH dynamic Cordis plugin development: agent preset, demo plugins and templates |
| 906 | [ADDD1118/dsh-update](https://github.com/ADDD1118/dsh-update) | 0 | 2026-08-22 | 2026-08-22 | DeepSeek Harness (dsh) check-for-updates plugin — 右上角检查更新 UI + 关闭后自动升级 (npm / update-dsh.ps1) |
| 907 | [adrianleb/dsh-tmux-cc](https://github.com/adrianleb/dsh-tmux-cc) | 0 | 2026-08-25 | 2026-08-26 | A persistent, responsive tmux control-mode cockpit for DeepSeek Harness Web. |
| 908 | [AFAP/dsh-trajectory-traceview](https://github.com/AFAP/dsh-trajectory-traceview) | 0 | 2026-08-26 | 2026-08-26 | 轨迹视图插件：把 DeepSeek Harness Web GUI 会话的 AI 执行流程渲染为可回放的横向时间轴（minimap / 搜索 / 回放 / 步骤与子调用详情 / 原始请求分析 / Markdown 导出）。 |
| 909 | [AGSQ11/dsh-subagent-model-visibility](https://github.com/AGSQ11/dsh-subagent-model-visibility) | 0 | 2026-08-21 | 2026-08-22 | A small DeepSeek Harness plugin that shows the actual provider/model used by a subagent directly inside the existing native subagent tool-call row. |
| 910 | [AIMarshallLee/dsh-mcp-orchestrator](https://github.com/AIMarshallLee/dsh-mcp-orchestrator) | 0 | 2026-08-19 | 2026-08-23 | MCP orchestration layer for DeepSeek Harness — multi-server routing, health monitoring, fallback, and tool aggregation |
| 911 | [AIMarshallLee/dsh-obsidian-bridge](https://github.com/AIMarshallLee/dsh-obsidian-bridge) | 0 | 2026-08-18 | 2026-08-23 | Bidirectional knowledge bridge between DeepSeek Harness and Obsidian Vault — FTS5 search, draft writing, session linking |
| 912 | [AIMarshallLee/dsh-teacher-preset](https://github.com/AIMarshallLee/dsh-teacher-preset) | 0 | 2026-08-19 | 2026-08-23 | Teacher-focused vertical industry preset for DeepSeek Harness — lesson plans, rubrics, quizzes, and teaching materials generation |
| 913 | [aixlb/dsh-bcc](https://github.com/aixlb/dsh-bcc) | 0 | 2026-08-21 | 2026-08-22 | 包拆拆 for DeepSeek Harness: video to script/storyboard/style guide. dsh-plugin. |
| 914 | [AKI2253/Sidor_Character](https://github.com/AKI2253/Sidor_Character) | 0 | 2026-08-24 | 2026-08-24 | SIDOR 人设卡 —— DeepSeek Harness 附属插件：批量导入人设卡（.persona.md / 酒馆角色卡），自由加载/更换人设，会话内即时应用 + Agent 预设持久化。 |
| 915 | [AKUSH99/dsh-balance-chip](https://github.com/AKUSH99/dsh-balance-chip) | 0 | 2026-08-26 | 2026-08-26 | DeepSeek API balance in the DSH sidebar footer and bottom-right pill - live status dot plus amount, 60s refresh, API key stays in the local credential store |
| 916 | [alaxrpg/dsh-adaptive-model-router](https://github.com/alaxrpg/dsh-adaptive-model-router) | 0 | 2026-08-14 | 2026-08-25 | Adaptive model discovery, evaluation, tiering, and subagent routing for DeepSeek Harness |
| 917 | [aleleppy/leppy-loop-deepseek](https://github.com/aleleppy/leppy-loop-deepseek) | 0 | 2026-08-22 | 2026-08-22 | Native Leppy Loop bundle for DeepSeek Harness |
| 918 | [alex-dsh-plugin/open-in-vscode](https://github.com/alex-dsh-plugin/open-in-vscode) | 0 | 2026-08-24 | 2026-08-24 | DeepSeek Harness (dsh) Web 插件：工作区一键打开 VSCode，对话内文件路径点击跳转 VSCode（支持 文件:行:列） |
| 919 | [alexfengrui/dsh-client-ui-skin-real-madrid](https://github.com/alexfengrui/dsh-client-ui-skin-real-madrid) | 0 | 2026-08-25 | 2026-08-25 | Real Madrid dual-mode skin for DeepSeek Harness: Bernabeu night stadium (dark) and white-kit pinstripes (light). Unofficial fan work. |
| 920 | [AlexKaiqi/dsh-block-to-file](https://github.com/AlexKaiqi/dsh-block-to-file) | 0 | 2026-08-17 | 2026-08-22 | simple runtime ability to map a block to file, such that bash can access |
| 921 | [AlexKaiqi/dsh-temporary-workspace](https://github.com/AlexKaiqi/dsh-temporary-workspace) | 0 | 2026-08-18 | 2026-08-25 | Isolated temporary Workspaces for DeepSeek Harness |
| 922 | [alexpadholol/dsh-plugin-fusion](https://github.com/alexpadholol/dsh-plugin-fusion) | 0 | 2026-08-23 | 2026-08-23 | llm自采样插件 |
| 923 | [AliceLJY/dsh-thumb](https://github.com/AliceLJY/dsh-thumb) | 0 | 2026-08-21 | 2026-08-25 | A phone shell for the DeepSeek Harness (dsh) web GUI — sidebar becomes an overlay drawer, settings goes full-screen single column. Zero hardcoded host class hashes. |
| 924 | [aliuguofa/dsh-traffic-light](https://github.com/aliuguofa/dsh-traffic-light) | 0 | 2026-08-24 | 2026-08-24 | 一个 DeepSeek Harness Web UI 插件：在聊天输入框区域显示一盏红 / 黄 / 绿三色信号灯，实时反映当前会话的状态，点击可查看详情。 |
| 925 | [AllenLogo/dsh-software-tools](https://github.com/AllenLogo/dsh-software-tools) | 0 | 2026-08-21 | 2026-08-22 | DSH 侧边栏【软件工具】管理器:勾选本机 WSL/Windows 软件工具并注入模型系统提示,随插件自带 add-software-tool 技能。Sidebar software-tools manager for DeepSeek Harness Web. |
| 926 | [an4nsi/dsh-fork-view](https://github.com/an4nsi/dsh-fork-view) | 0 | 2026-08-21 | 2026-08-22 | DSH web plugin: replaces the native workspace browser in the left sidebar with a session tree in the style of pi-web by agegr. |
| 927 | [AnakinCao/dsh-code-nav](https://github.com/AnakinCao/dsh-code-nav) | 0 | 2026-08-26 | 2026-08-26 | DSH web plugin (dsh-better-sidebar companion): code preview with per-language syntax highlighting, symbol outline navigation and in-file search |
| 928 | [AnakinCao/dsh-md-export](https://github.com/AnakinCao/dsh-md-export) | 0 | 2026-08-26 | 2026-08-26 | DSH web plugin (dsh-better-sidebar companion): export the current .md file to standalone HTML (Mermaid inlined) or PDF - export button on the markdown toolbar |
| 929 | [anaksunamu/dsh-vidfetch](https://github.com/anaksunamu/dsh-vidfetch) | 0 | 2026-08-24 | 2026-08-24 | Give your DeepSeek Harness agent an on-demand video downloader |
| 930 | [andyfan1094/dsh-minimax-usage-pro](https://github.com/andyfan1094/dsh-minimax-usage-pro) | 0 | 2026-08-21 | 2026-08-22 | DSH bundle plugin showing MiniMax Token Plan / Subscription usage in Settings. Pro edition using webServer routes (host.call is unavailable to trusted bundle plugins on DSH 0.1.0-rc.8). |
| 931 | [ant404/dsh-media-gen](https://github.com/ant404/dsh-media-gen) | 0 | 2026-08-21 | 2026-08-22 | DSH plugin: generate images and videos via OpenAI-compatible providers, with dedicated settings menu and workspace media_gen output. |
| 932 | [Anyway-one/dsh-balance](https://github.com/Anyway-one/dsh-balance) | 0 | 2026-08-26 | 2026-08-26 | 为 DeepSeek Harness 提供持久化的余额与用量显示插件，让您随时掌握资源消耗情况，无需离开工作区。 |
| 933 | [anzhaohao/DragView](https://github.com/anzhaohao/DragView) | 0 | 2026-08-24 | 2026-08-25 | Drag-and-drop file attachments and secure in-app previews for DSH. |
| 934 | [anzhaohao/dsh-side-chat-plus-plus](https://github.com/anzhaohao/dsh-side-chat-plus-plus) | 0 | 2026-08-23 | 2026-08-23 | Codex 式多标签侧聊增强 - dsh-side-chat 破坏式 fork(多标签+整条消息引用+去 More details) |
| 935 | [aqiane/dsh-client-ui-period-hint](https://github.com/aqiane/dsh-client-ui-period-hint) | 0 | 2026-08-21 | 2026-08-22 | 在输入栏显示当前dsAPI价格时段 |
| 936 | [ArmyWas/dsh-codex-compat-canary](https://github.com/ArmyWas/dsh-codex-compat-canary) | 0 | 2026-08-25 | 2026-08-25 | Detect Codex App Server protocol drift that DeepSeek Harness cannot safely interpret. |
| 937 | [Asher-2000/dsh-artist-mode](https://github.com/Asher-2000/dsh-artist-mode) | 0 | 2026-08-22 | 2026-08-25 | DSH 艺术家模式 — 对话式设计交付预设（HTML 原生设计 / 反 AI slop / 5维评审 / Agnes AI 生图生视频） |
| 938 | [Asher-2000/dsh-inline-images](https://github.com/Asher-2000/dsh-inline-images) | 0 | 2026-08-24 | 2026-08-25 | 对话内联图片/视频:LLM 回复中输出的本地图片路径在消息正文直接渲染,视频可点击播放。修复增强版(URL自动修正/刷新持久化/反向代理兼容)。 |
| 939 | [asuramaya/osiris](https://github.com/asuramaya/osiris) | 0 | 2026-08-04 | 2026-08-22 | The persistent memory and coordination graph for AI agents (MCP, DeepSeek Harness, Claude Code, Cursor) |
| 940 | [AwesomeHou/dsh-trace-collapse](https://github.com/AwesomeHou/dsh-trace-collapse) | 0 | 2026-08-15 | 2026-08-25 | DeepSeek Harness web plugin: collapse the agent trajectory while always keeping the agent's final output; default-collapse after final output is on by default (configurable in Settings). |
| 941 | [B1lli/dsh-learning-bundle](https://github.com/B1lli/dsh-learning-bundle) | 0 | 2026-08-22 | 2026-08-24 | Proof-carrying correction learning for DSH: explicit adoption, scoped recall, and reconstructable delivery. |
| 942 | [BaiLiang-233/dsh-off-peak-schedule-widget](https://github.com/BaiLiang-233/dsh-off-peak-schedule-widget) | 0 | 2026-08-25 | 2026-08-25 | 价格时段输入队列调度 Harness 插件（dsh-plugin）：高峰拦截输入进休眠区，低谷按队列投递到目标对话 |
| 943 | [baiyuscc13724-max/dsh-godot-preview](https://github.com/baiyuscc13724-max/dsh-godot-preview) | 0 | 2026-08-25 | 2026-08-25 | Independent Godot 4 Web and native preview plugin for DeepSeek Harness |
| 944 | [bamboostrip/dsh-llm-capabilities](https://github.com/bamboostrip/dsh-llm-capabilities) | 0 | 2026-08-26 | 2026-08-26 | DSH plugin: auto-detect and configure model capabilities (reasoningEfforts + input modalities) for llm-pi-ai. Successor to dsh-reasoning-efforts. |
| 945 | [BarrierFly/apx-watchdog](https://github.com/BarrierFly/apx-watchdog) | 0 | 2026-08-26 | 2026-08-26 | 牛来写的东西 |
| 946 | [bbboy31/dsh-terminal-tabs](https://github.com/bbboy31/dsh-terminal-tabs) | 0 | 2026-08-26 | 2026-08-26 | Terminals view tab for DeepSeek Harness web UI — live background job count, streaming output, one-click kill |
| 947 | [BenYuan-Nolove-onani/dsh-token-stats](https://github.com/BenYuan-Nolove-onani/dsh-token-stats) | 0 | 2026-08-15 | 2026-08-23 | Token usage statistics plugin for DeepSeek Harness — per-window consumption metrics with an enable/disable switch, right in Settings.----------DeepSeek Harness 的 Token 用量统计插件：按时间窗统计消耗指标，设置页内随时启停。 |
| 948 | [berserk0501/dsh-soundscape](https://github.com/berserk0501/dsh-soundscape) | 0 | 2026-08-26 | 2026-08-26 | DSH 本机思考与工具音效插件，支持 MediaPlayer、WAV/MP3、自定义映射和设置面板 |
| 949 | [bescriptkiddie/dsh-wechat-collector](https://github.com/bescriptkiddie/dsh-wechat-collector) | 0 | 2026-08-26 | 2026-08-26 | DSH-native WeChat Official Account collector and ContentStudio handoff. |
| 950 | [bf185003/dsh-favicon-status](https://github.com/bf185003/dsh-favicon-status) | 0 | 2026-08-21 | 2026-08-24 | Browser tab status indicator plugin for DeepSeek Harness (dsh web): paints the document favicon from the sessions list projection - green done / amber waiting / blue running, spinning while work executes. |
| 951 | [Bigesila-B/dsh-media-forge](https://github.com/Bigesila-B/dsh-media-forge) | 0 | 2026-08-26 | 2026-08-26 | DSH Media Forge plugin: agent + skills workflow for media-generation APIs, with a sidebar skill panel (zh/en docs) |
| 952 | [bigfurma-bot/dsh-attention](https://github.com/bigfurma-bot/dsh-attention) | 0 | 2026-08-22 | 2026-08-24 | Approval attention watcher for DeepSeek Harness: bell sound + tab-title flash whenever an approval needs the owner's decision |
| 953 | [bigfurma-bot/dsh-todos](https://github.com/bigfurma-bot/dsh-todos) | 0 | 2026-08-22 | 2026-08-24 | Persistent shared to-do list for DeepSeek Harness: web UI tab + agent tools over one JSON store, writable from both sides |
| 954 | [bigfurma-bot/dsh-voice-dictation](https://github.com/bigfurma-bot/dsh-voice-dictation) | 0 | 2026-08-22 | 2026-08-24 | Push-to-talk voice dictation for DeepSeek Harness: mic button in the composer transcribes via local Parakeet STT into your message draft |
| 955 | [bigfurma-bot/dsh-web-restart](https://github.com/bigfurma-bot/dsh-web-restart) | 0 | 2026-08-25 | 2026-08-26 | One-click restart for DeepSeek Harness Web UI — arm-to-confirm button pinned to the Settings › General corner, live status dot, detached Linux restarter. Linux port of 1123762794/dsh-web-restart |
| 956 | [bigfurma-bot/dsh-websearch-mcp](https://github.com/bigfurma-bot/dsh-websearch-mcp) | 0 | 2026-08-22 | 2026-08-24 | Local web search for DeepSeek Harness via MCP — Bing/Brave/DuckDuckGo scraping, no API keys, agent-installable |
| 957 | [birdmanhj/dsh-mv-session](https://github.com/birdmanhj/dsh-mv-session) | 0 | 2026-08-25 | 2026-08-25 | A plug-in for Deepseek Harness that easy to move/rename session from old workspace to new workspace. |
| 958 | [BISTU-guheihei/DSH-SessionManager](https://github.com/BISTU-guheihei/DSH-SessionManager) | 0 | 2026-08-26 | 2026-08-26 | DSH 会话管理工具：可视化/命令行查看与删除历史聊天记录，自动清理缓存残留 |
| 959 | [bitterSmilezzz/dsh-ui-tweaks](https://github.com/bitterSmilezzz/dsh-ui-tweaks) | 0 | 2026-08-19 | 2026-08-23 | DeepSeek Harness 的界面增强插件：模型选择器（推理强度滑块）、粘贴/拖拽上传、插件列表增强、请求重试设置、全局快捷键、桌面通知 |
| 960 | [biyuhao/dsh-model-proxy](https://github.com/biyuhao/dsh-model-proxy) | 0 | 2026-08-22 | 2026-08-23 | DSH plugin: per-model proxy routing (http/https/socks5) with a settings UI — e.g. opencode/muse-spark-1.2-contributor needs a proxy while sibling models stay direct |
| 961 | [bo961386926/dolphin-pet-plugin](https://github.com/bo961386926/dolphin-pet-plugin) | 0 | 2026-08-26 | 2026-08-26 | Cute desktop pet for DeepSeek Harness - custom name, upload your own pet image, or generate one with AI. DSH 桌面宠物插件 |
| 962 | [Bobnemimimmi/dsh-always-status-bar](https://github.com/Bobnemimimmi/dsh-always-status-bar) | 0 | 2026-08-26 | 2026-08-26 | 始终显示消息下的 status bar，无需鼠标悬停 |
| 963 | [bochen2029-pixel/dsh-first-hop](https://github.com/bochen2029-pixel/dsh-first-hop) | 0 | 2026-08-25 | 2026-08-26 | Your agent wakes on evidence, not on a clock. A community plugin for DeepSeek Harness: watches the streams your harness already carries and decides - hold, flag, counsel, or wake. Local judge, shadow by default, MIT. |
| 964 | [boheastill/phone-eye](https://github.com/boheastill/phone-eye) | 0 | 2026-08-25 | 2026-08-25 | Let your AI agent see and operate a real Android phone — vision + UI-tree fusion over adb, for any MCP client (Claude Code, Codex, dsh…) |
| 965 | [BrianHIO-x/dsh-think-expand](https://github.com/BrianHIO-x/dsh-think-expand) | 0 | 2026-08-22 | 2026-08-22 | DeepSeek Harness plugin that auto-expands Think rows while reasoning |
| 966 | [BrucePayton/dsh-plugin-graphgpt](https://github.com/BrucePayton/dsh-plugin-graphgpt) | 0 | 2026-08-22 | 2026-08-23 | Run validated GraphGPT workflows as native DeepSeek Harness tools |
| 967 | [buchylx/create-dsh-content-plugin](https://github.com/buchylx/create-dsh-content-plugin) | 0 | 2026-08-26 | 2026-08-26 | Zero-dependency CLI that scaffolds a content-automation DSH plugin (Dev.to/GitHub/Bluesky/Mastodon). Like create-vite, for DSH. |
| 968 | [buildbeforewepitch/agentscars](https://github.com/buildbeforewepitch/agentscars) | 0 | 2026-08-21 | 2026-08-22 | A public commons of real AI-agent failure patterns ("scars") — searchable via API and MCP. Live at agentscars.com. |
| 969 | [c2j/dsh-swarmforge](https://github.com/c2j/dsh-swarmforge) | 0 | 2026-08-23 | 2026-08-24 | SwarmForge migrate as a DeepSeek Harness Plugin |
| 970 | [CarlMarkswx/deepseek-multimodel](https://github.com/CarlMarkswx/deepseek-multimodel) | 0 | 2026-08-24 | 2026-08-24 | Unified vision and image-generation plugin suite for DeepSeek Harness |
| 971 | [Castem114/dsh-visioncraft](https://github.com/Castem114/dsh-visioncraft) | 0 | 2026-08-26 | 2026-08-26 | 为 DeepSeek Harness（DSH）Web 量身打造的双插件扩展，为纯文本模型补齐"视觉"短板 |
| 972 | [chancoki/dsh-model-search-plugin](https://github.com/chancoki/dsh-model-search-plugin) | 0 | 2026-08-24 | 2026-08-24 | 为 DeepSeek Harness (DSH) Web GUI 提供模型搜索功能的插件——在模型选择弹窗中添加关键字搜索框，快速筛选模型。 |
| 973 | [change979666/ox-alpha-dsh](https://github.com/change979666/ox-alpha-dsh) | 0 | 2026-08-25 | 2026-08-25 | [Model Hub for DSH] Lightweight model/provider integration toolkit for DeepSeek Harness Desktop - one plugin installs Ox Alpha (stealth/ox-alpha), plus custom models, custom OpenAI-compatible providers, health check, discovery and rollback. bilingual zh/en |
| 974 | [chaoliu615/dsh-agnes](https://github.com/chaoliu615/dsh-agnes) | 0 | 2026-08-20 | 2026-08-26 | 为在dsh中使用Agnes AI的免费图片、视频生成功能而开发，欢迎使用！欢迎提issues。 |
| 975 | [Che-Year/dsh-pet-lulu](https://github.com/Che-Year/dsh-pet-lulu) | 0 | 2026-08-26 | 2026-08-26 | A cute terminal and web pet plugin for DeepSeek Harness (dsh), using assets from lulu and capybara projects. |
| 976 | [chemmy-11/dsh-xuegulin](https://github.com/chemmy-11/dsh-xuegulin) | 0 | 2026-08-24 | 2026-08-25 | Vault observation plugin for DeepSeek Harness: Obsidian vault metadata snapshot + edit stats + observation panel |
| 977 | [chendefine/dsh-better-sidebar-onlyoffice](https://github.com/chendefine/dsh-better-sidebar-onlyoffice) | 0 | 2026-08-24 | 2026-08-25 | DSH web plugin: open and edit .docx/.xlsx/.pptx in the better-sidebar editor through a self-hosted ONLYOFFICE Document Server (JWT-signed config, atomic save-back, live refresh on AI edits) |
| 978 | [chendefine/dsh-web-search-aggregation](https://github.com/chendefine/dsh-web-search-aggregation) | 0 | 2026-08-23 | 2026-08-23 | Aggregated web-search provider for DeepSeek Harness (DSH): one prioritized queue over AnySearch / TinyFish / Tavily with multi-key rotation and ordered fallback. |
| 979 | [chengoak/dsh-font-size](https://github.com/chengoak/dsh-font-size) | 0 | 2026-08-21 | 2026-08-22 | DSH Web GUI plugin: 'Conversation font size' slider (12-22 px) in Settings → General. |
| 980 | [ChengxiuCDP/dsh-migrate-codex](https://github.com/ChengxiuCDP/dsh-migrate-codex) | 0 | 2026-08-23 | 2026-08-23 | DSH plugin: safely migrate a Codex environment between machines (/migrate-codex command + codex-migration skill) |
| 981 | [chenyedamw/dropshipping-product-scout](https://github.com/chenyedamw/dropshipping-product-scout) | 0 | 2026-08-22 | 2026-08-25 | Dropshipping Product Scout MCP 服务的 Claude Code 插件 —— 精选商品搜索、库存查询与物流估算  |
| 982 | [cinderzhan/dsh-plugin-dew](https://github.com/cinderzhan/dsh-plugin-dew) | 0 | 2026-08-26 | 2026-08-26 | See what your other coding agents are doing from inside DSH: Claude Code, Codex, Cursor and DSH sessions, their state, and their scheduled tasks. |
| 983 | [Cinnamobot/dsh-disclosure-tweaks](https://github.com/Cinnamobot/dsh-disclosure-tweaks) | 0 | 2026-08-25 | 2026-08-25 | Auto-expand/collapse DSH conversation disclosure rows (Think, tool calls, context, todo, queue) with per-type Settings toggles. Manual toggles are never overridden. |
| 984 | [Cinnamobot/dsh-nothing-skin](https://github.com/Cinnamobot/dsh-nothing-skin) | 0 | 2026-08-25 | 2026-08-25 | Nothing Phone style skin for DeepSeek Harness — dot-matrix background, Space Grotesk/Mono, monochrome + signal red, per-feature Settings toggles |
| 985 | [Circleyan/whiteboat-dsh](https://github.com/Circleyan/whiteboat-dsh) | 0 | 2026-08-25 | 2026-08-25 | Whiteboat for DeepSeek Harness; the quiet water surface is the first feature slice. |
| 986 | [cKNKSnd/dsh-model-provider-badge](https://github.com/cKNKSnd/dsh-model-provider-badge) | 0 | 2026-08-19 | 2026-08-23 | DeepSeek Harnes 输入框当前模型提供商名称 |
| 987 | [CLASSLU/dsh-telegram-bridge](https://github.com/CLASSLU/dsh-telegram-bridge) | 0 | 2026-08-24 | 2026-08-24 | Telegram bridge for DeepSeek Harness (dsh): chat with your DSH agent from Telegram — access control, skills, workspace browsing, file transfer. |
| 988 | [cmhaoren-sudo/dsh-tab-status](https://github.com/cmhaoren-sudo/dsh-tab-status) | 0 | 2026-08-22 | 2026-08-23 | DSH plugin: leave long-running tasks and watch yellow/green/blue on the Firefox, Chrome, or Edge tab. 长程任务可切出去，标签仍能看到状态。 |
| 989 | [co-Elly/dsh-plugin-vision](https://github.com/co-Elly/dsh-plugin-vision) | 0 | 2026-08-22 | 2026-08-22 | 👁️ Give your DeepSeek Harness the gift of sight — enables pure-text LLMs to analyze images via Zhipu's free GLM-4V-Flash vision model |
| 990 | [Co-Kyo/dsh-interview-forge](https://github.com/Co-Kyo/dsh-interview-forge) | 0 | 2026-08-22 | 2026-08-22 | interview-forge-plugin for deepseek harness |
| 991 | [coffee-man666/dsh-lens](https://github.com/coffee-man666/dsh-lens) | 0 | 2026-08-22 | 2026-08-23 | Repository and agent-runtime analysis skills as an installable DeepSeek Harness (dsh) plugin |
| 992 | [ConTr0L0/dsh-balance-monitor](https://github.com/ConTr0L0/dsh-balance-monitor) | 0 | 2026-08-22 | 2026-08-25 | dsh-balance-monitor 是 DeepSeek Harness（DSH）的插件：在侧边栏实时显示 API 余额，按官方峰谷价目（每日自动从 DeepSeek 官方文档同步）精确计算每次请求成本，按会话/模型/日期拆分消耗统计，并支持每日、累计、请求次数三类上限（可硬拦截后续 LLM 请求）。Web 端与桌面端通用，计费口径已与 DeepSeek 平台账单逐项对账 |
| 993 | [cslht11/dsh-custom-patches](https://github.com/cslht11/dsh-custom-patches) | 0 | 2026-08-18 | 2026-08-24 | DSH (DeepSeek Harness) 自定义增强补丁集：输入历史 + 编辑最后一条消息并重新生成。Custom enhancements for the DeepSeek Harness Web GUI via compiled-artifact patches. |
| 994 | [cslht11/dsh-provider-config](https://github.com/cslht11/dsh-provider-config) | 0 | 2026-08-26 | 2026-08-26 | DSH (DeepSeek Harness) LLM 供应商配置模板与限流重试机制最佳实践（SenseNova 脱敏版）。Provider config templates + retry-policy best practices for DSH, sanitized. |
| 995 | [cslht11/dsh-ssh-remote](https://github.com/cslht11/dsh-ssh-remote) | 0 | 2026-08-20 | 2026-08-24 | DeepSeek Harness SSH 远程工作区插件（多机并行）：同时连接多台服务器，Agent 直接查看/编辑/执行远程文件。基于 flymysql/dsh-remote (MIT) 适配 0.1.1-rc.2 |
| 996 | [cstarc/dsh-skill-mcp-bridge](https://github.com/cstarc/dsh-skill-mcp-bridge) | 0 | 2026-08-26 | 2026-08-26 | dsh 项目桥接插件：自动导入 .claude/.agents/.trae skills 并桥接 MCP 服务器（HTTP/SSE + stdio），GUI 开关控制、状态持久化 |
| 997 | [da-beda/dsh-lockstep](https://github.com/da-beda/dsh-lockstep) | 0 | 2026-08-24 | 2026-08-24 | Pin-aware updater for DeepSeek Harness. Check lockfile drift, plan pin bumps, never float to latest. |
| 998 | [daetz-coder/DSH-Mobile](https://github.com/daetz-coder/DSH-Mobile) | 0 | 2026-08-24 | 2026-08-25 | DSH-Mobile · 把 DeepSeek Harness 装进口袋 — scan-to-pair Android companion for the official DeepSeek Harness Web UI. DeepSeek Harness 手机配套：扫码配对、状态通知、桌面远程控制。 |
| 999 | [dat-lequoc/dsh-shots](https://github.com/dat-lequoc/dsh-shots) | 0 | 2026-08-22 | 2026-08-22 | Shots tab for DeepSeek Harness: live screenshot player over a browser daemon's shots/ feed (dsh plugin) |
| 1000 | [david0702/dsh-cost](https://github.com/david0702/dsh-cost) | 0 | 2026-08-26 | 2026-08-26 | DSH (DeepSeek Harness) 对话底部费用显示插件：按每笔请求时间+模型分批计费，分时段明细，模型归属，读图金额，余额。 |
| 1001 | [DavidRm1911/dsh-llm-subscription](https://github.com/DavidRm1911/dsh-llm-subscription) | 0 | 2026-08-24 | 2026-08-25 | Native DeepSeek Harness LLM adapter for Claude Code / Antigravity CLI subscriptions — no API key |
| 1002 | [DavidRm1911/dsh-subscription-gateway](https://github.com/DavidRm1911/dsh-subscription-gateway) | 0 | 2026-08-24 | 2026-08-25 | OpenAI-compatible gateway that lets DeepSeek Harness use your existing Claude Code / Antigravity / Ollama logins instead of a paid API key |
| 1003 | [dddzzz123-dz/dsh-read-image-plugin](https://github.com/dddzzz123-dz/dsh-read-image-plugin) | 0 | 2026-08-22 | 2026-08-22 | Image input fallback for DeepSeek Harness with native multimodal model detection and Volcengine Ark vision. |
| 1004 | [DecresLuna/DSH-Service](https://github.com/DecresLuna/DSH-Service) | 0 | 2026-08-22 | 2026-08-22 | DSH Service - DeepSeek Harness Mac 菜单栏服务管理器 |
| 1005 | [DeepseekHarnessPlugins/Notification](https://github.com/DeepseekHarnessPlugins/Notification) | 0 | 2026-08-26 | 2026-08-26 | DeepseekHarnessPlugin |
| 1006 | [DeepVite/dsh-model-selector](https://github.com/DeepVite/dsh-model-selector) | 0 | 2026-08-23 | 2026-08-26 | 梁文谷插件 · DeepSeek Harness 模型选择器升级：一级菜单模型/思考档位选择 + 自定义模型别名 + 高峰低谷计价倒计时。Apache-2.0 |
| 1007 | [delock/dsh-pr-board](https://github.com/delock/dsh-pr-board) | 0 | 2026-08-26 | 2026-08-26 | Maintainer PR review queue board for DeepSeek Harness: five-state tracking (waiting on me / waiting on author / ready to merge / merged / inbox), sidebar counters, fullscreen kanban, polling, and back-to-you transition toasts. |
| 1008 | [Demigod-cyber/dsh-angelina-theme](https://github.com/Demigod-cyber/dsh-angelina-theme) | 0 | 2026-08-26 | 2026-08-26 | DSH主题插件——直到大地变成一颗酸橙（Angelina 浅蓝主题） |
| 1009 | [DemoJ/proactive-notify](https://github.com/DemoJ/proactive-notify) | 0 | 2026-08-20 | 2026-08-22 | 一个运行在 DeepSeek Harness（DSH）Web GUI 上的消息通知插件 |
| 1010 | [Destined-at-Dawn/dsh-visual-workbench](https://github.com/Destined-at-Dawn/dsh-visual-workbench) | 0 | 2026-08-25 | 2026-08-26 | A DSH visual workbench for Obsidian-style knowledge spaces and local Comfy MCP workflows. |
| 1011 | [DevViking-Persike/dsh-docker](https://github.com/DevViking-Persike/dsh-docker) | 0 | 2026-08-22 | 2026-08-22 | DeepSeek Harness plugin: Docker container, image, log, and Compose tools for the agent, over the local Docker CLI |
| 1012 | [DevViking-Persike/dsh-git-graph](https://github.com/DevViking-Persike/dsh-git-graph) | 0 | 2026-08-25 | 2026-08-26 | DeepSeek Harness plugin: a Git commit-graph view with lanes, refs, and worktree management |
| 1013 | [DevViking-Persike/dsh-monaco](https://github.com/DevViking-Persike/dsh-monaco) | 0 | 2026-08-22 | 2026-08-22 | DeepSeek Harness plugin: serves the Monaco editor distribution over a host HTTP route, so an editor plugin needs no CDN |
| 1014 | [dongsheng123132/dsh-artifact-promotion-proof](https://github.com/dongsheng123132/dsh-artifact-promotion-proof) | 0 | 2026-08-26 | 2026-08-26 | Offline proof that one immutable artifact followed a declared promotion chain |
| 1015 | [dongsheng123132/dsh-attestation-proof](https://github.com/dongsheng123132/dsh-attestation-proof) | 0 | 2026-08-25 | 2026-08-25 | Offline content-addressed DSSE/in-toto attestation proof for DeepSeek Harness |
| 1016 | [dongsheng123132/dsh-break-glass-settlement-proof](https://github.com/dongsheng123132/dsh-break-glass-settlement-proof) | 0 | 2026-08-26 | 2026-08-26 | Offline content-addressed DSH proof for break-glass session settlement evidence |
| 1017 | [dongsheng123132/dsh-build-hermeticity-proof](https://github.com/dongsheng123132/dsh-build-hermeticity-proof) | 0 | 2026-08-26 | 2026-08-26 | Offline hash-only proof that recorded build accesses stayed within a declared closure |
| 1018 | [dongsheng123132/dsh-change-window-proof](https://github.com/dongsheng123132/dsh-change-window-proof) | 0 | 2026-08-26 | 2026-08-26 | Offline content-addressed DSH proof for change-window settlement evidence |
| 1019 | [dongsheng123132/dsh-policy-waiver-proof](https://github.com/dongsheng123132/dsh-policy-waiver-proof) | 0 | 2026-08-25 | 2026-08-26 | Offline content-addressed proof that temporary DSH policy waivers stayed within approved bounds |
| 1020 | [dongsheng123132/dsh-principal-binding-proof](https://github.com/dongsheng123132/dsh-principal-binding-proof) | 0 | 2026-08-25 | 2026-08-26 | Offline content-addressed proof of pseudonymous authority binding across DSH execution surfaces |
| 1021 | [dongsheng123132/dsh-reproducible-build-proof](https://github.com/dongsheng123132/dsh-reproducible-build-proof) | 0 | 2026-08-26 | 2026-08-26 | Offline content-addressed proof that independent build receipts reproduced byte-identical specified artifacts |
| 1022 | [dongsheng123132/dsh-retention-settlement-proof](https://github.com/dongsheng123132/dsh-retention-settlement-proof) | 0 | 2026-08-25 | 2026-08-25 | Body-free retention settlement and non-resurrection evidence for DeepSeek Harness |
| 1023 | [dongsheng123132/dsh-tool-surface-proof](https://github.com/dongsheng123132/dsh-tool-surface-proof) | 0 | 2026-08-25 | 2026-08-26 | Deployment-scoped model-visible DSH tool surface conformance evidence |
| 1024 | [dongsheng123132/dsh-windows-settlement-proof](https://github.com/dongsheng123132/dsh-windows-settlement-proof) | 0 | 2026-08-25 | 2026-08-26 | Offline content-addressed proof that approved Windows control-plane changes settled across required surfaces |
| 1025 | [DosterBool/dsh-zombie-gc](https://github.com/DosterBool/dsh-zombie-gc) | 0 | 2026-08-22 | 2026-08-22 | DSH 插件：开机清理僵尸 agent（已收尾会话仍挂 registry，导致退出重进后输入框卡死） |
| 1026 | [dougen/dsh-deepseek-usage](https://github.com/dougen/dsh-deepseek-usage) | 0 | 2026-08-23 | 2026-08-23 | DeepSeek usage sidebar plugin for DeepSeek Harness: account balance (official API), current unit pricing and peak/off-peak indicator, zh/en UI. |
| 1027 | [DreamZhongJu/dsh-smart-model-router](https://github.com/DreamZhongJu/dsh-smart-model-router) | 0 | 2026-08-23 | 2026-08-24 | A configurable Smart Model Router bundle for DeepSeek Harness (DSH). |
| 1028 | [dsh-plugins/dsh-network-settings](https://github.com/dsh-plugins/dsh-network-settings) | 0 | 2026-08-21 | 2026-08-22 | A DeepSeek Harness plugin that bundles three network capabilities — User-Agent rewriting (from @dsh-plugin/dsh-user-agent), a HTTP / HTTPS-CONNECT / SOCKS5 proxy (from dsh-net-proxy), and configurable request auto-retry — all driven from a single 网络设置 (Network) tab in the Web settings. |
| 1029 | [dsh-plugins/dsh-plugin-market](https://github.com/dsh-plugins/dsh-plugin-market) | 0 | 2026-08-26 | 2026-08-26 | A structured plugin marketplace for DeepSeek Harness — each plugin described as JSON, auto-aggregated into a single plugins.json for the dsh-plugins.github.io site. DeepSeek Harness 结构化插件市场 —— 每个插件以 JSON 描述，自动聚合为单一 plugins.json 供 dsh-plugins.github.io 站点消费。 |
| 1030 | [dsh-plugins/dsh-user-agent](https://github.com/dsh-plugins/dsh-user-agent) | 0 | 2026-08-21 | 2026-08-22 | Rewrites the User-Agent sent by every outgoing HTTP request (LLM API calls and other global-fetch traffic) to a value of your choice, configured live from a dedicated UA 设置 (User-Agent) tab in the Web settings. 为 dsh 发出的所有出站 HTTP 请求（LLM API 调用等走全局 fetch 的流量）改写 User-Agent，并可在 Web 设置的 UA 设置 选项卡中实时配置。 |
| 1031 | [dshworks/dsh-ego-browser](https://github.com/dshworks/dsh-ego-browser) | 0 | 2026-08-24 | 2026-08-24 | ego lite browser automation for dsh that remembers — recall a site's learned tools, promote a working script into a new one, hand the user the keyboard for real. 7 tools, host-only, MIT. |
| 1032 | [dubeno/dsh-agent-plugin-bridge](https://github.com/dubeno/dsh-agent-plugin-bridge) | 0 | 2026-08-20 | 2026-08-25 | 将符合Agent Plugin规范的插件适配到DSH生态 |
| 1033 | [dujar/dsh-community-plugins](https://github.com/dujar/dsh-community-plugins) | 0 | 2026-08-25 | 2026-08-25 | DeepSeek Harness web-GUI plugin: discover and install community plugins from the dsh-plugin topic — searchable SQLite catalog, fork browser, local-plugin installs |
| 1034 | [dujar/dsh-restart](https://github.com/dujar/dsh-restart) | 0 | 2026-08-25 | 2026-08-25 | DeepSeek Harness web-GUI plugin: restart dsh web in one click, toggle installed plugins, git panel for local checkouts |
| 1035 | [dxsdyhm/dsh-adb-logcat](https://github.com/dxsdyhm/dsh-adb-logcat) | 0 | 2026-08-26 | 2026-08-26 | Android Studio-style ADB logcat viewer for the DSH Web GUI |
| 1036 | [elevenmoon999/dsh-clash-proxy](https://github.com/elevenmoon999/dsh-clash-proxy) | 0 | 2026-08-25 | 2026-08-25 | 智能分流 · 自包含 · 上手简单 —— DeepSeek Harness 规则分流代理插件（国内直连 / 国外走订阅节点），完全由 AI 生成。 |
| 1037 | [elizax/dsh-http-proxy](https://github.com/elizax/dsh-http-proxy) | 0 | 2026-08-26 | 2026-08-26 | 支持设置LLM的代理地址 |
| 1038 | [elonnzhang/dsh-plugin-template](https://github.com/elonnzhang/dsh-plugin-template) | 0 | 2026-08-21 | 2026-08-23 | DeepSeek Harness (dsh) 插件开发模版：最小化模版 + 全能力模版，含构建方式与加载到 dsh 的完整路径 |
| 1039 | [elonnzhang/dsh-system-prompt](https://github.com/elonnzhang/dsh-system-prompt) | 0 | 2026-08-23 | 2026-08-23 | DeepSeek Harness plugin for session-scoped system prompt inspection |
| 1040 | [emeryxu1-blip/dsh-matrix-skin](https://github.com/emeryxu1-blip/dsh-matrix-skin) | 0 | 2026-08-22 | 2026-08-24 | Black-first Matrix hacker skin for DeepSeek Harness (DSH) Web — live session-powered code rain and readable provider reasoning. |
| 1041 | [Emilia-awa/hermes-dsh-bridge](https://github.com/Emilia-awa/hermes-dsh-bridge) | 0 | 2026-08-24 | 2026-08-25 | Hermes ↔ DeepSeek Harness MCP bridge: drive dsh agents (tasks, sessions, files, presets, stats) from any MCP client. Hermes = brain, Harness = arms. |
| 1042 | [emircanerkul/dsh-terminal](https://github.com/emircanerkul/dsh-terminal) | 0 | 2026-08-18 | 2026-08-24 | Workspace-aware web terminal plugin for the DeepSeek Harness (dsh). Runs a streaming PTY terminal at /terminal and embeds a split-pane terminal dock powered by xterm.js. |
| 1043 | [entireyu/dsh-webui-plus](https://github.com/entireyu/dsh-webui-plus) | 0 | 2026-08-25 | 2026-08-25 | DeepSeek Harness Webui 增强插件，自带对话锚点、归档任务等功能 |
| 1044 | [esonx/dsh-workforce](https://github.com/esonx/dsh-workforce) | 0 | 2026-08-23 | 2026-08-23 | Project-scoped organization and long-lived AI workforce layer for DeepSeek Harness |
| 1045 | [ESxyzbil/dsh-official-document-mode](https://github.com/ESxyzbil/dsh-official-document-mode) | 0 | 2026-08-22 | 2026-08-23 | DSH ??????:?????? + ??????? + ???? |
| 1046 | [Ever0330/universal-vision](https://github.com/Ever0330/universal-vision) | 0 | 2026-08-24 | 2026-08-24 | Universal vision-model plugin for DeepSeek Harness, enabling image description using any configured vision model. |
| 1047 | [EvieHe/dsh-resume-headless](https://github.com/EvieHe/dsh-resume-headless) | 0 | 2026-08-24 | 2026-08-24 | DeepSeek Harness (dsh) bundle: headless one-shot session resume. `dsh --profile headless --resume <session-id> "task"` continues a persisted session (history and turn numbering carry on), prints and exits. Overrides the official headless runner via ctx.agents.resume(); install with `dsh plugin add github:EvieHe/dsh-resume-headless#v0.1.1`. |
| 1048 | [exoticknight/dsh-theme-eink-retro](https://github.com/exoticknight/dsh-theme-eink-retro) | 0 | 2026-08-26 | 2026-08-26 | A paper-and-ink client-side theme for DeepSeek Harness with Balanced and Immersive modes. |
| 1049 | [Fabian-698/dsh-plugin-dev](https://github.com/Fabian-698/dsh-plugin-dev) | 0 | 2026-08-25 | 2026-08-25 | DeepSeek Harness (DSH) plugin development agent skill: 6 form typology, verify-plugin.mjs P1-P13 gate, scaffold generator, security discipline, and curated ecosystem backfills. An Agent Skill (SKILL.md), not an npm bundle. |
| 1050 | [fan56/dsh-feishu](https://github.com/fan56/dsh-feishu) | 0 | 2026-08-23 | 2026-08-26 | dsh plugin: drive an existing dsh session from Feishu/Lark — outbound-only bot, /resume picker, run status card |
| 1051 | [fan56/dsh-llm-net-retry](https://github.com/fan56/dsh-llm-net-retry) | 0 | 2026-08-22 | 2026-08-22 | dsh plugin: bounded retry for gateway network_error failures the stock retry policy cannot classify |
| 1052 | [fanfan6/dsh-model-search](https://github.com/fanfan6/dsh-model-search) | 0 | 2026-08-22 | 2026-08-22 | DSH 模型搜索插件 - 跨平台快速筛选模型 |
| 1053 | [fastengiel-kurai/dsh-peekfile-everything](https://github.com/fastengiel-kurai/dsh-peekfile-everything) | 0 | 2026-08-19 | 2026-08-22 | DSH local file search, clickable path detection, and floating preview plugin with optional EverythingCLI integration. |
| 1054 | [fatatalia/dsh-ledger](https://github.com/fatatalia/dsh-ledger) | 0 | 2026-08-18 | 2026-08-25 | dsh 只读记账仪表盘插件：会话页「记账」Tab 展示 beancount 账本月度快照（收支总览/资产结构动态分组/支出分类/最近交易），只读，复用 ledger.py，Fava 保留做深度分析 |
| 1055 | [fatatalia/dsh-turn-guard](https://github.com/fatatalia/dsh-turn-guard) | 0 | 2026-08-23 | 2026-08-25 | dsh turn-guard plugin: per-step timeout for agent turns (防模型退化死循环) |
| 1056 | [faye0526/dsh-backup-btn](https://github.com/faye0526/dsh-backup-btn) | 0 | 2026-08-26 | 2026-08-26 | DSH 一键备份按钮 - 浮动按钮备份 DSH 数据到 GitHub Gist |
| 1057 | [fbzz/readproof](https://github.com/fbzz/readproof) | 0 | 2026-08-21 | 2026-08-22 | Readproof — the lockfile and replay primitive for what AI agents read: stable identity, freshness policy, content-addressed snapshots, per-run manifests, diff, byte-exact replay, evidence bundles. |
| 1058 | [firestige/execution-system](https://github.com/firestige/execution-system) | 0 | 2026-08-17 | 2026-08-25 | Host-neutral execution boundary for workflow-self-recursive: resolves one exact Workflow Package, binds an immutable Delivery Manifest, coordinates the Delivery, emits bounded OTLP observations. Install via dsh plugin add wsr-dsh-intake · 与宿主无关的 Agent 工作流执行边界：解析并校验确定的工作流包，绑定不可变交付清单，协调交付并发出有界观测。 |
| 1059 | [Fisfzy/dsh-danus](https://github.com/Fisfzy/dsh-danus) | 0 | 2026-08-23 | 2026-08-25 | Verifier-gated multi-agent mathematical proof-search orchestration, native to DeepSeek Harness: content-addressed fact graph, role-gated tools, cold-start verifier, worker swarm, paper/report rendering. TypeScript, cross-platform. Based on Danus (frenzymath). |
| 1060 | [fishOfOUC/plugin-ui-controls](https://github.com/fishOfOUC/plugin-ui-controls) | 0 | 2026-08-23 | 2026-08-23 | Plugin control composer panel: the conversation.input.plugins seat over the pluginInventory Remote |
| 1061 | [Flan246/dsh-latex-guard](https://github.com/Flan246/dsh-latex-guard) | 0 | 2026-08-26 | 2026-08-26 | LaTeX compile check and BibTeX lint/fill/audit tools for DeepSeek Harness and any agent. dsh plugin + CLI + SKILL.md. |
| 1062 | [Flan246/dsh-lit-search](https://github.com/Flan246/dsh-lit-search) | 0 | 2026-08-26 | 2026-08-26 | Academic literature search, citation and BibTeX tools for DeepSeek Harness and any agent (Crossref + OpenAlex). dsh plugin + CLI + SKILL.md. |
| 1063 | [Flonger/dsh-balance-vision](https://github.com/Flonger/dsh-balance-vision) | 0 | 2026-08-25 | 2026-08-25 | DeepSeek balance & session cost for DSH web UI, with official weekday peak/off-peak pricing and deepseek-v4-flash-vision-exp vision model support (same rate as flash) |
| 1064 | [Flonger/dsh-multi-clear](https://github.com/Flonger/dsh-multi-clear) | 0 | 2026-08-25 | 2026-08-26 | Multi-select clear (archive) workspace conversations and bulk-delete empty workspaces in the DSH sidebar, with workspace-level selection, tri-state checkboxes and confirm dialogs |
| 1065 | [flowingboy/dsh-local-perf](https://github.com/flowingboy/dsh-local-perf) | 0 | 2026-08-23 | 2026-08-23 | Durable DeepSeek Harness bundle: local-model performance tuning as a re-installable plugin layer (compaction, tool-result pruning, time context, cloud title routing, text-toolcall guard) — survives dsh updates |
| 1066 | [flyhigao/dsh-produced-file-paths](https://github.com/flyhigao/dsh-produced-file-paths) | 0 | 2026-08-20 | 2026-08-23 | DSH Web plugin to show and copy absolute paths for produced files |
| 1067 | [FMDD61/dsh-oauth-copilot](https://github.com/FMDD61/dsh-oauth-copilot) | 0 | 2026-08-23 | 2026-08-24 | GitHub Copilot OAuth sign-in and model route for DeepSeek Harness |
| 1068 | [fogmodel/dsh-workspace-jump](https://github.com/fogmodel/dsh-workspace-jump) | 0 | 2026-08-23 | 2026-08-23 | DSH web plugin: quickly create or switch to a workspace from a directory path via the sidebar Workspace button. |
| 1069 | [founder987/dsh-dev-ui](https://github.com/founder987/dsh-dev-ui) | 0 | 2026-08-25 | 2026-08-26 | 适合编码研发的UI界面 |
| 1070 | [fplj-fplj/dsh-ua-headers](https://github.com/fplj-fplj/dsh-ua-headers) | 0 | 2026-08-23 | 2026-08-25 | 为 DeepSeek Harness (DSH) 定制的 User-Agent 与请求头插件：按模型匹配改写 UA / 合并自定义请求头，遵循 dsh-ecosystem-spec 生态规范。A dsh-ecosystem-spec compliant plugin to customize User-Agent and request headers per model. |
| 1071 | [Francesco502/dsh-quota](https://github.com/Francesco502/dsh-quota) | 0 | 2026-08-26 | 2026-08-26 | AI Quota and Token Usage Monitor for DeepSeek Harness (Codex, Cursor, Antigravity, OpenCode-Go) |
| 1072 | [frederico-kluser/dsh-plugin-dev-agent-skill](https://github.com/frederico-kluser/dsh-plugin-dev-agent-skill) | 0 | 2026-08-22 | 2026-08-22 | Global agent skill: create, extend, secure, test and publish Cordis plugins for the DeepSeek Harness (DSH). Verified-by-measurement API surface (ctx.webServer, spawn(spec)), frontend levers, IPC, security, testing, packaging & publishing. |
| 1073 | [FriendsHL/dsh-reviewed-development-orchestrator](https://github.com/FriendsHL/dsh-reviewed-development-orchestrator) | 0 | 2026-08-26 | 2026-08-26 | Reviewed five-stage software-development orchestration for DeepSeek Harness |
| 1074 | [Frog755/dsh-wallpaper](https://github.com/Frog755/dsh-wallpaper) | 0 | 2026-08-15 | 2026-08-24 | Persistent wallpaper plugin for DeepSeek Harness with opacity, blur, and a fixed web origin. |
| 1075 | [FYHC1/dsh-web-manager](https://github.com/FYHC1/dsh-web-manager) | 0 | 2026-08-20 | 2026-08-23 | dsh-plugin + Windows tray manager for DeepSeek Harness WebUI (dsh web): standalone Edge app-window with the official whale icon, quick-launch desktop shortcuts for Windows/WSL, systemd hosting, runtime bridge, self-update. Legacy shortcut-only plugin (v1.x): https://github.com/FYHC1/dsh-webui-installer |
| 1076 | [FYHC1/dsh-webui-installer](https://github.com/FYHC1/dsh-webui-installer) | 0 | 2026-08-20 | 2026-08-23 | Legacy dsh plugin (v1.x, EOL): one-click desktop shortcuts that launch the DeepSeek Harness WebUI (dsh web) as a standalone app window on Windows / WSL / Linux. Need tray-based background management (multi-instance, systemd, self-update)? Use dsh-web-manager instead: https://github.com/FYHC1/dsh-web-manager |
| 1077 | [Gan332/dsh-typography](https://github.com/Gan332/dsh-typography) | 0 | 2026-08-23 | 2026-08-23 | Typography plugin for DeepSeek Harness - independent interface & code fonts, online presets, zero-conversion local font library (woff2/ttf/otf) |
| 1078 | [Gaochenyuen/dsh-scopus-searcher](https://github.com/Gaochenyuen/dsh-scopus-searcher) | 0 | 2026-08-24 | 2026-08-25 | Deep literature research agent as a Deepseek-Harness preset powered by Scopus API. |
| 1079 | [gaowei-AFK/dsh-prompt-polish](https://github.com/gaowei-AFK/dsh-prompt-polish) | 0 | 2026-08-26 | 2026-08-26 | Prompt polish ✨ — one-click rewrite of rough input into a structured professional prompt for DeepSeek Harness WebUI |
| 1080 | [gausszhou/dsh-opencode-session-id](https://github.com/gausszhou/dsh-opencode-session-id) | 0 | 2026-08-22 | 2026-08-24 | dsh session IDs for opencode, zero config. |
| 1081 | [gausszhou/dsh-where-am-i](https://github.com/gausszhou/dsh-where-am-i) | 0 | 2026-08-20 | 2026-08-24 | Neofetch for DeepSeek Harness. |
| 1082 | [gavenma/dsh-autoresearch-preset](https://github.com/gavenma/dsh-autoresearch-preset) | 0 | 2026-08-25 | 2026-08-25 | AutoResearch Project Mode preset for DeepSeek Harness. |
| 1083 | [Gcd1949/dsh-tools](https://github.com/Gcd1949/dsh-tools) | 0 | 2026-08-21 | 2026-08-22 | DeepSeek Harness (dsh) utilities: session-manager plugin & Windows control panel |
| 1084 | [geekyfoxlab/dsh-subagents](https://github.com/geekyfoxlab/dsh-subagents) | 0 | 2026-08-26 | 2026-08-26 | Focused child-agent delegation (scout, researcher, worker, reviewer, oracle, delegate) and multi-agent workflows (council, parallel review, review loop) for DeepSeek Harness. |
| 1085 | [GitNoHup/macaron-theme](https://github.com/GitNoHup/macaron-theme) | 0 | 2026-08-26 | 2026-08-26 | 🍬 马卡龙毛玻璃主题（Macaron Glassmorphism Theme）— DeepSeek Harness 动态主题插件：四套马卡龙配色、145° 双色渐变、毛玻璃卡片；日间上色 / 夜间自动清除并记忆恢复。 |
| 1086 | [goldgish/dsh-agent-trace](https://github.com/goldgish/dsh-agent-trace) | 0 | 2026-08-26 | 2026-08-26 | Agent Trace — visualize an agent's reasoning, parallel tool calls, and results as an interactive DAG inside DeepSeek Harness. |
| 1087 | [GooDAnDReaDY/dsh-grok-xsearch](https://github.com/GooDAnDReaDY/dsh-grok-xsearch) | 0 | 2026-08-21 | 2026-08-22 | x_search tool for DeepSeek Harness via separate SuperGrok OAuth (X/Twitter search) |
| 1088 | [GooDAnDReaDY/dsh-image-gen](https://github.com/GooDAnDReaDY/dsh-image-gen) | 0 | 2026-08-18 | 2026-08-23 | Image generation for DeepSeek Harness: a generate_image tool backed by the FAL queue API, with the picture shown inline in the conversation |
| 1089 | [GooDAnDReaDY/dsh-lanmode](https://github.com/GooDAnDReaDY/dsh-lanmode) | 0 | 2026-08-20 | 2026-08-25 | Settings over the LAN for DeepSeek Harness |
| 1090 | [GooDAnDReaDY/dsh-messenger-gateway](https://github.com/GooDAnDReaDY/dsh-messenger-gateway) | 0 | 2026-08-26 | 2026-08-26 | Telegram messenger bridge for DeepSeek Harness (sessions, steer, homes, TTS voice notes) |
| 1091 | [GooDAnDReaDY/dsh-model-sync](https://github.com/GooDAnDReaDY/dsh-model-sync) | 0 | 2026-08-23 | 2026-08-25 | Automatic model catalog synchronization for API-key DeepSeek Harness providers: refreshes the model list from the provider instead of hand-editing it |
| 1092 | [GooDAnDReaDY/dsh-subscriptions](https://github.com/GooDAnDReaDY/dsh-subscriptions) | 0 | 2026-08-21 | 2026-08-25 | OAuth subscription LLM providers for DeepSeek Harness (Codex, Claude, Grok, Antigravity) |
| 1093 | [GooDAnDReaDY/dsh-usage-guard](https://github.com/GooDAnDReaDY/dsh-usage-guard) | 0 | 2026-08-24 | 2026-08-25 | Keeps a malformed token-usage sample from taking a whole session history down with it: a missing counter is recovered or zeroed before the harness folds it, so replay never yields NaN. |
| 1094 | [GroupWork888/dsh-plugin-archived-sessions](https://github.com/GroupWork888/dsh-plugin-archived-sessions) | 0 | 2026-08-25 | 2026-08-26 | Browse and read archived DeepSeek Harness sessions from a sidebar panel. A read-only viewer: it does not restore sessions to the sidebar. |
| 1095 | [guo6x/dsh-shipcheck](https://github.com/guo6x/dsh-shipcheck) | 0 | 2026-08-25 | 2026-08-26 | Evidence-first frontend release checks for DeepSeek Harness: real browser inspection, visual baselines, and reproducible reports. |
| 1096 | [GuoFengyu110429/dsh-high-fee-alert](https://github.com/GuoFengyu110429/dsh-high-fee-alert) | 0 | 2026-08-24 | 2026-08-25 | 一个由DSH制作的插件，用于在峰谷中的峰时段进行提醒以节省费用。 |
| 1097 | [hanzhangzzz/dsh-computer-use](https://github.com/hanzhangzzz/dsh-computer-use) | 0 | 2026-08-25 | 2026-08-26 | Computer use plugin for DeepSeek Harness: structure-first browser driving over a Playwright provider |
| 1098 | [haoyu-qi/dsh-zentao](https://github.com/haoyu-qi/dsh-zentao) | 0 | 2026-08-15 | 2026-08-26 | 面向 DeepSeek Harness 的 AVCON Web 界面定制与个人禅道 CLI 工作中心 |
| 1099 | [harness-home/harness-ai-app](https://github.com/harness-home/harness-ai-app) | 0 | 2026-08-21 | 2026-08-26 | Mobile client for Harness AI — follow, answer and approve your hosted agent sessions from your phone. Expo + React Native, talks only to your own server. |
| 1100 | [harness-home/harness-ai-desktop](https://github.com/harness-home/harness-ai-desktop) | 0 | 2026-08-21 | 2026-08-26 | Desktop client for Harness AI — an Electron app that boots the DeepSeek Harness (dsh) agent runtime in-process on loopback, with hosted sessions, remote approvals and a gated plugin market. |
| 1101 | [harness-home/harness-ai-plugins](https://github.com/harness-home/harness-ai-plugins) | 0 | 2026-08-26 | 2026-08-26 | Community plugin catalog for Harness AI: a scanner over the public npm registry, and the snapshot it publishes. |
| 1102 | [hecailiaoPFS/firecrawl-research-engine](https://github.com/hecailiaoPFS/firecrawl-research-engine) | 0 | 2026-08-24 | 2026-08-24 | Deep technical research & verification skill for LLM agents: Firecrawl search-first, graceful degradation, anti-hallucination citations. Works with DSH / Claude Code / Codex / Cursor. |
| 1103 | [heiheiha798/dsh-plugin-response-window](https://github.com/heiheiha798/dsh-plugin-response-window) | 0 | 2026-08-24 | 2026-08-24 | DeepSeek Harness (DSH) web plugin: wrap each prompt-to-prompt turn's response (tool calls + assistant text) in a bounded-height scrollable window/slide, Grok-build style. |
| 1104 | [helibeiqi/dsh-intent-network](https://github.com/helibeiqi/dsh-intent-network) | 0 | 2026-08-23 | 2026-08-23 | 将用户意图解析为可编辑、可观测、可学习的多跳工具调用图，消费 CDP 语义与 adapter 桥接工具 |
| 1105 | [hellofuture2068/dsh-simple-view](https://github.com/hellofuture2068/dsh-simple-view) | 0 | 2026-08-26 | 2026-08-26 | Declutter DeepSeek Harness chat: hide agent execution-log rows, tighten spacing & fonts, bubble messages, and set a "reply concisely" system-prompt instruction. |
| 1106 | [HellowVirgil/dsh-antv-ava](https://github.com/HellowVirgil/dsh-antv-ava) | 0 | 2026-08-25 | 2026-08-25 | AntV AVA plugin for DeepSeek Harness with streaming narrative text and charts |
| 1107 | [HenryHwong/dsh-ui-billing](https://github.com/HenryHwong/dsh-ui-billing) | 0 | 2026-08-25 | 2026-08-25 | Billing widget plugin for the DeepSeek Harness Web GUI: current-session cost and API balance at the sidebar foot (dsh-plugin) |
| 1108 | [HenryHwong/dsh-ui-turn-rail](https://github.com/HenryHwong/dsh-ui-turn-rail) | 0 | 2026-08-25 | 2026-08-25 | Turn progress rail plugin for the DeepSeek Harness Web GUI (dsh-plugin) |
| 1109 | [henrytang2011win-coder/dsh-task-sounds](https://github.com/henrytang2011win-coder/dsh-task-sounds) | 0 | 2026-08-25 | 2026-08-25 | 为你的DeepSeek harness添加任务结束和提问时的提示音 |
| 1110 | [hi-fangj/dsh-models-radar](https://github.com/hi-fangj/dsh-models-radar) | 0 | 2026-08-26 | 2026-08-26 | Model capability radar plugin for the DeepSeek Harness Web GUI |
| 1111 | [Hjay1101/dsh-ios-control](https://github.com/Hjay1101/dsh-ios-control) | 0 | 2026-08-22 | 2026-08-22 | DeepSeek Harness 插件：手机扫码遥控电脑上的 agent —— 在 dsh-remote-link 基础上增强会话持久化（dsh 重启后已配对设备保持登录）、iOS 主屏图标等 |
| 1112 | [hjdhnx/dsh-desktop](https://github.com/hjdhnx/dsh-desktop) | 0 | 2026-08-22 | 2026-08-23 | DeepSeek Harness 桌面端 -- 从 Electron 迁移到 Tauri(Rust 壳 + Node Sidecar)架构 |
| 1113 | [hnlisf/dsh-crypto-analyst](https://github.com/hnlisf/dsh-crypto-analyst) | 0 | 2026-08-24 | 2026-08-24 | 加密货币深度调研智能体 DSH 插件：5 步思维链研报 + 报告工作台 + 数据可视化 + MD/PDF 导出 |
| 1114 | [Hoemr/dsh-better-overleaf](https://github.com/Hoemr/dsh-better-overleaf) | 0 | 2026-08-24 | 2026-08-24 | Overleaf tab for DSH better-sidebar: direct-CDP login, project mirrors under <workspace>/overleaf/, git/API sync, sidebar file preview |
| 1115 | [Hoemr/dsh-quicklook](https://github.com/Hoemr/dsh-quicklook) | 0 | 2026-08-24 | 2026-08-24 | QuickLook-style space-key large preview for DSH better-sidebar: press Space on the active file tab for an instant image/PDF/text overlay |
| 1116 | [honlnk/dsh-input-assist](https://github.com/honlnk/dsh-input-assist) | 0 | 2026-08-23 | 2026-08-25 | Input assistant for DeepSeek Harness Web UI: inline AI completion (FIM) and Chinese-friendly typo checking |
| 1117 | [horizon105457/tsstream](https://github.com/horizon105457/tsstream) | 0 | 2026-08-26 | 2026-08-26 | 🌊 Agent-native time-series streaming for DeepSeek Harness (DSH plugin) — terminal/serial byte streams → indexed, queryable, event-driven timeline. 19 tools · 9 operators · 🧪 experimental |
| 1118 | [htfc786/dsh-awake](https://github.com/htfc786/dsh-awake) | 0 | 2026-08-16 | 2026-08-23 | dsh-awake · 守夜人：在 agent 任务执行期间阻止操作系统休眠 |
| 1119 | [huangfuren/dsh-outline-auto](https://github.com/huangfuren/dsh-outline-auto) | 0 | 2026-08-25 | 2026-08-26 | DSH (DeepSeek Harness) web plugin: search and read company Outline knowledge base documents from conversations (outline_search / outline_get_document). |
| 1120 | [Huauauaa/dsh-chatbi](https://github.com/Huauauaa/dsh-chatbi) | 0 | 2026-08-24 | 2026-08-24 | a chatbi dsh |
| 1121 | [huermi/dsh-JEPA-adapter](https://github.com/huermi/dsh-JEPA-adapter) | 0 | 2026-08-24 | 2026-08-25 | 适配调用JEPA模型的插件，提供一个本地的JEPA模型项目（需要进一步训练持续学习，已完成基本工具调用），可在家用计算机配置上运行。A plugin adapted to call the JEPA model, providing a local JEPA model project (requires further training for continual learning; basic tool calling has been completed) that can run on a home computer CPU. |
| 1122 | [HULILI-com/dsh-namecheck](https://github.com/HULILI-com/dsh-namecheck) | 0 | 2026-08-26 | 2026-08-26 | dsh plugin for checking domain availability and trademark screening of candidate product names |
| 1123 | [hxt9805/dsh-remote-tailscale](https://github.com/hxt9805/dsh-remote-tailscale) | 0 | 2026-08-22 | 2026-08-22 | DSH plugin: open the local DSH web UI on your other Tailscale devices |
| 1124 | [hyperion2144/dsh-desktop-tauriapp](https://github.com/hyperion2144/dsh-desktop-tauriapp) | 0 | 2026-08-18 | 2026-08-23 | Tauri 2 desktop shell wrapping the DeepSeek Harness Web GUI (macOS + Windows) — tray daemon, auto-launch/reuse of local dsh, --patch plugin injection, mobile access via LAN/tunnel pairing with cloudflared one-click tunnel. |
| 1125 | [hyperion2144/dsh-hashline-edittool](https://github.com/hyperion2144/dsh-hashline-edittool) | 0 | 2026-08-20 | 2026-08-22 | Hash-anchored read/edit/undo_last_edit tools for DeepSeek Harness (dsh) |
| 1126 | [hzpeng57/dsh-lens-rail](https://github.com/hzpeng57/dsh-lens-rail) | 0 | 2026-08-25 | 2026-08-25 | Codex-style left message navigation rail for DeepSeek Harness |
| 1127 | [hzthzt/dsh-summary-panel](https://github.com/hzthzt/dsh-summary-panel) | 0 | 2026-08-23 | 2026-08-23 | Extensible Codex-style pinned summary panel for DeepSeek Harness Web. |
| 1128 | [icearia0219/dsh-memory-spaces](https://github.com/icearia0219/dsh-memory-spaces) | 0 | 2026-08-25 | 2026-08-25 | User-governed local memory spaces for DeepSeek Harness — explicitly share selected sessions with previewable, versioned, provenance-aware recall. |
| 1129 | [ichabodcole/dsh-plugin-monitor](https://github.com/ichabodcole/dsh-plugin-monitor) | 0 | 2026-08-25 | 2026-08-26 | A Deepseek harness monitor plugin.  |
| 1130 | [icyaaaww/dsh-tool-failure-circuit-breaker](https://github.com/icyaaaww/dsh-tool-failure-circuit-breaker) | 0 | 2026-08-24 | 2026-08-24 | DeepSeek Harness plugin that blocks repeated identical failed tool calls |
| 1131 | [icyaaaww/dsh-tui-secret-guard](https://github.com/icyaaaww/dsh-tui-secret-guard) | 0 | 2026-08-26 | 2026-08-26 | Blocks high-confidence secrets before dsh-TUI sends them to a model, compliant with dsh ecosystem manifest v0.15. |
| 1132 | [imaginevoldermert/dsh-minimal-launcher-plugin](https://github.com/imaginevoldermert/dsh-minimal-launcher-plugin) | 0 | 2026-08-23 | 2026-08-23 | A minimal Windows launcher plugin for DeepSeek Harness |
| 1133 | [imkingjh999/dsh-adaptive-effort](https://github.com/imkingjh999/dsh-adaptive-effort) | 0 | 2026-08-26 | 2026-08-26 | DSH plugin: auto reasoning_effort (low/high/max) per turn via MiniMax complexity scorer + token ledger + per-reply metadata label |
| 1134 | [imlishiyuan/dsh-keep-running](https://github.com/imlishiyuan/dsh-keep-running) | 0 | 2026-08-24 | 2026-08-24 | A watchdog plugin for DeepSeek Harness: on a **quota / rate-limit (HTTP 429)** error, it automatically creates a fixed-interval scheduled task that keeps delivering a "continue the task" prompt until it succeeds or you take over. DeepSeek Harness 的 watchdog 插件：遇到 **配额/限流（HTTP 429）** 时，自动创建一个固定间隔的定时任务，到点持续投递「继续任务」的提示，直到任务成功或你手动接手。 |
| 1135 | [inoricon1/dsh-frontier-math](https://github.com/inoricon1/dsh-frontier-math) | 0 | 2026-08-25 | 2026-08-25 | Evidence-gated frontier mathematics research workflow for DeepSeek Harness |
| 1136 | [isirin1131/dsh-easy-galgame](https://github.com/isirin1131/dsh-easy-galgame) | 0 | 2026-08-23 | 2026-08-23 | Easy Galgame 模式：一个文件 = 角色卡 + 世界书 + 剧本 + 规则 + 状态的 all-in-one 提示词。DSH 插件提供 galgame_read / galgame_write / galgame_ask 与 Galgame 模式系统提示词。 |
| 1137 | [ivvan3016/dsh-ui-pricing](https://github.com/ivvan3016/dsh-ui-pricing) | 0 | 2026-08-24 | 2026-08-25 | user-configurable cost pricing for dsh |
| 1138 | [ivvan3016/dsh-ui-task-notify](https://github.com/ivvan3016/dsh-ui-task-notify) | 0 | 2026-08-23 | 2026-08-24 | endows dsh with the ability to notify after the task is completed |
| 1139 | [Jackywxsz/DSH-Creator](https://github.com/Jackywxsz/DSH-Creator) | 0 | 2026-08-25 | 2026-08-26 | Jacky Creator：面向内容创作者的 DeepSeek Harness 本地内容与运营工作台 |
| 1140 | [jadehare/dsh-model-controller](https://github.com/jadehare/dsh-model-controller) | 0 | 2026-08-21 | 2026-08-24 | 为 DeepSeek Harness 提供基于关键词和语义分类的动态模型路由插件，可按任务自动选择模型与推理强度。 |
| 1141 | [JanEickholt/dsh-inline-diff](https://github.com/JanEickholt/dsh-inline-diff) | 0 | 2026-08-25 | 2026-08-26 | See every file edit inline in the DeepSeek Harness chat — always-open side-by-side diffs for edit/write tool calls |
| 1142 | [jedzqer/dsh-retry-plugin](https://github.com/jedzqer/dsh-retry-plugin) | 0 | 2026-08-21 | 2026-08-22 | 一款用于DeepSeek Harness（DSH）的插件，可以在AI API请求错误时自动发送继续的消息以重试。A plugin for DeepSeek Harness (DSH) that automatically sends continuation messages to retry when AI API requests fail. |
| 1143 | [Jensen-Yao/dsh-model-palette](https://github.com/Jensen-Yao/dsh-model-palette) | 0 | 2026-08-26 | 2026-08-26 | Global provider-aware model command palette and optional OpenRouter media tools for DeepSeek Harness. |
| 1144 | [jer67107-cyber/dsh-skin-chengzi](https://github.com/jer67107-cyber/dsh-skin-chengzi) | 0 | 2026-08-24 | 2026-08-25 | 橙子 · 深海蓝调 — DSH Web 皮肤中心深海蓝护眼皮肤（Deep sea blue skin for DSH web skin-center） |
| 1145 | [jerryqx/dsh-xiaoyuzhou](https://github.com/jerryqx/dsh-xiaoyuzhou) | 0 | 2026-08-26 | 2026-08-26 | DSH (DeepSeek Harness) 小宇宙播客插件：免登录播放/扫码登录/订阅同步/搜索，Web 播放条与面板 + podcast_play 工具 |
| 1146 | [jerryqx/dsh-ximalaya](https://github.com/jerryqx/dsh-ximalaya) | 0 | 2026-08-25 | 2026-08-25 | DeepSeek Harness 喜马拉雅播客插件：搜索/播放/收藏 + ximalaya_play 模型工具 |
| 1147 | [jiang12345-code/dsh-multi-role-debate](https://github.com/jiang12345-code/dsh-multi-role-debate) | 0 | 2026-08-26 | 2026-08-26 | 多角色并行论证 DSH 插件：codex/claude 实体 + DSH Judge 汇总 + 结果回对话 + 直接对话（聚合包 dsh-multi-role-debate） |
| 1148 | [jiaoTaiLang404/dsh-model-ocean-selector](https://github.com/jiaoTaiLang404/dsh-model-ocean-selector) | 0 | 2026-08-24 | 2026-08-24 | A DeepSeek Harness plugin with a vertical model list and an animated Three.js particle reasoning-effort control |
| 1149 | [JiayiXie-jpg/dsh-desktop-pet](https://github.com/JiayiXie-jpg/dsh-desktop-pet) | 0 | 2026-08-26 | 2026-08-26 | 一只住在 DSH 网页里的养成系桌宠：随编码活动升级进化、语音打气，还能用 AI 生成专属的透明动画形象。 |
| 1150 | [Jiazliang/dsh-worktree](https://github.com/Jiazliang/dsh-worktree) | 0 | 2026-08-22 | 2026-08-22 | Fork-like git worktree for DeepSeek Harness (DSH): create an isolated git worktree from a workspace/session and open a new session in it — optionally forking the conversation so the child inherits all history and works on its own branch. |
| 1151 | [jieguanya/tugu-dsh-balance-widget](https://github.com/jieguanya/tugu-dsh-balance-widget) | 0 | 2026-08-22 | 2026-08-22 | DeepSeek Harness (DSH) 余额插件：实时余额/今日消耗/7-30天趋势图 |
| 1152 | [jiesou/dsh-nous-portal-free-provider](https://github.com/jiesou/dsh-nous-portal-free-provider) | 0 | 2026-08-24 | 2026-08-24 | Nous Portal free-tier provider for dsh |
| 1153 | [JinRyu-online/dsh-svn-plugin](https://github.com/JinRyu-online/dsh-svn-plugin) | 0 | 2026-08-24 | 2026-08-24 | 面向 DeepSeek Harness Web GUI 的 SVN（Subversion）版本控制面板插件。以独立 tab 融入 dsh-better-sidebar 右侧边栏 |
| 1154 | [Jinsight-gif/dsh-plugin-gitbash](https://github.com/Jinsight-gif/dsh-plugin-gitbash) | 0 | 2026-08-23 | 2026-08-23 | DeepSeek Harness 插件：在 DSH 会话里运行 Windows 侧 Git for Windows Bash（WSL 自动探测路径）。Run commands on the Windows host's Git for Windows Bash from DeepSeek Harness — WSL-aware, auto-detects git-bash. |
| 1155 | [jo32/dsh-hackernews-reader](https://github.com/jo32/dsh-hackernews-reader) | 0 | 2026-08-23 | 2026-08-24 | A dsh-plugin Hacker News reader with app-scoped AI conversations for DeepDeck. |
| 1156 | [jo32/dsh-nga-reader](https://github.com/jo32/dsh-nga-reader) | 0 | 2026-08-23 | 2026-08-24 | A dsh-plugin NGA reader with app-scoped AI conversations for DeepDeck. |
| 1157 | [jo32/dsh-video-sherlock](https://github.com/jo32/dsh-video-sherlock) | 0 | 2026-08-26 | 2026-08-26 | A local-first, evidence-backed video investigation app for DeepDeck. |
| 1158 | [joao-paulo-santos/dsh-approval-diff](https://github.com/joao-paulo-santos/dsh-approval-diff) | 0 | 2026-08-25 | 2026-08-26 | DSH plugin: replace file-change approval prompts with a real diff review (line diffs, word highlights, disk-sourced context, one file per card) |
| 1159 | [joao-paulo-santos/dsh-approval-first](https://github.com/joao-paulo-santos/dsh-approval-first) | 0 | 2026-08-25 | 2026-08-26 | Approval-first edit/write for DeepSeek Harness: shadow tools ask the user BEFORE a mutation the standing sandbox policy would deny, so the model never has to repeat a tool call with sandbox_permissions. In-policy writes stay silent, out-of-policy targets get an approval card on the first call. |
| 1160 | [JoaquinDG/dsh-governor](https://github.com/JoaquinDG/dsh-governor) | 0 | 2026-08-23 | 2026-08-24 | Behavioural supervision for DeepSeek Harness agents: retry storms, reasoning-budget burn, and a backstop that survives host suspend. |
| 1161 | [JohnXu22786/subtitle-studio](https://github.com/JohnXu22786/subtitle-studio) | 0 | 2026-08-23 | 2026-08-23 | Multi-language subtitle translation workflow for dsh: SRT/VTT parsing, sentence-level LLM translation, bilingual merge, alignment validation |
| 1162 | [JollY-Life/jolly-dsh-vision](https://github.com/JollY-Life/jolly-dsh-vision) | 0 | 2026-08-21 | 2026-08-22 | ModLens 风格的 DeepSeek Harness 视觉桥接插件：deepseek-v4-pro 当大脑、deepseek-v4-flash-vision-exp 当眼睛，提供 vision 工具与 (ds vision) 视觉孪生模型，让纯文本模型也能看图、直接贴图。 |
| 1163 | [jsoncode/dsh-get-balance](https://github.com/jsoncode/dsh-get-balance) | 0 | 2026-08-23 | 2026-08-24 | 余额与费用查询插件，支持多账号查询，实时token实时统计，中英双语，界面交互直观、开箱即用 |
| 1164 | [JularDepick/dsh-system-monitor-plugin](https://github.com/JularDepick/dsh-system-monitor-plugin) | 0 | 2026-08-23 | 2026-08-24 | A plugin for dsh: monitor the resource utilization of dsh system processes and report the results to the user in the form of charts. |
| 1165 | [junarch/voice_for_dsh](https://github.com/junarch/voice_for_dsh) | 0 | 2026-08-22 | 2026-08-23 | DSH Web 语音朗读插件：每轮输出口语化转写后朗读（代码/表格自动跳过）；免费浏览器 TTS + 可选豆包云 TTS。Read-aloud plugin for DeepSeek Harness web. |
| 1166 | [jyao-SUSE-power-group/dsh-provider-rate-limit](https://github.com/jyao-SUSE-power-group/dsh-provider-rate-limit) | 0 | 2026-08-23 | 2026-08-23 | dsh-provider-rate-limit |
| 1167 | [jypjypjypjyp/dsh-agent-teams](https://github.com/jypjypjypjyp/dsh-agent-teams) | 0 | 2026-08-19 | 2026-08-25 | AgentTeams plugin for DeepSeek Harness |
| 1168 | [kaixinguo360/dsh-bsk-ws-bridge](https://github.com/kaixinguo360/dsh-bsk-ws-bridge) | 0 | 2026-08-26 | 2026-08-26 | DeepSeek Harness BrowserSkill 桥接插件：把本机 bsk daemon 的 WebSocket 经浏览器信道暴露给远程 BrowserSkill 扩展。配套的修改版 BrowserSkill 扩展：https://github.com/kaixinguo360/BrowserSkill-DSH-Remote |
| 1169 | [KamChiHei/dsh-deepseek-usage-monitor](https://github.com/KamChiHei/dsh-deepseek-usage-monitor) | 0 | 2026-08-21 | 2026-08-22 | DeepSeek Harness (dsh) plugin: token usage accounting and account balance with a live status card in DSH Web |
| 1170 | [kane-le/dsh-deepseek-usage](https://github.com/kane-le/dsh-deepseek-usage) | 0 | 2026-08-25 | 2026-08-25 | DeepSeek API 用量与余额查看插件（DSH Plugin）· /usage 命令实时查询余额并汇总本机 token 用量 |
| 1171 | [keke-shy/dsh-desktop](https://github.com/keke-shy/dsh-desktop) | 0 | 2026-08-16 | 2026-08-22 | Minimal Electron desktop shell embedding the official DeepSeek Harness web profile |
| 1172 | [KeS1Ke/dsh-exit](https://github.com/KeS1Ke/dsh-exit) | 0 | 2026-08-24 | 2026-08-25 | A focused DeepSeek Harness web plugin that adds a safe, confirmed host-exit control. |
| 1173 | [Kevoyuan/dsh-trading212](https://github.com/Kevoyuan/dsh-trading212) | 0 | 2026-08-24 | 2026-08-25 | Read-only Trading 212 portfolio dashboard and dsh tools for holdings, history, risk, and trade markers. |
| 1174 | [KeyboardPrince/dsh-skill-manager](https://github.com/KeyboardPrince/dsh-skill-manager) | 0 | 2026-08-22 | 2026-08-22 | DSH 设置界面中的技能管理器插件：可视化管理全局/项目级 Skill（导入、编辑、删除、启用/禁用 SKILL.md 目录） |
| 1175 | [Kickstartparty3459/dsh-ios](https://github.com/Kickstartparty3459/dsh-ios) | 0 | 2026-08-22 | 2026-08-23 | Run live iOS simulators and your real iPhone over USB inside DeepSeek Harness conversations with 22 agent tools, MJPEG previews, and SwiftUI hot reload. |
| 1176 | [kikomaotu/ccs-balance](https://github.com/kikomaotu/ccs-balance) | 0 | 2026-08-22 | 2026-08-26 | DSH 插件：同步 cc-switch 各 provider 余额，按日/月/总量统计 token 用量与花费（支持中转站币种与汇率设置） |
| 1177 | [kittimzhe/dsh-session-recall](https://github.com/kittimzhe/dsh-session-recall) | 0 | 2026-08-25 | 2026-08-26 | Cross-session full-text recall for DeepSeek Harness: the model-facing recall tool searches past session transcripts via ctx.sessionQuery, with a persistent FTS index |
| 1178 | [kkaktus463/dsh-plugin-desktop](https://github.com/kkaktus463/dsh-plugin-desktop) | 0 | 2026-08-23 | 2026-08-23 | Opens the DeepSeek Harness Web UI in a native window instead of a browser tab. |
| 1179 | [Kompetenzteam/dsh-locale-de](https://github.com/Kompetenzteam/dsh-locale-de) | 0 | 2026-08-23 | 2026-08-23 | German UI translation plugin for DeepSeek Harness (locale de): registers all locale namespaces in German. Deutsche UI-Uebersetzung fuer den DeepSeek Harness. |
| 1180 | [kongdexu/dsh-win-notify](https://github.com/kongdexu/dsh-win-notify) | 0 | 2026-08-25 | 2026-08-25 | Real Windows OS toasts for DeepSeek Harness: task-finished / needs-input / needs-approval alerts in Notification Center. Windows-only, zero runtime dependencies. |
| 1181 | [kovey/dsh-nvim-tui](https://github.com/kovey/dsh-nvim-tui) | 0 | 2026-08-21 | 2026-08-25 | dsh's tui base on nvim |
| 1182 | [krystal-cao/deepseek-harness-swift](https://github.com/krystal-cao/deepseek-harness-swift) | 0 | 2026-08-25 | 2026-08-25 | 基于 AppKit、SwiftUI 与 WKWebView 的 DSH 原生 macOS 桌面壳，提供设置中心、DSH 版本管理、插件管理、通知和 Sparkle 应用更新。 |
| 1183 | [kuanfu0430/dsh-sidebar-branch-chat](https://github.com/kuanfu0430/dsh-sidebar-branch-chat) | 0 | 2026-08-24 | 2026-08-24 | Adds a Branch Chat tab to dsh-better-sidebar: independent archived sessions with a context digest and the same tools as the main agent. |
| 1184 | [L3n3L/dsh-disk-cleaner](https://github.com/L3n3L/dsh-disk-cleaner) | 0 | 2026-08-22 | 2026-08-22 | Windows disk space analysis and safe cleanup plugin for DeepSeek Harness |
| 1185 | [Lanzgale/dsh-repo-browser](https://github.com/Lanzgale/dsh-repo-browser) | 0 | 2026-08-25 | 2026-08-26 | Repository Browser plugin for DeepSeek Harness — right-side GitHub repo list with local grouping and quick actions (move / private / archive) |
| 1186 | [LaoQianwocao/dsh-client-ui-board](https://github.com/LaoQianwocao/dsh-client-ui-board) | 0 | 2026-08-22 | 2026-08-23 | DSH Web 展板插件：会话视图第三标签，多层白板 + 锚点连线 |
| 1187 | [LaoQianwocao/dsh-sound-player](https://github.com/LaoQianwocao/dsh-sound-player) | 0 | 2026-08-22 | 2026-08-23 | DSH Web 音效播放器插件（悬浮窗 + 情况触发音效 + 供其他插件使用的 API） |
| 1188 | [lasdrder0705/dsh-chat-zone-std](https://github.com/lasdrder0705/dsh-chat-zone-std) | 0 | 2026-08-26 | 2026-08-26 | dsh-std Community v0.15 chat zone: ~/dsh_CHAT/<date>/chatN as Tools and Commands. Install adapter-dsh first. |
| 1189 | [lasdrder0705/dsh-pro-vision-std](https://github.com/lasdrder0705/dsh-pro-vision-std) | 0 | 2026-08-26 | 2026-08-26 | dsh-std Community v0.15 ModelProvider: V4-Pro with Flash-Vision captions. Install adapter-dsh first. |
| 1190 | [law-star-cn/lawstar-dsh-mcp](https://github.com/law-star-cn/lawstar-dsh-mcp) | 0 | 2026-08-24 | 2026-08-24 | DeepSeek Harness plugin for LawStar MCP (legal-data): one-click API Key connect |
| 1191 | [lcsdg/dsh-quick-prompts](https://github.com/lcsdg/dsh-quick-prompts) | 0 | 2026-08-25 | 2026-08-25 | Quick-prompts bar for DeepSeek Harness (dsh): per-category snippet chips above the composer, orange placeholder highlighting, two-column prompt/category management, and per-session category memory. |
| 1192 | [lemoncat7/dsh-remote-settings-compat](https://github.com/lemoncat7/dsh-remote-settings-compat) | 0 | 2026-08-22 | 2026-08-25 | Remote settings compatibility plugin for DeepSeek Harness |
| 1193 | [lemoncat7/dsh-ssh](https://github.com/lemoncat7/dsh-ssh) | 0 | 2026-08-23 | 2026-08-25 | SSH sessions, SFTP, terminals, proxies and port forwarding for DeepSeek Harness |
| 1194 | [lemoncat7/dsh-web-search](https://github.com/lemoncat7/dsh-web-search) | 0 | 2026-08-25 | 2026-08-25 | Configurable and secure multi-provider web search for DeepSeek Harness |
| 1195 | [LeoChen98/dsh-worktable-notebook-to-ppt](https://github.com/LeoChen98/dsh-worktable-notebook-to-ppt) | 0 | 2026-08-26 | 2026-08-26 | 基于 dsh-worktable 工作台搭建的「课本到 PPT」自动化工作流插件——在 DeepSeek Harness 中一键将 Jupyter Notebook 转化为专业可编辑的演示文稿（.pptx），让知识沉淀与分享更高效。 |
| 1196 | [leonardoxr/dsh-codex-usage](https://github.com/leonardoxr/dsh-codex-usage) | 0 | 2026-08-22 | 2026-08-24 | OpenAI Codex plan usage indicator for DeepSeek Harness |
| 1197 | [leonardoxr/dsh-coding-tools](https://github.com/leonardoxr/dsh-coding-tools) | 0 | 2026-08-23 | 2026-08-24 | Secure bounded coding tools for DeepSeek Harness |
| 1198 | [leonardoxr/dsh-image-preview](https://github.com/leonardoxr/dsh-image-preview) | 0 | 2026-08-23 | 2026-08-24 | Inline read_image previews for DeepSeek Harness |
| 1199 | [leonardoxr/dsh-status-bar-config](https://github.com/leonardoxr/dsh-status-bar-config) | 0 | 2026-08-23 | 2026-08-24 | Configurable conversation statistics row for DeepSeek Harness |
| 1200 | [leonardoxr/dsh-workspace-git](https://github.com/leonardoxr/dsh-workspace-git) | 0 | 2026-08-22 | 2026-08-24 | DeepSeek Harness plugin for cloning Git repositories as workspaces |
| 1201 | [LeonSone/dsh-trash](https://github.com/LeonSone/dsh-trash) | 0 | 2026-08-22 | 2026-08-22 | A DeepSeek Harness (DSH) plugin: every delete operation goes through a recoverable trash store — accidental deletes are one restore away. |
| 1202 | [lhh666-6/dsh-copy-fix](https://github.com/lhh666-6/dsh-copy-fix) | 0 | 2026-08-23 | 2026-08-24 | Fix DSH Desktop copy buttons by bridging clipboard writes to the Electron main process. |
| 1203 | [lhh666-6/dsh-paste-file](https://github.com/lhh666-6/dsh-paste-file) | 0 | 2026-08-23 | 2026-08-24 | Paste/drop files into the DSH composer, save them under the current workspace, and insert relative paths. |
| 1204 | [lhh666-6/dsh-update-check](https://github.com/lhh666-6/dsh-update-check) | 0 | 2026-08-23 | 2026-08-24 | DSH update checker for the DSH Desktop installer channel and GitHub source releases, with one-click download/update. |
| 1205 | [lhh666-6/dsh-usage-cost](https://github.com/lhh666-6/dsh-usage-cost) | 0 | 2026-08-23 | 2026-08-24 | Real-time DeepSeek token usage and cost meter for DSH: status-bar capsule plus detail panel, local-only persistence. |
| 1206 | [lianginx/dsh-quote-selection](https://github.com/lianginx/dsh-quote-selection) | 0 | 2026-08-22 | 2026-08-22 | ❝ Quote selected chat text into the composer as a Markdown blockquote · DeepSeek Harness Web UI 插件：选中会话文字，一键引用 |
| 1207 | [lianginx/dsh-timeline-enhance](https://github.com/lianginx/dsh-timeline-enhance) | 0 | 2026-08-25 | 2026-08-25 | DSH Web UI plugin: auto-fold chat timeline processes + Deep diving fun tips |
| 1208 | [liangzhipengdamon-maker/GovernLoop-DSH](https://github.com/liangzhipengdamon-maker/GovernLoop-DSH) | 0 | 2026-08-23 | 2026-08-25 | GovernLoop-DSH automatically connects DeepSeek Harness agents to independent ChatGPT review with checkpoints and evidence. |
| 1209 | [liceses/dsh-hmm-wait](https://github.com/liceses/dsh-hmm-wait) | 0 | 2026-08-22 | 2026-08-26 | 化口水为乐趣，把大肥鱼流的口水变成游戏连击！ |
| 1210 | [lihaoran0412/dsh-narrative-engine](https://github.com/lihaoran0412/dsh-narrative-engine) | 0 | 2026-08-25 | 2026-08-25 | DeepSeek Harness 沉浸叙事双向创作引擎：导入小说为可游玩世界，游玩后反向写成同人小说。仅处理虚构成年人(18+/adult)。 |
| 1211 | [lilightspeed/dsh-seekbuddy](https://github.com/lilightspeed/dsh-seekbuddy) | 0 | 2026-08-23 | 2026-08-23 | Desktop pet peer client for DeepSeek Harness (DSH): /api + WebSocket client, MCP server, desktop shell (Electron). |
| 1212 | [lim12137/dsh-llm-extra-retry](https://github.com/lim12137/dsh-llm-extra-retry) | 0 | 2026-08-26 | 2026-08-26 | Extra model-request recovery for DeepSeek Harness: retries PI_AI_ERROR failures once after a fixed 20s delay; other error codes keep the built-in dsh-llm-retry exponential backoff. |
| 1213 | [LionGateOS/dsh-local-voice-dictation](https://github.com/LionGateOS/dsh-local-voice-dictation) | 0 | 2026-08-21 | 2026-08-23 | Local voice plugin for DeepSeek Harness: microphone dictation with local STT plus assistant-response Kokoro TTS playback. |
| 1214 | [lionheartjie/DSH_Shell](https://github.com/lionheartjie/DSH_Shell) | 0 | 2026-08-23 | 2026-08-25 | DeepSeek Harness 的 Rust/Tauri 套壳 |
| 1215 | [lispking/dsh-devpanel](https://github.com/lispking/dsh-devpanel) | 0 | 2026-08-24 | 2026-08-24 | A developer toolkit for the DeepSeek Harness (DSH) web console: a real multi-tab PTY terminal plus an AI-output file browser. |
| 1216 | [little3tar/dsh-backup](https://github.com/little3tar/dsh-backup) | 0 | 2026-08-23 | 2026-08-24 | 由于 dsh 的自定义范围太大，很难通过一个插件或者程序来完美备份自己的配置，所以我觉得可以通过 ai 来分析哪些配置需要备份、可以备份，以及在新的环境中如何恢复。有了这个 skills 导出的配置文件，任意 agent 都可以帮助恢复 dsh 的配置。 |
| 1217 | [LittleFishStars/dsh-opencode-tui](https://github.com/LittleFishStars/dsh-opencode-tui) | 0 | 2026-08-16 | 2026-08-22 | 为 DeepSeek Harness 制作的仿 OpenCode 的 TUI 界面插件 |
| 1218 | [liujia-io/dsh-image-picker](https://github.com/liujia-io/dsh-image-picker) | 0 | 2026-08-26 | 2026-08-26 | Paperclip image-picker button for the DeepSeek Harness web composer - pick reference images via the system file dialog and feed them into the official attachment pipeline. |
| 1219 | [liuke-zhu/zhenxin-ai-video-manager](https://github.com/liuke-zhu/zhenxin-ai-video-manager) | 0 | 2026-08-25 | 2026-08-25 | 真的爱你：本地智能视频管家 Skill —— 说一句「真的爱你」，接管从素材分析到成片交付的完整剪辑流程 |
| 1220 | [liukj98/dsh-ui-tools](https://github.com/liukj98/dsh-ui-tools) | 0 | 2026-08-19 | 2026-08-22 | deepseek harness tools 插件 |
| 1221 | [liyongzheng666/dsh-browser-bridge](https://github.com/liyongzheng666/dsh-browser-bridge) | 0 | 2026-08-22 | 2026-08-22 | DSH browser bridge plugin + Firefox extension: browsers read/control via localhost WebSocket |
| 1222 | [lizhi00001/dsh-tools-plugins](https://github.com/lizhi00001/dsh-tools-plugins) | 0 | 2026-08-24 | 2026-08-24 | 将简短或模糊的指令改写为结构化 Prompt |
| 1223 | [lmh-2026/dsh-periscope](https://github.com/lmh-2026/dsh-periscope) | 0 | 2026-08-23 | 2026-08-24 | DSH plugin: keep text-only DeepSeek models (V4-Flash / V4-Pro) and auto-route image-bearing requests to the official vision model (deepseek-v4-flash-vision-exp) - no manual model switching. |
| 1224 | [lnetrit-alt/dsh-system-control](https://github.com/lnetrit-alt/dsh-system-control) | 0 | 2026-08-26 | 2026-08-26 | DSH web plugin: sidebar-embedded DeepSeek balance readout with a black minimalist full-shutdown button. |
| 1225 | [loiasdi/dsh-prompthub-ecosystem](https://github.com/loiasdi/dsh-prompthub-ecosystem) | 0 | 2026-08-26 | 2026-08-26 | PromptHub Ecosystem for DeepSeek Harness (DSH): bilingual Plugin and Skill catalog with GitHub and local tarball installation. |
| 1226 | [Lorodn4x/dsh-firecrawl](https://github.com/Lorodn4x/dsh-firecrawl) | 0 | 2026-08-25 | 2026-08-26 | Firecrawl web search and markdown scrape providers for DeepSeek Harness ctx.web seam |
| 1227 | [Lorodn4x/dsh-voice](https://github.com/Lorodn4x/dsh-voice) | 0 | 2026-08-25 | 2026-08-26 | Voice messages for DeepSeek Harness web UI: Edge TTS playback button plus agent-sent voice notes |
| 1228 | [lovezi0/dsh-model-extension](https://github.com/lovezi0/dsh-model-extension) | 0 | 2026-08-24 | 2026-08-25 | DSH自定义模型提供商时无法设置推理模式与多模态，可通过扩展插件解决 |
| 1229 | [lovezi0/dsh-web-noOpenBrowser](https://github.com/lovezi0/dsh-web-noOpenBrowser) | 0 | 2026-08-20 | 2026-08-23 | deepseek harness服务启动不要打开浏览器 |
| 1230 | [LucienLL/dsh-peak-price-panel](https://github.com/LucienLL/dsh-peak-price-panel) | 0 | 2026-08-23 | 2026-08-24 | DeepSeek Harness plugin: peak/off-peak price watch, live account balance with tiered low-balance alerts, and a top-up button for the main web UI |
| 1231 | [LucienLL/dsh-service-watchdog](https://github.com/LucienLL/dsh-service-watchdog) | 0 | 2026-08-24 | 2026-08-24 | DeepSeek Harness plugin: restart/status of the DSH web service with a detached self-healing watchdog, second-confirmation, and login autostart |
| 1232 | [LucienLL/dsh-session-id](https://github.com/LucienLL/dsh-session-id) | 0 | 2026-08-24 | 2026-08-24 | Show and copy the current session ID in the DeepSeek Harness web UI header |
| 1233 | [LucienLL/dsh-session-memo](https://github.com/LucienLL/dsh-session-memo) | 0 | 2026-08-25 | 2026-08-26 | DSH 对话侧边备忘录插件：GitHub 同步状态 / npm 发布状态 / 项目版本 / 备忘标签，与 dsh-session-status 弱联动 |
| 1234 | [LucienLL/dsh-session-status](https://github.com/LucienLL/dsh-session-status) | 0 | 2026-08-25 | 2026-08-26 | DSH 对话状态标签插件：给每个对话设置项目状态（进行中/已结项/搁置中 + 自定义标签/icon），会话列表与头部可见，跨浏览器持久化 |
| 1235 | [LuckVd/dsh-pin-color](https://github.com/LuckVd/dsh-pin-color) | 0 | 2026-08-22 | 2026-08-23 | DeepSeek Harness (DSH) web 插件：会话置顶（本组/工作区全局）+ 会话 tab 颜色 + emoji，host 持久化，纯 DOM 增强不改 DSH 源码 |
| 1236 | [lunarmoon26/harness-alchemist](https://github.com/lunarmoon26/harness-alchemist) | 0 | 2026-08-23 | 2026-08-24 | One scaffold, five agent harnesses — portable coding-agent plugins for Claude Code, Codex, OpenCode, Antigravity, and DeepSeek Harness. |
| 1237 | [lurejewel/dsh-usage-plugin](https://github.com/lurejewel/dsh-usage-plugin) | 0 | 2026-08-25 | 2026-08-25 | Lightweight, native sidebar usage panel for DeepSeek Harness: official balance + token usage history from session logs. |
| 1238 | [luweiyabo/dsh-whale-pet](https://github.com/luweiyabo/dsh-whale-pet) | 0 | 2026-08-23 | 2026-08-24 | DeepSeek Harness Web UI 的开源鲸鱼桌宠插件，支持 Agent 状态感知、多种透明动画、点击拖拽、屏幕漫游、自定义动作与触发规则。 |
| 1239 | [luxueliu/luxueliu-dsh-md-writing-tools](https://github.com/luxueliu/luxueliu-dsh-md-writing-tools) | 0 | 2026-08-25 | 2026-08-26 | 给 DSH 侧边栏的 Markdown 编辑器补上加粗、斜体、标题、格式刷等写作快捷键 |
| 1240 | [luxueliu/luxueliu-dsh-story](https://github.com/luxueliu/luxueliu-dsh-story) | 0 | 2026-08-26 | 2026-08-26 | DSH fiction writing: Continue-style lore drop, plot handoff, clean transcript, character/world cards |
| 1241 | [lw-storm/dsh-plugin-version-management](https://github.com/lw-storm/dsh-plugin-version-management) | 0 | 2026-08-24 | 2026-08-25 | This plugin provides version management and rollback capabilities. When another plugin causes an error that prevents DSH from launching, forcing you to clear all plugins, this plugin can quickly restore every locally saved plugin configuration. |
| 1242 | [LXFLGH/dsh-deepseek-relay](https://github.com/LXFLGH/dsh-deepseek-relay) | 0 | 2026-08-25 | 2026-08-26 | DeepSeek relay station adapter for deepseek-harness with reasoning-effort control |
| 1243 | [lyuwen/dsh-as-service](https://github.com/lyuwen/dsh-as-service) | 0 | 2026-08-26 | 2026-08-26 | Running DSH as a service on the background |
| 1244 | [lzxcs/archive-vault-pro](https://github.com/lzxcs/archive-vault-pro) | 0 | 2026-08-26 | 2026-08-26 | 归档会话库：查看所有工作区的已归档会话、只读回看内容、右键取消归档（不影响官方逻辑）。 |
| 1245 | [lzxcs/btw-pro](https://github.com/lzxcs/btw-pro) | 0 | 2026-08-26 | 2026-08-26 | /btw 旁路问答：不打断当前会话（含流式输出中），基于当前上下文回答一个问题；答案以「旁答」命令结果行显示在主会话里，不进入主模型上下文。 |
| 1246 | [lzxcs/chat-width-pro](https://github.com/lzxcs/chat-width-pro) | 0 | 2026-08-26 | 2026-08-26 | 对话页面宽度设置：把固定的内容宽度暴露到设置页，默认 748px（应用当前宽度）。 |
| 1247 | [lzxcs/dsh-enter-swap](https://github.com/lzxcs/dsh-enter-swap) | 0 | 2026-08-26 | 2026-08-26 | Swap the web UI composer shortcuts: Ctrl/Meta+Enter inserts a newline, Shift+Enter sends. |
| 1248 | [lzxcs/dsh-tray-notify](https://github.com/lzxcs/dsh-tray-notify) | 0 | 2026-08-26 | 2026-08-26 | DSH → 托盘通知：agent 停顿 / 提问 / 计划审批 / 授权时调用 notify-sender.py 弹窗（--source dsh，托盘按蓝色主题区分于 Claude Code）。纯 node 侧插件。 |
| 1249 | [lzxcs/edit-diff-pro](https://github.com/lzxcs/edit-diff-pro) | 0 | 2026-08-26 | 2026-08-26 | Claude Code 风格的 edit/write diff 卡片：±3 行上下文、绝对行号、可配置默认展开（默认折叠）。 |
| 1250 | [lzxcs/file-diff-pro](https://github.com/lzxcs/file-diff-pro) | 0 | 2026-08-26 | 2026-08-26 | 产物文件点击弹窗查看本轮 diff（代码类文件）；非代码文件维持桌面打开。 |
| 1251 | [lzxcs/lag-trace-pro](https://github.com/lzxcs/lag-trace-pro) | 0 | 2026-08-26 | 2026-08-26 | DSH web UI performance recorder: auto-captures page jank (long animation frames, long tasks, frame freezes) with context snapshots, stored under ~/.dsh/perf/ |
| 1252 | [lzxcs/paste-file-path-pro](https://github.com/lzxcs/paste-file-path-pro) | 0 | 2026-08-26 | 2026-08-26 | Pasting non-image files into the web composer inserts their paths as @file references (host-side clipboard reading). |
| 1253 | [lzyuan549/dsh-plugin-auth](https://github.com/lzyuan549/dsh-plugin-auth) | 0 | 2026-08-22 | 2026-08-22 | Username/password authentication gate for the DeepSeek Harness Web UI |
| 1254 | [MaRi23333/dsh-grok-kit](https://github.com/MaRi23333/dsh-grok-kit) | 0 | 2026-08-24 | 2026-08-25 | DeepSeek Harness 的 Grok 插件：OAuth 登录、主循环融合网页/X 搜索与 Imagine。第三方非官方项目。 |
| 1255 | [mario03690/dsh-devkit](https://github.com/mario03690/dsh-devkit) | 0 | 2026-08-22 | 2026-08-22 | The small deterministic operations an agent needs mid-task. JSON/YAML round-trip, JSON Schema v |
| 1256 | [mario03690/dsh-duizhang](https://github.com/mario03690/dsh-duizhang) | 0 | 2026-08-22 | 2026-08-22 | Reconciliation: statements, invoices and ledgers that have to balance. Bank/credit statement PD |
| 1257 | [mario03690/dsh-kuajing](https://github.com/mario03690/dsh-kuajing) | 0 | 2026-08-22 | 2026-08-22 | Cross-border commerce: HS codes, customs invoices, mainland reachability. HS/HTS code lookup an |
| 1258 | [mario03690/dsh-validate](https://github.com/mario03690/dsh-validate) | 0 | 2026-08-22 | 2026-08-22 | test |
| 1259 | [mario03690/dsh-writer](https://github.com/mario03690/dsh-writer) | 0 | 2026-08-22 | 2026-08-22 | Long-form drafts with the structure already decided. Blog posts, press releases, product and jo |
| 1260 | [Mars-Sea/dsh-deeppilot](https://github.com/Mars-Sea/dsh-deeppilot) | 0 | 2026-08-24 | 2026-08-24 | Native iPhone companion plugin for DeepSeek Harness — sessions, approvals, questions, notifications, and secure remote access. |
| 1261 | [Marsax110/dsh-model-fixer](https://github.com/Marsax110/dsh-model-fixer) | 0 | 2026-08-25 | 2026-08-25 | 模型无关的沙箱升级修正 + 按模型定制的协议提示段：任何模型（GPT 系最常见）在工具调用中错误携带 sandbox_permissions/justification 导致 'not strictly wider' 死循环时自动剥离；并按会话模型动态注入适配提示段。非 bundle 插件，HMR 实时生效。 |
| 1262 | [marshfolx/dsh-rescue-tui](https://github.com/marshfolx/dsh-rescue-tui) | 0 | 2026-08-24 | 2026-08-25 | a minimal emergency maintenance tui used when web ui is broken |
| 1263 | [masknull/dsh-fetch-models-search](https://github.com/masknull/dsh-fetch-models-search) | 0 | 2026-08-26 | 2026-08-26 | DSH plugin: adds a search box to the Fetch available models candidate dialog in DSH settings (browser-side DOM enhancement). DSH 插件：为「获取可用模型」候选弹窗增加搜索过滤。 |
| 1264 | [masknull/dsh-session-prompt](https://github.com/masknull/dsh-session-prompt) | 0 | 2026-08-23 | 2026-08-25 | DSH 插件:在每个会话的系统提示词最顶部注入自定义提示词,并可在 Web 设置页中即时编辑。 |
| 1265 | [Max-Null/dsh-capture](https://github.com/Max-Null/dsh-capture) | 0 | 2026-08-22 | 2026-08-25 | Dual-engine screen capture for DeepSeek Harness: box-select + red-box annotation, composer insertion (SSiD shell / plain DSH getDisplayMedia) · 双引擎屏幕截图：框选 + 红框标注，图片直入会话输入框 |
| 1266 | [Mengshang-spec/dsh-plugin-trustlens](https://github.com/Mengshang-spec/dsh-plugin-trustlens) | 0 | 2026-08-23 | 2026-08-23 | Read-only DSH plugin security auditor with current-session model review |
| 1267 | [mengxingGG/dsh-plugin-marketplace](https://github.com/mengxingGG/dsh-plugin-marketplace) | 0 | 2026-08-25 | 2026-08-25 | GitHub plugin discovery and one-click profile installation for DeepSeek Harness |
| 1268 | [Meteor-system/superpowers-for-dsh](https://github.com/Meteor-system/superpowers-for-dsh) | 0 | 2026-08-25 | 2026-08-26 | SuperPowers for DSH: portable Superpowers skills and a native DeepSeek Harness preset |
| 1269 | [meyaomiao/dsh-github-workbench](https://github.com/meyaomiao/dsh-github-workbench) | 0 | 2026-08-26 | 2026-08-26 | DSH 插件:在侧边栏使用 GitHub —— 仓库目录树 + Issues/PR/Actions 页签,支持建 Issue/PR、评论、合并、重跑 CI;better-sidebar 页签与独立面板双形态 |
| 1270 | [mhdfy1988/dsh-codex-auth](https://github.com/mhdfy1988/dsh-codex-auth) | 0 | 2026-08-23 | 2026-08-26 | ChatGPT/Codex authorization plugin for DeepSeek Harness |
| 1271 | [mhdfy1988/dsh-skill-manager](https://github.com/mhdfy1988/dsh-skill-manager) | 0 | 2026-08-24 | 2026-08-26 | Non-invasive Skill lifecycle manager for DeepSeek Harness |
| 1272 | [mhdfy1988/dsh-skin-platform](https://github.com/mhdfy1988/dsh-skin-platform) | 0 | 2026-08-23 | 2026-08-26 | Independent multi-package skin platform for DeepSeek Harness |
| 1273 | [mienfong/dsh-session-mgr](https://github.com/mienfong/dsh-session-mgr) | 0 | 2026-08-24 | 2026-08-24 | Session manager for the DeepSeek Harness web UI: move, archive, restore, backup/export and import conversations across workspaces. Trilingual (English / 简体 / 繁體). |
| 1274 | [ming-14/dsh-forwarder](https://github.com/ming-14/dsh-forwarder) | 0 | 2026-08-23 | 2026-08-24 | Make DeepSeek Harness (DSH) accessible over the local area network for other devices such as phones and tablets to access without modifying any DSH configuration |
| 1275 | [Minglink/dsh-better-sidebar](https://github.com/Minglink/dsh-better-sidebar) | 0 | 2026-08-25 | 2026-08-25 | 开放的侧边栏底座，支持三方拓展注册新侧边栏页面 |
| 1276 | [Minglink/dsh-deep-whale](https://github.com/Minglink/dsh-deep-whale) | 0 | 2026-08-25 | 2026-08-25 | 适用于 DeepSeek Harness 的鲸鱼娘系列皮肤主题 |
| 1277 | [Minglink/dsh-plugin-agent-workflow](https://github.com/Minglink/dsh-plugin-agent-workflow) | 0 | 2026-08-25 | 2026-08-25 | DeepSeek Harness Agent Workflow 工作流引擎插件 |
| 1278 | [Minglink/modlens](https://github.com/Minglink/modlens) | 0 | 2026-08-25 | 2026-08-25 | DeepSeek Harness 外挂视觉多模态与 OCR 桥接插件 |
| 1279 | [mingzeng21/dsh-stock-mentions](https://github.com/mingzeng21/dsh-stock-mentions) | 0 | 2026-08-23 | 2026-08-25 | 你在 DSH 对话中提到的股票名称或股票代码，会自动变成可点击按钮——点一下，行情和资讯就在右侧侧边栏展开。 |
| 1280 | [minyang-chen/dsh-stock-lookup](https://github.com/minyang-chen/dsh-stock-lookup) | 0 | 2026-08-25 | 2026-08-25 | DSH plugin: resolve company names to stock symbols via SEC EDGAR and fetch live quotes via Yahoo Finance |
| 1281 | [MisRightW/dsh-taskboard](https://github.com/MisRightW/dsh-taskboard) | 0 | 2026-08-20 | 2026-08-21 | dsh-taskboard |
| 1282 | [Missher12/dsh-missher-evolution](https://github.com/Missher12/dsh-missher-evolution) | 0 | 2026-08-24 | 2026-08-25 | Privacy-bounded self-improvement plugin for DeepSeek Harness |
| 1283 | [MitsukiJoe/dsh-better-ux](https://github.com/MitsukiJoe/dsh-better-ux) | 0 | 2026-08-17 | 2026-08-23 | Web UX kit for DeepSeek Harness: session row actions and a large model picker |
| 1284 | [MitsukiJoe/dsh-vision-router-inline](https://github.com/MitsukiJoe/dsh-vision-router-inline) | 0 | 2026-08-17 | 2026-08-23 | Display companion for dsh-vision-router: square picture button on each original model row |
| 1285 | [miuzel/dsh-subagent-ui](https://github.com/miuzel/dsh-subagent-ui) | 0 | 2026-08-26 | 2026-08-26 | Searchable workspace subagent manager for DeepSeek Harness Web |
| 1286 | [mobaixingyao/dsh-inform](https://github.com/mobaixingyao/dsh-inform) | 0 | 2026-08-25 | 2026-08-25 | dsh-inform 是一款为 deepseek harness开发的任务提醒插件，能够在 DSH 完成任务、需要批准 或 需要回答 时自动调用系统通知发出提醒 |
| 1287 | [MochiNek0/dsh-vendor-login](https://github.com/MochiNek0/dsh-vendor-login) | 0 | 2026-08-25 | 2026-08-25 | Sign in to AI coding plans that have no API key — Claude Pro/Max/Team, ChatGPT Plus/Pro, Copilot, SuperGrok — from the dsh settings UI. |
| 1288 | [Modellix/dsh-modellix](https://github.com/Modellix/dsh-modellix) | 0 | 2026-08-24 | 2026-08-25 | DeepSeek Harness plugin for Modellix Web Search and Web Fetch. |
| 1289 | [Momojie-S/dsh-subagent-cleanup](https://github.com/Momojie-S/dsh-subagent-cleanup) | 0 | 2026-08-25 | 2026-08-26 | DSH 插件: 子agent会话清理 —— 会话自清 + 运维侧跨workspace大扫除(归档可逆/可彻底删除) |
| 1290 | [Momojie-S/dsh-subagent-idle-delivery](https://github.com/Momojie-S/dsh-subagent-idle-delivery) | 0 | 2026-08-25 | 2026-08-25 | DSH plugin: hold busy-parent subagent notices, deliver as fresh turns when idle (hold-and-release) |
| 1291 | [Monicaxixi/dsh-loglens](https://github.com/Monicaxixi/dsh-loglens) | 0 | 2026-08-24 | 2026-08-24 | DeepSeek Harness dsh-plugin for bounded, cursor-aware log inspection |
| 1292 | [Moolmool114/dsh-client-ui-recipes](https://github.com/Moolmool114/dsh-client-ui-recipes) | 0 | 2026-08-23 | 2026-08-23 | Interface Recipes — a DeepSeek Harness dsh.client plugin: user-defined, switchable chat-surface display schemes (timeline, result panel, process groups, catalog, dimming). |
| 1293 | [moreWax/dsh-prime-agent](https://github.com/moreWax/dsh-prime-agent) | 0 | 2026-08-24 | 2026-08-25 | Closed learning loop for DeepSeek Harness: Prime Agent memory/skills bridge + OKF/OpenWiki provenance-aware knowledge serving |
| 1294 | [moreWax/dsh-remote-exec](https://github.com/moreWax/dsh-remote-exec) | 0 | 2026-08-24 | 2026-08-25 | SSH / MOSH / SAM remote execution providers for DeepSeek Harness — run the agent locally, execute on your servers |
| 1295 | [mtaech/dsh-browser-tool](https://github.com/mtaech/dsh-browser-tool) | 0 | 2026-08-25 | 2026-08-25 | DSH 浏览器工具：驱动 Chromium 标签页（headless / CDP attach / 拉起桌面应用 / 经 Browser Relay 接管真实 Chrome），open-close-run 三段式 + tab 脚本 API，移植自 oh-my-pi |
| 1296 | [MuAllen/dsh-gateway-wallet](https://github.com/MuAllen/dsh-gateway-wallet) | 0 | 2026-08-24 | 2026-08-26 | 读取当前 API key 在站点账本上的剩余额度和实扣，支持 Sub2API、New API 与 DeepSeek 官方，不是本地 token 估算。 |
| 1297 | [Muredsa/dsh-benchup](https://github.com/Muredsa/dsh-benchup) | 0 | 2026-08-26 | 2026-08-26 | Install with npm i dsh-benchup. Reproducible, profile-aware benchmarks for DeepSeek Harness — compare models, plugins, prompts, and agent strategies. |
| 1298 | [Mutton-hub/adatile-mcp](https://github.com/Mutton-hub/adatile-mcp) | 0 | 2026-08-22 | 2026-08-23 | AdaTile-MCP: high-resolution image adaptive tiling MCP server for DeepSeek vision model (deepseek-v4-flash-vision-exp). L1-L6 pipeline (fastpath, saliency, adaptive tiling, Files API assembly, streaming VLM, rule-based merge) + eval harness. Setup: clone, run setup.bat, add your agent MCP config -> see README. |
| 1299 | [MuziiXzx/dsh-taskdone-notify](https://github.com/MuziiXzx/dsh-taskdone-notify) | 0 | 2026-08-23 | 2026-08-23 | 任务完成时通知用户 |
| 1300 | [navid-kianfar/dsh-add-assets](https://github.com/navid-kianfar/dsh-add-assets) | 0 | 2026-08-26 | 2026-08-26 | Options plate on the DeepSeek Harness composer's + button — pick files and folders from the project or anywhere on the machine, upload from your device, or run a slash command — with inline path chips and a Claude Code-style attachment preview. |
| 1301 | [navid-kianfar/dsh-advanced-sidebar](https://github.com/navid-kianfar/dsh-advanced-sidebar) | 0 | 2026-08-26 | 2026-08-26 | Advanced sidebar operations for the DeepSeek Harness Web Client: git changes, a terminal, a file browser, a dev-server preview, background tasks, Open in, Archive and Delete. |
| 1302 | [navid-kianfar/dsh-memory](https://github.com/navid-kianfar/dsh-memory) | 0 | 2026-08-26 | 2026-08-26 | Persistent, searchable, per-project memory for the DeepSeek Harness: decisions, rules, and session context in a queryable DuckDB file, with the rule set injected into every model request — plus a full management UI in the Web Client. |
| 1303 | [navid-kianfar/dsh-tasks-manager](https://github.com/navid-kianfar/dsh-tasks-manager) | 0 | 2026-08-26 | 2026-08-26 | DeepSeek Harness plugin: a project task board kept with the project as a queryable SQLite file, with a kanban/list view in the Web Client, model-facing task tools, and cards you can dispatch to the agent as background jobs. |
| 1304 | [navid-kianfar/dsh-usage-info](https://github.com/navid-kianfar/dsh-usage-info) | 0 | 2026-08-26 | 2026-08-26 | Context occupancy and account balance for the DeepSeek Harness Web Client — a session-header readout with a swappable balance provider. |
| 1305 | [navid-kianfar/dsh-worktree](https://github.com/navid-kianfar/dsh-worktree) | 0 | 2026-08-26 | 2026-08-26 | Git worktrees and branches for the DeepSeek Harness Web Client: a session-header chip that switches branches, creates worktrees, and opens them as harness workspaces. |
| 1306 | [Nay-1/dsh-skill-manage](https://github.com/Nay-1/dsh-skill-manage) | 0 | 2026-08-22 | 2026-08-22 | DeepSeek Harness 技能管理设置页插件：图形化管理用户级/项目级技能的安装、卸载与调用启停 |
| 1307 | [NecromanAlbert/dsh-i-have-adhd](https://github.com/NecromanAlbert/dsh-i-have-adhd) | 0 | 2026-08-26 | 2026-08-26 | Always-on ADHD-friendly output for every DeepSeek Harness session. Host systemPrompt, not a skill catalog item. |
| 1308 | [NecromanAlbert/dsh-self-restart](https://github.com/NecromanAlbert/dsh-self-restart) | 0 | 2026-08-26 | 2026-08-26 | Any DSH session can request a Desktop restart, then the same persisted session is resumed and followup'd with its mission. |
| 1309 | [NecromanAlbert/dsh-show-media](https://github.com/NecromanAlbert/dsh-show-media) | 0 | 2026-08-25 | 2026-08-25 | Show a local image or short video inside the current DeepSeek Harness conversation card. |
| 1310 | [NecromanAlbert/dsh-skill-slash-fuzzy](https://github.com/NecromanAlbert/dsh-skill-slash-fuzzy) | 0 | 2026-08-25 | 2026-08-26 | Resolve unique kebab-case skill substrings in DeepSeek Harness slash tokens. |
| 1311 | [NeoRrrr/dsh-project-skill-paths](https://github.com/NeoRrrr/dsh-project-skill-paths) | 0 | 2026-08-25 | 2026-08-25 | Project-scoped custom Skill roots for DeepSeek Harness |
| 1312 | [NevermindZZT/dsh-manager-plugin](https://github.com/NevermindZZT/dsh-manager-plugin) | 0 | 2026-08-23 | 2026-08-24 | dsh manger 远程工具对应使用的 dsh 插件，直接完成 dsh 远程访问 |
| 1313 | [NexusAgentX/dsh-advisor](https://github.com/NexusAgentX/dsh-advisor) | 0 | 2026-08-23 | 2026-08-26 | dsh plugin bundle porting the rpiv advisor subsystem: an on-demand zero-parameter advisor() tool that forwards the full session to a separately-configured reviewer model. |
| 1314 | [nienieai/dsh-canmv-k230-bridge](https://github.com/nienieai/dsh-canmv-k230-bridge) | 0 | 2026-08-21 | 2026-08-26 | DSH 动态插件：桥接 CanMV K230 开发板（悬浮面板 + 串口运行脚本与预览） |
| 1315 | [ningbonb/dsh-client-ui-brand](https://github.com/ningbonb/dsh-client-ui-brand) | 0 | 2026-08-26 | 2026-08-26 | Custom product name and logo branding for DeepSeek Harness Web 自定义 DeepSeek Harness Web 端 logo 和产品名称 |
| 1316 | [nishuoyang/dsh-wallpaper-bg](https://github.com/nishuoyang/dsh-wallpaper-bg) | 0 | 2026-08-15 | 2026-08-25 | DeepSeek Harness Web UI Standalone Wallpaper Background Plugin: Three sources including built-in wallpapers, custom uploads, and Wallpaper Engine library (read-only). Supports image, video, and scene preview rendering, along with adjustments for overlay, blur, brightness, and safe zoom. |
| 1317 | [NIU-001-LIU/dsh-chat-timeline-plus](https://github.com/NIU-001-LIU/dsh-chat-timeline-plus) | 0 | 2026-08-25 | 2026-08-25 | DeepSeek Harness timeline with hover Q&A preview and panel pin |
| 1318 | [niushuanan/dsh-adaptive-update](https://github.com/niushuanan/dsh-adaptive-update) | 0 | 2026-08-26 | 2026-08-26 | Check upstream manually or every six hours, use a narrowly scoped agent for compatibility work, and switch atomically with rollback. |
| 1319 | [niushuanan/dsh-image-vision](https://github.com/niushuanan/dsh-image-vision) | 0 | 2026-08-26 | 2026-08-26 | Let vision-capable models read native attachments while giving text-only models an image tool that supports follow-up questions. |
| 1320 | [niushuanan/dsh-model-usage](https://github.com/niushuanan/dsh-model-usage) | 0 | 2026-08-26 | 2026-08-26 | Inspect model quotas, periods, and refresh state by provider in Settings, with data loaded only when the user opens the page. |
| 1321 | [niushuanan/dsh-multi-window](https://github.com/niushuanan/dsh-multi-window) | 0 | 2026-08-26 | 2026-08-26 | Open multiple independent conversations side by side, each with isolated navigation, drafts, and runtime state. |
| 1322 | [niushuanan/dsh-parallel-worktree](https://github.com/niushuanan/dsh-parallel-worktree) | 0 | 2026-08-26 | 2026-08-26 | Move parallel tasks into isolated Git worktrees, inspect conflicts, and merge the results safely into the current branch. |
| 1323 | [niushuanan/dsh-pure-chat](https://github.com/niushuanan/dsh-pure-chat) | 0 | 2026-08-26 | 2026-08-26 | Start a chat immediately without a workspace, work mode, or execution permissions while keeping image and text-file uploads. |
| 1324 | [niushuanan/dsh-selection-memory](https://github.com/niushuanan/dsh-selection-memory) | 0 | 2026-08-26 | 2026-08-26 | Quote, discuss, or remember selected conversation text, then maintain durable context in separate editable user and AI memories. |
| 1325 | [niushuanan/dsh-skill-manager](https://github.com/niushuanan/dsh-skill-manager) | 0 | 2026-08-26 | 2026-08-26 | Browse installed Skills, their files, and content in Settings, then adaptively import from a file, folder, ZIP, or GitHub with AI. |
| 1326 | [niushuanan/dsh-teamwork](https://github.com/niushuanan/dsh-teamwork) | 0 | 2026-08-26 | 2026-08-26 | Run collaborating agents and external experts concurrently under one coordinating agent, then bring every result back into the current task. |
| 1327 | [niushuanan/dsh-token-overview](https://github.com/niushuanan/dsh-token-overview) | 0 | 2026-08-26 | 2026-08-26 | See tokens, cache usage, calls, active periods, and estimated cost across AI clients on the whole computer. |
| 1328 | [niushuanan/dsh-whale-girl](https://github.com/niushuanan/dsh-whale-girl) | 0 | 2026-08-26 | 2026-08-26 | Add a native cross-page companion whose presence, shortcuts, and feedback follow the current DSH session state. |
| 1329 | [NiuZhuang/dsh-git-ai](https://github.com/NiuZhuang/dsh-git-ai) | 0 | 2026-08-22 | 2026-08-23 | A DeepSeek Harness plugin that records which files the agent edited, with which model, and in which session into git-ai |
| 1330 | [Nkjv2/dsh-ui-pet](https://github.com/Nkjv2/dsh-ui-pet) | 0 | 2026-08-23 | 2026-08-23 | A canvas sprite-sheet pet plugin for the DeepSeek Harness web GUI. A dsh bundle + client plugin that renders a pointer-following mascot in the shell.overlay layer. MIT licensed. |
| 1331 | [NonchalantLudens/dsh-side-dir](https://github.com/NonchalantLudens/dsh-side-dir) | 0 | 2026-08-23 | 2026-08-24 | Project directory preview for the DeepSeek Harness web GUI — details-panel file tree + read-only file preview via a fenced /dirpreview command |
| 1332 | [nxz1026/SinglePlayer](https://github.com/nxz1026/SinglePlayer) | 0 | 2026-08-22 | 2026-08-22 | 单身汉播放器，适配DeepSeek harness web的播放器，支持多平台聚合。Bachelor Player is a media player designed to integrate with DeepSeek Harness Web, supporting multi-platform content aggregation. |
| 1333 | [Nyzeep/dsh-thinking-level](https://github.com/Nyzeep/dsh-thinking-level) | 0 | 2026-08-25 | 2026-08-25 | A thinking-level (reasoning effort) selector for the DeepSeek Harness Web UI — shows only the levels the current model declares and prefers max by default |
| 1334 | [of1102/dsh-web-search-ark](https://github.com/of1102/dsh-web-search-ark) | 0 | 2026-08-25 | 2026-08-25 | Volcengine Ark web-search provider plugin for DeepSeek Harness |
| 1335 | [oksure/dsh-mobile-comfort](https://github.com/oksure/dsh-mobile-comfort) | 0 | 2026-08-25 | 2026-08-25 | Touch-device comfort fixes for the DeepSeek Harness web client: ghost tooltip suppression + touch-action policy |
| 1336 | [oneirictouch/dsh-explorer-editor](https://github.com/oneirictouch/dsh-explorer-editor) | 0 | 2026-08-22 | 2026-08-22 | 左侧边栏的“资料浏览器”和主工作区的“文本编辑器”，页签方式展示，适合讨厌工作区被过度分割的人。 |
| 1337 | [Oscar-Williams/dsh-deepatlas](https://github.com/Oscar-Williams/dsh-deepatlas) | 0 | 2026-08-22 | 2026-08-22 | Local capability assurance and evidence-backed plugin navigation for DeepSeek Harness. |
| 1338 | [outprintHelloLi/dsh-piggy-bank](https://github.com/outprintHelloLi/dsh-piggy-bank) | 0 | 2026-08-25 | 2026-08-25 | dsh插件：DeepSeek 余额展示 |
| 1339 | [Parker-xia/dsh-research-refs](https://github.com/Parker-xia/dsh-research-refs) | 0 | 2026-08-26 | 2026-08-26 | DSH plugin: tidy messy pasted citations into uniformly formatted references (refs_parse / refs_verify / refs_dedup / refs_format + research-refs skill) |
| 1340 | [Pasumao/dsh-plugin-windows-guard](https://github.com/Pasumao/dsh-plugin-windows-guard) | 0 | 2026-08-25 | 2026-08-25 | DeepSeek Harness (dsh) Windows 环境防坑守则 skill 插件（纯数据）：编码/转义/路径/进程/乱码预防规则，无修复工具 |
| 1341 | [paulalesius/dsh-openai-api](https://github.com/paulalesius/dsh-openai-api) | 0 | 2026-08-24 | 2026-08-24 | OpenAI-compatible /v1/chat/completions (streaming and non-streaming) and /v1/models endpoint on the DSH web server. |
| 1342 | [pharaohnie/dsh-rtk-tools](https://github.com/pharaohnie/dsh-rtk-tools) | 0 | 2026-08-25 | 2026-08-25 | DSH plugin: expose rtk (Rust Token Killer) as wide-category Tools — save 60-90% tokens on shell output with softRewriteBash routing |
| 1343 | [phillarmonic/dsh-llm-kimi](https://github.com/phillarmonic/dsh-llm-kimi) | 0 | 2026-08-25 | 2026-08-25 | A Kimi K3 connector plugin for the DeepSeek Harness LLM capability |
| 1344 | [piaohua/dsh-schedule-command](https://github.com/piaohua/dsh-schedule-command) | 0 | 2026-08-22 | 2026-08-22 | DeepSeek Harness 的 /schedule 定时任务命令 —— 一句话创建会话内单次/周期任务，⏰ 标识自动识别定时会话。/schedule command for DeepSeek Harness — create session-local one-shot/recurring tasks in plain language; ⏰ marks schedule sessions at a glance. |
| 1345 | [pick1e-morty/dsh-suggest-reply](https://github.com/pick1e-morty/dsh-suggest-reply) | 0 | 2026-08-22 | 2026-08-23 | 帮我想想 —— 一个基于 DSH-better-sidebar 的侧边栏 tab：用你自己写的 system prompt 对主对话最新一条 AI 回复生成候选回复，点击直填输入框。 |
| 1346 | [pipiwolve/dsh-baidu-ocr](https://github.com/pipiwolve/dsh-baidu-ocr) | 0 | 2026-08-25 | 2026-08-26 | Baidu cloud OCR bundle for DeepSeek Harness: drag images/PDFs in, OCR to Markdown with PaddleOCR-VL or Unlimited-OCR. 百度云 OCR 插件：拖入图片/PDF 识别为 Markdown 并写入本地文件。 |
| 1347 | [popeye1113/dsh-question-jump-bar](https://github.com/popeye1113/dsh-question-jump-bar) | 0 | 2026-08-25 | 2026-08-25 | DSH Web 插件：会话右侧的问题索引标尺（Question Jump Bar），每个刻度一次提问，悬停预览、点击/键盘跳转。 |
| 1348 | [Practice019/dsh-doubao-plugin](https://github.com/Practice019/dsh-doubao-plugin) | 0 | 2026-08-22 | 2026-08-23 | DSH 插件：通过本地 Quicker 转发（doubao web2api） 提供 `doubao_ask` 动态搜索/图片生成/多模态识图工具， 并支持**粘贴图片 → 本地路径**（paste-to-path）。 |
| 1349 | [princeofdream/dsh-codebase-memory-mcp](https://github.com/princeofdream/dsh-codebase-memory-mcp) | 0 | 2026-08-25 | 2026-08-25 | dsh-codebase-memory-mcp |
| 1350 | [qewregrfhnm/dsh-session-manager](https://github.com/qewregrfhnm/dsh-session-manager) | 0 | 2026-08-22 | 2026-08-22 | Full session management plugin for DeepSeek Harness (DSH) web UI: delete/trash/restore, workspace grouping, move sessions between workspaces, unread markers, context compaction threshold. Fully local, bilingual zh/en. |
| 1351 | [qianxiao1213/zcode-usage-stats](https://github.com/qianxiao1213/zcode-usage-stats) | 0 | 2026-08-22 | 2026-08-22 | 仿zcode的使用统计 - DSH Token 用量统计插件(趋势图/仪表盘/活跃热力图) v0.1.0 |
| 1352 | [qiaoji1990-alt/aifred-dsh-task-ledger](https://github.com/qiaoji1990-alt/aifred-dsh-task-ledger) | 0 | 2026-08-25 | 2026-08-25 | Provider-neutral task lifecycle and idempotent event ledger plugin for DeepSeek Harness. Works standalone for any DSH project and optionally integrates with Aifred through a bridge. |
| 1353 | [qingmumingyang/dsh-doc-toolkit](https://github.com/qingmumingyang/dsh-doc-toolkit) | 0 | 2026-08-23 | 2026-08-24 | DSH 文档读写工具包 - PDF/DOCX/XLSX/CSV 读写与 PDF 导出（利用dsh制作的，希望能帮到你们） |
| 1354 | [qingshanyuluo/dsh-mobile-ux](https://github.com/qingshanyuluo/dsh-mobile-ux) | 0 | 2026-08-25 | 2026-08-26 | DeepSeek Harness mobile: CSS-only UI plugin, password-protected Cloudflare tunnel and a tiny Android WebView app - use DSH on your phone. |
| 1355 | [qiqiangvae/dsh-my-favorites](https://github.com/qiqiangvae/dsh-my-favorites) | 0 | 2026-08-24 | 2026-08-24 | dsh 收藏夹插件，可以收藏网址和会话，支持快捷键切换会话 |
| 1356 | [qiufengcrl/dsh-ip-https](https://github.com/qiufengcrl/dsh-ip-https) | 0 | 2026-08-26 | 2026-08-26 | DeepSeek Harness plugin: remote settings + Let's Encrypt IP certificates |
| 1357 | [Qiwei-QW/dsh-r-ide](https://github.com/Qiwei-QW/dsh-r-ide) | 0 | 2026-08-22 | 2026-08-24 | A four-pane R IDE (Editor / Console / Environment / Plots) integrated into DeepSeek Harness as a tab of [dsh-better-sidebar](https://github.com/omdsh-dev/DSH-better-sidebar), with one dedicated R process per conversation. |
| 1358 | [quan-v/dsh-safe-gate](https://github.com/quan-v/dsh-safe-gate) | 0 | 2026-08-25 | 2026-08-25 | dsh 装前守门:OSV 供应链扫描 + 插件契约检查。 Pre-flight safety gate for dsh plugins/MCP. |
| 1359 | [QuanQQQ/dsh-plugin-dev-manager](https://github.com/QuanQQQ/dsh-plugin-dev-manager) | 0 | 2026-08-24 | 2026-08-26 | Stable control plane for isolated DeepSeek Harness plugin development |
| 1360 | [Quophic/dsh-plugin-installer](https://github.com/Quophic/dsh-plugin-installer) | 0 | 2026-08-18 | 2026-08-23 | DeepSeek Harness（dsh）插件安全安装/卸载器：自动备份配置、失败自动回滚（卸载失败自动重新安装插件）、重启并做健康检查。\| Safe dsh plugin installer & uninstaller: config backup, rollback (reinstall on uninstall failure), restart & health check. |
| 1361 | [RagnarPitla/dsh-field-guide](https://github.com/RagnarPitla/dsh-field-guide) | 0 | 2026-08-24 | 2026-08-24 | An evidence-badged field guide to DeepSeek Harness (dsh), plus a working plugin. Every claim marked with how it was verified. Independent and unofficial. |
| 1362 | [raktim-mondol/dsh-tui-en](https://github.com/raktim-mondol/dsh-tui-en) | 0 | 2026-08-22 | 2026-08-22 | English-only fork of dsh-TUI — Claude Code-style terminal UI for DeepSeek Harness |
| 1363 | [rand0wn/dsh-malware-audit](https://github.com/rand0wn/dsh-malware-audit) | 0 | 2026-08-21 | 2026-08-22 | DeepSeek Harness (dsh) plugin: real AST-based scan of installed plugins for malicious-intent patterns, with an optional periodic schedule and auto-quarantine on critical findings. Advisory-by-default, not an antivirus signature database. |
| 1364 | [Ranz-Feng/dsh-web-import](https://github.com/Ranz-Feng/dsh-web-import) | 0 | 2026-08-26 | 2026-08-26 | Import DeepSeek Web (chat.deepseek.com) chat history into DeepSeek Harness as resumable, workspace-grouped sessions with original titles preserved. |
| 1365 | [raydez/dsh-pet-plugin](https://github.com/raydez/dsh-pet-plugin) | 0 | 2026-08-18 | 2026-08-22 | deepseek harness pet plugin（桌面宠物插件） |
| 1366 | [rayfalling/dsh-tool-visibility](https://github.com/rayfalling/dsh-tool-visibility) | 0 | 2026-08-25 | 2026-08-26 | DSH plugin: control which tool schemas are injected into the DeepSeek Harness model context — settings UI + tools.restrict filter + persisted state |
| 1367 | [rchen1207/dsh-password-generator](https://github.com/rchen1207/dsh-password-generator) | 0 | 2026-08-24 | 2026-08-25 | 生成密码，只生不存 |
| 1368 | [RichDavidMu/create-dsh-plugin](https://github.com/RichDavidMu/create-dsh-plugin) | 0 | 2026-08-20 | 2026-08-24 | Scaffold a DeepSeek Harness plugin project — a working plugin with one model-facing tool, a profile bundle that mounts it, dsh's own toolchain, and documentation an agent can follow without reading dsh's source. |
| 1369 | [rjn32s/dsh-whois-plugin](https://github.com/rjn32s/dsh-whois-plugin) | 0 | 2026-08-22 | 2026-08-23 | RDAP-backed whois tool plugin for DeepSeek Harness (dsh) — look up domain registration data as a model tool |
| 1370 | [robauto-ai/dsh-growth](https://github.com/robauto-ai/dsh-growth) | 0 | 2026-08-21 | 2026-08-22 | Digital growth and commerce harness. Grow your brand and transact agent to agent. Monetize your repo or skill via Robauto or let the agent grow your site traffic.  Deepseek harness plugin, works with MetaAI, Copilot, Grok, Claude, Google, Bing, Hubspot and Perplexity agents.  |
| 1371 | [robbin810130/dsh-rtk](https://github.com/robbin810130/dsh-rtk) | 0 | 2026-08-24 | 2026-08-24 | Community DSH plugin that applies explicit RTK command-output filtering to bash tools at boot. |
| 1372 | [robbywang25/dsh-llm-mlx](https://github.com/robbywang25/dsh-llm-mlx) | 0 | 2026-08-25 | 2026-08-26 | DeepSeek Harness plugin for local MLX-LM models with loopback-only defaults and optional managed server startup |
| 1373 | [Rock-ql/dsh-git-branch](https://github.com/Rock-ql/dsh-git-branch) | 0 | 2026-08-25 | 2026-08-25 | DSH Desktop plugin: git branch pill in the composer, with local/remote listing and confirmed checkout \| DSH 对话栏 Git 分支胶囊 |
| 1374 | [rocklau/dsh-ui-tool-graph](https://github.com/rocklau/dsh-ui-tool-graph) | 0 | 2026-08-22 | 2026-08-22 | Tool-call value graph tab for the DeepSeek Harness (dsh) Web UI: cost/duration/error weights over conversation trajectories with one-click next-turn optimization prompts. |
| 1375 | [royenheart/dsh-migrate-bot](https://github.com/royenheart/dsh-migrate-bot) | 0 | 2026-08-25 | 2026-08-26 | Automatically migrate dsh plugins to the new version. |
| 1376 | [rudyz666/dsh-bili-asr](https://github.com/rudyz666/dsh-bili-asr) | 0 | 2026-08-23 | 2026-08-23 | 解析 B站视频链接，提取完整脚本/字幕：优先字幕轨，无字幕用本地 whisper 转写，导出 SRT/TXT/JSON。DeepSeek Harness 插件，跨平台 Windows/macOS/Linux（纯 Node）。 |
| 1377 | [runfali/dsh-paperclip](https://github.com/runfali/dsh-paperclip) | 0 | 2026-08-24 | 2026-08-24 | dsh 零侵入式 bundle 插件：📎 输入框上传按钮 + 待发送文件浮层（仅文件名，可移除）· read_document 多格式读取工具（txt / pdf / docx / xlsx / json / md / ini / conf，支持 offset/limit 分页）· 设置 → 通用设置一个开关。标准 Cordis bundle 插件，不改 DSH 源码，内容寻址落盘去重，深浅色主题自适应。 |
| 1378 | [runfali/dsh-skill-curator](https://github.com/runfali/dsh-skill-curator) | 0 | 2026-08-25 | 2026-08-25 | 为 dsh 打造的自动技能策展插件：每 N 轮真实对话，后台起一个评审子代理阅读会话摘要，主动把值得沉淀的经验提炼为 ~/.dsh/skills/<name>/SKILL.md - 把 Hermes 的「后台评审自我改进」闭环移植到 DSH，零侵入 bundle 插件，不改 dsh 源码。 |
| 1379 | [RyensX/dsh-remote-gateway](https://github.com/RyensX/dsh-remote-gateway) | 0 | 2026-08-23 | 2026-08-24 | 提供安全的反向代理，使DeepSeek Harness可以远程访问，随时随地和AI对话。/ Provides a secure reverse proxy, enabling DeepSeek Harness to be accessed remotely and to converse with AI anytime, anywhere. |
| 1380 | [Ryu6Zero/dsh-hindsight](https://github.com/Ryu6Zero/dsh-hindsight) | 0 | 2026-08-25 | 2026-08-26 | 🧠 Cross-session memory for DeepSeek Harness backed by Hindsight. Self-contained dsh-plugin: /hindsight commands + hindsight_recall/remember/status/list/forget agent tools. Lightweight, no dsh-mnemon, no orchestrator. |
| 1381 | [S-AN-Shu/dsh-skill-manager](https://github.com/S-AN-Shu/dsh-skill-manager) | 0 | 2026-08-25 | 2026-08-26 | Security-bounded Agent Skill management and GitHub marketplace plugin for DeepSeek Harness and DSH Desktop |
| 1382 | [s1lencewill/dsh-markdown-reader](https://github.com/s1lencewill/dsh-markdown-reader) | 0 | 2026-08-23 | 2026-08-23 | DSH Web GUI full-screen Markdown reader with GFM, outline, KaTeX, Mermaid, and relative resource navigation. |
| 1383 | [SA1992X/dsh-ctrl-enter-submit](https://github.com/SA1992X/dsh-ctrl-enter-submit) | 0 | 2026-08-25 | 2026-08-26 | 轻松换行 |
| 1384 | [SaitoAsuka1121/dsh-client-ui-elasticsearch](https://github.com/SaitoAsuka1121/dsh-client-ui-elasticsearch) | 0 | 2026-08-24 | 2026-08-24 | dsh elasticsearch plugin |
| 1385 | [sam-midlight/dsh-loop-rescue](https://github.com/sam-midlight/dsh-loop-rescue) | 0 | 2026-08-22 | 2026-08-22 | DRAFT — DeepSeek Harness guard that breaks an agent out of a tool-call loop and escalates to a stronger model for one concrete next action. Window-based detection with a progress epoch, so it catches cycles the stock single-slot repeat guard resets away. |
| 1386 | [sandersyao/dsh-plugin-ui-session-fork](https://github.com/sandersyao/dsh-plugin-ui-session-fork) | 0 | 2026-08-25 | 2026-08-25 | deepseek harness 插件 增加会话分组方式“树形” |
| 1387 | [sANDzER0/dsh-hippocampus](https://github.com/sANDzER0/dsh-hippocampus) | 0 | 2026-08-26 | 2026-08-26 | Cross-session project memory for DeepSeek Harness — capture / consolidate / recall, keyword + optional local-Ollama semantic search. Inspired by magic-context. |
| 1388 | [savageops/dsh-rich-context](https://github.com/savageops/dsh-rich-context) | 0 | 2026-08-26 | 2026-08-26 | Agent instruction manager for DSH — edit and template the AGENTS.md files the harness actually reads (global + per-workspace) |
| 1389 | [savageops/dsh-rich-questions](https://github.com/savageops/dsh-rich-questions) | 0 | 2026-08-26 | 2026-08-26 | Rich branching survey system for DeepSeek Harness (DSH) Web GUI — ask_survey tool with branch graphs, delayed hover insights, Mermaid diagrams, quick mode, reroll/push/discuss actions |
| 1390 | [savageops/dsh-rich-tracking](https://github.com/savageops/dsh-rich-tracking) | 0 | 2026-08-26 | 2026-08-26 | Percent-progress scoreboard for DeepSeek Harness — evidence-bound rows, git-captured checkpoints, pursue/align/dismiss operator whip |
| 1391 | [sazzadurrahmaan/dsh-telegram](https://github.com/sazzadurrahmaan/dsh-telegram) | 0 | 2026-08-22 | 2026-08-22 | Telegram channel for DeepSeek Harness — chat with your agent from Telegram, with a deny-by-default allowlist and in-chat approval for destructive tools. |
| 1392 | [sd1g1/dsh-muse-total-tps](https://github.com/sd1g1/dsh-muse-total-tps) | 0 | 2026-08-21 | 2026-08-22 | DSH Web 插件：Muse Spark 使用包含 TTFT 的总生成时间计算 TPS |
| 1393 | [sdoygb/geometry-knowledge](https://github.com/sdoygb/geometry-knowledge) | 0 | 2026-08-26 | 2026-08-26 | 几何论（共扼谱几何 CSG）知识库插件 for DeepSeek Harness: 纯离线 BM25 检索，零运行时依赖 |
| 1394 | [secyborg/dsh-command-rail](https://github.com/secyborg/dsh-command-rail) | 0 | 2026-08-25 | 2026-08-25 | DSH web plugin: a Codex-style command-history rail covering the WHOLE session |
| 1395 | [secyborg/dsh-compact-chat-ui](https://github.com/secyborg/dsh-compact-chat-ui) | 0 | 2026-08-25 | 2026-08-25 | DSH web plugin: a settings card to tune chat reading density — font size, line height, and block spacing of the conversation area (assistant markdown + user bubbles), applied live |
| 1396 | [secyborg/dsh-find-bar](https://github.com/secyborg/dsh-find-bar) | 0 | 2026-08-25 | 2026-08-25 | DSH web plugin: a Cmd/Ctrl+F find bar (like the browser's built-in find) for the desktop Electron shell, which has none |
| 1397 | [secyborg/dsh-glm-web-search](https://github.com/secyborg/dsh-glm-web-search) | 0 | 2026-08-26 | 2026-08-26 | DSH host plugin: GLM (Zhipu) web-search provider for the ctx.web seam — structured results, no model turn, reuses your ZAI coding key |
| 1398 | [ShadowQuill/DialogueContextBridge](https://github.com/ShadowQuill/DialogueContextBridge) | 0 | 2026-08-26 | 2026-08-26 | 对话上下文桥接 — 为大语言模型(LLM)/AI 智能体的对话做跨会话上下文桥接的 DSH 插件：把一次对话的共识打包成可移植快照，一键引入新对话（三层快照 / SQLite+FTS5 / AES-256-GCM） |
| 1399 | [shao-01-test/dsh-chat-rail](https://github.com/shao-01-test/dsh-chat-rail) | 0 | 2026-08-26 | 2026-08-26 | dsh-chat-rail — DeepSeek Harness 聊天右侧导航拉条插件：按「提问→回答」轮次显示彩色节点（绿/黄/红/蓝表状态），点击即跳转对应提问与回答段落，悬停展开状态面板，刚回答完有闪光动画，关键词自动提炼成短句。一个拉条，快速定位整场对话。 |
| 1400 | [shaomingbo/dsh-open-in-editor](https://github.com/shaomingbo/dsh-open-in-editor) | 0 | 2026-08-26 | 2026-08-26 | Open DSH Web produced files in a configurable local macOS IDE |
| 1401 | [shaomingbo/dsh-session-reference-copy](https://github.com/shaomingbo/dsh-session-reference-copy) | 0 | 2026-08-23 | 2026-08-24 | Copy canonical cross-session references from the DeepSeek Harness Web session header. |
| 1402 | [sharewiner/dsh-model-management](https://github.com/sharewiner/dsh-model-management) | 0 | 2026-08-25 | 2026-08-25 | DSH model management, synchronized model visibility, and OpenAI Responses web search. |
| 1403 | [shendeguize/AgentSideCar](https://github.com/shendeguize/AgentSideCar) | 0 | 2026-08-22 | 2026-08-25 | A local-first CLI for observing AI-agent sessions |
| 1404 | [shendeguize/Remote_DSH_Center](https://github.com/shendeguize/Remote_DSH_Center) | 0 | 2026-08-20 | 2026-08-24 | One-page local manager and CLI for local and remote dsh web instances, with SSH tunnels for remote hosts. |
| 1405 | [shine-233/dsh-waimao](https://github.com/shine-233/dsh-waimao) | 0 | 2026-08-25 | 2026-08-25 | 外贸获客插件 for DeepSeek Harness (dsh): Google 三层搜客 + WhatsApp 客服审核台 + 邮件触达闭环 (ICP 评分/跟进序列/CRM/报价PDF), 零依赖 |
| 1406 | [ShineFree7/dsh-daily-log](https://github.com/ShineFree7/dsh-daily-log) | 0 | 2026-08-23 | 2026-08-23 | Daily work log plugin for DeepSeek Harness: /daily scaffold + daily_log_write/read/list tools, YYYY-MM-DD.md + theme-aware HTML dashboard |
| 1407 | [shizhanyu13/dsh-ironbound-policy](https://github.com/shizhanyu13/dsh-ironbound-policy) | 0 | 2026-08-26 | 2026-08-26 | @shizhanyu13/dsh-ironbound-policy — DSH plugin: Ironbound hard-gate guard. Blocks dangerous shell commands before they reach a tool, with a double-layer degrade counter over tools/execute. dsh-plugin. |
| 1408 | [shizhanyu13/dsh-waom](https://github.com/shizhanyu13/dsh-waom) | 0 | 2026-08-26 | 2026-08-26 | @shizhanyu13/dsh-waom — DSH plugin: autonomous-ops (WAOM). Monitor / decide / drive a subagent fix / evaluate independently (GAN). dsh-plugin. |
| 1409 | [shuaihaoV/dsh-mcp-skill-control](https://github.com/shuaihaoV/dsh-mcp-skill-control) | 0 | 2026-08-25 | 2026-08-25 | DSH（DeepSeek Harness）Web GUI 的 MCP 服务器管理面板：状态查看、启停/重启、新增/删除、JSON 导入，以及本地技能启停控制。 |
| 1410 | [Shyboy0499/dsh-git-tools](https://github.com/Shyboy0499/dsh-git-tools) | 0 | 2026-08-26 | 2026-08-26 | Local git tools for DeepSeek Harness (dsh): git_status, git_diff, git_log, git_commit |
| 1411 | [sidleo/dsh-desktop](https://github.com/sidleo/dsh-desktop) | 0 | 2026-08-22 | 2026-08-22 | DeepSeek Harness 桌面壳：打开应用=启动 dsh web 服务并加载界面，关闭应用=自动停止服务。Electron desktop shell for DeepSeek Harness (DSH) |
| 1412 | [sidleo/skill-filesystem-plus](https://github.com/sidleo/skill-filesystem-plus) | 0 | 2026-08-17 | 2026-08-23 | Configurable skill discovery provider for DeepSeek Harness (DSH): cwd/project/ancestors/global layers with editable parent dirs, plugin card UI, disk persistence |
| 1413 | [sijie-ni-0214/dsh-subagent-error-details](https://github.com/sijie-ni-0214/dsh-subagent-error-details) | 0 | 2026-08-26 | 2026-08-26 | DSH plugin: deliver the real failure reason (e.g. RATE_LIMIT 429) to the parent agent when a background subagent fails |
| 1414 | [siweimofang/dsh-plugin-zhishe-baojia-shenhe](https://github.com/siweimofang/dsh-plugin-zhishe-baojia-shenhe) | 0 | 2026-08-21 | 2026-08-22 | 知设装修报价审核DSH插件 - 支持视觉OCR截图输入 |
| 1415 | [siweimofang/dsh-plugin-zhishe-bikeng-qa](https://github.com/siweimofang/dsh-plugin-zhishe-bikeng-qa) | 0 | 2026-08-21 | 2026-08-22 | 知设装修避坑问答DSH插件 |
| 1416 | [siweimofang/dsh-plugin-zhishe-common](https://github.com/siweimofang/dsh-plugin-zhishe-common) | 0 | 2026-08-22 | 2026-08-22 | 知设 DSH 插件共享基础设施 - 知识库加载/检索/基准价格/风险评估 |
| 1417 | [siweimofang/dsh-plugin-zhishe-zaojia-gusuan](https://github.com/siweimofang/dsh-plugin-zhishe-zaojia-gusuan) | 0 | 2026-08-22 | 2026-08-22 | 知设装修造价估算DSH插件 |
| 1418 | [siweimofang/zhishe-a2a](https://github.com/siweimofang/zhishe-a2a) | 0 | 2026-08-22 | 2026-08-22 | 知设AI装修顾问 - 主仓库(知识库+DSH插件+GEO) |
| 1419 | [SLin-code/dsh-skill-manager](https://github.com/SLin-code/dsh-skill-manager) | 0 | 2026-08-24 | 2026-08-24 | Minimal, security-focused local Skill Manager for DeepSeek Harness Web. |
| 1420 | [slohmaier/dsh-a11y-announcer](https://github.com/slohmaier/dsh-a11y-announcer) | 0 | 2026-08-21 | 2026-08-25 | Accessibility plugin for DeepSeek Harness web UI: announces tool calls and finished assistant messages via aria-live for screen readers |
| 1421 | [snail-vs/dsh-llm-oauth](https://github.com/snail-vs/dsh-llm-oauth) | 0 | 2026-08-22 | 2026-08-22 | OAuth login plugin for DeepSeek Harness (DSH), enabling subscription LLM accounts such as ChatGPT Plus/Pro to work without API keys. |
| 1422 | [soarGuo/dsh-skin-lab](https://github.com/soarGuo/dsh-skin-lab) | 0 | 2026-08-25 | 2026-08-25 | Skin Lab for the DSH Web GUI: token browser, live try-on, theme freeze, spectrum presets with SVG backdrops, custom backdrop upload. Everything is a plugin. |
| 1423 | [sol5766/dshm](https://github.com/sol5766/dshm) | 0 | 2026-08-20 | 2026-08-22 | deepseek harnes HarmonyOS PC client |
| 1424 | [songying2024/dsh-bookmarks-dock](https://github.com/songying2024/dsh-bookmarks-dock) | 0 | 2026-08-22 | 2026-08-22 | DeepSeek Harness (DSH) left-side bookmark dock plugin |
| 1425 | [soulYANG/dsh-baogongtou](https://github.com/soulYANG/dsh-baogongtou) | 0 | 2026-08-26 | 2026-08-26 | 包工头：DeepSeek Harness 工作 agent 皮肤。能力还是 dsh，嘴和按钮是包工头。 |
| 1426 | [Sparrived/dsh-plugin-workspace-skill](https://github.com/Sparrived/dsh-plugin-workspace-skill) | 0 | 2026-08-22 | 2026-08-22 | DSH Cordis plugin: skill-create authoring guide + workspace-level skill isolation for .dsh/skills |
| 1427 | [SpringNyan/dsh-public-proxy](https://github.com/SpringNyan/dsh-public-proxy) | 0 | 2026-08-22 | 2026-08-24 | A DeepSeek Harness plugin that exposes the DSH Web UI for LAN access |
| 1428 | [sqs404/dsh-client-ui-beautify](https://github.com/sqs404/dsh-client-ui-beautify) | 0 | 2026-08-23 | 2026-08-23 | DeepSeek Harness UI beautify plugin / one-click skin: settings-backed switch, aurora background, glass panels |
| 1429 | [squirrel20/dsh-cron](https://github.com/squirrel20/dsh-cron) | 0 | 2026-08-26 | 2026-08-26 | Unattended scheduled jobs for the DeepSeek Harness (dsh): agent/command tasks on cron schedules |
| 1430 | [squirrelbullet/dsh-client-ui-vibecontroller](https://github.com/squirrelbullet/dsh-client-ui-vibecontroller) | 0 | 2026-08-21 | 2026-08-22 | Floating controller overlay for DeepSeek Harness with voice input and game-like button layout. |
| 1431 | [ssheleg/agent-stack](https://github.com/ssheleg/agent-stack) | 0 | 2026-08-06 | 2026-08-26 | Production patterns for agent systems, in four agent skills: orchestrator loops and memory layers, the harness (system prompts, tool descriptions, technique choice), evals that judge trajectories rather than answers, MCP and A2A interop — plus the wallet under reselling LLM access. Loads in DeepSeek Harness (dsh). |
| 1432 | [ssheleg/sheleg-dev](https://github.com/ssheleg/sheleg-dev) | 0 | 2026-08-06 | 2026-08-26 | Money in, tracking, sign-in, speed — the integration layer a product reaches once it has users. Seven agent skills: Stripe subscription billing reconciled into your own database, crypto payments, GA4/Ads/Meta under Consent Mode v2, Google sign-in, Core Web Vitals, Sentry error tracking. Loads in DeepSeek Harness (dsh). |
| 1433 | [ssheleg/telegram-dev](https://github.com/ssheleg/telegram-dev) | 0 | 2026-08-25 | 2026-08-26 | Telegram development split by the API each surface speaks: the official Bot API for bots, MTProto/Telethon for user accounts, and Mini Apps for the web layer whose whole security model is one signed blob. Three agent skills for Claude Code, Cursor and 70+ agents. Loads in DeepSeek Harness (dsh). |
| 1434 | [sskkde/dsh-oh-my-agent](https://github.com/sskkde/dsh-oh-my-agent) | 0 | 2026-08-25 | 2026-08-25 | oh-my-openagent (OmO) core capabilities ported as a DeepSeek Harness plugin: ultrawork, role delegation, rules engine, boulder memory, hooks, Sisyphus main-prompt discipline |
| 1435 | [StabCut/dsh-plugin-restart-desktop](https://github.com/StabCut/dsh-plugin-restart-desktop) | 0 | 2026-08-21 | 2026-08-24 | DSH Desktop sidebar restart button: orderly relaunch of DSH Desktop from the sidebar settings row (based on desktopActions.requestRestart). |
| 1436 | [STARDUSTLC666/dsh-dream](https://github.com/STARDUSTLC666/dsh-dream) | 0 | 2026-08-26 | 2026-08-26 | DSH 做梦插件：会话回放（梦原料）→ 反思 → 梦境日记（记忆巩固）。多帧 zstd 会话读取，零运行时依赖。Dream plugin for DeepSeek Harness: session replay, reflection, dream journal. |
| 1437 | [starefinger/dsh-llm-qwen-local](https://github.com/starefinger/dsh-llm-qwen-local) | 0 | 2026-08-26 | 2026-08-26 | 面向 DeepSeek Harness(dsh)的 LLM 适配器插件:驱动由 OpenAI 兼容服务的本地部署 Qwen3.8-27B 模型。支持按模型多模态开关、完全可配置的推理档位、请求图像投影,以及中英双语 Web 设置页。 |
| 1438 | [Starlight-bananice/dsh-zhushou](https://github.com/Starlight-bananice/dsh-zhushou) | 0 | 2026-08-24 | 2026-08-25 | DSH 侧边栏助手插件（dsh-zhushou）：在侧边栏管理/选择助手，选中后在 DSH 会话内直接以助手人设对话；不选则保持原生会话。 |
| 1439 | [striveh/dsh-capability-resolver](https://github.com/striveh/dsh-capability-resolver) | 0 | 2026-08-25 | 2026-08-25 | Read-only local capability and community plugin discovery for DeepSeek Harness |
| 1440 | [stultuss/dsh-clear-tool-results](https://github.com/stultuss/dsh-clear-tool-results) | 0 | 2026-08-25 | 2026-08-25 | DSH 宿主插件：每轮对话结束后，把该轮的原始工具结果归档（tool result）到会话目录（tool-result-logs），并从上下文中清除，减少 Token 消耗；模型可用 read_tool_result_log 工具按轮次或时间自主读取归档数据。 |
| 1441 | [suanniniu/dsh-standard-toolkit](https://github.com/suanniniu/dsh-standard-toolkit) | 0 | 2026-08-17 | 2026-08-23 | DeepSeek Harness 标准工具插件(Standard ToolKit):工具管家——平时工具不占位,会话按需自动装载/用完自动收纳,省token;支持 load_tool / register_new_tool 现场造工具。Tool manager plugin for DeepSeek Harness / dsh. |
| 1442 | [SuCriss/dsh-leekbox](https://github.com/SuCriss/dsh-leekbox) | 0 | 2026-08-26 | 2026-08-26 | 韭菜盒子 LeekBox — A股看盘助手 · DeepSeek Harness (DSH) web 插件 |
| 1443 | [SuiBbinggan/dsh-cn-plugin-center](https://github.com/SuiBbinggan/dsh-cn-plugin-center) | 0 | 2026-08-25 | 2026-08-25 | China-friendly plugin center for DeepSeek Harness with curated and verified community plugins. |
| 1444 | [Suixin04/dsh-session-migrator](https://github.com/Suixin04/dsh-session-migrator) | 0 | 2026-08-24 | 2026-08-25 | DeepSeek Harness 可视化跨设备会话迁移插件｜Visual cross-device session migration with drag-and-drop ZIP, JSONL, and folder imports. |
| 1445 | [sujiu0616-art/DSH-CustomWallpapers-Glassmorphism-Theme](https://github.com/sujiu0616-art/DSH-CustomWallpapers-Glassmorphism-Theme) | 0 | 2026-08-21 | 2026-08-22 | dsh可自定义壁纸玻璃风主题 |
| 1446 | [sujiu222/dsh-one-click-archive](https://github.com/sujiu222/dsh-one-click-archive) | 0 | 2026-08-22 | 2026-08-23 | One-click time-based conversation archiving for the DeepSeek Harness Web GUI |
| 1447 | [sunnystarye-ui/dsh-plugin-text-quote](https://github.com/sunnystarye-ui/dsh-plugin-text-quote) | 0 | 2026-08-24 | 2026-08-24 | Codex-style text annotation for DeepSeek Harness conversations / 对话文字批注插件 |
| 1448 | [sunnywangzi/dsh-server-admin](https://github.com/sunnywangzi/dsh-server-admin) | 0 | 2026-08-22 | 2026-08-22 | DSH 服务器管理面板：在线重启/停止、systemd 一键保活、在线安装插件、状态监控、活跃会话、命令终端 \| DSH Server Admin: online restart/stop, systemd keep-alive, plugin install, status monitor, active sessions, command terminal |
| 1449 | [SuperstructureJH/dsh-workbuddy-ppt](https://github.com/SuperstructureJH/dsh-workbuddy-ppt) | 0 | 2026-08-26 | 2026-08-26 | Editable PPTX generation for DSH with bundled authoring skills and deterministic PPTD validation |
| 1450 | [susirial/dsh-traebao](https://github.com/susirial/dsh-traebao) | 0 | 2026-08-23 | 2026-08-23 | Conversation-aware TRAE Bao digital pet for DeepSeek Harness Desktop |
| 1451 | [suyukun/dsh-plugin-publish](https://github.com/suyukun/dsh-plugin-publish) | 0 | 2026-08-26 | 2026-08-26 | Ship your skills, grow your influence — a model-agnostic publishing protocol for AI agent skills: preflight checks, GitHub repo, index PRs, marketplace submissions, promo copy. 把 agent 技能标准化发布到 GitHub 的流程协议。 |
| 1452 | [suyukun/dsh-tech-selection](https://github.com/suyukun/dsh-tech-selection) | 0 | 2026-08-26 | 2026-08-26 | Stop letting your AI guess — a research protocol for tech decisions that any AI agent (DSH/Claude/Cursor/Codex) can follow: quantified requirements, T1-T6 source tiers, quality gates, traceable verdicts. 模型无关的技术选型调研协议。 |
| 1453 | [svcomplex-dev/dsh-svw-waveform](https://github.com/svcomplex-dev/dsh-svw-waveform) | 0 | 2026-08-24 | 2026-08-24 | DeepSeek Harness plugin for viewing and analyzing VCD/FST waveforms with SVW. |
| 1454 | [syncended/deepseek-harness-usage](https://github.com/syncended/deepseek-harness-usage) | 0 | 2026-08-26 | 2026-08-26 | Token usage, model cost analytics, trends, and activity heatmaps for DeepSeek Harness |
| 1455 | [tang-zhilei/dsh-group-chat-view](https://github.com/tang-zhilei/dsh-group-chat-view) | 0 | 2026-08-21 | 2026-08-22 | DSH group chat style conversation view plugin |
| 1456 | [TARS-snail/dsh-notify](https://github.com/TARS-snail/dsh-notify) | 0 | 2026-08-25 | 2026-08-26 | Desktop notifications for DeepSeek Harness sessions, only while you are away |
| 1457 | [tatselkrik/dsh-web-search-ddg](https://github.com/tatselkrik/dsh-web-search-ddg) | 0 | 2026-08-24 | 2026-08-24 | Keyless DuckDuckGo web search provider for DeepSeek Harness (ctx.web seam) — no API keys, no accounts, zero tokens per search. Strict-mode scraping, redirect unwrapping, dedupe, entity-safe parsing, committed builds, one-command profile install. |
| 1458 | [termanli/dsh-fulltext-search](https://github.com/termanli/dsh-fulltext-search) | 0 | 2026-08-24 | 2026-08-24 | A DSH (DeepSeek Harness) Web GUI plugin that searches file contents in the current session working directory from the sidebar file manager (dsh-better-sidebar), returning file + line number + matching line preview. |
| 1459 | [TestTheBoy/dsh_plugin_file_attach](https://github.com/TestTheBoy/dsh_plugin_file_attach) | 0 | 2026-08-26 | 2026-08-26 | Add files to context |
| 1460 | [TheChengXi/dsh-session-sync](https://github.com/TheChengXi/dsh-session-sync) | 0 | 2026-08-25 | 2026-08-25 | 广播会话修改实现多窗口同步  |
| 1461 | [TheHeartFickle/dsh-conversation-folding](https://github.com/TheHeartFickle/dsh-conversation-folding) | 0 | 2026-08-21 | 2026-08-22 | DSH 对话流渲染增强插件 —— 折叠过程，保留正文，长对话更清爽。 |
| 1462 | [TheHeartFickle/dsh-solo-agent](https://github.com/TheHeartFickle/dsh-solo-agent) | 0 | 2026-08-21 | 2026-08-26 | DSH 插件：向用户 agent-presets 注入 `solo` preset,优化上下文占用和模型调度。 |
| 1463 | [thinkingpeach-sketch/wan3-agent-skills](https://github.com/thinkingpeach-sketch/wan3-agent-skills) | 0 | 2026-08-19 | 2026-08-22 | Portable WAN3 image and video generation skills for AI coding agents |
| 1464 | [thomasvvugt/dsh-kanban-flow](https://github.com/thomasvvugt/dsh-kanban-flow) | 0 | 2026-08-25 | 2026-08-25 | Agent-driven kanban board for DeepSeek Harness: one board per workspace, per-task agent sessions, guarded human/agent workflow |
| 1465 | [thomasvvugt/dsh-wide-stats-footer](https://github.com/thomasvvugt/dsh-wide-stats-footer) | 0 | 2026-08-24 | 2026-08-25 | Removes the width clamp on the DeepSeek Harness composer stats footer — long turn/token stats lines span the full composer width instead of truncating |
| 1466 | [Tieboyh/dsh-chat-enhancer](https://github.com/Tieboyh/dsh-chat-enhancer) | 0 | 2026-08-24 | 2026-08-24 | Focused conversation enhancements for DeepSeek Harness Web, starting with zoomable fullscreen Mermaid diagrams. |
| 1467 | [Tieboyh/dsh-notes-markdown](https://github.com/Tieboyh/dsh-notes-markdown) | 0 | 2026-08-24 | 2026-08-24 | Editable Markdown notes in the DeepSeek Harness sidebar |
| 1468 | [Tieboyh/dsh-usage-center](https://github.com/Tieboyh/dsh-usage-center) | 0 | 2026-08-24 | 2026-08-24 | Native DSH settings page for daily provider usage, subscription quotas, balances, and API price estimates. |
| 1469 | [tiger0012/dsh-we-wallpaper-sync](https://github.com/tiger0012/dsh-we-wallpaper-sync) | 0 | 2026-08-26 | 2026-08-26 | Reusable skill: browse/search/download Wallpaper Engine (Steam 431960) workshop wallpapers and wire them into the DSH skin center, bypassing the Steam HTTP block and region-mismatch sign-in block. |
| 1470 | [Tiko9527/dsh-image-tiler](https://github.com/Tiko9527/dsh-image-tiler) | 0 | 2026-08-23 | 2026-08-23 | DSH high-resolution image tiler: slices large images into <=800x800 tiles before sending to DeepSeek. Highly AI-native, only DeepSeek participation. |
| 1471 | [Tiko9527/task-router](https://github.com/Tiko9527/task-router) | 0 | 2026-08-23 | 2026-08-23 | DSH task delegation router plugin: main model plans/verifies, sub-models search/browse/code/verify. Highly AI-native, built with GLM/DeepSeek/Qwen assistance. |
| 1472 | [tkwkeven/dsh-lark](https://github.com/tkwkeven/dsh-lark) | 0 | 2026-08-20 | 2026-08-22 | Feishu/Lark channel for DeepSeek Harness: prefix-created task sessions, thread routing, streaming thinking cards, interactive questions, media delivery, lifecycle notices, runtime policies, web mirror |
| 1473 | [tkwkeven/dsh-sim-restart](https://github.com/tkwkeven/dsh-sim-restart) | 0 | 2026-08-20 | 2026-08-22 | Simulated-restart testing for DeepSeek Harness plugins: verifies plugins survive restart (module eval → apply → smoke → dispose) in isolated subprocesses, with a resident auto-watcher and agent feedback loop |
| 1474 | [tkwkeven/dsh-tool-github](https://github.com/tkwkeven/dsh-tool-github) | 0 | 2026-08-20 | 2026-08-22 | GitHub REST API tools and web GUI panel for DeepSeek Harness: bind account, search code/issues, manage PRs, clone workspaces |
| 1475 | [tkwkeven/dsh-ytdlp](https://github.com/tkwkeven/dsh-ytdlp) | 0 | 2026-08-20 | 2026-08-22 | Video/audio download tools for DeepSeek Harness, powered by yt-dlp (video_info / video_download) |
| 1476 | [todayer/todayer-dsh-telegram-bridge](https://github.com/todayer/todayer-dsh-telegram-bridge) | 0 | 2026-08-24 | 2026-08-26 | DeepSeek Harness Telegram bridge (bot) plugin, Hermes-style: per-topic sessions, DM topics, group gating, media, commands. Fork/extension of hi-wenw/dsh-telegram-channel. |
| 1477 | [Triple3h/dsh-image-read](https://github.com/Triple3h/dsh-image-read) | 0 | 2026-08-19 | 2026-08-23 | DSH native plugin: structured image analysis via multimodal APIs (read_image_mimo tool) with provider failover, caching, SSRF protection and a Web UI config card. DSH 原生插件：多模态识图，返回结构化 JSON 证据，支持故障转移/缓存/SSRF 防护/Web 配置卡片。 |
| 1478 | [Triple3h/dsh-input-enhancement](https://github.com/Triple3h/dsh-input-enhancement) | 0 | 2026-08-20 | 2026-08-23 | DSH Web plugin: input enhancement — paste text collapse, file/folder attachment paste & drag-drop, bubble attachment folding, message fold, attachment management & cleanup. DSH Web 插件：输入增强——粘贴文本折叠、附件上传、消息折叠。 |
| 1479 | [Triple3h/dsh-reasoning-effort](https://github.com/Triple3h/dsh-reasoning-effort) | 0 | 2026-08-19 | 2026-08-23 | DSH Web plugin: per-model reasoning-effort configuration and selection — settings page + slider embedded in the model picker. DSH Web 插件：逐模型推理力度配置与选择（设置页 + 模型选择器内嵌滑块）。 |
| 1480 | [Triple3h/dsh-rxresume](https://github.com/Triple3h/dsh-rxresume) | 0 | 2026-08-23 | 2026-08-23 | DSH plugin that talks to the Reactive Resume REST API directly: create, read, patch, and manage resumes over /api/openapi with an API key. 直接对接 Reactive Resume REST API 管理简历的 DSH 插件。 |
| 1481 | [Triple3h/dsh-session-enhance](https://github.com/Triple3h/dsh-session-enhance) | 0 | 2026-08-19 | 2026-08-23 | DSH Web plugin: session sidebar enhancements — copy session ID from the context menu, etc. DSH Web 插件：会话栏增强（上下文菜单一键复制会话 ID 等）。 |
| 1482 | [Triple3h/dsh-stats-expand](https://github.com/Triple3h/dsh-stats-expand) | 0 | 2026-08-20 | 2026-08-23 | DSH Web client plugin: unwrap the session stats bar to full-width, click to toggle truncation (preference persisted). DSH Web 客户端插件：会话底部统计条解除限宽、单行完整铺满，点击可切回官方截断。 |
| 1483 | [TropicWiden/dsh-history-question-nav](https://github.com/TropicWiden/dsh-history-question-nav) | 0 | 2026-08-25 | 2026-08-25 | A DeepSeek Harness web plugin that lists every question you ask in the current session in a right-side panel, and scrolls to the matching answer when you click one.  DeepSeek Harness Web 插件：在窗口右侧列出当前会话的每个提问，点击即定位到对应回答。 |
| 1484 | [TTsdzb/dsh-global-proxy](https://github.com/TTsdzb/dsh-global-proxy) | 0 | 2026-08-21 | 2026-08-22 | 更好的代理支持。 |
| 1485 | [tuofangzhe/dsh-plugins](https://github.com/tuofangzhe/dsh-plugins) | 0 | 2026-08-24 | 2026-08-24 | Community plugin registry for DeepSeek Harness (DSH) plugins, Skills & MCP — DSH 插件目录与中文安装配置教程 · 52dsh.com |
| 1486 | [TussalZeus18028/dsh-conflict-checker](https://github.com/TussalZeus18028/dsh-conflict-checker) | 0 | 2026-08-26 | 2026-08-26 | Detect DeepSeek Harness plugin conflicts and internal issues; manage plugins (enable/disable/uninstall) from a settings page. |
| 1487 | [uckkk/dsh-fat-loss-cal](https://github.com/uckkk/dsh-fat-loss-cal) | 0 | 2026-08-20 | 2026-08-21 | 减脂热量计算 |
| 1488 | [uckkk/dsh-future-cbdc](https://github.com/uckkk/dsh-future-cbdc) | 0 | 2026-08-21 | 2026-08-21 | 央行数字货币 |
| 1489 | [uckkk/dsh-future-fusion](https://github.com/uckkk/dsh-future-fusion) | 0 | 2026-08-21 | 2026-08-21 | 核聚变能源 |
| 1490 | [uckkk/dsh-future-longevity](https://github.com/uckkk/dsh-future-longevity) | 0 | 2026-08-21 | 2026-08-21 | 长寿医学 |
| 1491 | [uckkk/dsh-gift-etiquette](https://github.com/uckkk/dsh-gift-etiquette) | 0 | 2026-08-21 | 2026-08-21 | 送礼避讳 |
| 1492 | [uckkk/dsh-k2c](https://github.com/uckkk/dsh-k2c) | 0 | 2026-08-21 | 2026-08-21 | 开尔文转摄氏 |
| 1493 | [uckkk/dsh-kenya](https://github.com/uckkk/dsh-kenya) | 0 | 2026-08-21 | 2026-08-21 | 肯尼亚国家 |
| 1494 | [uckkk/dsh-palau](https://github.com/uckkk/dsh-palau) | 0 | 2026-08-21 | 2026-08-21 | 帕劳国 |
| 1495 | [udsy19/dsh-toolcall-stream-repair](https://github.com/udsy19/dsh-toolcall-stream-repair) | 0 | 2026-08-24 | 2026-08-24 | DeepSeek Harness plugin: repairs malformed streaming tool-call deltas before they reach the block assembler |
| 1496 | [Unintendedz/dsh-session-workspace](https://github.com/Unintendedz/dsh-session-workspace) | 0 | 2026-08-23 | 2026-08-24 | Move cold DeepSeek Harness sessions between registered workspaces |
| 1497 | [Unintendedz/dsh-ui-enhancements](https://github.com/Unintendedz/dsh-ui-enhancements) | 0 | 2026-08-23 | 2026-08-23 | Small, focused UI enhancements for DeepSeek Harness |
| 1498 | [Ury479/dsh-wukong-zenfire](https://github.com/Ury479/dsh-wukong-zenfire) | 0 | 2026-08-25 | 2026-08-25 | Wukong Zenfire skin plugin for DeepSeek Harness (DSH) WebUI and Desktop |
| 1499 | [valkia/dsh-plugin-computer-use](https://github.com/valkia/dsh-plugin-computer-use) | 0 | 2026-08-24 | 2026-08-24 | Computer Use plugin for DeepSeek Harness using Open Computer Use MCP |
| 1500 | [valkia/dsh-plugin-git-log](https://github.com/valkia/dsh-plugin-git-log) | 0 | 2026-08-24 | 2026-08-24 | Git Log commit graph and history workbench for DeepSeek Harness |
| 1501 | [veermetri05/dsh-plugins](https://github.com/veermetri05/dsh-plugins) | 0 | 2026-08-25 | 2026-08-25 | Collection of DeepSeek Harness (DSH) plugins — web-search-omp ported from oh-my-pi (23 providers, fallback chain, credential-free) |
| 1502 | [Victor-770/dsh-plugin-directory](https://github.com/Victor-770/dsh-plugin-directory) | 0 | 2026-08-14 | 2026-08-25 | DeepSeek Harness 插件目录：中英双语、按功能分类、README 全文搜索、按热度排序。 |
| 1503 | [vimalinx/Dsh-dev](https://github.com/vimalinx/Dsh-dev) | 0 | 2026-08-22 | 2026-08-22 | Version-aware workspace core for building DeepSeek Harness plugins |
| 1504 | [vinokok/dsh-external-access-guide](https://github.com/vinokok/dsh-external-access-guide) | 0 | 2026-08-24 | 2026-08-24 | 远程 VPS 上部署 DSH 并通过 HTTPS 安全开放外网访问 \| Deploy DSH on a remote VPS and expose it securely over HTTPS |
| 1505 | [vINyLogY/dsh-bluebubbles](https://github.com/vINyLogY/dsh-bluebubbles) | 0 | 2026-08-22 | 2026-08-23 | Who needs openclaw? |
| 1506 | [vladlearns/dsh-fs-deny-policy](https://github.com/vladlearns/dsh-fs-deny-policy) | 0 | 2026-08-24 | 2026-08-25 | DeepSeek Harness plugin: a deployment deny list of filesystem roots the model may never touch |
| 1507 | [vritser/dsh-emacs](https://github.com/vritser/dsh-emacs) | 0 | 2026-08-23 | 2026-08-25 | An Emacs client for DeepSeek Harness |
| 1508 | [wang-junjian/dsh-github-trending](https://github.com/wang-junjian/dsh-github-trending) | 0 | 2026-08-23 | 2026-08-24 | DeepSeek Harness 插件 GitHub Trending |
| 1509 | [wangyong1972/dsh-computer-use-macos](https://github.com/wangyong1972/dsh-computer-use-macos) | 0 | 2026-08-22 | 2026-08-23 | Native macOS computer-use plugin for DeepSeek Harness with trusted mouse/keyboard control, screenshots, and multi-display selection. |
| 1510 | [wangyuanchuan2022/dsh-mobile-ux](https://github.com/wangyuanchuan2022/dsh-mobile-ux) | 0 | 2026-08-25 | 2026-08-25 | 一个包、零配置：把 DeepSeek Harness 网页版在手机宽度下的体验从头打磨一遍——响应式抽屉布局、字号/间距适配、≥44px 触控目标、按钮/菜单/表格移动端交互、安全区适配。桌面宽度显示与使用完全不受影响。 |
| 1511 | [wangzhanchao883/dsh-screenshot-capture](https://github.com/wangzhanchao883/dsh-screenshot-capture) | 0 | 2026-08-24 | 2026-08-24 | Point-and-shoot screenshot capture plugin for DeepSeek Harness: clipboard watcher + system floating window (comment & key-point, copy/save-doc/save-image) + instant OCR (Tongyi Qianwen) + Obsidian per-day merging + evening AI organization. 指哪拍哪 · DSH 截图即存插件:剪贴板监听 + 系统级悬浮窗 + 即时 OCR + Obsidian 按天合并 + 晚间 AI 整理 |
| 1512 | [wantosure/dsh-plugin-browser-memory](https://github.com/wantosure/dsh-plugin-browser-memory) | 0 | 2026-08-26 | 2026-08-26 | Local-first DeepSeek Harness plugin for searching Chrome, Edge, and Brave bookmarks, history, and downloads. |
| 1513 | [WayneYu430/dsh-voice-agent](https://github.com/WayneYu430/dsh-voice-agent) | 0 | 2026-08-24 | 2026-08-25 | a full duplex voice mode for DSH |
| 1514 | [webkubor/dsh-mirror](https://github.com/webkubor/dsh-mirror) | 0 | 2026-08-26 | 2026-08-26 | Let the AI know you. 从 think 链学习你的偏好，让 DSH 越用越懂你 |
| 1515 | [wenhao4126/dsh-herdr](https://github.com/wenhao4126/dsh-herdr) | 0 | 2026-08-26 | 2026-08-26 | Expose Herdr workspaces, panes, and coding agents as DeepSeek Harness tools. |
| 1516 | [wertyBSd/dsh-local-llm](https://github.com/wertyBSd/dsh-local-llm) | 0 | 2026-08-20 | 2026-08-24 | Local LLM integration plugin for DeepSeek Harness |
| 1517 | [wheam/dsh-session-groups](https://github.com/wheam/dsh-session-groups) | 0 | 2026-08-22 | 2026-08-23 | Provider-owned virtual session groups for the DeepSeek Harness Web sidebar. |
| 1518 | [Wilfred-wei/dsh-fingerprint-relay](https://github.com/Wilfred-wei/dsh-fingerprint-relay) | 0 | 2026-08-23 | 2026-08-24 | DSH plugin: managed local fingerprint relays so DSH can reach providers that gate on the client's TLS fingerprint |
| 1519 | [Wilson-Lai-Ab/dsh-idea-style](https://github.com/Wilson-Lai-Ab/dsh-idea-style) | 0 | 2026-08-21 | 2026-08-26 | DSH plugin |
| 1520 | [windrover/dsh-long-term-memory](https://github.com/windrover/dsh-long-term-memory) | 0 | 2026-08-25 | 2026-08-26 | Layered deterministic long-term memory for DeepSeek Harness: CJK-aware BM25 recall, JSONL storage, per-assembly context injection, write guards and threat scanning. |
| 1521 | [wkfedor/deepseek-harness-voice-input](https://github.com/wkfedor/deepseek-harness-voice-input) | 0 | 2026-08-22 | 2026-08-23 | Local voice typing and speech-to-text plugin for DeepSeek Harness (dsh), powered by multilingual Whisper. |
| 1522 | [wly8691-jpg/dsh-office-com](https://github.com/wly8691-jpg/dsh-office-com) | 0 | 2026-08-26 | 2026-08-26 | DSH plugin: COM-driven real Office automation (VBA/pivot/recalc/layout) |
| 1523 | [Wodexinhaoleng-Kasssa/dsh-reader](https://github.com/Wodexinhaoleng-Kasssa/dsh-reader) | 0 | 2026-08-22 | 2026-08-22 | In-browser novel reader for the dsh web GUI: online book-source search, chapter-by-chapter reading in a chat-style view, and whole-book TXT download. |
| 1524 | [wolfsonliu/zotero-skill](https://github.com/wolfsonliu/zotero-skill) | 0 | 2026-08-25 | 2026-08-25 | An agent-usable Zotero skill for AI agent — search, read, and write your local Zotero library through a single Python CLI. \| 面向 AI  Agent 的 Zotero 技能：通过单一 Python CLI 搜索、读取、写入本地 Zotero 文献库。 |
| 1525 | [woshishadowhunter/dsh-seed-society](https://github.com/woshishadowhunter/dsh-seed-society) | 0 | 2026-08-25 | 2026-08-25 | Yogacara eight-consciousness agent society plugin for DeepSeek Harness: mneme memory consolidation tuning, llm-deepseek reasoning fix, MCP society bridge, and six seed skills |
| 1526 | [wpc725562-dotcom/deepfusion](https://github.com/wpc725562-dotcom/deepfusion) | 0 | 2026-08-25 | 2026-08-25 | DeepFusion: DSH x Reasonix 融合 Agent 引擎 (DeepSeek-native 编排 + 前缀缓存优化) |
| 1527 | [writeCasually/dsh-opencode-go-models](https://github.com/writeCasually/dsh-opencode-go-models) | 0 | 2026-08-23 | 2026-08-23 | DSH 插件：自动同步 opencode-go 模型清单到 pi-ai catalog，按官方文档精确标记协议（anthropic-messages / openai-completions / openai-responses）与多模态支持 |
| 1528 | [WSL043/dsh-native-image-viewer](https://github.com/WSL043/dsh-native-image-viewer) | 0 | 2026-08-26 | 2026-08-26 | Native zoom, pan, download, gallery, and region-note image viewer for DeepSeek Harness |
| 1529 | [WSYXIUBA/dsh-plugin-starmap](https://github.com/WSYXIUBA/dsh-plugin-starmap) | 0 | 2026-08-21 | 2026-08-22 | 🪐 DSH 插件星座图 — DeepSeek Harness 插件依赖关系可视化（自动扫描/分类/依赖图） |
| 1530 | [wuruihi/dsh-memory-loader](https://github.com/wuruihi/dsh-memory-loader) | 0 | 2026-08-24 | 2026-08-24 | DSH plugin: deterministic two-level memory injection (global + project MEMORY.md + today's notes) at session start |
| 1531 | [Wuxie233/dsh-plugin-blank-session-gc](https://github.com/Wuxie233/dsh-plugin-blank-session-gc) | 0 | 2026-08-18 | 2026-08-23 | Keep at most one unused blank DSH conversation |
| 1532 | [wuyiwuaa1-ship-it/dsh-read-image-jpeg-fallback](https://github.com/wuyiwuaa1-ship-it/dsh-read-image-jpeg-fallback) | 0 | 2026-08-25 | 2026-08-26 | DSH plugin that converts read_image PNG/WebP attachments to JPEG for LM Studio compatibility. |
| 1533 | [wwskills/dsh-long-memory](https://github.com/wwskills/dsh-long-memory) | 0 | 2026-08-25 | 2026-08-25 | Long-term cross-session memory plugin for DeepSeek Harness |
| 1534 | [wwwwwald/dsh-story](https://github.com/wwwwwald/dsh-story) | 0 | 2026-08-21 | 2026-08-23 | One prompt to cinematic story. AI-powered script-to-video pipeline for DeepSeek Harness. |
| 1535 | [xain/ui-beep](https://github.com/xain/ui-beep) | 0 | 2026-08-26 | 2026-08-26 | **dsh-beep** — an agent-heartbeat sonification plugin for the DeepSeek Harness Web surface. |
| 1536 | [xhqm-xyz/mira_live2d](https://github.com/xhqm-xyz/mira_live2d) | 0 | 2026-08-22 | 2026-08-23 | DSH Live2D 看板娘插件：会话界面浮层（拖拽/滚轮缩放/右键表情菜单）+ 模型可说话（OpenAI/阿里 TTS）+ MCP 工具（状态/切模型/表情动画开关/思考等待表情） |
| 1537 | [xiaobaiyg09/dsh-pickdom](https://github.com/xiaobaiyg09/dsh-pickdom) | 0 | 2026-08-23 | 2026-08-23 | PickDOM - 在 DSH 中框选本地 HTML 与 Web 页面元素，并将结构化引用交给 Agent |
| 1538 | [XIAOke8698/dsh-lego-plugin](https://github.com/XIAOke8698/dsh-lego-plugin) | 0 | 2026-08-23 | 2026-08-24 | DeepSeek Harness（DSH）Web 界面插件的乐高式可视化视图 |
| 1539 | [XiaoWind/dsh-btw](https://github.com/XiaoWind/dsh-btw) | 0 | 2026-08-26 | 2026-08-26 | DeepSeek Harness plugin: a /btw slash command to add notes without interrupting the agent |
| 1540 | [XiaoWind/dsh-vault](https://github.com/XiaoWind/dsh-vault) | 0 | 2026-08-26 | 2026-08-26 | DeepSeek Harness plugin: portable workspace vault for DSH conversations and logs |
| 1541 | [XiaoWind/dsh-weneedfirst](https://github.com/XiaoWind/dsh-weneedfirst) | 0 | 2026-08-21 | 2026-08-22 | DeepSeek Harness plugin: make the chain of thought open with We need instead of Let me |
| 1542 | [xiaoyaoPanPan/dsh-media](https://github.com/xiaoyaoPanPan/dsh-media) | 0 | 2026-08-24 | 2026-08-24 | DeepSeek Harness (dsh) 插件：把挂载目录变成可检索的媒体库 - 视频/图片自动打标、语义检索、系统打开与资源管理器定位 |
| 1543 | [xiaozhiaixue/dsh-model-toggle](https://github.com/xiaozhiaixue/dsh-model-toggle) | 0 | 2026-08-15 | 2026-08-22 | 在DSH中一键切换Flash/Pro，都是MAX |
| 1544 | [xiaozhiaixue/dsh-session-id](https://github.com/xiaozhiaixue/dsh-session-id) | 0 | 2026-08-17 | 2026-08-22 | 在DSH会话区底部显示会话ID，点击一下就能复制 |
| 1545 | [xiaxi626/dsh-skills-nexus](https://github.com/xiaxi626/dsh-skills-nexus) | 0 | 2026-08-22 | 2026-08-22 | 通用 DSH skill 枢纽。安装一次，即可把任意含 SKILL.md 的 GitHub 仓库注册为 DSH skill——一条命令添加一个。skill 仓库无需 Cordis 插件代码或 package.json。Universal DSH skill adapter. Install once, then register any GitHub repo containing a SKILL.md as a DSH skill — one command per repo. No Cordis plugin code or package.json needed in the skill repo. |
| 1546 | [xie-tj/dsh-subagent](https://github.com/xie-tj/dsh-subagent) | 0 | 2026-08-24 | 2026-08-24 | Named subagent profiles with configurable model routing and reasoning for DeepSeek Harness |
| 1547 | [XingPeng-Pixel/dsh-commandcode-usage](https://github.com/XingPeng-Pixel/dsh-commandcode-usage) | 0 | 2026-08-24 | 2026-08-25 | DSH插件：实时监测Command Code用量，侧边栏挂件+仪表盘迷你挂件显示 |
| 1548 | [xinvxueyuan/cordis-plugin-github](https://github.com/xinvxueyuan/cordis-plugin-github) | 0 | 2026-08-17 | 2026-08-23 | Cordis / DeepSeek Harness plugin — normalized GitHub API tools for AI agents (gh CLI by default, native HTTP fallback) |
| 1549 | [xiong18166089606-design/dsh-trade-assistant](https://github.com/xiong18166089606-design/dsh-trade-assistant) | 0 | 2026-08-24 | 2026-08-24 | 外贸询盘回复与多语言产品文案工具（DeepSeek Harness 插件）- 询盘解析、回复结构、本地化文案，零模型依赖 |
| 1550 | [xiuyuan18/dsh-auto-approve](https://github.com/xiuyuan18/dsh-auto-approve) | 0 | 2026-08-25 | 2026-08-25 | Unofficial community plugin: automatic review of sandbox escalation requests for DeepSeek Harness (Codex Guardian-style) plus an /approve slash command |
| 1551 | [xiyi123465/dsh-usage-calendar](https://github.com/xiyi123465/dsh-usage-calendar) | 0 | 2026-08-25 | 2026-08-26 | DeepSeekAPI余额查询插件 |
| 1552 | [xobexo/dsh-auto-model-switcher](https://github.com/xobexo/dsh-auto-model-switcher) | 0 | 2026-08-26 | 2026-08-26 | 国产模型优先，按任务类型自动切换模型，支持可视化配置面板 |
| 1553 | [xtd1145/dsh-full-access-switch](https://github.com/xtd1145/dsh-full-access-switch) | 0 | 2026-08-23 | 2026-08-24 | DSH one-time Full access switch: no per-session confirmation for new workspaces/conversations |
| 1554 | [xuqingsakura/dsh-subagent-team](https://github.com/xuqingsakura/dsh-subagent-team) | 0 | 2026-08-22 | 2026-08-22 | 一个官方 bundle 形态的独立插件，可经 GitHub / npm 安装到 DSH（桌面端与 web 端皆可）。 提供模型可见的角色工具（team_read / team_write / team_code_write / team_code_review …）， 以及一套真正的事件驱动团队运行时（建队 / 成员 / 任务依赖 / 邮箱 / 自动调度 / 右下角活动浮层）。 |
| 1555 | [xusuyang030218/dsh-preview-ui](https://github.com/xusuyang030218/dsh-preview-ui) | 0 | 2026-08-24 | 2026-08-24 | DSH (DeepSeek Harness) file preview & editor plugin: in-browser workspace file tree, multi-format preview, online editing, version history, search. DSH 文件预览插件。 |
| 1556 | [xuviga/dsh-plugin-mnemosyne](https://github.com/xuviga/dsh-plugin-mnemosyne) | 0 | 2026-08-25 | 2026-08-26 | Mnemosyne - an error-memory plugin for DeepSeek Harness that learns from the agent's own mistakes and blocks recurring ones |
| 1557 | [xyzs996/dsh-switch-cost](https://github.com/xyzs996/dsh-switch-cost) | 0 | 2026-08-24 | 2026-08-25 | DeepSeek Harness (dsh) plugin to compare LLM API cost across models and providers: prices the current session on the model that ran it, then reprices the same token counts against 15 routes on file. DeepSeek peak/off-peak resolved per UTC hour, cache read and write priced separately, every rate with its source and check date. |
| 1558 | [y2zyyr/dsh-restart-control](https://github.com/y2zyyr/dsh-restart-control) | 0 | 2026-08-18 | 2026-08-23 | @y2zyyr/dsh-restart-button — one-click Restart DSH button in Settings → General (DSH Desktop), using the official desktopRuntime.requestRestart() facade. |
| 1559 | [Ya-MiC/hermes](https://github.com/Ya-MiC/hermes) | 0 | 2026-08-23 | 2026-08-23 | Ya-MiC GitHub 全景索引 / Curated index of Ya-MiC's repos & stars — DeepSeek Harness (DSH) compliant, multilingual, multi-branch |
| 1560 | [Ya-MiC/zhanzhen](https://github.com/Ya-MiC/zhanzhen) | 0 | 2026-08-24 | 2026-08-26 | 湛箴 — 中小企业审计风险平台 v1 框架（FastAPI + Vue3，规则引擎本地运行，证据哈希链） |
| 1561 | [yangbobo2021/relay-dsh-plugin-files](https://github.com/yangbobo2021/relay-dsh-plugin-files) | 0 | 2026-08-24 | 2026-08-26 | Workspace file explorer side-view plugin for DeepSeek Harness Workbench. |
| 1562 | [yangbobo2021/relay-dsh-plugin-manager](https://github.com/yangbobo2021/relay-dsh-plugin-manager) | 0 | 2026-08-26 | 2026-08-26 | A standalone plugin manager for DeepSeek Harness. |
| 1563 | [yangbobo2021/relay-dsh-plugin-terminal](https://github.com/yangbobo2021/relay-dsh-plugin-terminal) | 0 | 2026-08-24 | 2026-08-26 | Provider-neutral interactive terminal bottom-view plugin for DeepSeek Harness Workbench. |
| 1564 | [yangbobo2021/relay-dsh-plugin-workbench](https://github.com/yangbobo2021/relay-dsh-plugin-workbench) | 0 | 2026-08-24 | 2026-08-26 | Extensible Workbench shell plugin for DeepSeek Harness with public side and bottom view contracts. |
| 1565 | [yangdongzhen590/dsh-knj-menu](https://github.com/yangdongzhen590/dsh-knj-menu) | 0 | 2026-08-23 | 2026-08-24 | Third-party menu manager for DeepSeek Harness: collects plugin menu entries with fold/collapse and pinned items. |
| 1566 | [yangkunlun/dsh-fairy](https://github.com/yangkunlun/dsh-fairy) | 0 | 2026-08-22 | 2026-08-22 | DeepSeek Harness 的多窗插件 |
| 1567 | [yankihue/deepseek-harness-voice-mode](https://github.com/yankihue/deepseek-harness-voice-mode) | 0 | 2026-08-23 | 2026-08-25 | Voice mode for DeepSeek Harness: live captions, push-to-talk, spoken agent replies, barge-in, and real thread control via ElevenLabs. |
| 1568 | [yaodongH/dsh-doc-review](https://github.com/yaodongH/dsh-doc-review) | 0 | 2026-08-23 | 2026-08-23 | dsh-doc-review — DeepSeek Harness Web 文档审阅弹窗插件：设计文档与方案审阅以全幅渲染 Markdown 弹窗呈现 (Design documents & plan reviews in a full rendered-Markdown modal) |
| 1569 | [yaopushen/dsh-plugin-background-tasks](https://github.com/yaopushen/dsh-plugin-background-tasks) | 0 | 2026-08-23 | 2026-08-24 | Antigravity-style run_command for DeepSeek Harness: 10s sync window, auto background promotion, completion reports |
| 1570 | [Yaya716/dsh-add-image-button](https://github.com/Yaya716/dsh-add-image-button) | 0 | 2026-08-23 | 2026-08-23 | Persistent "Add image" button in the composer tool row for DeepSeek Harness Web: opens the system file picker (image/*, multi-select) and routes selected images through the official draft attachment pipeline. |
| 1571 | [Yaya716/dsh-msg-nav-track](https://github.com/Yaya716/dsh-msg-nav-track) | 0 | 2026-08-25 | 2026-08-25 | Conversation message navigation rail for DeepSeek Harness Web: a track on the right side of the session scroll area with ▲/▼ endpoints and evenly spaced dots for user messages; click a dot to jump exactly to that message. |
| 1572 | [Ycet/dsh-session-plus](https://github.com/Ycet/dsh-session-plus) | 0 | 2026-08-24 | 2026-08-25 | DSH 会话增强插件：一键打开工作区 · 模型提供商菜单头部 · 选中文本加入对话 / DSH session enhancement plugin: open workspace · provider header · add selected text to conversation |
| 1573 | [ydlstartx/dsh-pdf-reader](https://github.com/ydlstartx/dsh-pdf-reader) | 0 | 2026-08-22 | 2026-08-23 | AI-powered PDF reader for DeepSeek Harness with annotations, multi-PDF workflows, mixed image-text evidence, and on-demand OCR. |
| 1574 | [yejiming/dsh-ppt](https://github.com/yejiming/dsh-ppt) | 0 | 2026-08-25 | 2026-08-26 | PPT design preset and editable PPTX production tools for DeepSeek Harness |
| 1575 | [Yicijiuhaobala/dsh-session-delete](https://github.com/Yicijiuhaobala/dsh-session-delete) | 0 | 2026-08-24 | 2026-08-24 | Adds a "Delete session" item to the DSH session-row context menu (next to rename/fork/archive) — permanently removes session logs from disk, with live-session protection. |
| 1576 | [Yiklek/dsh-settings-manager](https://github.com/Yiklek/dsh-settings-manager) | 0 | 2026-08-23 | 2026-08-24 | DSH web plugin: manage how plugin sections appear in the global Settings dialog — show/hide, reorder, rename, and make the settings navigation scrollable — without touching upstream. |
| 1577 | [YiyuZh/dsh-skillflux](https://github.com/YiyuZh/dsh-skillflux) | 0 | 2026-08-21 | 2026-08-22 | DeepSeek Harness 动态 Skill 运行时管理器，自动发现、路由、挂载和卸载 Agent Skills |
| 1578 | [ylxmf2005/dsh-openai-server-compaction](https://github.com/ylxmf2005/dsh-openai-server-compaction) | 0 | 2026-08-21 | 2026-08-22 | OpenAI Responses adapter with durable server-side compaction for DeepSeek Harness. |
| 1579 | [ylxmf2005/dsh-scheduled](https://github.com/ylxmf2005/dsh-scheduled) | 0 | 2026-08-23 | 2026-08-23 | Durable heartbeat and cron automations for DeepSeek Harness |
| 1580 | [yogeek/dsh-plugin-toggle](https://github.com/yogeek/dsh-plugin-toggle) | 0 | 2026-08-25 | 2026-08-26 | Enable/disable DeepSeek Harness (dsh) plugins from Settings > Plugins, grouped into collapsible categories |
| 1581 | [yongshuai0314/dsh-i-have-adhd](https://github.com/yongshuai0314/dsh-i-have-adhd) | 0 | 2026-08-26 | 2026-08-26 | ADHD-friendly output shaping for DeepSeek Harness: one system-prompt section with adhd_on/adhd_off/adhd_status tools, persisted across restarts. Inspired by ayghri/i-have-adhd (MIT). |
| 1582 | [yoshino-xiao7/dsh-grok-provider](https://github.com/yoshino-xiao7/dsh-grok-provider) | 0 | 2026-08-26 | 2026-08-26 | DeepSeek Harness 的社区 Grok Build Provider：官方 CLI 浏览器 OAuth、动态模型、流式工具调用与额度面板。Community Grok Build provider with official CLI OAuth, dynamic models, streaming tools, and a quota dashboard. |
| 1583 | [YpipaQ/dsh-whale-usage](https://github.com/YpipaQ/dsh-whale-usage) | 0 | 2026-08-23 | 2026-08-23 | dsh-whale-usage: a self-contained DeepSeek Harness (DSH) plugin that bridges the whale-widget and usage-stats plugins (balance widget + accounting/real-time-token/app-usage settings). Personal localization bridge, MIT. |
| 1584 | [yth1120/dsh-web-workbench](https://github.com/yth1120/dsh-web-workbench) | 0 | 2026-08-23 | 2026-08-23 | Public mirror for the dsh-external/dsh-web-workbench plugin suite; canonical organization repository is private by org policy. |
| 1585 | [YUANMINGXUE/dsh-search](https://github.com/YUANMINGXUE/dsh-search) | 0 | 2026-08-26 | 2026-08-26 | Local-browser web search & page fetch plugin for DeepSeek Harness (dsh): browser_search / browser_fetch over Chrome DevTools Protocol, no API key. |
| 1586 | [YuemingHub/Ming-Capability-Pack](https://github.com/YuemingHub/Ming-Capability-Pack) | 0 | 2026-08-21 | 2026-08-22 | 依托于deepseek harness  做真有用的插件 |
| 1587 | [yul761/dsh-blackjack](https://github.com/yul761/dsh-blackjack) | 0 | 2026-08-20 | 2026-08-25 | Third-party community perk game: play blackjack inside dsh and win model credit spendable only through this plugin. Not affiliated with any model vendor. \| 社区第三方福利小游戏：在 dsh 里玩 21 点，赢取仅限本插件内消费的模型额度。与任何模型厂商无关。 |
| 1588 | [yumm007/dsh-reveal-files](https://github.com/yumm007/dsh-reveal-files) | 0 | 2026-08-23 | 2026-08-24 | A dual-face DeepSeek Harness plugin that adds a folder icon next to the "Produces" row |
| 1589 | [yummy4727/dsh-context-branch](https://github.com/yummy4727/dsh-context-branch) | 0 | 2026-08-21 | 2026-08-22 | Context-branching conversation tree plugin for DeepSeek Harness. Avoid cold-start waste and show full tool/reasoning steps. |
| 1590 | [YupegLV/dsh-chat-log](https://github.com/YupegLV/dsh-chat-log) | 0 | 2026-08-25 | 2026-08-25 | Fold DSH session logs into clean chat logs: stream fragments merged, nothing else dropped. /chat + browser download.  把 DSH 会话日志折叠成聊天记录：流式碎片合并，其余内容一行不丢。/chat 命令 + 浏览器下载。 |
| 1591 | [yustillrain/dsh-plugin-tool-repository](https://github.com/yustillrain/dsh-plugin-tool-repository) | 0 | 2026-08-26 | 2026-08-26 | DSH 插件仓库 第三方插件 让你可视化管理已安装的 skill/插件 对skill/插件功能进行介绍和分类  |
| 1592 | [YuYangOUC/dsh-power-button](https://github.com/YuYangOUC/dsh-power-button) | 0 | 2026-08-24 | 2026-08-24 | Self-contained power control for DeepSeek Harness: sidebar power button, restart/shutdown engine. |
| 1593 | [YYfather/dsh-balance](https://github.com/YYfather/dsh-balance) | 0 | 2026-08-23 | 2026-08-24 | DeepSeek Harness 余额与开销插件：状态栏显示 DeepSeek/MiMo 余额与逐请求计费开销（本会话/本次活跃/最近一次/上次对话），支持多模型+峰谷定价与花费超线提醒 |
| 1594 | [YYfather/dsh-mimo-plugin](https://github.com/YYfather/dsh-mimo-plugin) | 0 | 2026-08-23 | 2026-08-24 | MiMo (Xiaomi) tools as a standard DeepSeek Harness Cordis dynamic plugin: web search, image/audio/video understanding, ASR transcription, TTS, voice design and voice cloning, with a first-use API key setup card and Settings page. |
| 1595 | [YYfather/dsh-token-vault](https://github.com/YYfather/dsh-token-vault) | 0 | 2026-08-23 | 2026-08-24 | Secure credential vault for DeepSeek Harness: tokens never leave the host — the agent runs gh/npm/npx/node/git with the token injected in the environment. Manage from 设置 → 凭证库 / 市场 → 已安装. |
| 1596 | [YZDame/dsh-suhuang-scroll](https://github.com/YZDame/dsh-suhuang-scroll) | 0 | 2026-08-25 | 2026-08-25 | DSH Web plugin for Suhuang Scroll grading controls in Better Sidebar |
| 1597 | [yzhangjy/dsh-path-anonymizer](https://github.com/yzhangjy/dsh-path-anonymizer) | 0 | 2026-08-23 | 2026-08-24 | DSH plugin: anonymize workspace-external file paths before model requests, with user confirmation |
| 1598 | [yzhangjy/dsh-pattern-search](https://github.com/yzhangjy/dsh-pattern-search) | 0 | 2026-08-23 | 2026-08-24 | DSH plugin: regex pattern search over the current conversation — /pattern-search window + pattern_search tool to observe model output behavior |
| 1599 | [zaalipro/dsh-workflows](https://github.com/zaalipro/dsh-workflows) | 0 | 2026-08-20 | 2026-08-23 | DeepSeek workflows exactly like grok build CLI. Adds /create-workflow and /workflows slash commands to DeepSeek harness |
| 1600 | [zbc0315/dsh-synomega](https://github.com/zbc0315/dsh-synomega) | 0 | 2026-08-25 | 2026-08-25 | Organic reaction prediction for DeepSeek Harness: retrosynthesis, forward prediction, route planning, SynScore, and multi-component evolution — with in-chat molecule, reaction, and route-tree visualisation. Runs entirely locally. |
| 1601 | [zdjmrq/dsh-chat-mode](https://github.com/zdjmrq/dsh-chat-mode) | 0 | 2026-08-26 | 2026-08-26 | DSH 插件：为 DeepSeek Harness 增加「对话」纯聊天模式（ChatGPT 式）——侧边栏新会话模式切换（DSH/对话）、对话会话仅提问+搜索工具、专属 \/chat 聊天工作区 |
| 1602 | [zengfr/AutoCoding](https://github.com/zengfr/AutoCoding) | 0 | 2026-08-21 | 2026-08-22 | AutoCoding UltraVibe — 无人值守自动化编程工程化 |
| 1603 | [zenvertao/dsh-inline-comments](https://github.com/zenvertao/dsh-inline-comments) | 0 | 2026-08-26 | 2026-08-26 | 选中即批注，刷新亦留存 —— DSH 行内批注插件 |
| 1604 | [zeros335882878/dsh-paper-survey](https://github.com/zeros335882878/dsh-paper-survey) | 0 | 2026-08-25 | 2026-08-25 | Literature survey agent for DeepSeek Harness (dsh): interpret-first workflow, 3 skills (paper-survey / paper-interpret / paper-deck), zero-dependency. 文献综述 Agent：解读先行 → 用户确认 → A/B 两页结构生成综述 PPT。 |
| 1605 | [zeroUsr0721/dsh-web-polysearch](https://github.com/zeroUsr0721/dsh-web-polysearch) | 0 | 2026-08-25 | 2026-08-26 | Multi-source web search tool for DeepSeek Harness — queries DeepSeek / DuckDuckGo / Exa / Google / Bing in parallel, merges results, fetches page content. Part of the [dsh-plugin](https://github.com/topics/dsh-plugin) ecosystem. |
| 1606 | [zhengjy01/dsh-task-dispatcher](https://github.com/zhengjy01/dsh-task-dispatcher) | 0 | 2026-08-25 | 2026-08-26 | Task dispatcher for DeepSeek Harness: use TickTick (滴答清单) 5️⃣AI as daily task dispatcher (timer + auto-execute + flomo/macOS notify) |
| 1607 | [zhou1736948757-cpu/dsh-auto-continue](https://github.com/zhou1736948757-cpu/dsh-auto-continue) | 0 | 2026-08-25 | 2026-08-25 | Automatically resumes replies cut off at the output token limit — built for self-hosted Ollama users with small output caps. · 回答被输出上限截断时自动续写，面向自部署 Ollama 用户。 |
| 1608 | [zhouStar7/dsh-kanban](https://github.com/zhouStar7/dsh-kanban) | 0 | 2026-08-25 | 2026-08-25 | AI-assisted local project task board for DeepSeek Harness (DSH) |
| 1609 | [zhubaodian1027/dsh-token-panel](https://github.com/zhubaodian1027/dsh-token-panel) | 0 | 2026-08-22 | 2026-08-22 | DSH Web GUI panel: AI quota (Kimi Coding, Codex Plus, DeepSeek…) + merged local token usage (DSH, Codex, Claude Code, Kimi Code, Hermes, Pi…). |
| 1610 | [zhulianxing/dsh-clawpay](https://github.com/zhulianxing/dsh-clawpay) | 0 | 2026-08-24 | 2026-08-24 | DeepSeek Harness (DSH) plugin |
| 1611 | [zhulianxing/dsh-kankan-mail](https://github.com/zhulianxing/dsh-kankan-mail) | 0 | 2026-08-24 | 2026-08-24 | DeepSeek Harness (DSH) plugin |
| 1612 | [zhulianxing/dsh-lookhere](https://github.com/zhulianxing/dsh-lookhere) | 0 | 2026-08-24 | 2026-08-24 | DeepSeek Harness (DSH) plugin |
| 1613 | [zhulianxing/dsh-starstack](https://github.com/zhulianxing/dsh-starstack) | 0 | 2026-08-24 | 2026-08-24 | DeepSeek Harness (DSH) plugin |
| 1614 | [ZhuoSir/dsh-chatops](https://github.com/ZhuoSir/dsh-chatops) | 0 | 2026-08-25 | 2026-08-25 | dsh-chatops 是 DeepSeek Harness 的 IM 桥接插件：微信扫码绑定官方 ClawBot 机器人（腾讯 iLink 协议），或接入飞书自建应用，即可在手机 IM 里列出/切换/驱动所有 DSH 会话——发文字就是发 prompt，任务完成自动推送结果，危险操作推送审批（飞书支持卡片按钮一键批准）。多通道并行、纯官方接口、零公网部署 |
| 1615 | [ziduup/dsh-programming-mode](https://github.com/ziduup/dsh-programming-mode) | 0 | 2026-08-24 | 2026-08-24 | DeepSeek Harness 编程模式组合包：标准模式之上强制执行 Superpowers 工程纪律(TDD、系统化调试、先计划后编码、完成前验证、代码审查)，内置全套 superpowers 技能，dsh plugin add 一键安装。 |
| 1616 | [ZiFan1117/bazidiy](https://github.com/ZiFan1117/bazidiy) | 0 | 2026-08-26 | 2026-08-26 | 基于 DeepSeek Harness 的八字五行手串定制插件 |
| 1617 | [zjuhbh/dsh-full-with-approval](https://github.com/zjuhbh/dsh-full-with-approval) | 0 | 2026-08-22 | 2026-08-23 | DSH profile plugin: full-access (GPU-capable) sandbox with per-operation approval for writes outside the workspace or to protected files. |
| 1618 | [Zn-Dk/dsh-mnemon-gc](https://github.com/Zn-Dk/dsh-mnemon-gc) | 0 | 2026-08-22 | 2026-08-23 | 接入 dsh-mnemon GC 治理插件：冲突驱动的正确性纠错，自动巡检报告。 |
| 1619 | [Zn-Dk/dsh-plugin-creator](https://github.com/Zn-Dk/dsh-plugin-creator) | 0 | 2026-08-21 | 2026-08-25 | Agent skill: scaffold and iterate DSH (DeepSeek Harness) out-of-tree Web plugins. |
| 1620 | [Zn-Dk/dsh-session-explorer](https://github.com/Zn-Dk/dsh-session-explorer) | 0 | 2026-08-24 | 2026-08-25 | DSH Web out-of-tree plugin: message-level full-text search + timeline visualization for sessions. |
| 1621 | [ZomiCC/ghost-refresh](https://github.com/ZomiCC/ghost-refresh) | 0 | 2026-08-25 | 2026-08-25 | Ghost Refresh (鬼影提神) |
| 1622 | [zootguru/dsh-vpn-ops](https://github.com/zootguru/dsh-vpn-ops) | 0 | 2026-08-22 | 2026-08-22 | Safety-gated WireGuard and VLESS Reality operations for DeepSeek Harness |
| 1623 | [zouyuanqing/dsh-verify-reflux](https://github.com/zouyuanqing/dsh-verify-reflux) | 0 | 2026-08-25 | 2026-08-25 | Three-plane probabilistic verifier for DeepSeek Harness: tiered logprob/sample/template judges, seeded tournament best-of-N, layered context reflux. |
| 1624 | [ZPA76/deepseek-pa-dsh-desktop](https://github.com/ZPA76/deepseek-pa-dsh-desktop) | 0 | 2026-08-26 | 2026-08-26 | DeepSeek-PA（DPA）是基于 DeepSeek Harness（DSH）构建的非官方模块化桌面工作台，提供独立的 Chat 与 Agent 空间、插件与 Skill 扩展、全局主题，以及可监督的多智能体集群项目。Unofficial modular desktop workspace for DeepSeek Harness (DSH), featuring separate Chat and Agent views, plugins, Skills, global themes, and supervised multi-agent projects. |
| 1625 | [zptalk0221-cpu/dsh-remote-desktop](https://github.com/zptalk0221-cpu/dsh-remote-desktop) | 0 | 2026-08-26 | 2026-08-26 | 远程桌面移动化插件：为 DeepSeek Harness 提供手机横屏外壳与中文输入法 |
| 1626 | [zsagi1368/dsh-webstack](https://github.com/zsagi1368/dsh-webstack) | 0 | 2026-08-23 | 2026-08-24 | WebStack (网栈) — integrated web search & fetch kernel plugin for DeepSeek Harness (DSH). 免费池开箱即搜 · SSRF 四道闸 · 双语诊断 |
| 1627 | [ztting01/dsh-agentenv-sandbox](https://github.com/ztting01/dsh-agentenv-sandbox) | 0 | 2026-08-24 | 2026-08-25 | AgentENV/E2B microVM execution-world bundle for DeepSeek Harness |
| 1628 | [ZutoMayoo/totoTheCat](https://github.com/ZutoMayoo/totoTheCat) | 0 | 2026-08-20 | 2026-08-22 | 在你的DeepSeek Harness中加入桌宠小猫托托的插件 |
| 1629 | [Zzc269/dsh-soft-glass-ui](https://github.com/Zzc269/dsh-soft-glass-ui) | 0 | 2026-08-16 | 2026-08-22 | Unofficial soft-glass visual theme plugin for DeepSeek Harness. |

## 从快照消失的已核准仓库 / Approved repositories missing from the snapshot

已核准但已不在当前快照中（删除或改名），核实后从 [data/approved.json](../approved.json) 移除或更新名称。

Approved but no longer present in the current snapshot (deleted or renamed) — after checking, remove them from [data/approved.json](../approved.json) or update the name.

- 0Ra1n416/DSH-GUI
- 222wcnm/dsh-manager
- 3yi2u34yu32/dsh-balance-peak
- 911218sky/dsh-llm-bounded-retry
- 918154429/dsh-codex-import
- AI-Scarlett/dsh-safe-plugin-manager
- AwesomeHou/dsh-trajectory-collapse
- Badegg404/dsh-code-review
- Baisbt/dsh-api-balance
- bitterSmilezzz/dsh-model-fix
- CarlMarkswx/dsh-imagen
- cdxDNRF/wishadel-theme
- Chillizu/MiopIIk
- dabaicai001/star-deepseek-harness-desktop
- daha1216/dsh-skill-adult-tension-narrative
- Daseanle/dsh-mcp-orchestrator
- Daseanle/dsh-obsidian-bridge
- Daseanle/dsh-teacher-preset
- ddtcorex/agent-dev-skills
- Deklan-Deng/Dcode
- drscrewdriver/dsh-switch-search
- dsh-external/chat-width
- dsh-external/dsh-agent-teams
- dsh-external/dsh-at-file
- dsh-external/dsh-automation
- dsh-external/dsh-bash-encoding
- dsh-external/dsh-better-browser
- dsh-external/dsh-book2skill
- dsh-external/dsh-computer-use
- dsh-external/dsh-custom-tool
- dsh-external/dsh-cyber-sec
- dsh-external/dsh-daily-fortune
- dsh-external/dsh-deepcel
- dsh-external/dsh-deeplink
- dsh-external/dsh-doctor
- dsh-external/dsh-easy-ctx-manager
- dsh-external/dsh-fun-ticker
- dsh-external/dsh-fun-typewriter
- dsh-external/dsh-fun-weather
- dsh-external/dsh-genui
- dsh-external/dsh-grok-tui
- dsh-external/dsh-handoff
- dsh-external/dsh-input-history
- dsh-external/dsh-island
- dsh-external/dsh-minigames
- dsh-external/dsh-my-rsi
- dsh-external/dsh-notification
- dsh-external/dsh-nowledge-mem
- dsh-external/dsh-open-in-vscode
- dsh-external/dsh-openmaic
- dsh-external/dsh-paste-input
- dsh-external/dsh-pet
- dsh-external/dsh-pet-corner
- dsh-external/dsh-pi-adapter
- dsh-external/dsh-plan-execute
- dsh-external/dsh-plannotator
- dsh-external/dsh-plugin-guide
- dsh-external/dsh-qq2006
- dsh-external/dsh-revive
- dsh-external/dsh-session-hub
- dsh-external/dsh-spotlight
- dsh-external/dsh-STAGE
- dsh-external/dsh-STAR
- dsh-external/dsh-tps
- dsh-external/dsh-turn-rewind
- dsh-external/dsh-ui-progress
- dsh-external/dsh-ui-whale
- dsh-external/dsh-vision-toolkit
- dsh-external/dsh-visualize
- dsh-external/dsh-webui-live-html
- dsh-external/oh-my-dsh
- EIGHTfs/dsh-bili-publisher
- EIGHTfs/dsh-git-push
- EIGHTfs/dsh-image-preview
- EIGHTfs/dsh-session-group
- EIGHTfs/dsh-session-manager
- EIGHTfs/dsh-task-completion
- EIGHTfs/dsh-test-env-entry
- EIGHTfs/dsh-test-sync-plugin
- ExploringBB/dsh-edit-regenerate
- ExploringBB/dsh-plugin-restart-desktop
- Francis-Xavier-code/dsh-balance-plugin
- fryghost/deepseek-eyes
- ggggggggggz/dsh-config
- GooDAnDReaDY/dsh-fal-image-gen
- GuoxinShan/dsh-yzj
- gushiaoke/dsh-qq-bot
- he110Warudo/dsh-window
- Hed1an/dsh-bring-local-llm
- Howe829/dsh-runtime
- htq20080119/dsh-token-stats
- JIAQI23333/dsh-visual-plan
- JimchengChina/dsh-action-outbox
- JimchengChina/dsh-frontier-repro
- joshryandavis/dsh-llm-kiro
- JxaMe/dsh-condense
- kaijia323/dsh-ymc-sidebar
- KannaKuron/dsh-deepseek-vision-bridge
- kedoupi/dsh-plugins
- KitDoesIt/dsh-compaction-instant
- lamost423/dsh-trace-compare
- LBurny/deepseek-harness-desktop
- lesliechowsh/dsh-memo
- liustack/aimanager
- liustack/pptfast
- lo2589/deepseek-harness-meida
- looput/dsn-finance-lab
- LVSUGARS/dsh-web-manager
- lvyunqi/dsh-memory-enhanced
- mattismegevand/dsh-dock
- mattismegevand/dsh-git
- mattismegevand/dsh-open
- mattismegevand/dsh-terminal
- mianyoubiaoqing/MistyMoon-DSH
- Mrzhailiming/deepseek-pet
- muvuula/DeepSeek-Harness-Core
- Nexus-Aethra/DSH-plugin-switch
- omdsh-dev/fabric
- omdsh-dev/Qwen-MM-Plugins
- openma-ai/deepseek-harness-typescript-sdk
- Physicolor/harness-ui-enhancer
- Physicolor/harness-widgets
- pppolf/dsh-webgate
- QLM1234/dsh-dynamic-assembler
- rayafriandion/deepseek-harness-tui
- raydez/deepseek-harness-pet-plugin
- riesbri/dsh-tui
- ruisenbai/dsh-inline-comments
- satan9394/dsh-a11y-audit
- satan9394/dsh-academic-research
- satan9394/dsh-adhd-friendly
- satan9394/dsh-agent-loop-engineering
- satan9394/dsh-agent-reach
- satan9394/dsh-agent-teams
- satan9394/dsh-ai-image-design
- satan9394/dsh-algorithmic-art
- satan9394/dsh-api-design
- satan9394/dsh-api-documentation
- satan9394/dsh-api-scaffolding
- satan9394/dsh-architecture
- satan9394/dsh-auth
- satan9394/dsh-autonomous-research
- satan9394/dsh-bash-scripting
- satan9394/dsh-bash-testing
- satan9394/dsh-bazel-build-optimization
- satan9394/dsh-before-you-build
- satan9394/dsh-better-interface
- satan9394/dsh-blockchain-web3
- satan9394/dsh-brand-design
- satan9394/dsh-brand-guidelines
- satan9394/dsh-brand-landingpage
- satan9394/dsh-browser-testing
- satan9394/dsh-cad-modeling
- satan9394/dsh-canvas-design
- satan9394/dsh-career-ops
- satan9394/dsh-caveman-speak
- satan9394/dsh-changelog
- satan9394/dsh-channel-assistant
- satan9394/dsh-cicd
- satan9394/dsh-cli-anything
- satan9394/dsh-cloud-cost-optimization
- satan9394/dsh-cloud-well-architected
- satan9394/dsh-code-review
- satan9394/dsh-code-simplify
- satan9394/dsh-codebase-design
- satan9394/dsh-codebase-scanner
- satan9394/dsh-colleague-creation
- satan9394/dsh-commit-message
- satan9394/dsh-content-distillation
- satan9394/dsh-content-marketing
- satan9394/dsh-context-engineering
- satan9394/dsh-contract-review
- satan9394/dsh-css-art-styles
- satan9394/dsh-data-engineering
- satan9394/dsh-data-quality
- satan9394/dsh-data-storytelling
- satan9394/dsh-database-design
- satan9394/dsh-dataset-curation
- satan9394/dsh-db-migration
- satan9394/dsh-debug-recovery
- satan9394/dsh-deployment-validation
- satan9394/dsh-deprecation
- satan9394/dsh-designmd
- satan9394/dsh-desktop-agent-gui
- satan9394/dsh-diagram-design
- satan9394/dsh-discernment-nudge
- satan9394/dsh-distributed-debugging
- satan9394/dsh-doc-coauthoring
- satan9394/dsh-doc-compiled-skills
- satan9394/dsh-docs-adr
- satan9394/dsh-document-generation
- satan9394/dsh-domain-modeling
- satan9394/dsh-dotnet-backend
- satan9394/dsh-doubt-driven-dev
- satan9394/dsh-e2e-testing
- satan9394/dsh-error-handling
- satan9394/dsh-event-driven-architecture
- satan9394/dsh-file-conversion
- satan9394/dsh-framework-migration
- satan9394/dsh-frontend-design
- satan9394/dsh-frontend-engineering
- satan9394/dsh-frontend-mobile
- satan9394/dsh-frontend-slides
- satan9394/dsh-full-stack-orchestration
- satan9394/dsh-functional-programming
- satan9394/dsh-game-development
- satan9394/dsh-geo-seo
- satan9394/dsh-gif-creator
- satan9394/dsh-git-guardrails
- satan9394/dsh-git-workflow
- satan9394/dsh-gitops
- satan9394/dsh-grill-me
- satan9394/dsh-hallmark-design
- satan9394/dsh-handoff
- satan9394/dsh-harness-os
- satan9394/dsh-hot-trends
- satan9394/dsh-hr-legal-compliance
- satan9394/dsh-html-ppt
- satan9394/dsh-html-template-library
- satan9394/dsh-humanizer-zh
- satan9394/dsh-hybrid-cloud
- satan9394/dsh-idea-refine
- satan9394/dsh-incremental
- satan9394/dsh-internal-comms
- satan9394/dsh-investment-research
- satan9394/dsh-issue-triage
- satan9394/dsh-javascript-typescript
- satan9394/dsh-karpathy-methodology
- satan9394/dsh-knowledge-brain
- satan9394/dsh-kpi-dashboard-design
- satan9394/dsh-kubernetes-operations
- satan9394/dsh-last30days
- satan9394/dsh-live-docs
- satan9394/dsh-llm-api-integration
- satan9394/dsh-llm-eval
- satan9394/dsh-llm-finetuning
- satan9394/dsh-marketing-growth
- satan9394/dsh-mcp-builder
- satan9394/dsh-meeting-minutes
- satan9394/dsh-merge-conflicts
- satan9394/dsh-microservices
- satan9394/dsh-mlops
- satan9394/dsh-model-gateway
- satan9394/dsh-monorepo
- satan9394/dsh-multi-cloud
- satan9394/dsh-observability
- satan9394/dsh-observability-tools
- satan9394/dsh-obsidian-vault
- satan9394/dsh-office-cli
- satan9394/dsh-operating-kit
- satan9394/dsh-opinion-analysis
- satan9394/dsh-parallel-agent-ade
- satan9394/dsh-parallel-dev
- satan9394/dsh-payment-processing
- satan9394/dsh-pci-compliance
- satan9394/dsh-pdf-processing
- satan9394/dsh-performance
- satan9394/dsh-persistent-memory
- satan9394/dsh-personal-content-discovery
- satan9394/dsh-planning
- satan9394/dsh-planning-files
- satan9394/dsh-plugin-eval
- satan9394/dsh-ponytail-dev
- satan9394/dsh-postmortem
- satan9394/dsh-ppt-creator
- satan9394/dsh-pptx-engineering
- satan9394/dsh-prompt-audit
- satan9394/dsh-prompt-engineering
- satan9394/dsh-prototype
- satan9394/dsh-python-development
- satan9394/dsh-quant-backtest
- satan9394/dsh-rag
- satan9394/dsh-recsys-pipeline
- satan9394/dsh-relationship-coach
- satan9394/dsh-repo-graphify
- satan9394/dsh-reverse-engineering
- satan9394/dsh-review-agent-governance
- satan9394/dsh-runbook
- satan9394/dsh-sales-automation
- satan9394/dsh-sast-security
- satan9394/dsh-scientific-research
- satan9394/dsh-screenshot-to-code
- satan9394/dsh-security-compliance
- satan9394/dsh-security-hardening
- satan9394/dsh-security-requirements
- satan9394/dsh-self-improving-agent
- satan9394/dsh-service-mesh
- satan9394/dsh-setup-wizard
- satan9394/dsh-shipping
- satan9394/dsh-signed-audit-trails
- satan9394/dsh-skill-creator
- satan9394/dsh-skill-optimization
- satan9394/dsh-skill-seekers
- satan9394/dsh-slo
- satan9394/dsh-social-publishing
- satan9394/dsh-social-simulation
- satan9394/dsh-source-driven
- satan9394/dsh-spec-driven
- satan9394/dsh-sql-optimization
- satan9394/dsh-startup-business-analyst
- satan9394/dsh-superpowers-essentials
- satan9394/dsh-swarm-prediction
- satan9394/dsh-systems-programming
- satan9394/dsh-taste-review
- satan9394/dsh-tdd
- satan9394/dsh-teach
- satan9394/dsh-tech-debt
- satan9394/dsh-terraform
- satan9394/dsh-test-desktop-app
- satan9394/dsh-theme-factory
- satan9394/dsh-threat-modeling
- satan9394/dsh-to-questionnaire
- satan9394/dsh-track-driven-dev
- satan9394/dsh-vector-search
- satan9394/dsh-virtual-eng-team
- satan9394/dsh-wayfinder
- satan9394/dsh-web-artifacts
- satan9394/dsh-web-clone
- satan9394/dsh-web-scripting
- satan9394/dsh-webapp-testing
- satan9394/dsh-workflow-loop
- satan9394/dsh-writing-beats
- satan9394/dsh-writing-for-agents
- satan9394/dsh-writing-fragments
- satan9394/dsh-writing-shape
- satan9394/dsh-x-twitter-research
- saurtone/dsh-tool-somark
- sd3247930/SkyDome
- seaskyblue/dsh-channel-feishu
- sidleo/skill-scan
- sjh9714/clippy-harness
- sjh9714/dsh-lean
- sjh9714/dsh-what-changed
- songoao25/dsh-song-memory
- tianji-qingtian/dsh-spec-loop
- TiantianFlow/dsh-tailscale-gateway
- TimeCraker/dsh-claude-import
- trewvip-arch/dsh-open-in-app
- TuringCorp-net/mosaic_compress
- vcxmug/dsh-enhance
- wings1848/dsh-economizer
- worldwonderer/oh-story-dsh
- WSL043/dsh-native-session-delete
- WSYXIUBA/dsh-plugin-constellation
- xie-tj/deepseek-harness-latest-user-message-revision
- y2zyyr/dsh-restart-button
- yamingmou/dsh-message-editor
- yhyfhgs/dsh-providers-extension
- yishengdaxiaonengjihui/dsh-plugin-manager
- zhoupengjie/dsh-motion-manager
- zhouzhencheng07/dsh-free-search
- zhouzhencheng07/dsh-memory
- zhu1090093659/dsh-web-ui
