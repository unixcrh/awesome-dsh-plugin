# 待审核仓库 / Pending review

> 新增到 `dsh-plugin` Topic 下、带有简介、尚未经维护者核实的仓库。本文件由 `scripts/update.mjs` 每日刷新，仅供审核使用，不是用户可见页面。
>
> Repositories newly added to the `dsh-plugin` topic that the maintainer has not verified yet. Refreshed daily by `scripts/update.mjs`; review-only, not a user-facing page.

- 生成时间 / Generated: **2026-08-31**
- 快照日期 / Snapshot date: **2026-08-31 (UTC)**
- 待审核 / Pending: **2652**
- 从快照消失的已核准仓库 / Approved repositories missing from the snapshot: **437**

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
| 1 | [Molunerfinn/PicGo](https://github.com/Molunerfinn/PicGo) | 27103 | 2017-12-12 | 2026-08-22 | :rocket: The Ultimate Image Uploader for Efficient Creators. Supports Obsidian, Typora, VS Code etc. and 60+ image hosting services  (S3, GitHub, Cloudflare R2, Imgur, Aliyun OSS...). Paste, upload, done. |
| 2 | [titanwings/distilly](https://github.com/titanwings/distilly) | 24207 | 2026-03-30 | 2026-08-24 | Distilly — Distill how they think into reusable Skills for any Agent or Bot. Formerly Colleague Skill（原同事 Skill）. |
| 3 | [anywhere-labs/dsh-desktop](https://github.com/anywhere-labs/dsh-desktop) | 22438 | 2026-08-13 | 2026-08-24 | 为 DeepSeek Harness (DSH) 插件生态打造的现代化桌面端解决方案。万物皆「插件」，桌面本身也是「插件」。 |
| 4 | [yjh051108/dsh-routing-suite](https://github.com/yjh051108/dsh-routing-suite) | 6997 | 2026-08-14 | 2026-08-23 | dsh-routing-suite — injector + router-standard kit: install the runtime injector first, then the task-aware reasoning-mode router preset (measured P1-P23). |
| 5 | [zhu1090093659/dsh-web](https://github.com/zhu1090093659/dsh-web) | 6591 | 2026-08-12 | 2026-08-24 | DeepSeek Harness (DSH) Web Plugin Aggregation Ecosystem · Everything is a plugin, distributed via the Creative Workshop |
| 6 | [huangruiteng/loopx](https://github.com/huangruiteng/loopx) | 5353 | 2026-05-31 | 2026-08-31 | Long-horizon agent control plane for durable, governed work across Codex, Claude Code, and other harnesses. |
| 7 | [agentscope-ai/ReMe](https://github.com/agentscope-ai/ReMe) | 3378 | 2024-08-29 | 2026-08-24 | ReMe: Memory Management Kit for Agents - Remember Me, Refine Me. |
| 8 | [Tiger3807861189/J-Space-Cognition-Suite-V3.7](https://github.com/Tiger3807861189/J-Space-Cognition-Suite-V3.7) | 3008 | 2026-07-22 | 2026-08-23 | J-Space Cognition Suite V3.7 - AI cognitive-enhancement Skills based on Anthropic's J-space global workspace research. \| 哔哩哔哩：Tiger380 (UID 3494375382321675) — https://space.bilibili.com/3494375382321675 |
| 9 | [chuspeeism/dashi-taskboard](https://github.com/chuspeeism/dashi-taskboard) | 2827 | 2026-07-24 | 2026-08-29 | 现代化可灵活嵌入的任务面板，支持 Codex、DeepSeek Harness |
| 10 | [zilliztech/memsearch](https://github.com/zilliztech/memsearch) | 2536 | 2026-02-09 | 2026-08-24 | A persistent, unified memory layer for all your AI agents (e.g. Claude Code, Codex, DSH), backed by Markdown and Milvus. |
| 11 | [dsh-tauri-desk/deepseek-harness-desktop](https://github.com/dsh-tauri-desk/deepseek-harness-desktop) | 1490 | 2026-08-14 | 2026-08-23 | DeepSeek Harness Tauri 桌面版 \| Only 5mb installer, zero environment setup, preset plugins, Windows / macOS / Linux. |
| 12 | [AdamPlatin123/dsh-plugin-radar](https://github.com/AdamPlatin123/dsh-plugin-radar) | 1438 | 2026-08-04 | 2026-08-28 | DSH Plugin Radar — 开源 DSH 插件生态雷达：自动发现 15900+ 候选、k8s 运行级实测 10000+、15 分钟快照管线；插件目录是其自动生成的 artifact |
| 13 | [Unclecheng-li/AI_Animation](https://github.com/Unclecheng-li/AI_Animation) | 1197 | 2026-04-11 | 2026-08-29 | 本项目整理了用于生成[炫酷 HTML 动画网页]的 AI Prompts，涵盖动画效果、3D 可视化、PPT 风格演示、UI 美化等多个类别。 |
| 14 | [platonai/Browser4](https://github.com/platonai/Browser4) | 1114 | 2018-03-12 | 2026-08-27 | Browser4 — an AI-native browser engine for autonomous agents, intelligent extraction, and large-scale web automation. |
| 15 | [wecode-ai/Wegent](https://github.com/wecode-ai/Wegent) | 766 | 2026-01-10 | 2026-08-30 | Plan, build, and deliver with an open-source, self-hostable AI workspace for coding, collaboration, and automation. |
| 16 | [vshulcz/deja-vu](https://github.com/vshulcz/deja-vu) | 745 | 2026-07-14 | 2026-08-23 | Search your past AI coding sessions — Claude Code, Codex, Cursor and 17 more. Indexes the session history they already wrote to disk, including months from before you installed it, and recalls it in any of them. No LLM, no embeddings, one local Go binary. |
| 17 | [Minglink/dsh-infinite-gen-3](https://github.com/Minglink/dsh-infinite-gen-3) | 726 | 2026-08-15 | 2026-08-31 | DeepSeek 专用破甲插件「无限三代」dsh-infinite-gen-3 — armor-breaking plugin for DeepSeek，破甲版：稳定化破甲，求 Star 收藏 ⭐ |
| 18 | [vibeinging/dsh-desktop](https://github.com/vibeinging/dsh-desktop) | 635 | 2026-08-13 | 2026-08-23 | DeepSeek Harness Desktop App: a local AI desktop workspace for DSH Sessions, projects, files, web research, plugins, and Office artifacts. |
| 19 | [chainbase-labs/Agentkey](https://github.com/chainbase-labs/Agentkey) | 623 | 2026-04-23 | 2026-08-25 | Connect your AI agent to the world — Web search, Social media, Crypto & On-chain data. One plugin, zero extra config. |
| 20 | [myYangyunfan/dsh_desktop](https://github.com/myYangyunfan/dsh_desktop) | 615 | 2026-08-13 | 2026-08-30 | DeepSeek Harness (dsh) Windows desktop client - bundled Node.js + dsh CLI, one-click launch |
| 21 | [Aisland-SJL/dsh-worktable](https://github.com/Aisland-SJL/dsh-worktable) | 411 | 2026-08-16 | 2026-08-24 | 🖥️ Agent-project workbench for DeepSeek Harness — sidebar app drawer + dockable split workspace + a live control room watching every project. |
| 22 | [Unclecheng-li/DeepSec](https://github.com/Unclecheng-li/DeepSec) | 370 | 2026-07-09 | 2026-08-25 | DeepSec — AI Security Offense & Defense Platform. Shield audits AI-generated code for hallucinated packages, missing safeguards & AI pattern errors in real time. Spear automates authorized penetration testing with 40+ skill packs, from recon to PoC.  |
| 23 | [yjh051108/dsh-router-standard](https://github.com/yjh051108/dsh-router-standard) | 365 | 2026-08-14 | 2026-08-23 | 已并入 dsh-routing-suite（单仓库化）；本仓库为历史镜像/归档 —— 注意力工程主线 v1.19.1/v34 研发线未发布。新代码见 github.com/yjh051108/dsh-routing-suite |
| 24 | [EthanYoQ/Invoice-Downloader](https://github.com/EthanYoQ/Invoice-Downloader) | 291 | 2026-03-02 | 2026-08-22 | 电子发票整理与报销准备工具：从邮箱批量收集 PDF/OFD/XML 发票，OCR 识别、分类归档并生成 Excel 汇总；提供 Windows/macOS 桌面版与 DSH 插件。 |
| 25 | [ericshang98/Perfect-Web-Clone](https://github.com/ericshang98/Perfect-Web-Clone) | 260 | 2026-01-06 | 2026-08-22 | Pixel-perfect clones of any webpage. Paste a URL, get a measured Vite + React replica. |
| 26 | [zenstory-ai/oh-story-dsh](https://github.com/zenstory-ai/oh-story-dsh) | 229 | 2026-08-19 | 2026-08-25 | A DSH plugin for novel writing and short-drama production, powered by Oh Story and Drama Skills. |
| 27 | [yjh051108/dsh-super-injector](https://github.com/yjh051108/dsh-super-injector) | 153 | 2026-08-13 | 2026-08-25 | 推荐组件（非必须）：DeepSeek Harness 运行时注入器；已随 dsh-routing-suite 单仓库化保留，本仓库继续维护/发布。 |
| 28 | [1692775560/dsh-Mimir-Academic-research](https://github.com/1692775560/dsh-Mimir-Academic-research) | 142 | 2026-08-20 | 2026-08-24 | Mimir — 一站式科研工作台插件：LaTeX 论文边写边编译、arXiv 文献管理、实验追踪、指标图表、GPU 服务器 SSH 任务编排，管理科研全周期。An open-source research workbench plugin for the whole research cycle. |
| 29 | [liguobao/ds-harness-remote](https://github.com/liguobao/ds-harness-remote) | 138 | 2026-08-14 | 2026-08-30 | 一个基于 DeepSeek Harness 插件机制构建的多端远程访问方案，通过安全、低延迟、端到端加密的 P2P 优先网络，支持从 PC、Android 和 Web 随时访问并操作远程 Harness。 (A multi-device remote access solution built on the DeepSeek Harness plugin system, enabling PC, Android, and Web clients to securely access and operate a remote Harness over a low-latency, end-to-end encrypted, P2P-first network.) |
| 30 | [theBigGavin/marketingdashboard](https://github.com/theBigGavin/marketingdashboard) | 134 | 2026-07-17 | 2026-08-30 | 面向金融与产业研究的一屏式实时行情大屏：A股/港股/美股指数、大宗商品、美债收益率、板块热点、主力资金流、7×24 快讯、产业链自选股、AI 大模型 Token 追踪。A real-time market research cockpit on a single screen: CN/HK/US indices, commodities, treasury yields, sector hotspots, capital flows, 7×24 news, industry-chain watchlists and AI token usage trends.  |
| 31 | [ZSeven-W/dsh-android](https://github.com/ZSeven-W/dsh-android) | 129 | 2026-08-21 | 2026-08-22 | DeepSeek Harness plugin for Android — build, run, and interact with a live emulator or USB device stream inside a conversation, driven entirely through adb. |
| 32 | [fangqian616/consensus-pipeline](https://github.com/fangqian616/consensus-pipeline) | 114 | 2026-07-16 | 2026-08-30 | Multi-agent department framework for long-form complex tasks, fighting AI hallucination, validated on academic research. 共识管线：多智能体部门长线任务解决框架，对抗AI幻觉，以学术研究为验证场景。 |
| 33 | [volcengine/ark-cli](https://github.com/volcengine/ark-cli) | 114 | 2026-06-15 | 2026-08-22 | The fastest way to put Volcengine Ark in your terminal and your AI agent — go from prompt to generated   media, multimodal answer, or deployed endpoint in a single command, no API glue code. |
| 34 | [Akimiya-z/codex-guard](https://github.com/Akimiya-z/codex-guard) | 110 | 2026-08-20 | 2026-08-23 | Quality gate for AI/Codex-generated pull requests: blocks TODO leftovers, leaked secrets, sloppy commits and red CI before they reach main. |
| 35 | [SLin-code/dsh-custom-skin](https://github.com/SLin-code/dsh-custom-skin) | 104 | 2026-08-24 | 2026-08-24 | DSH自定义壁纸/皮肤插件——Custom wallpapers and translucent skins for DeepSeek Harness Web |
| 36 | [Justin-sky/ai-art-engine](https://github.com/Justin-sky/ai-art-engine) | 96 | 2026-07-24 | 2026-08-31 | AI 艺术创作引擎，专业的短视频创作工具 |
| 37 | [Clarklevis1995/dsh-mobile](https://github.com/Clarklevis1995/dsh-mobile) | 83 | 2026-08-17 | 2026-08-23 | DeepSeek Harness Mobile 是一个面向 DeepSeek Harness 的原生 iOS 客户端。它通过 dsh-plugin-mobile-gateway 与 Harness 建立 WebSocket 连接，将工作区、会话、实时回复和 Agent 执行轨迹带到 iPhone，同时延续 DeepSeek WebUI 克制、清晰的视觉语言 |
| 38 | [Rain-kl/dsh-preset-plus](https://github.com/Rain-kl/dsh-preset-plus) | 63 | 2026-08-24 | 2026-08-24 | DSH 预设编辑器插件, 支持一键破甲. |
| 39 | [baihejiangnan/deepseek-harness-desktop](https://github.com/baihejiangnan/deepseek-harness-desktop) | 62 | 2026-08-21 | 2026-08-23 | DeepSeek Harness 三端兼容桌面启动器：多实例完全隔离、并行协作，协作画布编排 Agent 工作流；便携版 Exe 一键启动、仅约 18M（不超过 20M）；双隔离机制让兼容性极强，无论 DSH 本体如何更新，兼容原生到野生狗奶。 |
| 40 | [Jackywxsz/DSH-Creator](https://github.com/Jackywxsz/DSH-Creator) | 62 | 2026-08-25 | 2026-08-26 | Jacky Creator：面向内容创作者的 DeepSeek Harness 本地内容与运营工作台 |
| 41 | [lamost423/dsh-maze](https://github.com/lamost423/dsh-maze) | 60 | 2026-08-18 | 2026-08-26 | DeepSeek Harness 的执行迷宫——看 Agent 真实怎么干活：迷宫时间轴 · 数据轨道 · 确定性执行分析 · 多会话对比 \| The execution maze for DSH agents: maze timeline, per-step data tracks, deterministic execution analysis, multi-session comparison. Formerly dsh-trace-compare. |
| 42 | [yxxbc/dsh-balance-plugin](https://github.com/yxxbc/dsh-balance-plugin) | 58 | 2026-08-15 | 2026-08-23 | deepSeek 余额监控与用量统计（DSH 动态 Cordis 插件）：余额监控 · 官方充值入口 · 用量统计 · 三方插件管理 |
| 43 | [peiyuwang54/deepseek-harness-cli](https://github.com/peiyuwang54/deepseek-harness-cli) | 57 | 2026-08-14 | 2026-08-23 | DeepSeek CLI |
| 44 | [yuc16/PatentRadar](https://github.com/yuc16/PatentRadar) | 57 | 2026-05-05 | 2026-08-22 | 专利侵权分析系统 —— 输入专利公开号，产出竞品侵权分析报告；同时打包成 skill，可被任意 agent（dsh, codex, claudecode 等） 调用。 |
| 45 | [KelaoHu/dsh-lowtide](https://github.com/KelaoHu/dsh-lowtide) | 55 | 2026-08-23 | 2026-08-24 | Time-shifting task delegation for DeepSeek Harness (dsh): plan tasks at leisure, they run unattended off-peak, come back to a report. Human-adjudicated, desktop + web. |
| 46 | [JingxuanC/causal-memory](https://github.com/JingxuanC/causal-memory) | 54 | 2026-07-26 | 2026-08-24 | Causal memory layer for AI agents — MCP server that records decision→outcome relationships. Survives compaction. |
| 47 | [AgentDebugX/AgentDebugX](https://github.com/AgentDebugX/AgentDebugX) | 52 | 2026-07-10 | 2026-08-25 | 【EMNLP 2026 Demo】A debugging framework for agentic AI systems: diagnose failures, attribute root causes, recover with evidence, and validate fixes through reruns. |
| 48 | [xi-zhao/OpenQuantum](https://github.com/xi-zhao/OpenQuantum) | 48 | 2026-08-15 | 2026-08-23 | Open-source quantum Agent workspace with a desktop client, Web UI, messaging, Qiskit/MCP tools, and scientific validation |
| 49 | [T-Auto/dsh-ecosystem-spec](https://github.com/T-Auto/dsh-ecosystem-spec) | 46 | 2026-08-17 | 2026-08-22 | deepseek-harness TUI Plugin Access and Implementation Standards / deepseek-harness终端交互生态插件准入规范与实施标准 |
| 50 | [plolpl789/dsh-raw-html](https://github.com/plolpl789/dsh-raw-html) | 45 | 2026-08-21 | 2026-08-24 | VCP visual-synesthesia protocol plugin for DeepSeek Harness: render agent HTML output as real UI (cards / KaTeX math / Mermaid diagrams / built-in calligraphy fonts / zero-JS interactions), plug-and-play on any DSH environment |
| 51 | [niuhuoshan/launch-wechat-miniprogram](https://github.com/niuhuoshan/launch-wechat-miniprogram) | 42 | 2026-08-11 | 2026-08-31 | 面向完全新手的微信小程序 Agent Skill，从需求确认、原生 UI 和高保真原型，到 AppID、备案、开发测试、腾讯云后台、体验版、提审、发布及版本更新。 |
| 52 | [fandc520/dsh-comfyui](https://github.com/fandc520/dsh-comfyui) | 40 | 2026-08-20 | 2026-08-22 | 一个基于DeepSeek-Harness的ComfyUI插件 |
| 53 | [HakureiMonika/dsh-sandbox-escalation-fix](https://github.com/HakureiMonika/dsh-sandbox-escalation-fix) | 39 | 2026-08-16 | 2026-08-28 | Session-aware sandbox escalation compatibility plugin for DeepSeek Harness/DSH第三方模型会话沙箱升级兼容插件 |
| 54 | [BeforeWave/dsh-with-chatgpt](https://github.com/BeforeWave/dsh-with-chatgpt) | 38 | 2026-08-21 | 2026-08-24 | Bring ChatGPT’s reasoning to your local codebase. Work directly, or delegate larger tasks to DSH. |
| 55 | [PensiveFei/dsh-voice-scribe](https://github.com/PensiveFei/dsh-voice-scribe) | 31 | 2026-08-25 | 2026-08-25 | DSH voice input plugin: tap Alt to talk, get text in composer. Web Speech default (zero config), optional OpenAI-compatible ASR, polish via DSH LLM. |
| 56 | [HiWhaleW/dsh-toolbox](https://github.com/HiWhaleW/dsh-toolbox) | 29 | 2026-08-13 | 2026-08-25 | Local-first DeepSeek Harness plugins for product research, context routing, plugin preflight, and compatibility monitoring. |
| 57 | [10086ggqq/dsh_theme_terraria](https://github.com/10086ggqq/dsh_theme_terraria) | 27 | 2026-08-22 | 2026-08-23 | 把 DeepSeek Harness 的 AI 编码控制台变成泰拉瑞亚像素世界——向导陪你写代码，真实对话、工具审批、难度切换，单文件零依赖。 |
| 58 | [ARFCON/dsh-hotplug-hub](https://github.com/ARFCON/dsh-hotplug-hub) | 27 | 2026-08-19 | 2026-08-22 | DSH - Dseam |
| 59 | [FrankHu-HK/mnemosyne](https://github.com/FrankHu-HK/mnemosyne) | 26 | 2026-08-10 | 2026-08-27 | Mnemosyne OS 7.0.0 — zero-dependency, local-first AI memory system (MCP / API / CLI / Python). MIT. |
| 60 | [qkycir-123/dsh-run2skill](https://github.com/qkycir-123/dsh-run2skill) | 26 | 2026-08-19 | 2026-08-22 | Automatically turn successful DeepSeek Harness sessions into reusable, reviewable Agent Skills. |
| 61 | [hanshanyike/dsh-yolo](https://github.com/hanshanyike/dsh-yolo) | 24 | 2026-08-20 | 2026-08-25 | 把对话里说过的重要事情，变成持续可跟进的计划。  为 deepseek-harness 打造的个人助手：从对话中整理事项、跟踪变化，并在需要时提醒你。 |
| 62 | [ZSeven-W/dsh-harbor](https://github.com/ZSeven-W/dsh-harbor) | 24 | 2026-08-22 | 2026-08-25 | DeepSeek Harness (DSH) plugin: a read-only ledger for the plugins you already have installed — a capability inventory with file:line evidence, declared-vs-detected reconciliation, cross-profile version drift, and a diff of what changed since the last scan. |
| 63 | [extracurricular-ai/dsh-filesnap](https://github.com/extracurricular-ai/dsh-filesnap) | 22 | 2026-08-27 | 2026-08-27 | dsh-filesnap — 把对话和它改过的文件一起回退到某一轮之前,不需要 git 仓库. A blazing-fast rewind and redo plugin for DeepSeek Harness, powered by a 🦀 Rust core, tracking the conversion and the files it changed, no git required, low disk consumption |
| 64 | [398894496-arch/runtime36](https://github.com/398894496-arch/runtime36) | 19 | 2026-08-21 | 2026-08-22 | Second brain for coding agents. Seal the day, distill into Obsidian, hit that page tomorrow. Cursor, Codex, Claude Code, DeepSeek Harness. |
| 65 | [cofy-x/dsh-console](https://github.com/cofy-x/dsh-console) | 19 | 2026-08-24 | 2026-08-24 | A TypeScript and React/Ink terminal frontend for DeepSeek Harness. |
| 66 | [fishzjp/qa-skills](https://github.com/fishzjp/qa-skills) | 19 | 2026-06-24 | 2026-08-24 | 让 AI 像资深测试工程师一样工作：面向 AI Agent 的测试工程 Skill 框架——10 Skills + 共享知识库 + 类型决策矩阵（Claude Code / dsh 等 Agent 可用） |
| 67 | [dsh-blue/blue](https://github.com/dsh-blue/blue) | 18 | 2026-08-18 | 2026-08-22 | Blue: a TUI is not a package, it is a Cordis plugin tree — a modern terminal UI for DeepSeek Harness with hot-swappable render, interaction, and command plugins. |
| 68 | [lizhiyao/oh-my-knowledge](https://github.com/lizhiyao/oh-my-knowledge) | 18 | 2026-03-24 | 2026-08-24 | OMK — Evidence-backed evaluation and observability for prompts, RAG, skills, agents, and workflows. Native Codex, Claude Code, and DeepSeek Harness support. |
| 69 | [omdsh-dev/stent](https://github.com/omdsh-dev/stent) | 18 | 2026-08-06 | 2026-08-22 | 灵感来源于MC Fabric的Cordis/DSH hook处理器 |
| 70 | [chumingjun/dsh-harness-one](https://github.com/chumingjun/dsh-harness-one) | 17 | 2026-08-20 | 2026-08-27 | Visual AI workflow orchestrator for DeepSeek Harness (dsh): multi-agent DAGs, live execution, recovery, and Feishu integration. |
| 71 | [Ed-Marcavage/awesome-security-agent-harnesses](https://github.com/Ed-Marcavage/awesome-security-agent-harnesses) | 16 | 2026-08-03 | 2026-08-30 | AI agents for pentesting, code audit, fuzzing, vulnerability discovery, and reverse engineering — harnesses, sandboxes, security MCP servers, benchmarks, and evals. |
| 72 | [klarkxy/zhihu-search](https://github.com/klarkxy/zhihu-search) | 16 | 2026-06-17 | 2026-08-23 | 知乎开放平台接口，官方Zhihu Cli开源平替。 |
| 73 | [sqs404/dsh-portable](https://github.com/sqs404/dsh-portable) | 16 | 2026-08-16 | 2026-08-23 | DeepSeek Harness 免安装便携版（Windows）：官方 npm 包 + 内置 Node.js，双击 exe 即用，拷贝到任意 64 位 Windows 电脑独立运行 |
| 74 | [Suiwan/whale-purse](https://github.com/Suiwan/whale-purse) | 16 | 2026-08-14 | 2026-08-30 | A cute whale desktop pet for DeepSeek Harness that keeps an eye on your DeepSeek balance and session usage/cost. Drag her anywhere, click to open a live panel with real-time spend, peak/off-peak pricing, budget alerts, and history trends. |
| 75 | [NekroAI/nekro-nxt](https://github.com/NekroAI/nekro-nxt) | 15 | 2026-08-15 | 2026-08-26 | NekroNXT：基于 DeepSeek Harness（DSH）的多平台群聊智能体系统｜A DSH-powered multi-platform group-chat agent system |
| 76 | [aa2246740/dsh-watcher](https://github.com/aa2246740/dsh-watcher) | 14 | 2026-08-20 | 2026-08-25 | Read-only Agent work-path observer for DeepSeek Harness |
| 77 | [daha1216/dsh-adult-tension](https://github.com/daha1216/dsh-adult-tension) | 14 | 2026-08-19 | 2026-08-24 | DeepSeek自带破甲18+互动叙事 Skill：NPC 活人感（有记忆/立场/底线）、数百项素材库、随机开局可预锁、时间推进、全维 YAML 存档。 |
| 78 | [FishBottle7/opencode2dsh](https://github.com/FishBottle7/opencode2dsh) | 14 | 2026-08-29 | 2026-08-29 | DSH plugin — free OpenCode Zen models for DeepSeek Harness (DSH). Free LLM API, no API key needed. 在 DSH 中使用 OpenCode Zen 免费模型，无需 API key |
| 79 | [TiantianFlow/dsh-one-gateway](https://github.com/TiantianFlow/dsh-one-gateway) | 14 | 2026-08-16 | 2026-08-22 | Private DSH One Gateway — loopback, identity-first ingress for DeepSeek Harness |
| 80 | [TsFreddie/dsh-compaction-instant](https://github.com/TsFreddie/dsh-compaction-instant) | 14 | 2026-08-14 | 2026-08-22 | LLM-free lossless* compaction engine for DeepSeek Harness |
| 81 | [ddtcorex/govard](https://github.com/ddtcorex/govard) | 13 | 2026-02-08 | 2026-08-28 | Go-based local development orchestrator for Magento, Laravel, Symfony, Next.js, WordPress, and more. Docker stacks, SSL, Xdebug, and a desktop dashboard. |
| 82 | [Minglink/DeepSeek-Harness-Hub](https://github.com/Minglink/DeepSeek-Harness-Hub) | 13 | 2026-08-24 | 2026-08-25 | 🌐 DeepSeek 官方与开源生态插件市场 (deepseek.stream) 使用指南与一键安装协议规范 |
| 83 | [dabaicai001/star-dsh-desktop](https://github.com/dabaicai001/star-dsh-desktop) | 12 | 2026-06-04 | 2026-08-25 | StarHub — All-in-One DevOps Desktop Command Center。把开发运维每天要用到的工具收进同一个窗口:数据库客户端 · SSH 终端 · SFTP · Docker · AI 助手,以及 AI 驱动的沙箱桌面与 Android 实体机操作。 |
| 84 | [Physicolor/dsh-ui-harmonizer](https://github.com/Physicolor/dsh-ui-harmonizer) | 12 | 2026-08-15 | 2026-08-22 | Web UI polish layer for DeepSeek Harness: normalizes unfinished or self-contradictory official UI, reconciles style conflicts between installed plugins, and unifies the visual language via official design tokens. |
| 85 | [vritser/dsh-emacs](https://github.com/vritser/dsh-emacs) | 12 | 2026-08-23 | 2026-08-25 | An Emacs client for DeepSeek Harness |
| 86 | [havingautism/dsh-deepresearch](https://github.com/havingautism/dsh-deepresearch) | 11 | 2026-08-12 | 2026-08-22 | @deepseek-ai/dsh-deepresearch 把证据优先的 Codemini 研究工作区带到 DSH。它提供持久工作流状态、模型工具、生成的 deepResearch Remote namespace 和“深度研究”Web 工作区，同时组合宿主已有的 Web 与 subagent 能力。 |
| 87 | [IceApriler/dsh-remote-mobile](https://github.com/IceApriler/dsh-remote-mobile) | 11 | 2026-08-21 | 2026-08-23 | DeepSeek Harness 远程与移动端安全网关插件：零修改 DSH 底层代码安全开放局域网与 Tailscale 连接 \| DeepSeek Harness (DSH) Remote & Mobile Security Guard: safely opens Tailscale/LAN with zero core modifications, QR scan auth, RSA encryption & brute-force defense. |
| 88 | [Leon0555/dsh-lan-access](https://github.com/Leon0555/dsh-lan-access) | 11 | 2026-08-14 | 2026-08-24 | 一个DSH局域网内访问插件：让 DeepSeek Harness 可在局域网内被其他设备访问的 DSH 插件。同一局域网下，手机/平板/电脑打开浏览器即可直接访问你某台设备上的 DSH——无需 SSH、无需内网穿透，npm 一键安装。 |
| 89 | [liustack/pptwise](https://github.com/liustack/pptwise) | 11 | 2026-07-16 | 2026-08-23 | A real PowerPoint, not a picture or HTML. Tell your AI what to cover and pptwise builds an editable deck on your own machine. Agent skill + DSH plugin, no account and no API key to render. \| 真正的 PPT，不是图片也不是 HTML。跟 AI 说要讲什么，pptwise 在你自己电脑上做出一份能改的 PPT。Agent skill + DSH 插件，不用注册，渲染不用 API key。 |
| 90 | [riesbri/dshline](https://github.com/riesbri/dshline) | 11 | 2026-08-17 | 2026-08-23 | The terminal-native frontend for the DeepSeek Harness plugin ecosystem. |
| 91 | [Angel2518975237/deepseek-harness-hello-kitty-suite](https://github.com/Angel2518975237/deepseek-harness-hello-kitty-suite) | 10 | 2026-08-23 | 2026-08-23 | 💗 一套给 DeepSeek Harness 的粉色 Hello Kitty 主题皮肤 + 任务完成/提问提醒插件（Sweetheart Workspace Expressive skin & Hello Kitty Task-Done Notifier） |
| 92 | [daha1216/dsh-plugin-collection](https://github.com/daha1216/dsh-plugin-collection) | 10 | 2026-08-19 | 2026-08-22 | DeepSeek Harness（DSH）第三方插件精选目录：一键安装，条目均指向插件作者原仓库。 |
| 93 | [EarzuChan/DshVibeLearning](https://github.com/EarzuChan/DshVibeLearning) | 10 | 2026-08-22 | 2026-08-23 | A Vibe Learning Plugin made for DeepSeek Harness |
| 94 | [louke6572/dsh-whale-widget-plus](https://github.com/louke6572/dsh-whale-widget-plus) | 10 | 2026-08-25 | 2026-08-25 | 基于DeepSeek-Balance-Whale-Widget开发，新增了三版不同的表情，需要那个版本的表情可以自己让agent帮你换，增加了火山coding plan额度查询，新增加台词自定义切换增加，增加了表情与台词手动切换 |
| 95 | [tinqiao-oss/clawtouch-mcp](https://github.com/tinqiao-oss/clawtouch-mcp) | 10 | 2026-06-01 | 2026-08-29 | ClawTouch MCP server — exposes a real USB-HID keyboard/mouse (Raspberry Pi Pico 2) as Model Context Protocol tools for any LLM agent. MIT. |
| 96 | [yinhcao/yinchao-ai-music-skill](https://github.com/yinhcao/yinchao-ai-music-skill) | 10 | 2026-08-20 | 2026-08-24 | AI 音乐生成 Agent Skill：支持文字/歌词生成歌曲、参考音频创作、BGM 与歌曲续写 |
| 97 | [Elave-66/dsh-blue-sea-launcher](https://github.com/Elave-66/dsh-blue-sea-launcher) | 9 | 2026-08-21 | 2026-08-22 | Deepseek 二次元游戏/Galgame 风格启动图标。鲸鱼娘形象来源bilibili@上善无形 @ZipZipPipe，适合重度二次元使用，配合鲸鱼娘皮肤等二次元插件使用更佳！ |
| 98 | [keman-ai/dsh-skin-market](https://github.com/keman-ai/dsh-skin-market) | 9 | 2026-08-18 | 2026-08-27 | Skin marketplace for DeepSeek Harness — search and install community skins from dsh.a2hmarket.ai right in the settings page |
| 99 | [LaoYueHanNi/dsh-token-usage](https://github.com/LaoYueHanNi/dsh-token-usage) | 9 | 2026-08-14 | 2026-08-27 | 贴近 DSH 原生设计风格的 token 用量统计插件：实时记录每次请求的用量与费用，在 Web UI 中提供趋势图表、按模型定价明细和供应商配额显示。 |
| 100 | [liang-today/dsh-liangxiang](https://github.com/liang-today/dsh-liangxiang) | 9 | 2026-08-15 | 2026-08-23 | 众香成势，梁子显相。DeepSeek Harness 的 WebUI 插件，欢迎一起打梁。 |
| 101 | [lna-lab/distill-kura](https://github.com/lna-lab/distill-kura) | 9 | 2026-08-21 | 2026-08-22 | 蒸留蔵 — distilled long-term memory for agents: recall by meaning, writing gated by evidence, one kura per agent mode. Ships as a DeepSeek Harness plugin and an MCP server. |
| 102 | [tma1-ai/dsh-otel](https://github.com/tma1-ai/dsh-otel) | 9 | 2026-08-25 | 2026-08-25 | What a DeepSeek Harness run costs in tokens, money, and time. OpenTelemetry traces, metrics, and logs in GreptimeDB, with seven Grafana dashboards. |
| 103 | [xiaoksio/dsh-solution-explorer](https://github.com/xiaoksio/dsh-solution-explorer) | 9 | 2026-08-23 | 2026-08-23 | DSH Web GUI right sidebar: VS Code-style file explorer plus source control (git status, stage/unstage/discard, commit, diff, commit graph, sync fetch/pull/push, branch/remote management, git init, multi-repo, color-coded file status, file-type icons, image preview) with editable diff view, syntax-highlighted editor, and file operations. |
| 104 | [AngelosZou/dsh-multi-folder](https://github.com/AngelosZou/dsh-multi-folder) | 8 | 2026-08-14 | 2026-08-25 | Secondary working directories for a DeepSeek Harness project — edit a source repo, a test repo, and a docs repo side by side without leaving the primary workspace. |
| 105 | [awesome-deepseekharness/awesome-deepseek-harness](https://github.com/awesome-deepseekharness/awesome-deepseek-harness) | 8 | 2026-08-15 | 2026-08-27 | Awesome DeepSeek Harness (dsh) — curated awesome list of plugins, tools, skills & resources. Everything is a plugin. |
| 106 | [azwosile/dsh-highres-vision](https://github.com/azwosile/dsh-highres-vision) | 8 | 2026-08-24 | 2026-08-25 | 专供 deepseek-v4-flash-vision-exp 的高清识图增强插件：放宽 DSH 图片限制 + highres_read 分块识图工具。 |
| 107 | [greenthree/ProbHub-skill](https://github.com/greenthree/ProbHub-skill) | 8 | 2026-05-25 | 2026-08-30 | 算法竞赛出题自动化skill（个人出题习惯），支持完善题面、构造数据、组卷用typ编译pdf和生成domjudge题目包 |
| 108 | [hoyyang/dsh-mall](https://github.com/hoyyang/dsh-mall) | 8 | 2026-08-25 | 2026-08-25 | 全网最强 DeepSeek Harness 插件商场：全量收录 GitHub #dsh-plugin 生态插件，五维实用评分雷达图，智能搜索（AI 理解需求）、智能安装/更新/卸载（AI 装前审查+装后诊断）、一键批量更新、编辑精选与个性化推荐，自带 Skills 工具与 dsh-mall 技能，中英多语言界面。 |
| 109 | [LoserFox/marisa-distro](https://github.com/LoserFox/marisa-distro) | 8 | 2026-08-13 | 2026-08-25 | 魔理沙 DSH 整合包发行：29 插件 + 一键安装 + profile 直装 |
| 110 | [Nono-neko/dsh-browser](https://github.com/Nono-neko/dsh-browser) | 8 | 2026-08-21 | 2026-08-23 | Cordis bundle plugin for DeepSeek Harness(DSH). Built‑in multi‑tab browser powered by Puppeteer, provides browser_open/browser_read agent tools & workspace file preview inside DSH Web GUI. |
| 111 | [PeterTXPan/dsh-unreal-mcp](https://github.com/PeterTXPan/dsh-unreal-mcp) | 8 | 2026-08-25 | 2026-08-31 | DeepSeek Harness Bundle for Unreal Engine 5.8 via Unreal MCP |
| 112 | [Ramenne/DeepSeek-Harness-Gov](https://github.com/Ramenne/DeepSeek-Harness-Gov) | 8 | 2026-08-28 | 2026-08-28 | DeepSeek Harness 政务版：基于 deepseek-ai/deepseek-harness 的政务办事 WebUI 与红头公文插件 |
| 113 | [AngelosZou/graphlint](https://github.com/AngelosZou/graphlint) | 7 | 2026-07-01 | 2026-08-26 | Dead-code detection for AI-generated codebases: graphlint builds a dependency graph, finds code unreachable from any entry point to enable codebase cleanup and functional‑effectiveness understanding. |
| 114 | [Cerbur/clutch-dsh](https://github.com/Cerbur/clutch-dsh) | 7 | 2026-08-19 | 2026-08-22 | Open-source DSH plugins for DeepSeek Harness, clutch-dsh-worktree. |
| 115 | [chen731215-dev/dsh-tavern-v2](https://github.com/chen731215-dev/dsh-tavern-v2) | 7 | 2026-08-27 | 2026-08-27 | DeepSeek Harness Tavern Plugin - character card roleplay, worldbook management, preset switching, dark theme, memory summary, relationship graph, PolyForm-Noncommercial-Copyleft-1.0.0 |
| 116 | [Chinesezjc/dsh-tool-todo-tree](https://github.com/Chinesezjc/dsh-tool-todo-tree) | 7 | 2026-08-13 | 2026-08-24 | Nested (tree-shaped) todo_write tool plugin for DeepSeek Harness (DSH) — the mutually-exclusive alternative to the flat dsh-tool-todo |
| 117 | [Cyning12/dsh-coding-kit](https://github.com/Cyning12/dsh-coding-kit) | 7 | 2026-08-16 | 2026-08-24 | DSH plugin + gate CLI for ICVO coding standards. Load ≠ inject: call apply_coding_standards. CLI: npx dsh-coding-kit |
| 118 | [getpapi/papi](https://github.com/getpapi/papi) | 7 | 2026-06-12 | 2026-08-22 | Your AI starts every session from zero. Your project stays on course. Structured plan, build and review cycles for any MCP-capable AI coding tool. |
| 119 | [IcyCreamDAS/shidi-skill](https://github.com/IcyCreamDAS/shidi-skill) | 7 | 2026-08-03 | 2026-08-23 | AI4S 科研 Agent 技能 \| AI-for-Science research workflow skill for coding agents: literature review · experiment design · figures · paper reading — files out, cross-verified, zero deps \| 文献调研/实验方案/作图/精读，交付文件+交叉验证，零依赖，MIT |
| 120 | [imsai-sh/dsh-1024store](https://github.com/imsai-sh/dsh-1024store) | 7 | 2026-08-24 | 2026-08-26 | DeepSeek Harness plugin store, marketplace and hub — 11,000+ dsh plugins with search, rankings, install commands and a free public API. DeepSeek Harness 插件市场 / 插件商店：自动收集与格式校验，免费搜索 API。deepseek1024.com |
| 121 | [Max-Null/dsh-chinese-thinking](https://github.com/Max-Null/dsh-chinese-thinking) | 7 | 2026-08-15 | 2026-08-25 | One-line fix: inject a fixed system-prompt section so the agent always thinks and replies in Chinese, whatever the user's language · 中文思考：注入固定提示词，让 agent 始终用中文思考与回复（无论用户语言） |
| 122 | [MengYuil/dsh-ponytail](https://github.com/MengYuil/dsh-ponytail) | 7 | 2026-08-23 | 2026-08-23 | Lazy senior dev mode for DeepSeek Harness — ponytail port (always-on minimal-code ruleset, /ponytail-review/audit/debt/gain/help) |
| 123 | [RiemannRe3/DSH-RolePlay](https://github.com/RiemannRe3/DSH-RolePlay) | 7 | 2026-08-25 | 2026-08-27 | DeepSeek Harness 的 Tavern 角色卡兼容与原生 Agent RolePlay 插件。 |
| 124 | [sensedeal/cue-skills](https://github.com/sensedeal/cue-skills) | 7 | 2026-05-20 | 2026-08-24 | Cue Skills for Agents |
| 125 | [Tianbuyu-wwx/DSH-FormatForge](https://github.com/Tianbuyu-wwx/DSH-FormatForge) | 7 | 2026-06-10 | 2026-08-25 | FormatForge — DeepSeek Harness plugin: drag any file (PDF/DOCX/XLSX/EML…, 30+ formats) into dsh and it becomes AI-readable structured data. npm: @tianbuyu-wwx/dsh-formatforge |
| 126 | [Wenaixi/dsh-superpower](https://github.com/Wenaixi/dsh-superpower) | 7 | 2026-08-21 | 2026-08-22 | DSH port of obra/superpowers — 完整移植、中文化、DSH 原生 |
| 127 | [wowyuarm/dsh-agent-team](https://github.com/wowyuarm/dsh-agent-team) | 7 | 2026-08-23 | 2026-08-24 | Help humans organize tasks and let agents collaborate: durable Workspaces, Channels, Tasks, and managed Agent members for DeepSeek Harness |
| 128 | [artec/clat](https://github.com/artec/clat) | 6 | 2025-12-07 | 2026-08-23 | Cmd-Line Agent, a Rust foundation compatible with the DeepSeek Harness framework. 命令行智能体，兼容深度探索驾具的 Rust 基座。 |
| 129 | [chenzheshushi-commits/dsh-evolve](https://github.com/chenzheshushi-commits/dsh-evolve) | 6 | 2026-08-23 | 2026-08-23 | Self-evolving memory + skill lifecycle for DeepSeek Harness — durable cross-session memory with zero-token deterministic recall, tiered approval, reinforcement learning from repetition, and anti-bloat convergence for both skills and memory. |
| 130 | [fb0sh/dsh-pentester](https://github.com/fb0sh/dsh-pentester) | 6 | 2026-08-19 | 2026-08-29 | 基于 DeepSeek Harness 的多 Agent PTES 渗透测试编排插件，支持自动化侦察、漏洞分析、验证与报告，使用 Docker/Kali 隔离工具箱 \| Multi-agent PTES penetration testing plugin for DeepSeek Harness with automated recon, vulnerability analysis, validation, reporting, and Docker/Kali toolbox |
| 131 | [fuzhengwei/walioffice-dsh-plugin](https://github.com/fuzhengwei/walioffice-dsh-plugin) | 6 | 2026-08-19 | 2026-08-22 | Deepseek Harness Walioffice 办公软件 插件 |
| 132 | [Hanmiao33/dsh-bubble-explain](https://github.com/Hanmiao33/dsh-bubble-explain) | 6 | 2026-08-23 | 2026-08-24 | bubble-explain |
| 133 | [liceses/dsh-workspace-tree](https://github.com/liceses/dsh-workspace-tree) | 6 | 2026-08-18 | 2026-08-30 | 把 DSH Web 左侧栏的「工作区」重做为文件系统树双模式。核心原则： 工作区 = 目录强绑定——会话的 cwd 就是它所在的目录，环境真正隔离。 |
| 134 | [Physicolor/dsh-widgets](https://github.com/Physicolor/dsh-widgets) | 6 | 2026-08-15 | 2026-08-22 | Right-hand widget rail for DeepSeek Harness Web UI: live session stats (turns, LLM/tool time, TTFT, speed, cache, tokens) plus OpenCode Go quota via a same-origin host proxy; extensible widget registry. |
| 135 | [picoaide/picoaide-harness](https://github.com/picoaide/picoaide-harness) | 6 | 2026-08-16 | 2026-08-23 | PicoAide Harness：企业级 DeepSeek Harness 一体化平台。桌面客户端 + 本地智能体引擎 + 管理后台，支持私有化部署。 |
| 136 | [ppy-web/dsh-plugin-xiaomi-mimo-tts](https://github.com/ppy-web/dsh-plugin-xiaomi-mimo-tts) | 6 | 2026-08-20 | 2026-08-28 | 给DSH接入免费的 Xiaomi MiMo TTS API，支持使用预置/自定义声音朗读正文 |
| 137 | [qishuilalala/dsh-voice-mode](https://github.com/qishuilalala/dsh-voice-mode) | 6 | 2026-08-22 | 2026-08-23 | DSH 语音双工对话模式：流式 zipformer2 识别入可编辑草稿，可选唤醒词，Edge TTS 按句朗读 + 实时字幕，开口即打断（barge-in），无需 API Key。Full-duplex voice mode for DeepSeek Harness, no API key. |
| 138 | [SpookySandwich/dsh-plugin-message-edit](https://github.com/SpookySandwich/dsh-plugin-message-edit) | 6 | 2026-08-21 | 2026-08-22 | DSH 消息编辑插件：编辑已发送的消息并从该处分叉对话，气泡下方带版本计数与树状视图。Edit a sent message and branch from that point — version counter, tree view, placement presets. |
| 139 | [yyyy231209/ai-company-framework](https://github.com/yyyy231209/ai-company-framework) | 6 | 2026-08-18 | 2026-08-24 | Company Is a Word. 一句话开一家AI公司 - open-source multi-agent orchestration framework for non-developers. 小白5分钟拥有自己的AI公司，可DIY任意行业、调教子Agent、无限家公司，支持飞书遥控。MIT |
| 140 | [zrk222/code-factory](https://github.com/zrk222/code-factory) | 6 | 2026-07-08 | 2026-08-22 | Catch AI-generated tests that could never fail; wrap agent changes in local proof and evidence. Free core; proposed evidence-gated enterprise support SLA. |
| 141 | [zzhang82/Agent-Memory-Bridge](https://github.com/zzhang82/Agent-Memory-Bridge) | 6 | 2026-04-05 | 2026-08-23 | Persistent engineering memory for coding agents over MCP. |
| 142 | [AgentsDanceAI/deepseek-harness-cloud](https://github.com/AgentsDanceAI/deepseek-harness-cloud) | 5 | 2026-08-21 | 2026-08-22 | Accounts, credits and cloud agent workspaces for DeepSeek Harness — run it as a hosted product, or self-host in 5 minutes. |
| 143 | [baihui-ai/a2ui-render-in-dsh](https://github.com/baihui-ai/a2ui-render-in-dsh) | 5 | 2026-08-24 | 2026-08-25 | Interactive A2UI cards for the dsh web UI — quizzes, forms, charts and diagrams rendered inline in the conversation, with a full action loop back to the agent. |
| 144 | [caob23/dsh-browser-control](https://github.com/caob23/dsh-browser-control) | 5 | 2026-08-22 | 2026-08-23 | Chrome 浏览器扩展 + DeepSeek Harness 插件，让 AI Agent 直接操控你的真实浏览器。 |
| 145 | [CREAIT-nl/dsh-plugins](https://github.com/CREAIT-nl/dsh-plugins) | 5 | 2026-08-22 | 2026-08-23 | Plugins for DeepSeek Harness: deep research as an agent preset, per-model generation limits, Claude Code hook compatibility, and web fetch/search tools. |
| 146 | [dat-lequoc/dsh-kiro](https://github.com/dat-lequoc/dsh-kiro) | 5 | 2026-08-24 | 2026-08-25 | Kiro provider for DeepSeek Harness with Builder ID login, live model discovery, and reasoning effort controls |
| 147 | [EachSheep/dsh-mario-pixel-skin](https://github.com/EachSheep/dsh-mario-pixel-skin) | 5 | 2026-08-16 | 2026-08-23 | Unofficial Mario-inspired pixel-adventure skin for DeepSeek Harness. |
| 148 | [FuqiangCraft/dsh-desktop](https://github.com/FuqiangCraft/dsh-desktop) | 5 | 2026-08-24 | 2026-08-24 | Desktop companion plugin and native shell for DeepSeek Harness (DSH) |
| 149 | [hanxuanliang/dsh-chaos](https://github.com/hanxuanliang/dsh-chaos) | 5 | 2026-08-15 | 2026-08-23 | Durable multi-agent collaboration for DeepSeek Harness: channels, threads, tasks, and resumable agent sessions. |
| 150 | [HuaJi2077/empty-fort-strategy](https://github.com/HuaJi2077/empty-fort-strategy) | 5 | 2026-08-29 | 2026-08-29 | DSH插件，感受空城计的巧妙，消耗多余的Token。 |
| 151 | [Jason-skd/dsh-session-fork](https://github.com/Jason-skd/dsh-session-fork) | 5 | 2026-08-20 | 2026-08-22 | Makes the branch the building block of AI conversation management — parallel workflows, continuous and mergeable conversation memory |
| 152 | [JasonWei04/dsh-computer-use](https://github.com/JasonWei04/dsh-computer-use) | 5 | 2026-08-18 | 2026-08-22 | computer-use in dsh |
| 153 | [jiazz197-cmyk/omd-dsh](https://github.com/jiazz197-cmyk/omd-dsh) | 5 | 2026-08-23 | 2026-08-29 | Multi-mode agent presets for DeepSeek Harness — per-mode model routing + tiered subagent delegation. |
| 154 | [JohnnyTing/dsh-official-homepage-theme](https://github.com/JohnnyTing/dsh-official-homepage-theme) | 5 | 2026-08-24 | 2026-08-24 | 复刻 DeepSeek Harness 官方首页主题插件 |
| 155 | [keman-ai/dsh-skin-pack](https://github.com/keman-ai/dsh-skin-pack) | 5 | 2026-08-26 | 2026-08-27 | A full set of skins for DeepSeek Harness — one repository, each theme installable on its own |
| 156 | [LaoYueHanNi/dsh-git-worktree](https://github.com/LaoYueHanNi/dsh-git-worktree) | 5 | 2026-08-16 | 2026-08-30 | 在 Web 界面进行分支切换与 git worktree 隔离的 DSH 插件 |
| 157 | [lo2589/deepseek-harness-media](https://github.com/lo2589/deepseek-harness-media) | 5 | 2026-08-14 | 2026-08-24 | use glm/minimax/openai/claude api in your deepseek harness |
| 158 | [lunaship/dsh-links](https://github.com/lunaship/dsh-links) | 5 | 2026-08-18 | 2026-08-22 | Android companion for DeepSeek Harness: trusted-LAN pairing, mobile sessions, SSE approvals, experimental tunnels, and a planned DSH Links Relay. |
| 159 | [lw-storm/dsh-plugin-masterprompt](https://github.com/lw-storm/dsh-plugin-masterprompt) | 5 | 2026-08-27 | 2026-08-28 | This plugin is used for custom persona configuration. It facilitates users in code development and customized‑role setup, and supports flexible persona adjustments for each conversation. |
| 160 | [lxfu1/dsh-plugin-chart](https://github.com/lxfu1/dsh-plugin-chart) | 5 | 2026-08-21 | 2026-08-24 | DeepSeek Harness plugin that bundles the AntV chart visualization skill and a native chart-generation tool. |
| 161 | [monotykamary/dsh-factory](https://github.com/monotykamary/dsh-factory) | 5 | 2026-08-23 | 2026-08-24 | Durable dependency-graph task factory for DeepSeek Harness: recurring Agent work, safe checkout lanes, first-class queues, Triage, and artifacts. |
| 162 | [Moon-shiyue/dsh-github-connect](https://github.com/Moon-shiyue/dsh-github-connect) | 5 | 2026-08-22 | 2026-08-23 | 便携式 GitHub 连接插件 for DeepSeek Harness (DSH)：composer 左下角一键授权，AI 可通过 github_api 工具操作你的 GitHub。Portable GitHub connection plugin: OAuth device flow / PAT, proxy & system-CA aware. |
| 163 | [newborne/dsh-adb-ultimate](https://github.com/newborne/dsh-adb-ultimate) | 5 | 2026-08-19 | 2026-08-25 | Full-featured ADB device management plugin for DeepSeek Harness - control your Android device via AI |
| 164 | [nisconder/npm-safe-forDSH](https://github.com/nisconder/npm-safe-forDSH) | 5 | 2026-08-19 | 2026-08-23 | DeepSeek Harness plugin that checks npm packages before install — 22 supply-chain rules, deep tarball scans, CI gates, local-first. |
| 165 | [NOirBRight/dsh-mobile](https://github.com/NOirBRight/dsh-mobile) | 5 | 2026-08-15 | 2026-08-24 | Android client and Host pairing plugin for DeepSeek Harness |
| 166 | [ParticleLight/dsh-all-usage](https://github.com/ParticleLight/dsh-all-usage) | 5 | 2026-08-17 | 2026-08-29 | DeepSeek Harness 用量看板 / Usage dashboard: tokens, cache, model/provider/workspace analytics, DeepSeek balance, heatmap, and CSV export. |
| 167 | [ParticleLight/dsh-browser-plus](https://github.com/ParticleLight/dsh-browser-plus) | 5 | 2026-08-21 | 2026-08-22 | Enhanced shared browser for DeepSeek Harness: visible + AI-driven WebContentsView, ego-style page chrome, operation trail, JS dialog auto-accept, per-task windows & spaces, Electron 42.x pinned |
| 168 | [peterwangze/dsh-novel-writing](https://github.com/peterwangze/dsh-novel-writing) | 5 | 2026-08-21 | 2026-08-22 | DSH (DeepSeek Harness) 自动化小说写作发布流水线插件：claude-writing-workflow 迁移版 agent 预设 + 小说工作台（可视化/实时渲染/章节编辑）+ 多平台发布配置与数据驱动优化闭环 |
| 169 | [Phant0Meow/dsh-meow-cachebilling](https://github.com/Phant0Meow/dsh-meow-cachebilling) | 5 | 2026-08-22 | 2026-08-23 | 一个能帮你省钱的插件！缓存其实比你想象的贵！换窗口可以省缓存钱，但换窗口有顾虑，或许你懒得重新描述项目和规则，或者你还需要那个上下文。所以这个插件，就是为了告诉你，当前轮，纯粹上下文缓存的部分，到底花了你多少钱。这样你才心里有个底，判断什么时候该换窗口。 在dsh-plugin标签里全网找了，那么多计费插件，并没有人写这一项……真奇怪，难道只有我有这个需求吗？ |
| 170 | [rayafriandion/dsh-oc-tui](https://github.com/rayafriandion/dsh-oc-tui) | 5 | 2026-08-15 | 2026-08-24 | The plugin can use terminal UI like opencode/claude code and other CLI/TUI agents. |
| 171 | [recoluan/recowork](https://github.com/recoluan/recowork) | 5 | 2026-07-06 | 2026-08-27 | Give your AI a workflow. |
| 172 | [rogerdigital/dsh-searxng](https://github.com/rogerdigital/dsh-searxng) | 5 | 2026-08-16 | 2026-08-29 | DeepSeek Harness (dsh) plugin that adds a SearXNG-backed web_search provider to the ctx.web seam — free, self-hosted, key-less search instead of paid Exa/Perplexity APIs. |
| 173 | [See-Sol-Lab/DeepSeekGUI](https://github.com/See-Sol-Lab/DeepSeekGUI) | 5 | 2026-08-17 | 2026-08-27 | A Windows desktop client for DeepSeek Harness. V1 wraps the official Web UI; v2 (independent workbench) in development. |
| 174 | [sheep-programmer/dsh-web-search-free](https://github.com/sheep-programmer/dsh-web-search-free) | 5 | 2026-08-22 | 2026-08-22 | DSH 插件：免费网页搜索，双免费后端（Parallel 默认 + Exa 备用，均匿名免 key）+ 设置开关 + MCP server 双传输（stdio + HTTP/SSE 双端口），兼容 Claude Code / Codex \| Free web search for DeepSeek Harness: Parallel (default) + Exa (backup) free providers, settings toggle, and dual-transport MCP server (stdio + HTTP/SSE) for Claude Code / Codex |
| 175 | [skymecode/dsh-deep-diving](https://github.com/skymecode/dsh-deep-diving) | 5 | 2026-08-20 | 2026-08-22 | plugin for dsh deep diving  |
| 176 | [sqfcyily/dsh-workspace-files](https://github.com/sqfcyily/dsh-workspace-files) | 5 | 2026-08-25 | 2026-08-25 | 在DeepSeek Harness Web GUI 中浏览工作区的目录/文件，并结合 Git 显示文件改动。 |
| 177 | [suntianc/dsh-antigravity-auth](https://github.com/suntianc/dsh-antigravity-auth) | 5 | 2026-08-21 | 2026-08-22 | DeepSeek Harness plugin for Antigravity OAuth login and native Antigravity Auth capability bundle |
| 178 | [tta-lab/organon](https://github.com/tta-lab/organon) | 5 | 2026-03-18 | 2026-08-30 | Structure-aware tools for AI agents. Tree-sitter code editing, web page navigation, search. No daemon, no JSON, just stdin. |
| 179 | [Wenaixi/dsh-ponytail](https://github.com/Wenaixi/dsh-ponytail) | 5 | 2026-08-21 | 2026-08-22 | DSH 完整移植版 DietrichGebert/ponytail — 懒惰 senior 模式，hook注入 |
| 180 | [WSL043/dsh-chat-manager](https://github.com/WSL043/dsh-chat-manager) | 5 | 2026-08-15 | 2026-08-27 | 已归档：DeepSeek Harness 会话搜索、恢复与安全永久删除插件；现有 Release 保留，不再适配未来 DSH。 |
| 181 | [xiaosurongjia/dsh-improved-inline-edit](https://github.com/xiaosurongjia/dsh-improved-inline-edit) | 5 | 2026-08-28 | 2026-08-29 |  当你的DSH正在工作时，你可以不用停止对话就可以再次提出要求 |
| 182 | [xinchen03/minta](https://github.com/xinchen03/minta) | 5 | 2026-05-31 | 2026-08-23 | The context quality layer for AI agents — memory that checks itself: lifecycle governance, calibrated confidence, and   staged claim gates. Local-first, MCP 19 tools, DeepSeek Harness plugin. |
| 183 | [yu-wenchao/dsh-free-models-hub](https://github.com/yu-wenchao/dsh-free-models-hub) | 5 | 2026-08-26 | 2026-08-26 | 免费模型排行榜 · DeepSeek Harness 社区插件，在 DeepSeek Harness (DSH) Web UI 左侧边栏提供「免费模型榜」：分页浏览（每页 20 条、页码窗口、首页/末页）、 点击标题展开 API 调用地址 / 模型名称 / 【点击这里申请免费密钥key】按钮， 并支持一键配置到 设置 → 模型 → 自定义提供方 —— 用户只需自行粘贴免费 API Key |
| 184 | [ZekaiShi/evo-subagent](https://github.com/ZekaiShi/evo-subagent) | 5 | 2026-08-22 | 2026-08-24 | Unified DeepSeek Harness plugin: role-based subagent routing + per-agent evolution (prefercmd/memory as knowledge allow/deny lists), so repeated tasks start from proven commands and save tokens. Unified subagent routing and evolution: prefercmd/memory serve as knowledge allow/deny lists, saving tokens. |
| 185 | [zhouzhencheng07/dsh-kit](https://github.com/zhouzhencheng07/dsh-kit) | 5 | 2026-08-13 | 2026-08-23 | Page capability kit for DeepSeek Harness (dsh): terminal dock, file tree, source control, skills manager, phone access, background jobs and keyless web search in the browser UI |
| 186 | [zmh2000829/DSH-agent-bridge](https://github.com/zmh2000829/DSH-agent-bridge) | 5 | 2026-08-23 | 2026-08-23 | Use Grok Build inside DeepSeek Harness Web through ACP |
| 187 | [zmm863-commits/dsh-paperclip](https://github.com/zmm863-commits/dsh-paperclip) | 5 | 2026-08-16 | 2026-08-25 | DSH Web GUI paperclip button: a single 📎 button in the composer that opens a file picker (drag & drop supported) and inserts file contents into the textarea. 在 DSH Web 输入框右侧添加回形针按钮，点击选择/拖拽文件，内容自动插入输入框。 |
| 188 | [1Lyn-en/dsh-whale](https://github.com/1Lyn-en/dsh-whale) | 4 | 2026-08-15 | 2026-08-24 | DeepSeek Harness 极简回复插件，提供六档精简模式与 CyberUI 主题，可节省 60–75% 输出 Token｜A DSH plugin with six brevity modes and a CyberUI theme. |
| 189 | [ai-eks/dsh-docking-layout](https://github.com/ai-eks/dsh-docking-layout) | 4 | 2026-08-21 | 2026-08-29 | Organize unlimited conversation tabs into editor-style, drag-to-split groups for DeepSeek Harness Web. |
| 190 | [AlexPeng07/dsh-custom-plugin](https://github.com/AlexPeng07/dsh-custom-plugin) | 4 | 2026-08-22 | 2026-08-23 | dsh-custom-plugin是一个为 DeepSeek Harness (DSH) Web GUI 打造的增强插件。提供：背景天气特效/玻璃拟态、时间线轨道、项目文件夹、提示词库、对话导出、Mermaid 图表渲染、引用回复、余额查询与每日 Token 用量面板等多种便利功能 |
| 191 | [Azzygoatcoder/agent-useful-skills](https://github.com/Azzygoatcoder/agent-useful-skills) | 4 | 2026-06-17 | 2026-08-24 | 模块化 AI 科研/工程技能 monorepo（DeepSeek Harness / Claude Code 通用）— plugins/ + skills/ + bin 脚本 + LaTeX 模板，验证环驱动 |
| 192 | [Baisbt/dsh-GreaterClarity-plugin](https://github.com/Baisbt/dsh-GreaterClarity-plugin) | 4 | 2026-08-23 | 2026-08-23 | 对话快速定位，AI头像，支持导出对话流内容 |
| 193 | [chengdb/dsh-plugin-capability-panel](https://github.com/chengdb/dsh-plugin-capability-panel) | 4 | 2026-08-21 | 2026-08-26 | 在 Web GUI 里可视化管理项目的全部能力——Skills、MCP 服务器、快捷消息， 全部支持项目级 / 全局级双作用域，全部可以不离开浏览器完成安装、启停与分发 |
| 194 | [chipweaver/veripower](https://github.com/chipweaver/veripower) | 4 | 2026-06-11 | 2026-08-25 | An open-source agent flow from natural language spec through Verilog RTL and UVM verification to front-end signoff on commercial EDA tools |
| 195 | [clclyzybzjsq/deepseek-harness-yunoseek](https://github.com/clclyzybzjsq/deepseek-harness-yunoseek) | 4 | 2026-08-23 | 2026-08-23 | 一个基于tv动画yumemita中的人物千石由乃，使用剧照素材，应用于deepseek-harness的自定义配色插件；A custom color scheme plugin for deepseek-harness, based on the character Yuno Sengoku from the TV anime "Yumemita" |
| 196 | [cloveric/tarocub](https://github.com/cloveric/tarocub) | 4 | 2026-04-08 | 2026-08-29 | Feishu/Lark-first local AI agent gateway and native DeepSeek Harness plugin for Codex, Claude Code, Kimi Code, DeepSeek Harness, and Antigravity; Telegram optional. |
| 197 | [CWNU-Open-Source-Community/dsh-webgate](https://github.com/CWNU-Open-Source-Community/dsh-webgate) | 4 | 2026-08-16 | 2026-08-22 | DSH 远程访问插件：内网二维码 / cloudflared 隧道 / frp+自有服务器（含登录门户） |
| 198 | [ddtcorex/maestro-skills](https://github.com/ddtcorex/maestro-skills) | 4 | 2026-05-25 | 2026-08-22 | Universal AI Agent Development Skills Hub & Cordis Plugin for Govard, Magento 2, Laravel. Works with Claude Code, Codex CLI, OpenCode, GitHub Copilot, DeepSeek Harness. |
| 199 | [Decrabbityyy/dsh-discovery](https://github.com/Decrabbityyy/dsh-discovery) | 4 | 2026-08-19 | 2026-08-23 | DeepSeek Harness model discovery plugins for local engines and API gateways |
| 200 | [Drhushi/dsh-plugin-tav2](https://github.com/Drhushi/dsh-plugin-tav2) | 4 | 2026-08-25 | 2026-08-28 | DeepSeek Harness 插件 —— 对话式游戏本地化：跟 AI 助手说说话，完成游戏翻译全流程。引擎适配器架构，首发支持 Ren'Py。 |
| 201 | [edge-sky/dsh-oauth-adapter](https://github.com/edge-sky/dsh-oauth-adapter) | 4 | 2026-08-22 | 2026-08-24 | A OAuth adapter for DSH |
| 202 | [fashionmascherine-svg/dsh-polymarket-knowhow](https://github.com/fashionmascherine-svg/dsh-polymarket-knowhow) | 4 | 2026-08-22 | 2026-08-23 | DeepSeek Harness plugin (dsh-plugin): complete Polymarket superpowers — 31 verified tools across Gamma/CLOB/Data-API/Perps/RFQ/Bridge, embedded knowhow skill, live WebSocket stream. Read-only by default. |
| 203 | [fengyungithub/dsh-short-video-studio](https://github.com/fengyungithub/dsh-short-video-studio) | 4 | 2026-08-25 | 2026-08-25 | 基于deepseek harness和ComfyUI的AI视频创作工作台 |
| 204 | [Flycat43/liang-desktop-pet](https://github.com/Flycat43/liang-desktop-pet) | 4 | 2026-08-23 | 2026-08-24 | An unofficial desktop companion UI for DeepSeek Harness.梁圣 |
| 205 | [flymysql/dsh-memory](https://github.com/flymysql/dsh-memory) | 4 | 2026-08-14 | 2026-08-30 | DeepSeek Harness 跨会话记忆库：memory_remember/recall/forget 三个工具 + 系统提示注入，agent 持久化记忆 |
| 206 | [fxylabs/superself](https://github.com/fxylabs/superself) | 4 | 2026-07-23 | 2026-08-23 | The open Company State Runtime — version control for your project's state. Goals, decisions, work, and evidence outlive every chat, context window, and agent session. Ships the self CLI. |
| 207 | [GooDAnDReaDY/dsh-russian-lang](https://github.com/GooDAnDReaDY/dsh-russian-lang) | 4 | 2026-08-23 | 2026-08-23 | Russian localization for DeepSeek Harness web UI: adds Русский language option, translates core + plugin namespaces, Russian plural forms and typography. |
| 208 | [Guard42/dsh-humanize](https://github.com/Guard42/dsh-humanize) | 4 | 2026-08-24 | 2026-08-24 | Humanize 模式 — humanfia 流理念 × DeepSeek Harness 的 agent 预设：Flow 编排 · SHA-256 流锁 · HMAC 评审门禁 · 事件回放恢复 · 一行命令安装 · 可定制领域变体 |
| 209 | [guoxiucai/dsh-code](https://github.com/guoxiucai/dsh-code) | 4 | 2026-08-16 | 2026-08-28 | pi tui  style code agent base on deepseek harness |
| 210 | [Hilbert-beinghappy/dsh-plugin-clarify](https://github.com/Hilbert-beinghappy/dsh-plugin-clarify) | 4 | 2026-08-20 | 2026-08-22 | Off-transcript clarification Host plugin for DeepSeek Harness |
| 211 | [huang-chunc/dsh-user-message-timeline](https://github.com/huang-chunc/dsh-user-message-timeline) | 4 | 2026-08-22 | 2026-08-26 | dsh Web 悬浮药丸导轨：预览·跳转·分页，设置-插件-插件配置可切换左右贴边 |
| 212 | [Innocent-children/dev-flow](https://github.com/Innocent-children/dev-flow) | 4 | 2026-08-14 | 2026-08-22 | Local process control and recovery for Codex and DeepSeek Harness: explicit scope, verification budgets, and durable task state. |
| 213 | [JopenChen/dsh-go](https://github.com/JopenChen/dsh-go) | 4 | 2026-08-30 | 2026-08-31 | dsh-go 是一个纯 Go、进程内的 DeepSeek Harness Agent 实现 —— 让任意 Go 后端能以内嵌库的方式直接获得一个等价、具备规划能力的 Agent，无需界面、无需独立运行时。它不是又一个 ReAct 骨架，而是对 DSH 全量能力接缝的系统级复刻。 |
| 214 | [KannaKuron/dsh-gitbash-shell](https://github.com/KannaKuron/dsh-gitbash-shell) | 4 | 2026-08-23 | 2026-08-23 | DSH plugin: Git Bash shell for all agent modes on Windows (replaces pwsh executor) |
| 215 | [LaoQianwocao/dsh-sound-player](https://github.com/LaoQianwocao/dsh-sound-player) | 4 | 2026-08-22 | 2026-08-23 | DSH Web 音效播放器（设置页管理）：对话完成、发送消息、权限请求、被提问、服务终止、子代理运行完成、最后一个子代理运行完成等 7 类场景触发提示音；内置 Web Audio 合成音效与 Windows 系统提示音，可导入自定义音频并逐项绑定；提供 soundPlayer API 供其他插件集成 |
| 216 | [Lukeknow0/dsh-side-chat](https://github.com/Lukeknow0/dsh-side-chat) | 4 | 2026-08-21 | 2026-08-24 | Read-only side chat plugin for DeepSeek Harness (DSH) — ask temporary questions with inherited context while the parent agent keeps running. |
| 217 | [lutrodev/dsh-roleplay](https://github.com/lutrodev/dsh-roleplay) | 4 | 2026-08-25 | 2026-08-26 | Roleplay plugin suite for DeepSeek Harness: character cards, lorebooks, personas, presets, state, and conversation tools. |
| 218 | [Machine-126/dsh-alert-sound](https://github.com/Machine-126/dsh-alert-sound) | 4 | 2026-08-23 | 2026-08-23 | Notification sound + Chinese voice alerts for the DeepSeek Harness web GUI (approval / answer / completion / error), with a settings page. |
| 219 | [Max-Null/dsh-memory](https://github.com/Max-Null/dsh-memory) | 4 | 2026-08-15 | 2026-08-25 | Cross-session plaintext memory for DeepSeek Harness: suggested → human-approved, searchable, human owns the data · 跨会话明文记忆：模型写入待审核、人工确认生效，明文可审计 |
| 220 | [maxwell-feng/dsh-searxng-web](https://github.com/maxwell-feng/dsh-searxng-web) | 4 | 2026-08-22 | 2026-08-23 | DeepSeek Harness plugin: back the native web_search / web_fetch tools with your self-hosted SearXNG instance — keyless, private, no third-party search vendor. |
| 221 | [megatronyy/dsh-tradingagents](https://github.com/megatronyy/dsh-tradingagents) | 4 | 2026-08-22 | 2026-08-22 | TradingAgents for DeepSeek Harness: the 14-role A-share multi-agent analysis pipeline behind /trading-agent |
| 222 | [null119/dsh-mcp-manage](https://github.com/null119/dsh-mcp-manage) | 4 | 2026-08-17 | 2026-08-30 | DSH（DeepSeek Harness）Web GUI 插件：在设置页管理 MCP 服务器——列出已安装工具，添加/编辑/删除、启用/停用；组合配置提供的 MCP 同样可在运行时直接编辑、停用、移除并恢复，无需重启宿主。 |
| 223 | [Ottohere-Mourn/TeachReplay](https://github.com/Ottohere-Mourn/TeachReplay) | 4 | 2026-08-22 | 2026-08-22 | Teach once, replay anywhere — harness-agnostic Teach-by-Demonstration engine (Record → Compile → Replay → Verify) with OpenMausBot and DeepSeek Harness integrations. |
| 224 | [pgmi-builds/better-dsh](https://github.com/pgmi-builds/better-dsh) | 4 | 2026-08-16 | 2026-08-28 | Make your dsh ready for serious coding tasks. (Tools x Schemas)^REPL. skill://, ctx://, agent://, dvc://, dsh://, IPython REPL, Context as Variables, cross compaction recallable, full context revive. hash-edit, dvc://browser, subagent as a function, workflow as a function. |
| 225 | [RexCue/dsh-wallpaper](https://github.com/RexCue/dsh-wallpaper) | 4 | 2026-08-14 | 2026-08-30 | Wallpaper skin for the DeepSeek Harness (dsh) web UI: image background with opacity, mask and blur controls. |
| 226 | [scotthuang/agent-knock-knock](https://github.com/scotthuang/agent-knock-knock) | 4 | 2026-05-15 | 2026-08-31 | Control local Codex and Claude Code from OpenClaw through shared tmux terminals, with seamless human-agent handoff. |
| 227 | [Shaky77/weiwen-law-dsh](https://github.com/Shaky77/weiwen-law-dsh) | 4 | 2026-08-19 | 2026-08-27 | 唯稳律 (Weiwen's Law) 白箱风控 DSH 插件 — DeepSeek Harness 因果约束中间件 |
| 228 | [Shrbuz/dsh-session-buddy](https://github.com/Shrbuz/dsh-session-buddy) | 4 | 2026-08-23 | 2026-08-23 | DeepSeek Harness 插件：回复/提问/审批三类会话通知（系统原生 toast）+ 会话内梯子目录导航。DeepSeek Harness plugin: session notifications (reply/ask/approval) with native OS toasts + an in-conversation ladder outline. |
| 229 | [SSShooter/dsh-mindmap-live](https://github.com/SSShooter/dsh-mindmap-live) | 4 | 2026-08-23 | 2026-08-23 | DSH 实时思维导图插件：Agent 与你共编同一棵树，改动即时互相同步，支持停靠分屏与全屏专注两种视图 |
| 230 | [staff-os/dsh-workbench](https://github.com/staff-os/dsh-workbench) | 4 | 2026-08-22 | 2026-08-25 | An enterprise workbench for the DeepSeek Harness: AI employees, knowledge bases, skills, MCP servers and DSH plugins, all manageable from a running session. |
| 231 | [tdyangbo/PianpianUI](https://github.com/tdyangbo/PianpianUI) | 4 | 2026-08-23 | 2026-08-23 | 用于DeepSeek Harness的林翩翩主题UI插件。使用《哀鸿：城破十日记》的角色林翩翩作为页面半透明背景，并支持透明度和深度调节。 |
| 232 | [Tianbuyu-wwx/dsh-hermes-link](https://github.com/Tianbuyu-wwx/dsh-hermes-link) | 4 | 2026-08-23 | 2026-08-24 | Bidirectional bridge between Hermes Agent and DeepSeek Harness (DSH). v0.2.4 — single-bundle Cordis plugin replacing the archived hermes-foundation/-oneshot-arbitrate/-dispatch-bridge triad. |
| 233 | [tingfeng347/dsh-vscode-workbench](https://github.com/tingfeng347/dsh-vscode-workbench) | 4 | 2026-08-23 | 2026-08-24 | 在 DeepSeek Harness 中叠加 VS Code 风格的本地开发工作台。 |
| 234 | [tobysunsun/dsh-code-reading-coach](https://github.com/tobysunsun/dsh-code-reading-coach) | 4 | 2026-08-22 | 2026-08-22 | 代码研读教练：交互式引导研读论文对应的开源代码，五段研读法 |
| 235 | [Vesna-Strivozha/DSH-LLM-wiki-plugin](https://github.com/Vesna-Strivozha/DSH-LLM-wiki-plugin) | 4 | 2026-08-23 | 2026-08-23 | 基于Karpathy的wiki方法论搭建的插件，让你的DSH直接变身成LLM wiki，不需要Obsidian+Claudian插件，国内网络友好 |
| 236 | [vibe-any/dsh-plugin-save-token](https://github.com/vibe-any/dsh-plugin-save-token) | 4 | 2026-08-27 | 2026-08-27 | A DeepSeek Harness (dsh) dynamic plugin that cuts token cost without cutting model intelligence |
| 237 | [VinciBeans/deepseek-plugin-liangwengu](https://github.com/VinciBeans/deepseek-plugin-liangwengu) | 4 | 2026-08-22 | 2026-08-31 | 梁文谷 DSH 插件：在 Web GUI 右上角显示当前算力错峰时段（已适配deepseek 2026.08.22 公布的最新峰谷收费政策，工作日 09:00–12:00 与 14:00–18:00 为梁文峰，其余时间含整个周末为梁文谷），并实时倒计时当前时段剩余时间；谷期跨天计算，直达下一工作日 09:00。 |
| 238 | [vonweller/dsh-skillhub](https://github.com/vonweller/dsh-skillhub) | 4 | 2026-08-24 | 2026-08-24 | Browse skillhub.cn skills and install selected ones into ~/.dsh/skills |
| 239 | [wkscc310/dsh-client-ui-cpa-quota](https://github.com/wkscc310/dsh-client-ui-cpa-quota) | 4 | 2026-08-17 | 2026-08-30 | Easily view your CLiProxyAPI quota in DeepSeek Harness. |
| 240 | [wuliLiuyue/wxpilot](https://github.com/wuliLiuyue/wxpilot) | 4 | 2026-03-24 | 2026-08-22 | wxpilot — A CLI for automating WeChat Mini Programs, built for AI Agents. Lets an Agent drive the WeChat DevTools like a browser — page navigation, element interaction, state reading, network capture & mocking.  面向 AI Agent 的微信小程序自动化 CLI 让 Agent 像操作浏览器一样操作微信开发者工具——页面导航、元素交互、状态读取、网络抓包与 mock。 |
| 241 | [xianrui69/dsh-quick-phrases](https://github.com/xianrui69/dsh-quick-phrases) | 4 | 2026-08-26 | 2026-08-26 | DeepSeek Harness client plugin: quick-phrase chip bar above the composer + /-triggered phrase menu |
| 242 | [xxccdl/deepseek-harness-desktop](https://github.com/xxccdl/deepseek-harness-desktop) | 4 | 2026-08-15 | 2026-08-22 | DeepSeek Harness 桌面版 — Electron 壳层封装 dsh web，集成记忆查看、电脑控制、桌面设置、定时任务、快捷对话、预算血条等桌面插件。DeepSeek Harness Desktop — Electron shell wrapping dsh web with desktop-only plugins: memory viewer, computer use, desktop settings, scheduler, quick chat, and usage bar. |
| 243 | [yailPeralta/ast-mcp-server](https://github.com/yailPeralta/ast-mcp-server) | 4 | 2026-08-03 | 2026-08-29 | Correctness-oriented MCP server and batch CLI for compact structural reads and reviewed TypeScript/JavaScript edits. |
| 244 | [yangbobo2021/relay-dsh-plugin-claude](https://github.com/yangbobo2021/relay-dsh-plugin-claude) | 4 | 2026-08-23 | 2026-08-26 | Claude Code integration plugin for DeepSeek Harness, providing native Claude conversations powered by the Claude Agent SDK, with approvals, session continuity, and DSH tool support. |
| 245 | [yangbobo2021/relay-dsh-plugin-codex](https://github.com/yangbobo2021/relay-dsh-plugin-codex) | 4 | 2026-08-23 | 2026-08-26 | Codex integration plugin for DeepSeek Harness, providing native Codex conversations powered by the Codex App Server, with workspace, terminal, approval, and DSH tool support. |
| 246 | [yxy050208/multisim-mcp](https://github.com/yxy050208/multisim-mcp) | 4 | 2026-08-08 | 2026-08-23 | Unofficial MCP server for AI-driven NI Multisim circuit generation, simulation, data export, and reports |
| 247 | [Z-6354/dsh-version-autoupdate](https://github.com/Z-6354/dsh-version-autoupdate) | 4 | 2026-08-18 | 2026-08-28 | DSH version badge + one-click auto-update (dual-surface Cordis plugin) |
| 248 | [ziduup/dsh-programming-mode](https://github.com/ziduup/dsh-programming-mode) | 4 | 2026-08-24 | 2026-08-24 | DeepSeek Harness 编程模式组合包：标准模式之上强制执行 Superpowers 工程纪律(TDD、系统化调试、先计划后编码、完成前验证、代码审查)与常驻 Ponytail 代码量纪律，内置 20 个技能(14 superpowers + 6 ponytail)，dsh plugin add 一键安装。 |
| 249 | [zilliztech/dsh-milvus](https://github.com/zilliztech/dsh-milvus) | 4 | 2026-08-18 | 2026-08-24 | DeepSeek Harness(DSH) plugin for Milvus |
| 250 | [Zn-Dk/dsh-session-repair](https://github.com/Zn-Dk/dsh-session-repair) | 4 | 2026-08-22 | 2026-08-22 | DSH Web 会话诊断、可信备份与一键安全修复插件。 |
| 251 | [zp-home/dsh-weixin-clawbot](https://github.com/zp-home/dsh-weixin-clawbot) | 4 | 2026-08-21 | 2026-08-22 | Phone-to-DSH control through Tencent's official Weixin ClawBot/iLink channel \| 基于腾讯官方微信 ClawBot/iLink 的 DSH 手机远程控制插件 |
| 252 | [01men/ybkk-AIOS](https://github.com/01men/ybkk-AIOS) | 3 | 2026-08-21 | 2026-08-24 | 企业 AI 资源统一管理平台 —— 13 个 dsh/cordis 插件（IAM/OIDC/MCP/Skill 市场/Agent/审计/计费/插件市场），dsh plugin add 可直接安装 |
| 253 | [0xRabit/dsh-crypto-portfolio](https://github.com/0xRabit/dsh-crypto-portfolio) | 3 | 2026-08-22 | 2026-08-22 | A free, 100% self-hosted DeepSeek Harness plugin that unifies your on-chain and CEX assets. |
| 254 | [1014029855/dsh-context-lens](https://github.com/1014029855/dsh-context-lens) | 3 | 2026-08-23 | 2026-08-23 | Inspect, measure, search, and compare the exact provider-neutral context assembled by DeepSeek Harness. |
| 255 | [AbelKeithsun/dsh-question-nav](https://github.com/AbelKeithsun/dsh-question-nav) | 3 | 2026-08-21 | 2026-08-25 | In-session question minimap for the DeepSeek Harness Web GUI: a vertical column of round dots overlaid on the left edge of the conversation column, one dot per user question — hover enlarges and shows full text, click jumps to that message. |
| 256 | [addozhang/dsh-discord](https://github.com/addozhang/dsh-discord) | 3 | 2026-08-30 | 2026-08-31 | Discord-first adapter for DeepSeek Harness — sessions, streaming, approvals and controls from a Discord guild. |
| 257 | [AI-Scarlett/DSH-Store](https://github.com/AI-Scarlett/DSH-Store) | 3 | 2026-08-16 | 2026-08-25 | DSH STORE — third-party plugin marketplace and guarded lifecycle manager for DeepSeek Harness. |
| 258 | [ai4paper/apaper-plugin](https://github.com/ai4paper/apaper-plugin) | 3 | 2026-05-15 | 2026-08-24 | Claude Code plugin for academic paper authoring: bundles writing/figure/PDF skills with the apaper-mcp server. |
| 259 | [AlexKaiqi/dsh-multi-model-provider](https://github.com/AlexKaiqi/dsh-multi-model-provider) | 3 | 2026-08-17 | 2026-08-24 | Model catalog, portraits, Agent selection, and multimodal runtimes for DeepSeek Harness |
| 260 | [AndrasSama/dsh-omp-advisor](https://github.com/AndrasSama/dsh-omp-advisor) | 3 | 2026-08-24 | 2026-08-25 | Ward concil is oh-my-pi advisor subsystem ported to DeepSeek Harness — independent reviewer models watch your agent and advise it (nit injects, concern/blocker steer) it also include an auto resume and git checkpoints |
| 261 | [AngelosZou/dsh-python-env](https://github.com/AngelosZou/dsh-python-env) | 3 | 2026-08-16 | 2026-08-25 | Workspace-scoped Python virtual environment management for a DeepSeek Harness project — discover, create, install into, and remove virtual environments without sandbox, network, or subprocess pitfalls. |
| 262 | [AnLifeX/dsh-credits](https://github.com/AnLifeX/dsh-credits) | 3 | 2026-08-17 | 2026-08-29 | DeepSeek Harness（dsh web）额度插件：跟随当前模型显示官方余额或 OpenCode Go 订阅用量，支持本会话估算、跨会话累计消耗与可视化设置。 |
| 263 | [anweat/dsh-context-console](https://github.com/anweat/dsh-context-console) | 3 | 2026-08-22 | 2026-08-22 | Complete context workbench for DeepSeek Harness: trajectory, inventory, cache history, message forge, and session-log recovery |
| 264 | [AQian0/dsh-desktop](https://github.com/AQian0/dsh-desktop) | 3 | 2026-08-14 | 2026-08-23 | 基于Tauri的简易dsh桌面端套壳 \| A simple Tauri-based desktop wrapper for dsh |
| 265 | [better-er/dsh-live-token-stats](https://github.com/better-er/dsh-live-token-stats) | 3 | 2026-08-21 | 2026-08-26 | DSH Web 插件：基于 DeepSeek 官方 BPE 分词表，在 composer 下方实时渲染 token 状态带，显示流式 TPS、输出 token 与首字延迟，并对比上次 step 的估算与实际偏差；纯插件自包含，不改 DSH 源码 |
| 266 | [BigBlueBaby/codex2dsh](https://github.com/BigBlueBaby/codex2dsh) | 3 | 2026-08-24 | 2026-08-25 | 把 Codex（OpenAI Codex CLI / Desktop）的 MCP 服务器、技能、全局指令、记忆与会话历史一键迁移进 DeepSeek Harness（DSH）——可视化面板 + CLI，源码只读、dry-run 预览、密钥按原样迁移。 |
| 267 | [CaiZongyuan/dsh-ag-ui](https://github.com/CaiZongyuan/dsh-ag-ui) | 3 | 2026-08-23 | 2026-08-23 | AG-UI protocol gateway plugin for DeepSeek Harness |
| 268 | [chidaic/dsh-agent-notify](https://github.com/chidaic/dsh-agent-notify) | 3 | 2026-08-22 | 2026-08-22 | DSH Web GUI task-completion notifications: Windows system-level alerts (browser Notification API) when the agent finishes a task or needs your input - click-to-open session, background-only mode, settings page in Settings  |
| 269 | [chidaic/dsh-light-memory](https://github.com/chidaic/dsh-light-memory) | 3 | 2026-08-23 | 2026-08-23 | 轻量记忆系统插件：四个 Markdown 文件（USER/PROJECT/WORKLOG/CONVENTION）+ append/distill 两个动作，零外部部件，prefix-cache 友好 |
| 270 | [chuxumilk/dsh-404-panic-lock](https://github.com/chuxumilk/dsh-404-panic-lock) | 3 | 2026-08-23 | 2026-08-23 | 用DSH 开发的轻量化插件:按 Ctrl+Shift+L 一键把页面伪装成静态 404 截图,暂时锁死鼠标键盘,防止别人乱动电脑 |
| 271 | [DaiYuhangSustc/dsh-cae-plugin](https://github.com/DaiYuhangSustc/dsh-cae-plugin) | 3 | 2026-08-24 | 2026-08-24 | Mochi 🐶 — natural-language CAE plugin for DeepSeek Harness: one sentence in, a full CAD → mesh → solve → post-process pipeline out (CalculiX FEA + OpenFOAM CFD). \| 自然语言驱动的 CAE插件：一句话跑通 CAD → 网格 → 求解 → 后处理全链路（CalculiX 结构 + OpenFOAM CFD）。 |
| 272 | [daizihan233/dsh-my-go](https://github.com/daizihan233/dsh-my-go) | 3 | 2026-08-20 | 2026-08-22 | My tasks, where to GO????? |
| 273 | [DM010727/dsh-cline](https://github.com/DM010727/dsh-cline) | 3 | 2026-08-25 | 2026-08-25 | Deepseek harness 开源插件 — DSH (DeepSeek Harness) + Cline VS Code ecosystem fusion |
| 274 | [dong3434/dsh-auto-maintenance](https://github.com/dong3434/dsh-auto-maintenance) | 3 | 2026-08-24 | 2026-08-24 | DSH Auto Maintenance System - Diagnosis, Fix, Backup, Monitor |
| 275 | [drscrewdriver/dsh-session-search-toggle](https://github.com/drscrewdriver/dsh-session-search-toggle) | 3 | 2026-08-19 | 2026-08-22 | 给 DeepSeek Harness 侧边栏加一个会话内容检索——标题/内容一键切换，还能按用户/回复/工具筛选 |
| 276 | [dushaobindoudou/dsh-freeroute](https://github.com/dushaobindoudou/dsh-freeroute) | 3 | 2026-08-21 | 2026-08-26 | dsh free token route |
| 277 | [dygin/dsh-recover-context](https://github.com/dygin/dsh-recover-context) | 3 | 2026-08-19 | 2026-08-23 | dsh agent context make recover or reedit |
| 278 | [EasyTZ/dsh-desktop](https://github.com/EasyTZ/dsh-desktop) | 3 | 2026-08-20 | 2026-08-31 | Deepseek-Harness-Desktop |
| 279 | [EL4CTEO/roblox-devforum-mcp](https://github.com/EL4CTEO/roblox-devforum-mcp) | 3 | 2026-03-30 | 2026-08-30 | Give your AI coding agent the Roblox DevForum and official creator docs — check if a bug is already known, read the accepted answer, and verify APIs before writing Luau. |
| 280 | [enterhalf/dsh-web-network-optimizer](https://github.com/enterhalf/dsh-web-network-optimizer) | 3 | 2026-08-21 | 2026-08-22 | dsh网页端网络优化：通过缓存与压缩技术降低传输，从而大幅提升网页加载速度；同时提供网络断连指示与自动断网重连功能。非常适合追求极致性能或网络不稳定用户使用。Network optimization for the DSH web UI: reduces transfer size with caching and compression to greatly speed up page loading, plus a connection-drop indicator and automatic reconnection. Ideal for users pursuing peak performance or using unstable networks. |
| 281 | [ericw0315/dsh-usage-lite](https://github.com/ericw0315/dsh-usage-lite) | 3 | 2026-08-21 | 2026-08-22 | 为 DeepSeek Harness Web 界面提供简洁、优雅的余额与 Token 用量面板。  Compact provider balances and local token-usage analytics for the DeepSeek Harness Web UI. |
| 282 | [EternalNight996/dsh-theme](https://github.com/EternalNight996/dsh-theme) | 3 | 2026-08-22 | 2026-08-23 | DeepSeek Harness theme skin plugin - built-in themes / static image / dynamic 360-follow video. |
| 283 | [etony668/dsh-task-board](https://github.com/etony668/dsh-task-board) | 3 | 2026-08-23 | 2026-08-24 | DSH 项目任务看板插件：会话「任务看板」视图 + 父子任务树工具与技能 + 本地 JSON 存储（CodexFF 移植） |
| 284 | [exoticknight/dsh-labnana](https://github.com/exoticknight/dsh-labnana) | 3 | 2026-08-22 | 2026-08-22 | Labnana image generation for DeepSeek Harness: text-to-image / image-to-image / precise editing — chat image cards, credentials-domain API key, settingsScope UI |
| 285 | [f20880479-lab/dsh-peak-gate](https://github.com/f20880479-lab/dsh-peak-gate) | 3 | 2026-08-25 | 2026-08-25 | DeepSeek Harness 峰谷计费插件：高峰时段发送前确认（可勾选本次高峰段内不再提示），支持将消息排队到空闲时段（半价）自动发送；可拖拽悬浮队列窗口、调整发送顺序与时间。 |
| 286 | [faith1688/dsh-usage-meter-harness](https://github.com/faith1688/dsh-usage-meter-harness) | 3 | 2026-08-17 | 2026-08-25 | 专为 DeepSeek API 打造的实时用量 / 费用 / 余额计量插件 —— 在聊天输入框旁直接看到 tokens、花费与真实余额。 |
| 287 | [Fakek0f3sT/dsh-mcp-diff](https://github.com/Fakek0f3sT/dsh-mcp-diff) | 3 | 2026-08-27 | 2026-08-27 | Uniform diff cards for every file mutation in DeepSeek Harness Web — MCP filesystem (edit_file/write_file) and built-in edit/write, collapsed by default, with per-line highlighting |
| 288 | [FAVKTOXIC/dsh-theme-liquid-glass](https://github.com/FAVKTOXIC/dsh-theme-liquid-glass) | 3 | 2026-08-23 | 2026-08-24 | Apple Liquid Glass theme for DeepSeek Harness |
| 289 | [fengb3/dsh-session-icons](https://github.com/fengb3/dsh-session-icons) | 3 | 2026-08-22 | 2026-08-31 | DSH（DeepSeek Harness）Web 界面的会话标题图标插件：当模型为一次新会话生成标题时，宿主半用同一条路由发起一次辅助小请求，让模型按标题画一枚 24×24 单色 SVG 隐喻图标；浏览器半把它注入到左侧会话列表每行标题的左侧，跟随主题色。 |
| 290 | [Frog755/dsh-prompt-vault](https://github.com/Frog755/dsh-prompt-vault) | 3 | 2026-08-22 | 2026-08-22 | Prompt Vault: 输入框上方的提示词库（DSH 插件）— 📚 按钮展开面板，点条目一键填入 prompt。DeepSeek Harness prompt library plugin. |
| 291 | [GM-HZ/agent-dag-workflow](https://github.com/GM-HZ/agent-dag-workflow) | 3 | 2026-08-23 | 2026-08-29 | Host-neutral durable DAG workflows for Agents: CLI-native access, fixed MCP gateway, on-demand Skills, triggers, replay, and visual Canvas. |
| 292 | [guyuefangyuanl/dsh-memory](https://github.com/guyuefangyuanl/dsh-memory) | 3 | 2026-08-21 | 2026-08-22 | Cross-session persistent memory for the DeepSeek Harness: a model-facing memory tool, an always-on index section, and a bundled maintenance skill. |
| 293 | [gwsbhqt/dsh-insight](https://github.com/gwsbhqt/dsh-insight) | 3 | 2026-08-25 | 2026-08-27 | 洞察 — read-only insight panel for a DeepSeek Harness profile: where every plugin, service, tool and model came from, which config layer inserted or disabled it, and what is running right now. |
| 294 | [HaoyueQin/dsh-diff-stat](https://github.com/HaoyueQin/dsh-diff-stat) | 3 | 2026-08-24 | 2026-08-25 | DeepSeek Harness web plugin: inline +N −M diff badges on edit/write tool rows and a per-turn file change summary card. Scroll-windowed diffs, PTC/code-dispatch fallback, undo — no git required. |
| 295 | [harryopo/dsh-cloud-workspaces](https://github.com/harryopo/dsh-cloud-workspaces) | 3 | 2026-08-14 | 2026-08-31 | Cloud workspaces for DeepSeek Harness — pick Cloud (SSH) in the workspace picker and the agent's bash/read/write/edit/glob/grep tools transparently run on your Linux server over SSH. Zero remote install. |
| 296 | [Hilbert-beinghappy/dsh-plugin-auxiliary-runtime](https://github.com/Hilbert-beinghappy/dsh-plugin-auxiliary-runtime) | 3 | 2026-08-21 | 2026-08-22 | Auxiliary inference usage, limits, and cancellation runtime for official DeepSeek Harness plugins |
| 297 | [huyang218/dsh-desktop](https://github.com/huyang218/dsh-desktop) | 3 | 2026-08-17 | 2026-08-23 | Unofficial macOS/Windows desktop app for DeepSeek Harness (dsh): manages the runtime, supervises the server, and puts the web UI in a real window. |
| 298 | [hyrinx/dsh-plugin-open-with](https://github.com/hyrinx/dsh-plugin-open-with) | 3 | 2026-08-22 | 2026-08-25 | 在DeepSeek Harness Web 会话头部添加胶囊拆分按钮，一键在当前工作区打开VS Code、终端（CMD / PowerShell）和文件资源管理器。 |
| 299 | [imkelt/DSH-RAG](https://github.com/imkelt/DSH-RAG) | 3 | 2026-08-22 | 2026-08-24 | Local knowledge bases with explicit, source-backed retrieval for DeepSeek Harness Web. |
| 300 | [imkingjh999/dsh-deepsea](https://github.com/imkingjh999/dsh-deepsea) | 3 | 2026-08-23 | 2026-08-23 | DSH plugin: 深海摸鱼 —— context 越深潜得越深，答完摸鱼集镭射生物卡 \| Deep-sea slacking holo cards |
| 301 | [J0ss077/dsh-always-require-tools-approval](https://github.com/J0ss077/dsh-always-require-tools-approval) | 3 | 2026-08-24 | 2026-08-24 | Stop. Confirm. Run. A DeepSeek Harness plugin that pauses selected tools and waits for your explicit approval before every execution. |
| 302 | [Jarad-z/dsh-goalmesh](https://github.com/Jarad-z/dsh-goalmesh) | 3 | 2026-08-23 | 2026-08-24 | Goal-driven multi-agent orchestration for DeepSeek Harness — bounded DAG scheduling, nested delegation, typed evidence, and durable trajectory UI. |
| 303 | [JasonQQ/dsh-btw-plugin](https://github.com/JasonQQ/dsh-btw-plugin) | 3 | 2026-08-24 | 2026-08-25 | Codex-style /btw command for DeepSeek Harness: side questions answered in a conversation-seeded subagent context, without polluting the main context |
| 304 | [JimChen-g/dsh-action-outbox](https://github.com/JimChen-g/dsh-action-outbox) | 3 | 2026-08-16 | 2026-08-26 | Batch Review Inbox for DeepSeek Harness — stage, inspect, edit, approve, and commit exact tool side effects safely. |
| 305 | [jinxlux/xiao-theme-dsh-ui-plugin](https://github.com/jinxlux/xiao-theme-dsh-ui-plugin) | 3 | 2026-08-23 | 2026-08-29 | UI plugin for deepseek harness web |
| 306 | [joekytc/dsh-swarm](https://github.com/joekytc/dsh-swarm) | 3 | 2026-08-20 | 2026-08-24 | Run multi-agent task pipelines on DSH like a team — plan, execute, review, and deliver code through a visual kanban with provable completion. |
| 307 | [k-ying/dsh-vsceditor](https://github.com/k-ying/dsh-vsceditor) | 3 | 2026-08-25 | 2026-08-25 | DeepSeek Harness 内嵌 VSCode 编辑器插件：嵌入完整 code-server，agent 写文件时自动弹出红绿 diff 跟随（edit sync / file locking / follow mode） |
| 308 | [Kian-Oraish/dsh-prompt-enchant](https://github.com/Kian-Oraish/dsh-prompt-enchant) | 3 | 2026-08-23 | 2026-08-25 | 增强提示词魔法棒:DSH Web 对话输入框的灵活自适应提示词增强插件 |
| 309 | [lifeopsgo/dsh-capability-toggle-plugin](https://github.com/lifeopsgo/dsh-capability-toggle-plugin) | 3 | 2026-08-22 | 2026-08-22 | Toggle individual agent capabilities (skills, MCP, tools, prompt, approval, guards) from the DSH WebUI composer — session / project / global. DSH 各种能力（mcp/skill/tool等）多层级开关灵活控制 |
| 310 | [LINinLIN-0079/godot-asset-planner-public](https://github.com/LINinLIN-0079/godot-asset-planner-public) | 3 | 2026-08-21 | 2026-08-24 | Godot asset & project-goal management for DeepSeek Harness: godot_* model tools, /gap REST API, and a better-sidebar UI with asset manager, scene-tree viewer and Git panel. / DeepSeek Harness 的 Godot 资产与项目目标统一管理插件：godot_* 模型工具 + /gap REST 路由 + better-sidebar 界面（资产管理器 / 场景树查看器 / Git 版本控制）。 |
| 311 | [linxuhao/AItelier](https://github.com/linxuhao/AItelier) | 3 | 2026-04-04 | 2026-08-25 | AI-Atelier, the all in one personal "atelier" (means handcraft studio in french) that can adapt to your need. |
| 312 | [lispking/dsh-auto-evolve](https://github.com/lispking/dsh-auto-evolve) | 3 | 2026-08-22 | 2026-08-22 | A self-evolving plugin for DeepSeek Harness (dsh). It observes how the agent runs, proposes improvements to its own assets via the LLM, validates each proposal inside a sandboxed trial agent, and applies only verified mutations — with a versioned ledger and automatic rollback on regression. |
| 313 | [liyi3068238601-oss/dsh-comfyui-ctl](https://github.com/liyi3068238601-oss/dsh-comfyui-ctl) | 3 | 2026-08-31 | 2026-08-31 | Native DeepSeek Harness plugin for controlling ComfyUI queues, history, outputs, models, uploads, and generation. |
| 314 | [loadingvx/deepseeh-harness-ultra-slash](https://github.com/loadingvx/deepseeh-harness-ultra-slash) | 3 | 2026-08-17 | 2026-08-23 | /steer commands for deepseek-harness |
| 315 | [loeanxi/dsh-injection-guard](https://github.com/loeanxi/dsh-injection-guard) | 3 | 2026-08-19 | 2026-08-22 | Source-aware prompt injection protection for DeepSeek Harness |
| 316 | [log-li/dsh-automode](https://github.com/log-li/dsh-automode) | 3 | 2026-08-21 | 2026-08-22 | Claude Code-style auto approval layer for DeepSeek Harness: deterministic rules + two-stage classifier, circuit breaker, fail-to-human. Shadow mode day one. |
| 317 | [loyalchiiina/dsh-chat-image-lightbox](https://github.com/loyalchiiina/dsh-chat-image-lightbox) | 3 | 2026-08-23 | 2026-08-23 | DSH plugin: display images inline in chat with lightbox zoom, download (save-as), and prev/next navigation |
| 318 | [luxueliu/luxueliu-usage-command](https://github.com/luxueliu/luxueliu-usage-command) | 3 | 2026-08-20 | 2026-08-22 | 内置DSH指令，一键展示今日全局付费模型总消耗账单（人民币版）！按模型×分小时查当日¥消费，缓存命中/未命中/输出三档单价，官方/中转/套餐全覆盖 — DeepSeek Harness 插件 |
| 319 | [lxxz1918/dsh-theme-customizer](https://github.com/lxxz1918/dsh-theme-customizer) | 3 | 2026-08-22 | 2026-08-22 | DeepSeek Harness（DSH）Web 界面自定义主题插件：背景/文字/框线/细节全可视化调整，可导入导出预设，持久化保存。 |
| 320 | [mantonlove/dsh-prism-plugin](https://github.com/mantonlove/dsh-prism-plugin) | 3 | 2026-08-18 | 2026-08-26 | Prism · 棱镜 — a deeply customizable glassmorphism theme plugin for the DeepSeek Harness Web GUI |
| 321 | [MaRi23333/dsh-subagent-library](https://github.com/MaRi23333/dsh-subagent-library) | 3 | 2026-08-22 | 2026-08-23 | DeepSeek Harness 具名子代理库插件：settings 驱动的角色名册，list_subagents / delegate 工具与设置页。Named subagent roster plugin for DeepSeek Harness. |
| 322 | [Max-Null/dsh-draft-polish](https://github.com/Max-Null/dsh-draft-polish) | 3 | 2026-08-21 | 2026-08-25 | Draft polish for DeepSeek Harness: one-click LLM polish of your draft in the composer, rewrites it in place with session context · 草稿润色：发送前一键调用 LLM 润色草稿，结果回填输入框 |
| 323 | [maxmilian/dsh-sonarqube](https://github.com/maxmilian/dsh-sonarqube) | 3 | 2026-08-24 | 2026-08-24 | Read-only SonarQube Community Build tools for DeepSeek Harness |
| 324 | [modelbus/deepseek-harness-pro](https://github.com/modelbus/deepseek-harness-pro) | 3 | 2026-08-21 | 2026-08-23 | deepseek-harness-pro 是基于 deepseek-harness 的 Web+Electron 客户端，兼容已有的deepseek-harness环境，并支持一键部署最新版deepseek-harness。相比原web功能做出增强：新增实时任务看板、电脑管家（清理/调优/进程管理）、独立插件中心等功能。界面友好，跨平台，开源免费，让 deepseek-harness 更强大易用。 |
| 325 | [MoonlitDropOfBlood/dsh-agent-approval](https://github.com/MoonlitDropOfBlood/dsh-agent-approval) | 3 | 2026-08-18 | 2026-08-23 | DSH 的自动审批权限插件 |
| 326 | [MoonlitDropOfBlood/dsh-archive-manager](https://github.com/MoonlitDropOfBlood/dsh-archive-manager) | 3 | 2026-08-18 | 2026-08-23 | DSH的归档管理插件 |
| 327 | [MoonlitDropOfBlood/dsh-memory-manager](https://github.com/MoonlitDropOfBlood/dsh-memory-manager) | 3 | 2026-08-18 | 2026-08-23 | DSH基本的记忆功能 |
| 328 | [MoonlitDropOfBlood/dsh-token-stats](https://github.com/MoonlitDropOfBlood/dsh-token-stats) | 3 | 2026-08-18 | 2026-08-23 | dsh的token消耗的统计插件 |
| 329 | [MrmoLabs/dsh-mermaid](https://github.com/MrmoLabs/dsh-mermaid) | 3 | 2026-08-23 | 2026-08-23 | Render Mermaid code blocks as SVG diagrams in DeepSeek Harness Web, with diagram/code switching, streaming support, dark mode, strict security, and npm/GitHub installation. |
| 330 | [nicecx/dsh-relay](https://github.com/nicecx/dsh-relay) | 3 | 2026-08-18 | 2026-08-24 | DSH plugin: relay approval & question requests to any chat channel — iMessage, Email, WeChat built-in; Telegram/DingTalk/Feishu/Slack via a common adapter contract (src/channels/types.js) |
| 331 | [ningbonb/dsh-client-ui-brand](https://github.com/ningbonb/dsh-client-ui-brand) | 3 | 2026-08-26 | 2026-08-26 | Custom product name and logo branding for DeepSeek Harness Web 自定义 DeepSeek Harness Web 端 logo 和产品名称 |
| 332 | [nxz1026/dsh-tray](https://github.com/nxz1026/dsh-tray) | 3 | 2026-08-19 | 2026-08-22 | DeepSeek Harness — Custom Windows Tray Launcher |
| 333 | [papachong/deepseek-harness-tui](https://github.com/papachong/deepseek-harness-tui) | 3 | 2026-08-21 | 2026-08-25 | This is a standalone terminal for deepseek-harness (designed based on a plug-in approach), updated in sync with the official deepseek-harness repository, and inherits the capabilities of the official product. |
| 334 | [PenguinAndy/dsh-ezcommit-plugin](https://github.com/PenguinAndy/dsh-ezcommit-plugin) | 3 | 2026-08-22 | 2026-08-22 | One-click Git commit plugin for DSH: the session model splits workspace changes into reviewed Conventional Commits batches, with built-in sensitive-file filtering. |
| 335 | [pg527322814/dsh-bayes-predict](https://github.com/pg527322814/dsh-bayes-predict) | 3 | 2026-08-21 | 2026-08-22 | dsh-贝叶斯个股预测插件：多指标信号融合的上涨概率估计、趋势状态识别与持仓风险度量（A 股 + 美股） |
| 336 | [QinpanWan/dsh-hiboard-push](https://github.com/QinpanWan/dsh-hiboard-push) | 3 | 2026-08-23 | 2026-08-27 | Push task-completion messages to the Huawei HarmonyOS assistant-today (负一屏) card feed from DeepSeek Harness — wire-compatible with the OpenClaw today-task skill. |
| 337 | [qinyre/dsh-plugin-atlas](https://github.com/qinyre/dsh-plugin-atlas) | 3 | 2026-08-18 | 2026-08-23 | Archive manager (browse / unarchive / auto-rules) plus a Codex-style fisheye conversation rail for dsh.·归档管理与对话刻度尺插件 |
| 338 | [reatcat/l123-harness](https://github.com/reatcat/l123-harness) | 3 | 2026-08-22 | 2026-08-22 | L1-L2-L3 三级记忆 agent 底座：门禁、事件日志、周审提炼、TDD 执行流。Claude Code 插件。 |
| 339 | [rebron1900/dsh-mnemosyne](https://github.com/rebron1900/dsh-mnemosyne) | 3 | 2026-08-22 | 2026-08-23 | Mnemosyne 记忆层在 DeepSeek Harness 中的插件 — 本地优先、SQLite 支持的跨会话记忆。 |
| 340 | [robbywang25/dsh-codex-pins](https://github.com/robbywang25/dsh-codex-pins) | 3 | 2026-08-22 | 2026-08-25 | Codex-style pinned sessions for DeepSeek Harness — always visible above the sidebar list |
| 341 | [ruisenbai/dsh-annotation](https://github.com/ruisenbai/dsh-annotation) | 3 | 2026-08-17 | 2026-08-23 | Inline, batchable comments for DeepSeek Harness assistant replies |
| 342 | [sakthiveltofficial/dsh-git-plugins](https://github.com/sakthiveltofficial/dsh-git-plugins) | 3 | 2026-08-22 | 2026-08-22 | dsh-git: Git & source-control plugin suite for DeepSeek Harness — local git + GitHub/GitLab/Bitbucket/Azure DevOps/Gitea + self-evolving memory |
| 343 | [shangjian2023/dsh-rss-daily](https://github.com/shangjian2023/dsh-rss-daily) | 3 | 2026-08-22 | 2026-08-22 | dsh plugin: 46-source daily RSS digest, LLM-edited, delivered via webhook (ServerChan/PushDeer/WxWork/TG/Bark/gotify) |
| 344 | [SKzrui/DSH-CLI](https://github.com/SKzrui/DSH-CLI) | 3 | 2026-08-14 | 2026-08-22 | DSH‑CLI：轻量命令行，流式输出、工具调用、按目录恢复会话，密钥与模型灵活配置，一条命令对话 DeepSeek Harness。 \|  Lightweight CLI for DeepSeek Harness – streaming, tool calling, per‑dir session recovery, flexible config. Start with one command. |
| 345 | [SoMarkAI/dsh-tool-somark](https://github.com/SoMarkAI/dsh-tool-somark) | 3 | 2026-08-14 | 2026-08-24 | SoMark document parser tool (somark_parse) plugin for DeepSeek Harness |
| 346 | [soyoungzsy/soya-workflows](https://github.com/soyoungzsy/soya-workflows) | 3 | 2026-08-20 | 2026-08-21 | 🏭 SOYA Workflows — enterprise workflow skills for DeepSeek Harness: notify (webhook), docs (Yuque API), intel (RSS), report (daily/weekly/monthly).  企业工作流四件套 AI 技能。 |
| 347 | [Star-Guest/dsh-plugin-tavern](https://github.com/Star-Guest/dsh-plugin-tavern) | 3 | 2026-08-22 | 2026-08-22 | 酒馆（SillyTavern 精简版）DSH 插件：角色卡解析管理员 card-analyst + 角色扮演讲述者 roleplay |
| 348 | [SuCriss/dsh-leekbox](https://github.com/SuCriss/dsh-leekbox) | 3 | 2026-08-26 | 2026-08-26 | 韭菜盒子 LeekBox — A股看盘助手 · DeepSeek Harness (DSH) web 插件 |
| 349 | [sunzhentao/dsh--prompt--enhance](https://github.com/sunzhentao/dsh--prompt--enhance) | 3 | 2026-08-24 | 2026-08-24 | DeepSeek Harness提示词增强插件 |
| 350 | [Tannnnhauser/pivot-web-search](https://github.com/Tannnnhauser/pivot-web-search) | 3 | 2026-05-02 | 2026-08-24 | Resilient multi-provider web search & content extraction for Claude Code, DeepSeek Harness, and any MCP host — quota-aware failover, JS rendering, and a CLI. |
| 351 | [TaoruiLiu19/dsh-gsv](https://github.com/TaoruiLiu19/dsh-gsv) | 3 | 2026-08-25 | 2026-08-25 | 为 DSH (DeepSeek Harness) 打造的语音朗读插件——双模式可选： Edge 云端零配置即用（20+ 免费音色，联网即读）+  GSV 本地离线音色克隆；支持一键朗读、自动朗读、音色市场。 |
| 352 | [tiphareth0/dsh-sshworkspaces](https://github.com/tiphareth0/dsh-sshworkspaces) | 3 | 2026-08-28 | 2026-08-31 | Workspace-level SSH remote development plugin for DeepSeek Harness: transparent seam-routed fs, git & terminal across multiple hosts and workspaces, with a built-in 4-column IDE and SSH ops toolkit. 提供工作区级 SSH 远程开发的Deepseek Harness插件：文件/Git/终端按工作区透明路由，支持多服务器多工作区并行开发，内置四列 IDE 与 SSH 运维工具。 |
| 353 | [tuojc/dsh-browser-firefox](https://github.com/tuojc/dsh-browser-firefox) | 3 | 2026-08-22 | 2026-08-22 | Firefox browser-control plugin for DeepSeek Harness: one DSH plugin + one Firefox extension, driving your own Firefox over a token-authenticated WebSocket. Text-first toolset (snapshot/click/type/navigate/tab-stack) with screenshot as visual fallback. Firefox add-on available on AMO. Ported from Lum1104/dsh-browser (MIT). |
| 354 | [TuringCorp-net/mosaic-memory-compress](https://github.com/TuringCorp-net/mosaic-memory-compress) | 3 | 2026-06-08 | 2026-08-23 | Generic stateless dialogue compression that mimics human memory. LLM conversations stay bounded forever — no session management, no context overflow. Ships a ready-to-use adapter for DeepSeek Harness (DSH). |
| 355 | [UncleK/dsh-think-translate](https://github.com/UncleK/dsh-think-translate) | 3 | 2026-08-24 | 2026-08-26 | Thinking-chain UI translation for DeepSeek Harness: 8 target languages, local Ollama model primary with in-panel download, Google/Bing fallback |
| 356 | [vcxmug/dsh-evo](https://github.com/vcxmug/dsh-evo) | 3 | 2026-08-13 | 2026-08-23 | Native Firecrawl tools for DeepSeek Harness agents via MCP — one composition row, zero custom code |
| 357 | [wackyju2-beep/dsh-better](https://github.com/wackyju2-beep/dsh-better) | 3 | 2026-08-22 | 2026-08-23 | 更好的 DSH \| Unofficial dsh plugin: archived sessions & task notifications / 已归档会话管理 · 任务系统通知 |
| 358 | [Whale-Zhang/dsh-complete-chime](https://github.com/Whale-Zhang/dsh-complete-chime) | 3 | 2026-08-23 | 2026-08-23 | DSH plugin: play a chime when a conversation turn finishes. Built-in tones plus custom upload in Settings → Plugins. |
| 359 | [whisperflo/dsh-deepseek-console](https://github.com/whisperflo/dsh-deepseek-console) | 3 | 2026-08-22 | 2026-08-22 | DeepSeek 账户控制台：实时余额监控 / 用量与成本统计 / 消费额度管理 / 全局悬浮 HUD（官方 API 直连，Key 仅存本机） |
| 360 | [Wike-CHI/dsh-mobile](https://github.com/Wike-CHI/dsh-mobile) | 3 | 2026-08-24 | 2026-08-24 | Mobile device capability plugin for DeepSeek Harness: MobileService seam, mock/mobile-mcp providers, agent tools (observe/open_app/tap/type/back), tiered execution policy |
| 361 | [wuzhigouno-collab/dsh-rp-composer](https://github.com/wuzhigouno-collab/dsh-rp-composer) | 3 | 2026-08-23 | 2026-08-24 | TriComposer · DSH web 端 RP 结构化输入插件：台词/动作/心理分框填空、模板组装发送，从输入层消除 AI 对玩家言行的成分误识别。Structured tri-channel input composer for LLM roleplay on DeepSeek Harness. |
| 362 | [wycto/dsh-dock](https://github.com/wycto/dsh-dock) | 3 | 2026-08-21 | 2026-08-28 | dsh-dock · DeepSeek Harness 功能中枢：用一张管理面板统一注册、开关所有小功能（模型余额、Token 用量记录、任务动画等）。每个功能独立模块，支持开关与错误隔离，新功能即插即用。0.1.0 为基础框架，功能接入按 README 路线图迭代。 |
| 363 | [x102201/deepseek-harness-helper](https://github.com/x102201/deepseek-harness-helper) | 3 | 2026-08-25 | 2026-08-27 | 🖥️ 一台电脑无限多开 DeepSeek Harness · 🔀 每个实例=独立一套 dsh · 📐 可拖拽自定义分屏 · 📦 .dshpack 环境打包可卖 · 🪟🍎🐧 Win/macOS/Linux（x64 & ARM） |
| 364 | [xiangrui979/foresight](https://github.com/xiangrui979/foresight) | 3 | 2026-08-22 | 2026-08-22 | ForeSight: a temporal-aspect long-term memory plugin for DeepSeek Harness (dsh) |
| 365 | [Xingkong42/dsh-zh-labels](https://github.com/Xingkong42/dsh-zh-labels) | 3 | 2026-08-21 | 2026-08-22 | DSH 界面中文标签持久化插件 - Persistent Chinese UI labels for DeepSeek Harness |
| 366 | [xxccdl/DeepSeek-Harness-Mobile](https://github.com/xxccdl/DeepSeek-Harness-Mobile) | 3 | 2026-08-21 | 2026-08-23 | 在 Android 手机上运行 DeepSeek Harness AI 助手的 React Native 应用，内置 Termux + proot-distro 完整 Linux 环境，无需 root，支持手机控制 |
| 367 | [yamingmou/dsh-retrace](https://github.com/yamingmou/dsh-retrace) | 3 | 2026-08-19 | 2026-08-25 | Recall (撤回), edit-and-resend (编辑重发) and regenerate (重新生成) for DeepSeek Harness conversation messages — Web and Desktop plugin |
| 368 | [yangdongzhen590/dsh-knj-scheduler](https://github.com/yangdongzhen590/dsh-knj-scheduler) | 3 | 2026-08-23 | 2026-08-24 | Cron task scheduler for DeepSeek Harness: scheduled sessions with your prompt, workspace-aware placement, paginated execution history, open-session from the panel. |
| 369 | [yangdongzhen590/dsh-knj-workflow](https://github.com/yangdongzhen590/dsh-knj-workflow) | 3 | 2026-08-23 | 2026-08-24 | Config-driven development-task orchestration plugin for DeepSeek Harness: workflows + task management + stage progress UI. |
| 370 | [YiMlT/dsh-notify-yimit](https://github.com/YiMlT/dsh-notify-yimit) | 3 | 2026-08-22 | 2026-08-22 | DeepSeek Harness 通知插件:在 **任务完成 / 任务出错 / 运行中 / 等待审批 / 等待回答** 时提醒用户。 通知标题为对话标题;系统通知与自定义通知均支持**点击跳转到对应会话**。 |
| 371 | [Young4ever33/dsh-token-attention](https://github.com/Young4ever33/dsh-token-attention) | 3 | 2026-08-22 | 2026-08-22 | Token Check · 词元管理：DeepSeek Harness (DSH) 的 token 注意力管理面板——按任务/日/周/月记录 token 消耗与费用（命中/未命中/输出/推理），支持 DeepSeek 峰谷计价，并给出换对话、写 hand-off 的执行时机建议。 |
| 372 | [Yurzi/dsh-pdf-mineru](https://github.com/Yurzi/dsh-pdf-mineru) | 3 | 2026-08-24 | 2026-08-24 | Provider-independent DSH PDF parsing tools powered by MinerU. |
| 373 | [z-col/dsh-workspace-groups](https://github.com/z-col/dsh-workspace-groups) | 3 | 2026-08-21 | 2026-08-22 | DeepSeek Harness web client plugin: group sidebar workspaces into a configurable three-level tree (分类→项目→会话). Sidecar YAML rules. dsh-plugin. |
| 374 | [zh851233/docs-mode](https://github.com/zh851233/docs-mode) | 3 | 2026-08-25 | 2026-08-27 | You can use this plugin to complete the writing of technical documents, including development briefs, user manuals, reports/summary materials, and interface/API documentation, while reducing traces of AIGC. |
| 375 | [zhengjy01/dsh-skill-studio](https://github.com/zhengjy01/dsh-skill-studio) | 3 | 2026-08-23 | 2026-08-23 | Skill studio for DeepSeek Harness: visualize, edit and enable/disable agent skills from the web settings panel and via skillmgr_* tools |
| 376 | [zyh20041227/improved_vision_for_deepseek](https://github.com/zyh20041227/improved_vision_for_deepseek) | 3 | 2026-08-22 | 2026-08-23 | Full-coverage image tiling for DeepSeek Harness vision models, dense-text OCR, and document AI |
| 377 | [0neKbyte/dsh-approval-assistant_0neKbyte](https://github.com/0neKbyte/dsh-approval-assistant_0neKbyte) | 2 | 2026-08-23 | 2026-08-24 | deepseek 审批+问答+完成时添加提醒，可设置浏览器、系统通知、弹窗通知，可自拟音效 |
| 378 | [0QwQ0/dsh-discord-richpresence](https://github.com/0QwQ0/dsh-discord-richpresence) | 2 | 2026-08-22 | 2026-08-24 | dsh-plugin: push vague, user-configurable DSH interaction states to local Discord as Rich Presence |
| 379 | [173787247/dsh-wsl-open](https://github.com/173787247/dsh-wsl-open) | 2 | 2026-08-27 | 2026-08-27 | DeepSeek Harness plugin: open WSL Linux paths from chat in Windows. |
| 380 | [240xu/dsh-websearch](https://github.com/240xu/dsh-websearch) | 2 | 2026-08-20 | 2026-08-22 | Unified web search provider for DSH |
| 381 | [452926826/dsh-at-skill](https://github.com/452926826/dsh-at-skill) | 2 | 2026-08-25 | 2026-08-26 | Invoke DeepSeek Harness skills with @name and composer suggestions |
| 382 | [88514205-oss/dsh-ryoshu-slash](https://github.com/88514205-oss/dsh-ryoshu-slash) | 2 | 2026-08-16 | 2026-08-25 | DSH plugin: 天殺拔刀斬——带斩击特效的文件删除工具，强制审查防误删；official bundle, install via `dsh plugin --profile web add` github:88514205-oss/dsh-ryoshu-slash |
| 383 | [9931666/dsh-plugin-roundtable](https://github.com/9931666/dsh-plugin-roundtable) | 2 | 2026-08-22 | 2026-08-29 | （roundtable V0.2.2）把一次 DeepSeek Harness 会话，从"你和 AI 一对一聊天"，升级成"你 + 主持人(DeepSeek) + 一圈专家 AI 开圆桌会 |
| 384 | [afoxsss/dsh-conversation-map](https://github.com/afoxsss/dsh-conversation-map) | 2 | 2026-08-24 | 2026-08-24 | 会话地图（Conversation Minimap）—— DeepSeek Harness (dsh) Web 客户端插件。 |
| 385 | [ai-yukin/dsh-0-tools](https://github.com/ai-yukin/dsh-0-tools) | 2 | 2026-08-20 | 2026-08-25 | Zero-cost, zero-hassle toolkit for DeepSeek Harness (DSH): one-click free model setup (Zhipu GLM-4-Flash + OpenRouter Ox-Alpha) for complete beginners. 小白零门槛零费用套件。 |
| 386 | [Alain-Prot0s5/dsh-screenshot](https://github.com/Alain-Prot0s5/dsh-screenshot) | 2 | 2026-08-21 | 2026-08-22 | DeepSeek Harness Desktop 截图自动粘贴插件（需安装 DSH Desktop 版，仅 Win10/11，纯 AI 生成）：相机按钮 / 全局热键 Alt+A → 系统截图 → 自动粘贴进输入框 \| Screenshot-to-input plugin for DeepSeek Harness Desktop (DSH Desktop app required; Windows 10/11 only; AI-generated): camera button & global hotkey Alt+A -> snip -> auto-paste into composer |
| 387 | [AlexKaiqi/dsh-session-assistant](https://github.com/AlexKaiqi/dsh-session-assistant) | 2 | 2026-08-20 | 2026-08-24 | Session-scoped full-duplex voice assistant for DeepSeek Harness with safe drafting, explicit Agent submission, and optional knowledge curation. |
| 388 | [alextangson/dsh-dispatch](https://github.com/alextangson/dsh-dispatch) | 2 | 2026-08-23 | 2026-08-24 | 📱 Dispatch tasks to DeepSeek Harness (dsh) from your phone — approvals on your lock screen, isolated git worktrees, E2E encrypted, self-hostable. Like Claude Code Dispatch, for dsh. |
| 389 | [Aliuyanfeng/dsh-soul](https://github.com/Aliuyanfeng/dsh-soul) | 2 | 2026-08-31 | 2026-08-31 | The DeepSeek Harness Personalization Settings plugin is used to configure the nickname, response style, tone, and custom commands of the Agent. |
| 390 | [andyfan1094/dsh-codebase-memory](https://github.com/andyfan1094/dsh-codebase-memory) | 2 | 2026-08-21 | 2026-08-22 | DSH bundle that bridges the Codebase Memory MCP code knowledge graph into DSH via the official @deepseek-ai/dsh-mcp-client. |
| 391 | [andyfan1094/dsh-feishu](https://github.com/andyfan1094/dsh-feishu) | 2 | 2026-08-21 | 2026-08-22 | DSH Feishu self-built app integration: WebSocket inbound messages, OK-reaction acknowledgement, and turn replies on the original chat. |
| 392 | [andyfan1094/dsh-github](https://github.com/andyfan1094/dsh-github) | 2 | 2026-08-21 | 2026-08-22 | GitHub authentication and local Git workflow plugin for the dsh web GUI: accounts, repository browsing, clone, pull, push, status, commit, and a settings panel. |
| 393 | [andyfan1094/dsh-winrm](https://github.com/andyfan1094/dsh-winrm) | 2 | 2026-08-21 | 2026-08-22 | Remote Windows administration for the dsh web GUI: WinRM/PowerShell Remoting host config, PowerShell exec, streaming console, service and process management, base64-chunked file transfer, cluster execution, plus agent tools (winrm_list, winrm_exec, winrm_service, winrm_process, winrm_upload, winrm_download, winrm_cluster). Standalone Cordis plugin. |
| 394 | [AnLifeX/dsh-attention](https://github.com/AnLifeX/dsh-attention) | 2 | 2026-08-20 | 2026-08-29 | dsh 提醒插件：别错过需要你的时刻 |
| 395 | [anonRTtty/dsh-api-balance-displayer-plugin](https://github.com/anonRTtty/dsh-api-balance-displayer-plugin) | 2 | 2026-08-24 | 2026-08-24 | DeepSeek API 余额显示插件 / DeepSeek API balance display for DeepSeek Harness |
| 396 | [aorucshiea/dsh-plugin-toggle](https://github.com/aorucshiea/dsh-plugin-toggle) | 2 | 2026-08-24 | 2026-08-25 | Hot-plug enable/disable switches for installed DSH plugins |
| 397 | [aorucshiea/dsh-preset-switch](https://github.com/aorucshiea/dsh-preset-switch) | 2 | 2026-08-24 | 2026-08-25 | Optional mid-session agent-preset switching for DeepSeek Harness |
| 398 | [aorucshiea/dsh-safe-tui](https://github.com/aorucshiea/dsh-safe-tui) | 2 | 2026-08-24 | 2026-08-25 | DeepSeek Harness safe-mode recovery console: minimal TUI, history, repair, model/provider management |
| 399 | [ateen18/dsh-plugin-security-review](https://github.com/ateen18/dsh-plugin-security-review) | 2 | 2026-08-18 | 2026-08-24 | Security review gate for DeepSeek Harness (dsh) plugins: static pre-install vetting of malicious code, vulnerabilities and supply-chain risks (with deobfuscation decoding), runtime audit, optional tool-call guard, and a one-click web review/install/uninstall panel. |
| 400 | [AxelGoal/Deepharn](https://github.com/AxelGoal/Deepharn) | 2 | 2026-08-23 | 2026-08-24 | Un escritorio propio para DeepSeek Harness en macOS: frontend nuevo sobre su API, concha nativa en Swift y dos plugins. |
| 401 | [backrooms-yrc/dsh-openai-gateway](https://github.com/backrooms-yrc/dsh-openai-gateway) | 2 | 2026-08-23 | 2026-08-23 | Expose DeepSeek Harness (dsh) as an OpenAI-compatible API server — /v1/chat/completions + /v1/models, backed by real agent sessions with tools and workspaces. 把 DeepSeek Harness 暴露为 OpenAI 兼容 API 服务端。 |
| 402 | [baosfeng/my-dsh-plugins](https://github.com/baosfeng/my-dsh-plugins) | 2 | 2026-08-22 | 2026-08-22 | DSH（DeepSeek Harness）插件集合仓库：文件活动、思考增强、Mermaid 渲染、通知提醒、插件守护、Skill 管理、任务可靠性、插件开发模式等 8 个插件，独立版本、GitHub Release 发布 |
| 403 | [BaronCyrus/dsh-harness-ally](https://github.com/BaronCyrus/dsh-harness-ally) | 2 | 2026-08-22 | 2026-08-22 | DeepSeek Harness 联盟模式：自由组合 DSH、Claude Code、Codex 与全部已配置模型，保留原生 Agent 生命周期与实时执行过程。 |
| 404 | [BenjaminSHI4008/deepseek-pet-Seeki](https://github.com/BenjaminSHI4008/deepseek-pet-Seeki) | 2 | 2026-08-17 | 2026-08-23 | DeepSeek Harness 桌宠插件：透明置顶的桌面精灵（2D 像素风状态机） |
| 405 | [better-er/dsh-cache-billing](https://github.com/better-er/dsh-cache-billing) | 2 | 2026-08-28 | 2026-08-28 | DSH 缓存账单插件：上下文圆环弹层里实时算账，峰谷自动计价，第三方中转照常记账 |
| 406 | [better-er/dsh-edit-diff](https://github.com/better-er/dsh-edit-diff) | 2 | 2026-08-28 | 2026-08-28 | dsh·去重复 diff 展示插件 |
| 407 | [bettermen/xiashuo](https://github.com/bettermen/xiashuo) | 2 | 2026-08-23 | 2026-08-30 | 虾说教材写作 · dsh-course-writer — AI course-authoring workspace plugin for DeepSeek Harness (DSH). 三栏式工作台 · 九阶段门禁 · 课程/章节/资料库/知识图谱 · 导出 TXT/Word · 分享协作。Three-pane workspace, nine-phase gated workflow, lorebook, export & share. |
| 408 | [blackdm666/dsh-plugin-88api-image](https://github.com/blackdm666/dsh-plugin-88api-image) | 2 | 2026-08-22 | 2026-08-22 | 统一接入 Image2 与 Nano Banana 四款模型，覆盖文生图、多参考图编辑、2K/4K 输出、顺序批量任务、默认模型持久化和脱敏 Key 配置。 |
| 409 | [bluechips-zhao/dsh-receipt](https://github.com/bluechips-zhao/dsh-receipt) | 2 | 2026-08-24 | 2026-08-24 | DeepSeek Harness 对话使用情况记录超市小票插件：按模型统计的令牌使用量、调用次数、耗时和成本 \| Conversation usage receipt plugin for DeepSeek Harness: per-model token usage, calls, time and cost |
| 410 | [BlueChonk/dsh-cli-anything](https://github.com/BlueChonk/dsh-cli-anything) | 2 | 2026-08-27 | 2026-08-27 | 将 CLI-Anything 集成到 DSH (DeepSeek Harness) 的插件方案。安装后通过自然语言对话即可浏览、安装、启动和管理 100+ CLI 工具。 |
| 411 | [bowang-lab/dsh-medomni](https://github.com/bowang-lab/dsh-medomni) | 2 | 2026-08-19 | 2026-08-22 | deepseek harness plugin for medical image analysis |
| 412 | [Carrick-K7/dsh-ai-quota](https://github.com/Carrick-K7/dsh-ai-quota) | 2 | 2026-08-24 | 2026-08-24 | DeepSeek Harness plugin: AI subscription quotas & balances (Codex, Kimi, DeepSeek, OpenCode Go) — model tool, Settings page, composer chip |
| 413 | [caseyyy/dsh-goal-planner](https://github.com/caseyyy/dsh-goal-planner) | 2 | 2026-08-25 | 2026-08-25 | 目标驱动的每日任务计划器：多目标任务数据 + Web 每日预览面板，与微信提醒推送共享数据 · Goal-driven daily task planner for DSH: multi-goal tasks + daily preview panel, one data file with the WeChat reminder pipeline. |
| 414 | [cdxDNRF/dsh-wishadel-theme](https://github.com/cdxDNRF/dsh-wishadel-theme) | 2 | 2026-08-14 | 2026-08-24 | dsh主题维什戴尔风格 |
| 415 | [chenbin-dev/dsh-scan-mcp](https://github.com/chenbin-dev/dsh-scan-mcp) | 2 | 2026-08-23 | 2026-08-23 | 能够扫描本地claudecode、codex、codebuddy等Agent配置过的mcp工具的插件 |
| 416 | [chenjie1129/deepseek-harness-reliability-governor](https://github.com/chenjie1129/deepseek-harness-reliability-governor) | 2 | 2026-08-23 | 2026-08-24 | Evidence-gated completion and trusted code verification for DeepSeek Harness agents |
| 417 | [chensl139-ok/dsh-archived-panel](https://github.com/chensl139-ok/dsh-archived-panel) | 2 | 2026-08-23 | 2026-08-23 | DeepSeek Harness 插件:侧边栏「已归档」面板,可查看/打开/取消归档会话 A side panel that lists, opens, and unarchives archived sessions. |
| 418 | [Chinesezjc/dsh-tool-owned-render](https://github.com/Chinesezjc/dsh-tool-owned-render) | 2 | 2026-08-14 | 2026-08-24 | Design note and interactive prototype for tool-owned render: each tool owns its own result presentation, composing shared layout primitives instead of a central render-kind union. |
| 419 | [Chu-m/dsh-chat-continue](https://github.com/Chu-m/dsh-chat-continue) | 2 | 2026-08-22 | 2026-08-22 | Auto-retry failed API requests to keep DSH conversations going. Supports configurable status codes and error codes.  自动重试失败的 API 请求，让 DSH 对话不中断。支持自定义状态码和错误码。 |
| 420 | [chunfenxiazhi-collab/dsh-stability-audit](https://github.com/chunfenxiazhi-collab/dsh-stability-audit) | 2 | 2026-08-24 | 2026-08-25 | Scan installed dsh plugins and grade stability risk (hook surface, startup work, preflight, deps) with optional isolated install verification |
| 421 | [CJL-1995/dsh-memory-self-evolution](https://github.com/CJL-1995/dsh-memory-self-evolution) | 2 | 2026-08-30 | 2026-08-31 | dsh自动进化记忆系统 |
| 422 | [coldfish486/dsh-anime25d-pets](https://github.com/coldfish486/dsh-anime25d-pets) | 2 | 2026-08-23 | 2026-08-22 | Anime2.5DRig × DSH 桌宠：借助see-through，只凭一张干净背景的图像，即可获得带自动装配、发丝物理、表情动画和状态镜像的桌宠 |
| 423 | [crazy-L118/dsh-deepseek-balance-widget](https://github.com/crazy-L118/dsh-deepseek-balance-widget) | 2 | 2026-08-19 | 2026-08-24 | DeepSeek balance widget for the dsh web sidebar |
| 424 | [Crosery/dsh-viewer](https://github.com/Crosery/dsh-viewer) | 2 | 2026-08-31 | 2026-08-31 | Everything renders: images, video, audio, PDF, Office documents and local web pages inline in the DeepSeek Harness web UI, via a display_file tool. |
| 425 | [d3cker/dsh-open-terminal](https://github.com/d3cker/dsh-open-terminal) | 2 | 2026-08-23 | 2026-08-23 | OpenTerminal support for DeepSeek Harness |
| 426 | [d86e/dsh-doctor](https://github.com/d86e/dsh-doctor) | 2 | 2026-08-27 | 2026-08-27 | dsh-doctor: self-healing watchdog for the DeepSeek Harness web profile. Recovers from plugin-induced boot failures within 60s, runs an unbounded CLI doctor, captures every tool error, and watches all live sessions for stuck turns. |
| 427 | [DamonBao/dsh-dungeon-party](https://github.com/DamonBao/dsh-dungeon-party) | 2 | 2026-08-22 | 2026-08-22 | Safety-first five-agent orchestration plugin for DeepSeek Harness (DSH), with leases, scopes, checkpoints, validation, and recovery. |
| 428 | [ddtcorex/dsh-maestro-memory](https://github.com/ddtcorex/dsh-maestro-memory) | 2 | 2026-08-24 | 2026-08-25 | DSH plugin for durable, cross-session memory & todos — five tracks (global/user/project/key/daily), confirmation-gated writes, Git-backed sync, in-place adoption of ~/.dsh/memories. |
| 429 | [delock/dsh-pr-board](https://github.com/delock/dsh-pr-board) | 2 | 2026-08-26 | 2026-08-26 | Maintainer PR review queue board for DeepSeek Harness: five-state tracking (waiting on me / waiting on author / ready to merge / merged / inbox), sidebar counters, fullscreen kanban, polling, and back-to-you transition toasts. |
| 430 | [DevViking-Persike/dsh-cliproxy](https://github.com/DevViking-Persike/dsh-cliproxy) | 2 | 2026-08-22 | 2026-08-22 | DeepSeek Harness plugin: routes cliproxy-claude and cliproxy-openai through a local CLIProxyAPI, so the agent reaches your own CLI subscriptions |
| 431 | [DevViking-Persike/dsh-subscriptions](https://github.com/DevViking-Persike/dsh-subscriptions) | 2 | 2026-08-23 | 2026-08-24 | DeepSeek Harness plugin: use your own Claude and ChatGPT/Codex subscriptions as model providers, over each vendor's OAuth sign-in |
| 432 | [dingminhua/dsh-subagent-default-model](https://github.com/dingminhua/dsh-subagent-default-model) | 2 | 2026-08-16 | 2026-08-25 | Configurable default model for subagent delegations via settings.yaml, with single-model and multi-model round-robin/random strategies. |
| 433 | [dlssjdyka0019/dsh-launcher](https://github.com/dlssjdyka0019/dsh-launcher) | 2 | 2026-08-24 | 2026-08-24 | 管理多个隔离的 DeepSeek Harness (DSH) 实例的 Windows 桌面工具 |
| 434 | [elviass/dsh-cost-insights](https://github.com/elviass/dsh-cost-insights) | 2 | 2026-08-22 | 2026-08-22 | DeepSeek Harness 的用量、费用、Token、缓存、余额与模型价格分析插件。 |
| 435 | [Emilia-awa/hermes-dsh-bridge](https://github.com/Emilia-awa/hermes-dsh-bridge) | 2 | 2026-08-24 | 2026-08-25 | Hermes ↔ DeepSeek Harness MCP bridge: drive dsh agents (tasks, sessions, files, presets, stats) from any MCP client. Hermes = brain, Harness = arms. |
| 436 | [eomis/packhub-workbench-assistant](https://github.com/eomis/packhub-workbench-assistant) | 2 | 2026-08-23 | 2026-08-23 | DSH Desktop workbench installer, switcher, and updater |
| 437 | [everclear077/dsh-progressive-tools](https://github.com/everclear077/dsh-progressive-tools) | 2 | 2026-08-24 | 2026-08-27 | Progressive tool discovery for DeepSeek Harness — tiny stable surface, searchable catalog, real pipeline execution, context cache intact. |
| 438 | [ExplorerZYzhou/DSH-freeweb](https://github.com/ExplorerZYzhou/DSH-freeweb) | 2 | 2026-08-27 | 2026-08-27 | DSH 免费联网搜索插件（Parallel 后端，零依赖） |
| 439 | [falling-ts/dsh-force-compact](https://github.com/falling-ts/dsh-force-compact) | 2 | 2026-08-23 | 2026-08-26 | Aggressive context compaction for local-first agents. Runs Qwen3.8‑27B on self‑hosted llama.cpp at low context, shrinking history so the live prompt stays small, fast, and private—delivering a big‑window experience without API cost or data egress. 面向本地的激进上下文压缩插件。自托管 llama.cpp 低上下文运行 Qwen3.8‑27B,不断收缩历史、保持常驻 prompt 小而快,兼顾隐私与大窗口体验,零 API 成本、数据不出本机。 |
| 440 | [Fisfzy/dsh-cae-agent](https://github.com/Fisfzy/dsh-cae-agent) | 2 | 2026-08-21 | 2026-08-23 | 让 DeepSeek Harness (DSH) 通过原生工具直接操控本机 Abaqus/CAE 的 Cordis 插件。21 个 DSH 原生工具覆盖完整建模链（几何/材料/网格/接触/分析步/载荷/边界/作业/ODB），TypeScript 编写，socket bridge 直连本机（不走 MCP）。 |
| 441 | [FraYoshi/dsh-ui-models-invert-selection](https://github.com/FraYoshi/dsh-ui-models-invert-selection) | 2 | 2026-08-29 | 2026-08-29 | Invert selection in Deepseek Harness for when we are selecting models  |
| 442 | [Frog755/dsh-hybrid-memory](https://github.com/Frog755/dsh-hybrid-memory) | 2 | 2026-08-24 | 2026-08-24 | Hybrid memory plugin for DeepSeek Harness (DSH): L1 frozen-snapshot memory (MEMORY.md/USER.md, prefix-cache friendly) + L2 searchable knowledge base (facts + SQLite FTS5) + L3 multi-tool import (Hermes/Claude/Codex/WorkBuddy). 混合记忆插件：L1 冻结快照 + L2 可检索知识库 + L3 多工具导入。数据本地存储。 |
| 443 | [fu827707013/dsh-concurrency-guard](https://github.com/fu827707013/dsh-concurrency-guard) | 2 | 2026-08-26 | 2026-08-27 | DSH（DeepSeek Harness）并发请求监控与门闩插件。 |
| 444 | [fufengyuan/dsh-stool-plugin](https://github.com/fufengyuan/dsh-stool-plugin) | 2 | 2026-08-25 | 2026-08-27 | DSH 运维工具箱插件。将 stool 运维 CLI 的全部能力注册为 DSH 模型可调用的工具，无需手动操作即可让 Agent 自动执行服务器管理、日志搜索、数据库查询、CI/CD 部署等操作。 |
| 445 | [gameswu/dsh-human-coding](https://github.com/gameswu/dsh-human-coding) | 2 | 2026-08-26 | 2026-08-26 | DeepSeek Harness 增加古法编程模式，让模型监督你写代码！ |
| 446 | [genesis-agents/dsh-plugins](https://github.com/genesis-agents/dsh-plugins) | 2 | 2026-08-22 | 2026-08-24 | Plugins for DeepSeek Harness: a source library that reads 72 feeds and publishes podcasts, digests and reports, plus web search over Serper, Tavily and Brave |
| 447 | [GooDAnDReaDY/dsh-image-gen](https://github.com/GooDAnDReaDY/dsh-image-gen) | 2 | 2026-08-18 | 2026-08-23 | Image generation for DeepSeek Harness: generate_image tool backed by FAL queue API and OpenAI-compatible endpoints with inline UI preview |
| 448 | [GreenLv/dsh-session-insights](https://github.com/GreenLv/dsh-session-insights) | 2 | 2026-08-21 | 2026-08-22 | Local-first, evidence-backed workflow retrospectives for DeepSeek Harness |
| 449 | [Haniubub/seo-toolkit](https://github.com/Haniubub/seo-toolkit) | 2 | 2026-08-29 | 2026-08-30 | The SEO audit toolkit built for DeepSeek Harness (DSH) — runs locally, no Claude Code, no API key required. Self-contained port of claude-seo v2.2.5: 53 Python scripts + 24 sub-skills + 18 agents, weighted score, gated fan-out, schema.org, E-E-A-T, GBP, GEO/AI Overviews. |
| 450 | [HaoyueQin/dsh-deepseek-monitor](https://github.com/HaoyueQin/dsh-deepseek-monitor) | 2 | 2026-08-22 | 2026-08-22 | DeepSeek Harness web plugin: DeepSeek balance & platform usage monitoring inside the official Settings-Models-DeepSeek card, plus a live balance chip left of the model name in the composer tool row. Ported from DeepSeekMonitorWindows. |
| 451 | [Harvey-Will/dsh-vision-analysis](https://github.com/Harvey-Will/dsh-vision-analysis) | 2 | 2026-08-21 | 2026-08-22 | Vision tools for DeepSeek Harness: OCR, chart extraction, UI review, comparison & image-to-code via OpenAI- or Anthropic-compatible endpoints, with a built-in FREE anonymous vision source and automatic rate-limit failover. 支持 OpenAI/Anthropic 兼容视觉端点。 |
| 452 | [Harzva/dsh-agent-project-sync](https://github.com/Harzva/dsh-agent-project-sync) | 2 | 2026-08-23 | 2026-08-23 | Synchronize Codex and Claude project directories into native DeepSeek Harness workspaces. |
| 453 | [hatanokokosa/dsh-colorschemes](https://github.com/hatanokokosa/dsh-colorschemes) | 2 | 2026-08-22 | 2026-08-22 | A DSH ColorScheme Plugin |
| 454 | [HeyBobChan/canon-deepseek-harness-plugin](https://github.com/HeyBobChan/canon-deepseek-harness-plugin) | 2 | 2026-08-23 | 2026-08-24 | Canon integration plugin for DeepSeek Harness |
| 455 | [hi-fangj/dsh-models-radar](https://github.com/hi-fangj/dsh-models-radar) | 2 | 2026-08-26 | 2026-08-26 | Model capability radar plugin for the DeepSeek Harness Web GUI |
| 456 | [HiQ-AI/dingtalk-dsh-assistant](https://github.com/HiQ-AI/dingtalk-dsh-assistant) | 2 | 2026-08-25 | 2026-08-29 | 基于 DeepSeek Harness 的钉钉群聊常驻个人助理插件 |
| 457 | [HIT-HTML/dsh-ENHANCED](https://github.com/HIT-HTML/dsh-ENHANCED) | 2 | 2026-08-24 | 2026-08-25 | One plugin, every upgrade DeepSeek Harness lacks out of the box: multi-engine web search, skills & MCP managers, per-profile plugin toggles, session cleanup with hover-delete, one-click restart/shutdown, themes. Single tool surface, no telemetry. |
| 458 | [Hou-DL/dsh-token-pulse](https://github.com/Hou-DL/dsh-token-pulse) | 2 | 2026-08-24 | 2026-08-28 | Local Token heatmap plugin for DSH Web — GitHub-style calendar views, per-hour/week/month/quarter/year, fully local, zero billing. |
| 459 | [Howe829/dsh-insider](https://github.com/Howe829/dsh-insider) | 2 | 2026-08-20 | 2026-08-22 | Runtime observability and relationship graph for DeepSeek Harness and Cordis |
| 460 | [huanghai-lab/dsh-custom-instructions](https://github.com/huanghai-lab/dsh-custom-instructions) | 2 | 2026-08-15 | 2026-08-28 | DSH Web 安全自定义指令管理器：编辑全局 AGENTS.md，支持模板、Markdown 预览、历史恢复、导入导出与并发保护。 |
| 461 | [huaxiren6/DSH-EmailReader](https://github.com/huaxiren6/DSH-EmailReader) | 2 | 2026-08-20 | 2026-08-27 | IMAP email reader for DeepSeek Harness: list, read, and search mail via imapflow (email_list / email_read / email_search). |
| 462 | [huaxiren6/DSH-SmsWebhook](https://github.com/huaxiren6/DSH-SmsWebhook) | 2 | 2026-08-20 | 2026-08-27 | SMS forwarding webhook for DeepSeek Harness: receive pushes from phone SMS Forwarder apps, store them, expose sms_recent / sms_search tools. |
| 463 | [huyang218/dsh-plugins](https://github.com/huyang218/dsh-plugins) | 2 | 2026-08-18 | 2026-08-24 | Plugins for DeepSeek Harness (dsh) — 18 build-free ESM bundles: model-facing tools, runtime wrappers and web UI extensions. Installable by name, URL or local path from the dsh CLI, dsh Desktop or dsh Android. |
| 464 | [hw-cola/dsh-dynamic-agents](https://github.com/hw-cola/dsh-dynamic-agents) | 2 | 2026-08-25 | 2026-08-25 | DSH插件，动态AGENTS.md |
| 465 | [hyperion2144/dsh-subagent-pro](https://github.com/hyperion2144/dsh-subagent-pro) | 2 | 2026-08-20 | 2026-08-22 | DSH Web extension: live subagent monitor + role-based subagent routing + Claude Code style .dsh/agents/*.md persona injection |
| 466 | [ianho7/dsh-port-inspector](https://github.com/ianho7/dsh-port-inspector) | 2 | 2026-08-20 | 2026-08-30 | DeepSeek Harness 的 Windows Web 插件，可将本地 TCP 监听回溯至进程、会话与工具调用，保障编程助手安全处理端口冲突/A Windows DSH Web plugin for DeepSeek Harness that traces local TCP listeners back to processes, Sessions, and Tool Calls for safe Coding Agent port-conflict handling. |
| 467 | [iimaguest/phone-tunnel-pool](https://github.com/iimaguest/phone-tunnel-pool) | 2 | 2026-08-23 | 2026-08-28 | Refreshable Cloudflare quick-tunnel pool for the dsh web GUI — phone access with QR + embedded login |
| 468 | [imroc/dsh-project-prompt](https://github.com/imroc/dsh-project-prompt) | 2 | 2026-08-26 | 2026-08-26 | Private, per-project prompt rules for DeepSeek Harness — matched by git remote/repo/path, worktree-aware, never committed to the repo |
| 469 | [inmny/dsh-continue](https://github.com/inmny/dsh-continue) | 2 | 2026-08-24 | 2026-08-25 | 为 DeepSeek Harness 增加一个直接续跑按钮。当会话异常结束时，可以从现有上下文继续执行，不会引入其他提示词。 |
| 470 | [ipromise2021/dsh-omc-tui](https://github.com/ipromise2021/dsh-omc-tui) | 2 | 2026-08-15 | 2026-08-28 | DeepSeek Harness (DSH) 原生全功能终端交互界面 · Claude Code-styled Terminal TUI & CLI for DeepSeek Harness |
| 471 | [iskshadow195563/DeepSeek_Harness_Balance_Banner](https://github.com/iskshadow195563/DeepSeek_Harness_Balance_Banner) | 2 | 2026-08-22 | 2026-08-23 | 💵 DeepSeek 余额横幅(dsh 插件):页面顶部右侧(主题切换按钮左侧)同时显示 USD/CNY 余额,负值高亮,60s 自动刷新,一条命令安装 |
| 472 | [iskshadow195563/DeepSeek_Harness_Files_Panel](https://github.com/iskshadow195563/DeepSeek_Harness_Files_Panel) | 2 | 2026-08-22 | 2026-08-23 | 📁 右侧可折叠的 DeepSeek 上传文件管理面板(dsh 插件):列出/复制/清理 DeepSeek Files API 上传的图片,密钥零暴露,一条命令安装 |
| 473 | [iyam-x/iyam-dsh-desktop](https://github.com/iyam-x/iyam-dsh-desktop) | 2 | 2026-08-24 | 2026-08-22 | a deepseek harness desktop |
| 474 | [jackuh105/dsh-message-edit](https://github.com/jackuh105/dsh-message-edit) | 2 | 2026-08-23 | 2026-08-23 | Edit or undo your sent messages in DeepSeek Harness's Web GUI — hides everything after from chat view and model context. |
| 475 | [jarvisluk/dsh-projectless-session](https://github.com/jarvisluk/dsh-projectless-session) | 2 | 2026-08-18 | 2026-08-26 | Projectless sessions for DeepSeek Harness with isolated date-organized working directories |
| 476 | [JasonFreeLab/dsh-command-code-review](https://github.com/JasonFreeLab/dsh-command-code-review) | 2 | 2026-08-25 | 2026-08-25 | /code-review slash command for DeepSeek Harness — five parallel review lenses, per-finding confidence scoring, then a gh reply back on the pull request. |
| 477 | [JimChen-g/dsh-frontier-repro](https://github.com/JimChen-g/dsh-frontier-repro) | 2 | 2026-08-16 | 2026-08-26 | Evidence-first frontier AI radar and reproducibility gate for DeepSeek Harness |
| 478 | [jing-hy/dsh-unified-market](https://github.com/jing-hy/dsh-unified-market) | 2 | 2026-08-21 | 2026-08-27 | Unified plugin market for DSH Desktop (EAC): curated catalog + GitHub dsh-plugin + npm registry three sources; install/update management and .dshpack feature packs. 统一插件市场（三源聚合，EAC 特化）。 |
| 479 | [jinsiyu/dsh-code-server-app](https://github.com/jinsiyu/dsh-code-server-app) | 2 | 2026-08-25 | 2026-08-26 | 将code-server（VSCode网页版）打包安装到dsh内的插件，快速实现专业的文件编辑。Package and install code-server (the web version of VSCode) as a plugin within dsh to quickly achieve professional file editing. |
| 480 | [jisi71/dsh-memories](https://github.com/jisi71/dsh-memories) | 2 | 2026-08-21 | 2026-08-22 | Dual-ledger cross-session memory for DeepSeek Harness: auto-extracted long-term facts (MEMORY.md) + living project progress ledger (PROGRESS.md), recalled into every new session. Inspired by OpenAI Codex's memory pipeline. |
| 481 | [jiuge2467/DSH-Desktop](https://github.com/jiuge2467/DSH-Desktop) | 2 | 2026-08-18 | 2026-08-28 | 🐬 专为小白与极客打造的 DeepSeek Harness 桌面全栈工作台：内置小鲸鱼姬桌宠、多源 MCP 调试沙箱、持久化终端与看板 \| The Geek & Cozy Desktop Client for DeepSeek Harness with Whale-chan Mascot, MCP Hub & Terminal. |
| 482 | [jkamkk/dsh-liquid-glass-input](https://github.com/jkamkk/dsh-liquid-glass-input) | 2 | 2026-08-25 | 2026-08-25 | Liquid Glass input card for the DSH web GUI: kube.io SVG refraction with coupled-spring press animation |
| 483 | [JochenYang/dsh-app](https://github.com/JochenYang/dsh-app) | 2 | 2026-08-20 | 2026-08-28 |   A community-maintained branded desktop client for  DeepSeek Harness, Windows / macOS / Linux |
| 484 | [JohnXu22786/auditrail](https://github.com/JohnXu22786/auditrail) | 2 | 2026-08-23 | 2026-08-23 | Security auditing and session forensics for DeepSeek Harness (dsh): full tool-invocation-chain recording (who/what/files/status/duration) fr |
| 485 | [JohnXu22786/ci-runner](https://github.com/JohnXu22786/ci-runner) | 2 | 2026-08-23 | 2026-08-23 | Trigger GitHub Actions workflow runs and local test pipelines, stream their logs back, and on failure hand the tail of the log to DeepSeek f |
| 486 | [JohnXu22786/dsh-web-submit](https://github.com/JohnXu22786/dsh-web-submit) | 2 | 2026-08-23 | 2026-08-23 | DeepSeek Harness plugin: run headless-style tasks through the live dsh web process — CLI-invoked sessions appear in the Web UI in real time (POST /x/headless, GET status, SSE live events). |
| 487 | [joshryandavis/dsh-llm-aws-kiro](https://github.com/joshryandavis/dsh-llm-aws-kiro) | 2 | 2026-08-21 | 2026-08-24 | deeepseek-harness kiro provider |
| 488 | [jyao-SUSE-power-group/dsh-provider-rate-limit](https://github.com/jyao-SUSE-power-group/dsh-provider-rate-limit) | 2 | 2026-08-23 | 2026-08-23 | dsh-provider-rate-limit |
| 489 | [jypjypjypjyp/dsh-guardrail](https://github.com/jypjypjypjyp/dsh-guardrail) | 2 | 2026-08-25 | 2026-08-25 | DSH 插件：工具调用规范守卫（deny/warn 拦截 + 规则管理面板） |
| 490 | [KaichenCurry/dsh-design-mode](https://github.com/KaichenCurry/dsh-design-mode) | 2 | 2026-08-22 | 2026-08-23 | Agentic image Design Mode for DeepSeek Harness: infinite canvas, ask_user clarification, image tools, comments, and provider routing. |
| 491 | [kaijia323/dsh-sidebar](https://github.com/kaijia323/dsh-sidebar) | 2 | 2026-08-19 | 2026-08-26 | DSH Web Client 的 VSCode 风格文件树侧栏插件：虚拟化懒加载文件树，支持文本 / Markdown / 图片预览。 |
| 492 | [kanchengw/dsh-assembly.resume](https://github.com/kanchengw/dsh-assembly.resume) | 2 | 2026-08-25 | 2026-08-25 | Import local Codex and Claude sessions into DeepSeek Harness. |
| 493 | [KannaKuron/dsh-better-workspace](https://github.com/KannaKuron/dsh-better-workspace) | 2 | 2026-08-30 | 2026-08-30 | DSH web plugin: a hierarchical workspace tree for the sidebar — titles containing / group into virtual folders; the add-workspace flow gains a parent-group popup |
| 494 | [kikomaotu/ccs-balance](https://github.com/kikomaotu/ccs-balance) | 2 | 2026-08-22 | 2026-08-26 | DSH 插件：同步 cc-switch 各 provider 余额，按日/月/总量统计 token 用量与花费（支持中转站币种与汇率设置） |
| 495 | [Kilganon725/dsh-mic-dictation](https://github.com/Kilganon725/dsh-mic-dictation) | 2 | 2026-08-26 | 2026-08-27 | DeepSeek Harness client plugin: mic dictation button next to the Full access control |
| 496 | [kiligzzz/dsh-skill-mcp-manager](https://github.com/kiligzzz/dsh-skill-mcp-manager) | 2 | 2026-08-21 | 2026-08-30 | Capability Manager for DeepSeek Harness: manage MCP servers and Skills from a Settings-page UI (dual-face dsh plugin) |
| 497 | [kittimzhe/dsh-session-export](https://github.com/kittimzhe/dsh-session-export) | 2 | 2026-08-22 | 2026-08-22 | Human-readable session transcript export for DeepSeek Harness — /transcript writes Markdown/JSON to a host path via ctx.sessionQuery (dsh-plugin) |
| 498 | [kober-basket/dsh-cachescope](https://github.com/kober-basket/dsh-cachescope) | 2 | 2026-08-26 | 2026-08-28 | Prompt-cache observability and logical-input diagnostics for DeepSeek Harness. |
| 499 | [L3n3L/dsh-resume](https://github.com/L3n3L/dsh-resume) | 2 | 2026-08-21 | 2026-08-22 | AI 写简历容易，但写完总会遇到模板难看、排版溢出、页面留白、改一处全局变形等问题。dsh-resume 专注解决“内容生成后的视觉复核”：让 AI 和用户一起把简历调到真正适合投递的刚好一页。AI can write a resume, but the result often looks unbalanced, overflows the page, leaves large blank areas, or breaks after a small edit. dsh-resume focuses on visual review after generation, helping AI and users refine the resume into a polished. |
| 500 | [Lbunc/dsh-local-llm-controller](https://github.com/Lbunc/dsh-local-llm-controller) | 2 | 2026-08-21 | 2026-08-22 | 为DSH接入本地大模型能力：在「设置→插件」页一键启停本地 llama.cpp 大模型（双槽x双模态x双预设），卡片内配置、一条命令安装、自动注册，装完即用\| Enable local large model capabilities for DSH: One-click start/stop for local llama.cpp models (dual‑slot × dual‑modal × dual‑preset) right in Settings → Plugins; configure within the card, install with a single command, automatically register, and ready to use  |
| 501 | [lcohvne-tomorin/dsh-background](https://github.com/lcohvne-tomorin/dsh-background) | 2 | 2026-08-23 | 2026-08-24 | Custom background wallpaper plugin for DeepSeek Harness chat page — upload local image or image link, tune opacity and dark overlay, scope to chat area or full screen. |
| 502 | [LCYLYM/dsh-plugin-compat-guardian](https://github.com/LCYLYM/dsh-plugin-compat-guardian) | 2 | 2026-08-22 | 2026-08-22 | Repository-installed CI repair bot that keeps DeepSeek Harness plugins compatible with new DSH releases |
| 503 | [lengquan88/dsh-dual-auto](https://github.com/lengquan88/dsh-dual-auto) | 2 | 2026-08-21 | 2026-08-22 | Dual-model auto-routing plugin for DeepSeek Harness: low-cost direct / high-cost upgrade + escape-learning closed loop |
| 504 | [leolee9086/dsh-zhihu-tools](https://github.com/leolee9086/dsh-zhihu-tools) | 2 | 2026-08-22 | 2026-08-31 | 知乎数据开放平台 DSH 静态双面插件:17工具+精美卡片+串行化限流。QQ群1017854502 https://qm.qq.com/q/RAHJuyhQQ |
| 505 | [leonardoxr/dsh-auto-chat-titles](https://github.com/leonardoxr/dsh-auto-chat-titles) | 2 | 2026-08-22 | 2026-08-24 | Semantic, configurable chat titles for DeepSeek Harness |
| 506 | [leonardwwq/dsh-cultivation](https://github.com/leonardwwq/dsh-cultivation) | 2 | 2026-08-20 | 2026-08-26 | A DSH plugin that gives AI characters persistent relationships and evolving user models through long-term interaction. |
| 507 | [Letter2025/dsh-task-worktree](https://github.com/Letter2025/dsh-task-worktree) | 2 | 2026-08-18 | 2026-08-25 | Complete Git worktree support for DeepSeek Harness: task-scoped isolated checkouts on their own branches, recorded in a per-repo manifest that survives sessions and restarts |
| 508 | [lhbsaa/dsh-visibridge](https://github.com/lhbsaa/dsh-visibridge) | 2 | 2026-08-17 | 2026-08-23 | DeepSeek Harness vision plugin: analyze_image (structured OCR evidence) + capture_image (USB camera visual loop). 摄像头视觉闭环 + 结构化证据，支持 Ollama / DeepSeek / Xiaomi 三后端。 |
| 509 | [libiwolve/dsh-experience-library](https://github.com/libiwolve/dsh-experience-library) | 2 | 2026-08-24 | 2026-08-24 | dsh-experience-library: 更有经验的 DeepSeek - 经验验证固化层(实时采集/加工/三层检验/技能书/benchmark验证) |
| 510 | [LingYuYue1/dsh-workbench](https://github.com/LingYuYue1/dsh-workbench) | 2 | 2026-08-23 | 2026-08-23 | VSCode 风格工作台侧边栏：文件树 / 多标签预览 / CodeMirror 编辑 / 终端 / Git / 全库搜索 / 变更审查 \| Workbench sidebar panel for DeepSeek Harness |
| 511 | [Linux-System-0/peaklow](https://github.com/Linux-System-0/peaklow) | 2 | 2026-08-23 | 2026-08-23 | DeepSeek Harness (Cordis) 高峰/低峰自动调度插件：宿主 + 浏览器端 client 状态卡。dsh-plugin |
| 512 | [lishLRF/dsh-plugin-onekey](https://github.com/lishLRF/dsh-plugin-onekey) | 2 | 2026-08-22 | 2026-08-23 | 适配插件中心的一键安装/卸载 |
| 513 | [lispking/dsh-qq-skin](https://github.com/lispking/dsh-qq-skin) | 2 | 2026-08-22 | 2026-08-22 | A QQ NT messenger skin for DeepSeek Harness (dsh). Light and dark share one QQ NT language. |
| 514 | [liustack/summono](https://github.com/liustack/summono) | 2 | 2026-08-17 | 2026-08-24 | One click and DeepSeek Harness is running — the free launcher & installer for AI harnesses. 一键安装启动 DeepSeek Harness。 |
| 515 | [liyu34/dsh-wsl-tray](https://github.com/liyu34/dsh-wsl-tray) | 2 | 2026-08-22 | 2026-08-22 | 为运行在 WSL 里的 DeepSeek Harness（DSH）提供 Windows 桌面快捷方式与系统托盘启动器。 |
| 516 | [liznee/dsh-file-resource](https://github.com/liznee/dsh-file-resource) | 2 | 2026-08-22 | 2026-08-22 | DeepSeek Harness Web 的本地文件输入插件。在输入框原有的 + 菜单顶部增加 attach，并用分隔线与 Harness 原生命令区分；不会再增加一个单独按钮。Private local file attachments for DeepSeek Harness with native images and bounded document reading. |
| 517 | [lory69060/cn-intel-mcp-dsh](https://github.com/lory69060/cn-intel-mcp-dsh) | 2 | 2026-08-24 | 2026-08-24 | DeepSeek Harness plugin: China hard-tech supply chain intelligence (MCP: signal board / track record / Q&A) |
| 518 | [ltxlong/dsh-session-kit](https://github.com/ltxlong/dsh-session-kit) | 2 | 2026-08-22 | 2026-08-23 | 会话管理菜单、归档管理、轮次级删除、重新生成，话题快捷导航。Add a management menu for conversations, archive conversation management, delete by round, regenerate, and a quick topic navigation on the right. |
| 519 | [luckzhangfengbo/dsh-web-theme](https://github.com/luckzhangfengbo/dsh-web-theme) | 2 | 2026-08-29 | 2026-08-29 | deepseek harness 背景主题插件 |
| 520 | [Lxd-Ashe/dsh-codex-theme](https://github.com/Lxd-Ashe/dsh-codex-theme) | 2 | 2026-08-24 | 2026-08-24 | Codex 主题外观插件 for DeepSeek Harness（DSH）：把 Codex 主题配置（codex-theme-v1，80 款浅/深色主题）做成可在 DSH 中直接切换、可自定义的外观插件。 |
| 521 | [lywusichen/dsh-sidebar-buttons](https://github.com/lywusichen/dsh-sidebar-buttons) | 2 | 2026-08-23 | 2026-08-23 | 管理 DeepSeek Harness 左下侧栏按钮的插件：拖拽排序、显隐控制，隐藏按钮收进"更多"菜单，可统一按钮高度。 |
| 522 | [mackwan84/dsh-ui-mockup](https://github.com/mackwan84/dsh-ui-mockup) | 2 | 2026-08-26 | 2026-08-31 | DSH plugin for generating UI wireframes and high-fidelity mockups with DashScope Qwen/Wan and Volcengine Seedream. |
| 523 | [margbug01/dsh-ma-plugins](https://github.com/margbug01/dsh-ma-plugins) | 2 | 2026-08-15 | 2026-08-22 | DeepSeek Harness (DSH) plugins: Tavily+Exa web search, Oracle second opinion, GitHub Librarian, /handoff, session manager, and file drop. |
| 524 | [Max-Null/dsh-capture](https://github.com/Max-Null/dsh-capture) | 2 | 2026-08-22 | 2026-08-25 | Dual-engine screen capture for DeepSeek Harness: box-select + red-box annotation, composer insertion (SSiD shell / plain DSH getDisplayMedia) · 双引擎屏幕截图：框选 + 红框标注，图片直入会话输入框 |
| 525 | [Max-Null/dsh-skill-mcp-center](https://github.com/Max-Null/dsh-skill-mcp-center) | 2 | 2026-08-17 | 2026-08-25 | Skill & MCP center for DeepSeek Harness: manage skills and MCP servers in Settings, live MCP status in the sidebar · Skill 与 MCP 管理中心：设置里管理技能与 MCP 服务器，侧边栏实时状态 |
| 526 | [maxmilian/dsh-forge](https://github.com/maxmilian/dsh-forge) | 2 | 2026-08-24 | 2026-08-24 | DeepSeek Harness tools for self-hosted Gitea and Forgejo instances |
| 527 | [maxmilian/dsh-grafana-query](https://github.com/maxmilian/dsh-grafana-query) | 2 | 2026-08-26 | 2026-08-26 | Read-only Grafana metrics and alert tools for DeepSeek Harness (PromQL via datasource proxy). |
| 528 | [maxmilian/dsh-odoo](https://github.com/maxmilian/dsh-odoo) | 2 | 2026-08-26 | 2026-08-26 | Read-only Odoo tools for DeepSeek Harness, with an opt-in restricted draft-create tool. |
| 529 | [maxmilian/dsh-sentry](https://github.com/maxmilian/dsh-sentry) | 2 | 2026-08-26 | 2026-08-26 | Read-only Sentry issue and event tools for DeepSeek Harness. |
| 530 | [maxwell-feng/dsh-tinyfish-search](https://github.com/maxwell-feng/dsh-tinyfish-search) | 2 | 2026-08-30 | 2026-08-30 | TinyFish-backed web search provider for DeepSeek Harness (ctx.web) — 将内置 web_search 接入 TinyFish Search API 的 DeepSeek Harness 插件 |
| 531 | [menotbobbybrown/dsh-plugin-mcp](https://github.com/menotbobbybrown/dsh-plugin-mcp) | 2 | 2026-08-21 | 2026-08-22 | Universal Model Context Protocol (MCP) Bridge Plugin for DeepSeek Harness (dsh) — Everything is a Plugin |
| 532 | [meyaomiao/dsh-github-workbench](https://github.com/meyaomiao/dsh-github-workbench) | 2 | 2026-08-26 | 2026-08-26 | DSH 插件:在侧边栏使用 GitHub —— 仓库目录树 + Issues/PR/Actions 页签,支持建 Issue/PR、评论、合并、重跑 CI;better-sidebar 页签与独立面板双形态 |
| 533 | [meyaomiao/dsh-server-deck](https://github.com/meyaomiao/dsh-server-deck) | 2 | 2026-08-26 | 2026-08-28 | 服务器卡片仪表盘 for DeepSeek Harness — card dashboard (status/CPU/mem/disk) + one-click xterm terminal, better-sidebar tab or standalone drawer |
| 534 | [mhwww/DSH-Wallpaper-Engine](https://github.com/mhwww/DSH-Wallpaper-Engine) | 2 | 2026-08-23 | 2026-08-24 | DeepSeek Harness (dsh) 背景图片插件：内置默认图 / 自定义上传 / Wallpaper Engine 创意工坊一键应用 / 视频壁纸 ffmpeg 高清抽帧 |
| 535 | [ming-14/PTY-Agent](https://github.com/ming-14/PTY-Agent) | 2 | 2026-06-22 | 2026-08-31 |  Give your AI agent a real terminal: persistent PTY sessions, prompt-triggered returns, screen snapshots, and   TUI/GUI/crash awareness. |
| 536 | [mingzeng21/dsh-stock-mentions](https://github.com/mingzeng21/dsh-stock-mentions) | 2 | 2026-08-23 | 2026-08-25 | 你在 DSH 对话中提到的股票名称或股票代码，会自动变成可点击按钮——点一下，行情和资讯就在右侧侧边栏展开。 |
| 537 | [miuzel/dsh-subagent-ui](https://github.com/miuzel/dsh-subagent-ui) | 2 | 2026-08-26 | 2026-08-26 | Searchable workspace subagent manager for DeepSeek Harness Web |
| 538 | [mokuyoaxis/agent-guard](https://github.com/mokuyoaxis/agent-guard) | 2 | 2026-08-22 | 2026-08-23 | Make destructive AI-agent actions reversible by default — quarantine + audit + human escalation for rm/git destructive operations. Reliability infrastructure, not a sandbox. |
| 539 | [mqhe2007/dsh-pm](https://github.com/mqhe2007/dsh-pm) | 2 | 2026-08-21 | 2026-08-22 | dsh-pm is the ChunSun × DeepSeek Harness reference plugin: an AI-native project-delivery loop driven by ChunSun. Requirements / Runs / Steps / acceptance scenarios & cases / work-memory, a session delivery panel, and 28 chunsun_* model tools — with the platform as the single source of truth. MIT. |
| 540 | [MrElysium/convoport](https://github.com/MrElysium/convoport) | 2 | 2026-08-23 | 2026-08-24 | Capture AI conversations from any web chat, keep them 100% local, and port them into any agent as live sessions — not dead exports. |
| 541 | [mrRisega/dsh-remote](https://github.com/mrRisega/dsh-remote) | 2 | 2026-08-19 | 2026-08-27 | Remote control for DeepSeek Harness (dsh web) from any phone browser: tunnel-mode relay client with one-command install and self-hosting support |
| 542 | [MS666666/dsh-archive-manager](https://github.com/MS666666/dsh-archive-manager) | 2 | 2026-08-22 | 2026-08-22 | DeepSeek Harness归档管理器 |
| 543 | [mycyg/memory-palace](https://github.com/mycyg/memory-palace) | 2 | 2026-08-25 | 2026-08-25 | Event-based long-term memory for LLM agents — associative surfacing over query RAG. Closed-loop episodic events, budgeted injection, tiered forgetting. Claude Code hooks + DeepSeek Harness plugin, one shared .memory/ format. |
| 544 | [nabin-qq273274877/dsh-desktop](https://github.com/nabin-qq273274877/dsh-desktop) | 2 | 2026-08-31 | 2026-08-31 | DeepSeek Harness Desktop - 桌面启动器 (Tauri 2 + 内置 Node + 自动更新) |
| 545 | [Nagi-ovo/dsh-music-tui](https://github.com/Nagi-ovo/dsh-music-tui) | 2 | 2026-08-31 | 2026-08-31 | YesPlayMusic controls and now-playing status for dsh-TUI |
| 546 | [NaNQiQ/deepseek-harness-remote-ssh](https://github.com/NaNQiQ/deepseek-harness-remote-ssh) | 2 | 2026-08-24 | 2026-08-24 | 让 DeepSeek Harness（DSH） 使用原生工具直接操作远程 Linux 服务器，自由切换服务器 |
| 547 | [necokeine/dsh-codex-relay](https://github.com/necokeine/dsh-codex-relay) | 2 | 2026-08-22 | 2026-08-23 | Selectable Codex model provider for DeepSeek Harness over the local Codex app-server |
| 548 | [nikoart-liu/dsh-open-in-x](https://github.com/nikoart-liu/dsh-open-in-x) | 2 | 2026-08-24 | 2026-08-24 | 在 DeepSeek Harness Web 界面中，把当前会话的工作目录直接交给本机外部应用打开。 |
| 549 | [niuhuoshan/dsh-connect](https://github.com/niuhuoshan/dsh-connect) | 2 | 2026-08-29 | 2026-08-31 | DeepSeek Harness 数据源连接插件，支持数据库元数据发现、AI 语义建模、只读 SQL 查询和固定 HTTP API 调用 |
| 550 | [niushuanan/xiaozhuang-dsh](https://github.com/niushuanan/xiaozhuang-dsh) | 2 | 2026-08-23 | 2026-08-24 | Plugin-enhanced DeepSeek Harness distribution with Computer Use, Teamwork, model usage, and multi-worktree development. |
| 551 | [NOirBRight/dsh-llm-opencode-go](https://github.com/NOirBRight/dsh-llm-opencode-go) | 2 | 2026-08-26 | 2026-08-29 | OpenCode Go LLM provider plugin for DeepSeek Harness |
| 552 | [notload/dsh-session-toc](https://github.com/notload/dsh-session-toc) | 2 | 2026-08-23 | 2026-08-23 | 为 DeepSeek Harness Web UI 每个会话页右侧加一个类似deepseek网页端的常驻、可折叠的目录栏：每条用户提问对应一个条目，点击即可滚动定位到对应消息并高亮当前条目。 |
| 553 | [Nzssm1/dsh-a-stock-five-dimension](https://github.com/Nzssm1/dsh-a-stock-five-dimension) | 2 | 2026-08-21 | 2026-08-22 | A DeepSeek Harness (DSH) community agent preset for rigorous A-share five-dimension (technical/valuation/fundamental/capital-flow/news) standardized analysis: persona, skill knowledge base, hard risk gate, deterministic Python scoring core, Tencent-first collectors. Not an investment recommendation. |
| 554 | [omdsh-dev/dsh-file-trace](https://github.com/omdsh-dev/dsh-file-trace) | 2 | 2026-08-28 | 2026-08-30 | DSH Web UI 文件追踪插件：记录并查看模型读取/写入/编辑的文件，带行号内容与终端风逐行 diff(红删绿增蓝改)、hunk 上下文折叠、可拖拽高度。适配 DSH dsh-v0.1.2-alpha.1，纯客户端零核心改动。 |
| 555 | [oxgbl/dsh-no-cmd-launcher](https://github.com/oxgbl/dsh-no-cmd-launcher) | 2 | 2026-08-22 | 2026-08-22 | DSH background launcher: double-click icon to run dsh web without any cmd window, plus desktop start/stop shortcuts (npm/CLI installs, no DSH Desktop dependency) |
| 556 | [PetCT/dsh-Bio-image-dup-check](https://github.com/PetCT/dsh-Bio-image-dup-check) | 2 | 2026-08-25 | 2026-08-25 | 科研图片查重 DSH 插件 · 本地离线检测整图重复/翻转/旋转/缩放、copy-move、跨图区域复用与 PDF 稿件图片。A local-offline integrity checker for life-science figures (DeepSeek Harness plugin). |
| 557 | [PetCT/dsh-plugin-marketplace](https://github.com/PetCT/dsh-plugin-marketplace) | 2 | 2026-08-23 | 2026-08-23 | DSH 插件市场 · A plugin marketplace inside DeepSeek Harness — browse, search, favorite, one-click download community plugins |
| 558 | [ph4310822/dsh-edex-jarvis-ui](https://github.com/ph4310822/dsh-edex-jarvis-ui) | 2 | 2026-08-25 | 2026-08-27 | DeepSeek Harness eDEX-UI shell plugin — JARVIS variant: electric cyan HUD with VITAL SIGNS / RT-MONITOR / RT-LOG left bar, POWER CORE / RADAR right bar, JARVIS header |
| 559 | [pharaohnie/dsh-context-mode](https://github.com/pharaohnie/dsh-context-mode) | 2 | 2026-08-23 | 2026-08-24 | DSH 原生 Cordis 插件：知识库(FTS5)、路由强制、会话记忆、沙箱执行(Think-in-Code)——context-window 减负 |
| 560 | [PianoPrince/dsh-workspace-mover](https://github.com/PianoPrince/dsh-workspace-mover) | 2 | 2026-08-26 | 2026-08-30 | 拖拽跨工作区真迁移 DSH 会话：批量移动、挂错归位、分组合并；步步备份回滚，零 token 消耗 / Move DSH sessions across workspaces by drag & drop — true migration, batch move, misfiled homing, group merge; backups + rollback, zero tokens. |
| 561 | [pirate-608/dsh-multi-tools](https://github.com/pirate-608/dsh-multi-tools) | 2 | 2026-08-14 | 2026-08-31 | Multimodal tool suite for DeepSeek Harness: ModLens vision, local ComfyUI, Unity, creative apps, CAD, and Ren'Py. |
| 562 | [PolinniZhong/dsh-session-workbench](https://github.com/PolinniZhong/dsh-session-workbench) | 2 | 2026-08-21 | 2026-08-30 | Session Workbench for DeepSeek Harness: session-library full-text search + recall + conversation-view management (show/hide + reorder). 会话工作台：会话库（历史会话全文搜索与召回）+ 会话视图（标签栏显示/隐藏 + 拖拽排序）。 |
| 563 | [purezhi/dsh-plugin-whale3](https://github.com/purezhi/dsh-plugin-whale3) | 2 | 2026-08-22 | 2026-08-23 | 鲸鱼 for DeepSeek Harness |
| 564 | [pwping/moyu_games](https://github.com/pwping/moyu_games) | 2 | 2026-08-25 | 2026-08-25 | 一款Deepseek Harness Web UI 的摸鱼游戏插件，执行任务时,在右下角位置弹窗游戏窗口，任务执行时间玩玩益智游戏 |
| 565 | [Qian-Ning/prompt-skill-armory](https://github.com/Qian-Ning/prompt-skill-armory) | 2 | 2026-08-27 | 2026-08-30 | Managing prompts，, skills, MCP tools & wallpaper for DeepSeek Harness |
| 566 | [qingmomo233/dsh-thinking-language](https://github.com/qingmomo233/dsh-thinking-language) | 2 | 2026-08-16 | 2026-08-29 | 更改 deepseek harness 思考过程语言 |
| 567 | [QinpanWan/dsh-sky-skin](https://github.com/QinpanWan/dsh-sky-skin) | 2 | 2026-08-25 | 2026-08-27 | Sky: Children of the Light themed skin for DeepSeek Harness web UI - light children on a glowing star map, candlelight gold and starry night. 光遇·遇境主题皮肤。 |
| 568 | [qinyuehuan/dsh-whale-status](https://github.com/qinyuehuan/dsh-whale-status) | 2 | 2026-08-22 | 2026-08-23 | 把鲸鱼娘思考时的 deep diving 状态文案换成任意多句随机播放，蓝青水流动画，颜色/流速可自定义（DeepSeek Harness plugin） |
| 569 | [quaner1234-cmd/dsh-subagent-watchdog](https://github.com/quaner1234-cmd/dsh-subagent-watchdog) | 2 | 2026-08-23 | 2026-08-23 | DSH plugin that auto-continues a native continuable subagent once when it ends with explicit max-tokens termination — then stops. No loops, no timers, official seams only. |
| 570 | [qwert702/dsh-commander](https://github.com/qwert702/dsh-commander) | 2 | 2026-08-22 | 2026-08-23 | Commander for the DeepSeek Harness Web GUI: one conversation orchestrates others via <dsh-dispatch> protocol blocks, with automatic result receipts. |
| 571 | [qwert702/dsh-memory](https://github.com/qwert702/dsh-memory) | 2 | 2026-08-22 | 2026-08-23 | Long-term memory plugin for the DeepSeek Harness Web GUI: project+global stores, auto extraction/injection, small-model consolidation, Obsidian-style link graph. |
| 572 | [Rannist/balance-dsh](https://github.com/Rannist/balance-dsh) | 2 | 2026-08-23 | 2026-08-24 | DSH 插件：显示 DeepSeek 账户余额 + 会话 token/费用，含高峰/空闲计费 |
| 573 | [rayadesune/DeepSeek-Harness-chat-billing](https://github.com/rayadesune/DeepSeek-Harness-chat-billing) | 2 | 2026-08-17 | 2026-08-24 | 类原生计费插件 |
| 574 | [rayzhu1109/dsh-balance](https://github.com/rayzhu1109/dsh-balance) | 2 | 2026-08-22 | 2026-08-23 | balance record & usage tracking |
| 575 | [rickyfu0625-cell/dsh-billing-dashboard](https://github.com/rickyfu0625-cell/dsh-billing-dashboard) | 2 | 2026-08-24 | 2026-08-24 | DeepSeek Harness 用量看板插件：余额 / 消费 / token / 7 日趋势 / 一键充值 |
| 576 | [Ruiming-cn/dsh-better-at](https://github.com/Ruiming-cn/dsh-better-at) | 2 | 2026-08-21 | 2026-08-22 | Caches DSH Web file and session reference indexes for local @ filtering while preserving native mention insertion. |
| 577 | [Scorpio69t/teach-math-with-manim](https://github.com/Scorpio69t/teach-math-with-manim) | 2 | 2026-08-19 | 2026-08-31 | Teach Math with Manim — 图书《用 Manim 讲好数学》官方配套开源仓库 |
| 578 | [Sddft97/dsh-client-ui-skin-verdandi](https://github.com/Sddft97/dsh-client-ui-skin-verdandi) | 2 | 2026-08-22 | 2026-08-22 | Aether Gazer Verdandi-inspired skin for the DeepSeek Harness Web UI |
| 579 | [SeerableOfficial/dsh-web-search-toggle](https://github.com/SeerableOfficial/dsh-web-search-toggle) | 2 | 2026-08-22 | 2026-08-22 | DSH plugin: a per-session "Web Search" toggle that forces the agent to search the web before answering. |
| 580 | [Seetraum/harness-session-delete](https://github.com/Seetraum/harness-session-delete) | 2 | 2026-08-25 | 2026-08-25 | Deepseek Harness 删除会话 |
| 581 | [SeverusZh/dsh-skills-mcp-group-manager](https://github.com/SeverusZh/dsh-skills-mcp-group-manager) | 2 | 2026-08-28 | 2026-08-28 | DeepSeek Harness Skills & MCPs 分组管理器 — 分组管理 Skills、过滤模型技能目录、独立开关 MCP 服务器、左侧面板一键管理 / Group skills, filter the model skill catalog, toggle MCP servers, left panel UI |
| 582 | [shenjackyuanjie/dsh-sfw](https://github.com/shenjackyuanjie/dsh-sfw) | 2 | 2026-08-05 | 2026-08-23 | 为了防止你的好bro/同事看到内测dsh然后：？这是什么 |
| 583 | [Shizuku-keop/dsh-micro-inversion-standard](https://github.com/Shizuku-keop/dsh-micro-inversion-standard) | 2 | 2026-08-24 | 2026-08-24 | 一个可复用的 DSH Agent Preset：双阶段、Token 精益的编码智能体模式。  核心目标：把模型思维链的起手习惯从 "let me" 翻转为 "we need"，同时把上下文占用与 Token 消耗压到最低，并保持供应商 KV Cache 对未变前缀持续命中。 |
| 584 | [Shizuku-keop/dsh-plugin-brainstorm-visualizer](https://github.com/Shizuku-keop/dsh-plugin-brainstorm-visualizer) | 2 | 2026-08-24 | 2026-08-24 | DeepSeek Harness Brainstorming Visualization Plugin Seamlessly combining AI divergent reasoning with visual interaction, built specifically for solving complex problems |
| 585 | [Shyboy0499/dsh-git-tools](https://github.com/Shyboy0499/dsh-git-tools) | 2 | 2026-08-26 | 2026-08-26 | Local git tools for DeepSeek Harness (dsh): git_status, git_diff, git_log, git_commit |
| 586 | [shyuan-hub/dsh-compact-button](https://github.com/shyuan-hub/dsh-compact-button) | 2 | 2026-08-23 | 2026-08-23 | one-click Compact context button for the DSH Web context meter panel. |
| 587 | [Simon-yyy/dsh-theme-escook](https://github.com/Simon-yyy/dsh-theme-escook) | 2 | 2026-08-23 | 2026-08-23 | 为DeepSeek Harness桌面端打造的一款主题 |
| 588 | [Smith-yue/harness-plugin](https://github.com/Smith-yue/harness-plugin) | 2 | 2026-08-23 | 2026-08-23 | harness-plugin |
| 589 | [soarGuo/dsh-auto-vision](https://github.com/soarGuo/dsh-auto-vision) | 2 | 2026-08-24 | 2026-08-24 | Bridges images into text for non-vision DeepSeek Harness models — your message stays untouched, zero manual setup. |
| 590 | [SoberReport-AI/DeepGuard](https://github.com/SoberReport-AI/DeepGuard) | 2 | 2026-08-22 | 2026-08-23 | A dsh plugin security audit agents team can trigger a security audit and provide a security audit report by submitting an issue |
| 591 | [SpookySandwich/dsh-plugin-no-workspace](https://github.com/SpookySandwich/dsh-plugin-no-workspace) | 2 | 2026-08-22 | 2026-08-23 | DSH 免工作区插件：不选工作区也能直接开始对话，独立会话在侧边栏平铺显示，原生工作区界面保持不变。Start chatting without picking a workspace; standalone conversations list flat in the sidebar. |
| 592 | [squirrel20/dsh-cron](https://github.com/squirrel20/dsh-cron) | 2 | 2026-08-26 | 2026-08-26 | Unattended scheduled jobs for the DeepSeek Harness (dsh): agent/command tasks on cron schedules |
| 593 | [STARDUSTLC666/dsh-cite](https://github.com/STARDUSTLC666/dsh-cite) | 2 | 2026-08-15 | 2026-08-27 | DeepSeek Harness 参考文献插件：cite_lookup/check/format/bibtex/health 五工具，DOI 精确查询、Crossref 题录检索、GB/T 7714/APA/MLA/Chicago 格式化、有界并发 DOI 校验；纯 Node 全平台。· Citation tools for DeepSeek Harness agents. |
| 594 | [stas130286-blip/dsh-brainagent](https://github.com/stas130286-blip/dsh-brainagent) | 2 | 2026-08-22 | 2026-08-23 | BrainAgent — brain-inspired plugin for DeepSeek Harness (dsh): a pipeline of heuristic filters, statistical memory stores and context injections; reward-ledger + UCB1 bandit learning loop (RL-lite). 676 tests. Free noncommercial use. |
| 595 | [statem-li/dsh-triad](https://github.com/statem-li/dsh-triad) | 2 | 2026-08-28 | 2026-08-28 | DSH 三合一扩展插件：用量工作台 · 技能管理 · 长期记忆引擎。零 DSH 源码改动，一句话安装。 |
| 596 | [Stylelinzzz/dsh-chat-history](https://github.com/Stylelinzzz/dsh-chat-history) | 2 | 2026-08-17 | 2026-08-30 | Chat history TOC for DeepSeek Harness: a History conversation view tab listing user messages with auto-paging and click-to-jump back into the chat. / DeepSeek Harness 会话目录插件：用户消息历史一键跳转。 |
| 597 | [summer-521/deepseek-harness-desktop](https://github.com/summer-521/deepseek-harness-desktop) | 2 | 2026-08-15 | 2026-08-28 | DeepSeek Harness 的非官方桌面封装：本地优先、沙箱隔离，内置 dsh 版本管理与插件管理，支持自动更新与任务完成桌面通知（macOS）。 |
| 598 | [sumomok/dsh-plugins](https://github.com/sumomok/dsh-plugins) | 2 | 2026-08-23 | 2026-08-23 | DeepSeek Harness plugins by sumomok: quote earlier messages, edit & rerun a prompt, account balance & spend |
| 599 | [SUONSUN9527/deepseek-harness-flow-arrange](https://github.com/SUONSUN9527/deepseek-harness-flow-arrange) | 2 | 2026-08-31 | 2026-08-31 | Claude-orchestrator x Codex-executor distribution of DeepSeek Harness |
| 600 | [supersyh-sss/dsh-voice-assistant](https://github.com/supersyh-sss/dsh-voice-assistant) | 2 | 2026-08-29 | 2026-08-30 | Offline voice assistant for dsh web — wake word, speech dictation, voice edit commands & Chinese TTS. On-device sherpa-onnx WASM ASR, no Google dependency, works in China. |
| 601 | [swordordead/dsh-Veneer](https://github.com/swordordead/dsh-Veneer) | 2 | 2026-08-18 | 2026-08-31 | DIY你的小蓝鲸吧 |
| 602 | [T-MKT/dsh-customization-settings](https://github.com/T-MKT/dsh-customization-settings) | 2 | 2026-08-19 | 2026-08-22 | Provide generic UI customization settings for DeepSeek Harness, like wallpaper, theme color, etc.  |
| 603 | [TalkingRainTuT/dsh-VoiceChat](https://github.com/TalkingRainTuT/dsh-VoiceChat) | 2 | 2026-08-23 | 2026-08-23 | 一个DSH的语音聊天插件 \| Realtime voice chat plugin for DeepSeek Harness: configurable translate + multi-TTS + auto-start local servers. |
| 604 | [taxueseek/dsh-healthcheck](https://github.com/taxueseek/dsh-healthcheck) | 2 | 2026-08-15 | 2026-08-22 | DeepSeek Harness 环境体检插件：磁盘/内存/延迟/~/.dsh 膨胀/插件版本落后检测，历史基线趋势，只读不删。 |
| 605 | [taxueseek/dsh-snippets](https://github.com/taxueseek/dsh-snippets) | 2 | 2026-08-15 | 2026-08-22 | DeepSeek Harness 极简常用片段/命令工具箱：JSONL 存储，5 个工具，零依赖。AI 的收藏夹。 |
| 606 | [taxueseek/taxue-dsh-artisan](https://github.com/taxueseek/taxue-dsh-artisan) | 2 | 2026-08-19 | 2026-08-22 | taxue 画师：DeepSeek Harness 一体化视觉创作工具链（提示词反推/优化 + 多供应商生图，支持异步后台出图） |
| 607 | [the-thinker0/dsh-memory-search-plus](https://github.com/the-thinker0/dsh-memory-search-plus) | 2 | 2026-08-25 | 2026-08-26 | A local-first full-text memory search plugin for DeepSeek Harness, enabling fast cross-conversation search, message-level navigation, and intelligent retrieval of your AI coding history. |
| 608 | [theoneLee/deepseek-harness-sdk-go](https://github.com/theoneLee/deepseek-harness-sdk-go) | 2 | 2026-08-15 | 2026-08-27 | Go SDK for driving DeepSeek Harness |
| 609 | [Tkingxiao/dsh-novel-solo](https://github.com/Tkingxiao/dsh-novel-solo) | 2 | 2026-08-27 | 2026-08-27 | DeepSeek Harness 的「单核写作」插件：面向量化小模型做了充分的工具瘦身与输出加固，适合在本机用本地模型跑长篇小说流水线。 |
| 610 | [treers2/qq-operations](https://github.com/treers2/qq-operations) | 2 | 2026-08-25 | 2026-08-25 | QQ NT desktop automation for DeepSeek Harness (DSH) skill - dynamic UI Automation locate, dual mode, self-check; 操控 QQ NT 桌面版的 DSH skill（UIA 类名定位/双模式/自检） |
| 611 | [tristan-mcinnis/dsh-browser-vision](https://github.com/tristan-mcinnis/dsh-browser-vision) | 2 | 2026-08-22 | 2026-08-22 | Browser tool for DeepSeek Harness that can SEE the page: browser-use over CDP driven by deepseek-v4-flash-vision-exp. Reads canvas text, text inside images and rendered charts, returns schema-validated JSON, and reports per-run cost. |
| 612 | [try-works/dsh-browser-agent](https://github.com/try-works/dsh-browser-agent) | 2 | 2026-08-23 | 2026-08-23 | DeepSeek Harness bundle: a Chrome browser for agents (browser_goto / browser_evaluate / browser_screenshot tools) with a live two-way pane inside the DSH Web GUI. The browser engine is a fork of zenbu-labs/terminal-browser with the React Ink terminal UI replaced by a DSH tool surface and web pane. |
| 613 | [TYEclipse/dsh-musictheory](https://github.com/TYEclipse/dsh-musictheory) | 2 | 2026-08-24 | 2026-08-25 | Music theory math toolbox for DeepSeek Harness (dsh): note parsing, frequency/MIDI conversion, correctly spelled chords (26 qualities) and scales (17 types) — zero runtime dependencies |
| 614 | [uckkk/dsh-valley-meter](https://github.com/uckkk/dsh-valley-meter) | 2 | 2026-08-22 | 2026-08-22 | Minimal peak/valley electricity-price countdown widget for DeepSeek Harness: live off-peak countdown & period, official account balance, today's spend, configurable colors, minimal/detailed styles. |
| 615 | [vanhungbui-11/dsh-wallpaper-bridge](https://github.com/vanhungbui-11/dsh-wallpaper-bridge) | 2 | 2026-08-25 | 2026-08-25 | Wallpaper Engine bridge for DeepSeek Harness (DSH) on Windows |
| 616 | [vibeinging/dsh-red-alert](https://github.com/vibeinging/dsh-red-alert) | 2 | 2026-08-23 | 2026-08-23 | A real Red Alert 2 AI battlefield plugin for DeepSeek Harness with fog-safe control, live DSH Chat, and post-match learning. |
| 617 | [viplocco/dsh-delete-message](https://github.com/viplocco/dsh-delete-message) | 2 | 2026-08-22 | 2026-08-24 | DeepSeek Harness 消息级删除插件，用于避免用户误发或错误的助手消息污染会话上下文。 |
| 618 | [vuldin/yapa](https://github.com/vuldin/yapa) | 2 | 2026-03-24 | 2026-08-27 | Yet Another Personal Assistant |
| 619 | [Wanbinyu/dsh-concurrency-meter](https://github.com/Wanbinyu/dsh-concurrency-meter) | 2 | 2026-08-19 | 2026-08-25 | Read-only model request concurrency monitoring for DeepSeek Harness |
| 620 | [wang-junjian/dsh-artifact-viewer](https://github.com/wang-junjian/dsh-artifact-viewer) | 2 | 2026-08-24 | 2026-08-25 | DeepSeek Harness 插件：产物浏览器 |
| 621 | [wang-kaopu/dsh-cordis-devtools](https://github.com/wang-kaopu/dsh-cordis-devtools) | 2 | 2026-08-23 | 2026-08-26 | Give coding Agents runtime evidence for debugging and verifying DSH / Cordis plugins. 让 Coding Agent 获得用于调试和验证 DSH / Cordis 插件的运行时证据。 |
| 622 | [wangbobo-coder/gitee-ai-employee](https://github.com/wangbobo-coder/gitee-ai-employee) | 2 | 2026-08-24 | 2026-08-24 | Gitee AI 员工：在 issue 里 @ 机器人并指定目标分支，它自动克隆仓库开发、提交 PR，可自动合并并关闭 issue。Issue-driven Gitee AI developer for DeepSeek Harness. |
| 623 | [wangyuanchuan2022/dsh-prompt-optimizer](https://github.com/wangyuanchuan2022/dsh-prompt-optimizer) | 2 | 2026-08-23 | 2026-08-23 | 一键优化提示词：在输入框工具行（发送按钮左侧）新增「优化」按钮。 点击后读取当前草稿把草稿重写为结构更清晰的提示词，并直接写回输入框。 长文本支持（输入框架构修复）： 修复 composer 的长文本缺陷 |
| 624 | [wanyexin1998/dsh-workbench](https://github.com/wanyexin1998/dsh-workbench) | 2 | 2026-08-26 | 2026-08-26 | Community-maintained source preview for two-Pane DeepSeek Harness Web workflows |
| 625 | [wenbobodley/dsh-guandan](https://github.com/wenbobodley/dsh-guandan) | 2 | 2026-08-23 | 2026-08-24 | 掼蛋 Guandan card game plugin for DeepSeek Harness (DSH) - 掼蛋-中联储卫 / GUANDAN-中联储卫 |
| 626 | [Whale-Zhang/dsh-cron-tasks](https://github.com/Whale-Zhang/dsh-cron-tasks) | 2 | 2026-08-24 | 2026-08-24 | Scheduled tasks for DeepSeek Harness: sidebar jobs, isolated run history, cron/at schedules. |
| 627 | [whoisjiahao/dsh-feishu-channel](https://github.com/whoisjiahao/dsh-feishu-channel) | 2 | 2026-08-16 | 2026-08-22 | 飞书 × DeepSeek Harness 遥控器：在飞书聊天里驱动 DSH agent——流式富卡片、一键审批、按模型能力传图、费用与峰谷计量 |
| 628 | [wilburli/onlyMemory-plugin](https://github.com/wilburli/onlyMemory-plugin) | 2 | 2026-08-25 | 2026-08-25 | 零外部依赖的 LLM 长期记忆插件，专为 [DeepSeek Harness] 设计。 |
| 629 | [win4r/dsh-pi-review](https://github.com/win4r/dsh-pi-review) | 2 | 2026-08-23 | 2026-08-23 | Read-only Pi Agent code review plugin for DeepSeek Harness |
| 630 | [wishesl/dsh-launcher](https://github.com/wishesl/dsh-launcher) | 2 | 2026-08-28 | 2026-08-29 | Manage DSH plugins & runtime without launching it: plugin market, per-instance masking, version install. Wails v2 (Go + React).  DeepSeek Harness 桌面启动器：不启动 DSH 即可安全管理插件与本体——多实例/多版本一键启动、实时日志、npm 版本查询、插件市场（安装/卸载/开关/收藏/分享码）、实例级插件临时屏蔽。基于 Wails v2 (Go + React)。 |
| 631 | [Witherwithwinter/DeepSeek-Balance-Whale-Widget-Bowl](https://github.com/Witherwithwinter/DeepSeek-Balance-Whale-Widget-Bowl) | 2 | 2026-08-29 | 2026-08-31 | DeepSeek Harness（DSH）Web 界面右下角的常驻余额挂件。基于 MeteorNOX/DeepSeek-Balance-Whale-Widget 修改的铁盆鲸鱼娘版。 |
| 632 | [wp-a/dsh-academic-paper-search](https://github.com/wp-a/dsh-academic-paper-search) | 2 | 2026-08-29 | 2026-08-29 | DeepSeek Harness 的中文学术论文检索 Bundle：复用 Academic Paper Search MCP，支持多源检索去重、引用核验、引文图谱、MeSH、试验检索与审计导出。 |
| 633 | [WSL043/dsh-reasoning-slider](https://github.com/WSL043/dsh-reasoning-slider) | 2 | 2026-08-23 | 2026-08-27 | 已归档：DeepSeek Harness 模型感知推理强度滑杆；现有 Release 与演示保留，不再适配未来 DSH。 |
| 634 | [wyouwd1/dsh-opencode-models](https://github.com/wyouwd1/dsh-opencode-models) | 2 | 2026-08-24 | 2026-08-24 | Manage OpenCode Zen free-tier and Go-tier models in DeepSeek Harness: live listings from opencode.ai, drift per route, four agent tools plus an OpenCode Models settings section. |
| 635 | [x1shang/dsh-koin-lily-news](https://github.com/x1shang/dsh-koin-lily-news) | 2 | 2026-08-21 | 2026-08-26 | 菲奖得主强推的百合新闻订阅DSH插件 |
| 636 | [xiaoso456/dsh-run-config](https://github.com/xiaoso456/dsh-run-config) | 2 | 2026-08-23 | 2026-08-24 | Run configuration management for DeepSeek Harness (DSH) — IDEA-style run control for the web GUI: reusable LLM prompts and background commands, one click to launch. |
| 637 | [xie-tj/dsh-easy-exit](https://github.com/xie-tj/dsh-easy-exit) | 2 | 2026-08-21 | 2026-08-23 | DeepSeek Harness 最新用户消息编辑与重发插件（Host / Client 解耦） |
| 638 | [Xinyi21yf/deepseek-harness-plugins](https://github.com/Xinyi21yf/deepseek-harness-plugins) | 2 | 2026-08-23 | 2026-08-24 | Personal DeepSeek Harness plugins, designs, and learning notes |
| 639 | [XMoon/dsh-profile-settings](https://github.com/XMoon/dsh-profile-settings) | 2 | 2026-08-23 | 2026-08-23 | Per-profile settings overlay for DeepSeek Harness: global settings.yaml plus profiles/<name>/settings.patch.yml, transparently layered under ctx.settings |
| 640 | [xswt442-cmd/dsh-instance-manager](https://github.com/xswt442-cmd/dsh-instance-manager) | 2 | 2026-08-23 | 2026-08-24 | DSH 常驻插件：侧边栏面板统一查看并管理本机的 dsh 实例 \| Sidebar panel to list and manage local dsh web instances |
| 641 | [XuXcode/dsh-loghud](https://github.com/XuXcode/dsh-loghud) | 2 | 2026-08-23 | 2026-08-23 | Live Spring Boot error HUD with opt-in AI diagnosis for DeepSeek Harness |
| 642 | [yaoshuo530/dsh-prompt-enhancer](https://github.com/yaoshuo530/dsh-prompt-enhancer) | 2 | 2026-08-28 | 2026-08-28 | A prompt-enhancement plugin for DeepSeek Harness: an ✨ Enhance composer button that rewrites prompts with first-principles thinking using session context, and asks clarifying questions when key info is missing. |
| 643 | [yaways/dsh-subagent-claude-code-wrapper](https://github.com/yaways/dsh-subagent-claude-code-wrapper) | 2 | 2026-08-22 | 2026-08-22 | Let DSH subagents call any Claude-compatible CLI, not just the SDK-bundled one. Fork of @deepseek-ai/dsh-subagent-claude-code. |
| 644 | [Ycet/dsh-fun-turn-status](https://github.com/Ycet/dsh-fun-turn-status) | 2 | 2026-08-22 | 2026-08-23 | 替换 DSH 任务运行中的 Deep diving... 状态文案：30 秒随机轮换幽默文案，设置-插件-插件配置页可增删改（最多 50 条），与其他同类插件共存时优先级最高。 |
| 645 | [yhfgyyf/dsh-guardian-mode](https://github.com/yhfgyyf/dsh-guardian-mode) | 2 | 2026-08-23 | 2026-08-23 | Guardian preset for DeepSeek Harness with independent persistent Codex auditing |
| 646 | [yhyfhgs/dsh-model-hub](https://github.com/yhyfhgs/dsh-model-hub) | 2 | 2026-08-25 | 2026-08-25 | DeepSeek Harness plugin: provider sign-in, model catalog, and selection routing over a loopback-only /model-hub channel |
| 647 | [yingzaicc/dsh-editor-selection](https://github.com/yingzaicc/dsh-editor-selection) | 2 | 2026-08-23 | 2026-08-23 | 让 DSH 理解"用户此刻在编辑器里看着什么"。当你在编辑器中选中某个文件或行区间,后续对话自动聚焦于它——通过 @path:10-25 的环境知会行注入,而不是把文件内容塞进上下文。 |
| 648 | [yishengjun8/dsh-workspace-studio](https://github.com/yishengjun8/dsh-workspace-studio) | 2 | 2026-08-17 | 2026-08-26 | 允许显示工作区的文件树、浏览文件内容、并且允许对话中嵌入引用的文件内容、自由切换思维分支视图，目标是和VSCode相类似的开发体验 |
| 649 | [YiyuZh/dsh-skillflux](https://github.com/YiyuZh/dsh-skillflux) | 2 | 2026-08-21 | 2026-08-22 | DeepSeek Harness 动态 Skill 运行时管理器，自动发现、路由、挂载和卸载 Agent Skills |
| 650 | [yongshuai0314/dsh-readcache](https://github.com/yongshuai0314/dsh-readcache) | 2 | 2026-08-23 | 2026-08-24 | 为 DSH read 工具提供版本令牌校验的进程内结果缓存 \| Version-token-validated in-process result cache for the DSH read tool |
| 651 | [yu502950715yang/dsh-use-wallpaper](https://github.com/yu502950715yang/dsh-use-wallpaper) | 2 | 2026-08-17 | 2026-08-24 | DSH Web GUI 壁纸背景插件：从本机 Wallpaper Engine 壁纸库加载背景，wasm 渲染 scene 壁纸 |
| 652 | [yuioi666/dsh-plugin-model-capability](https://github.com/yuioi666/dsh-plugin-model-capability) | 2 | 2026-08-27 | 2026-08-31 | Model Capability Manager for DSH Web: thinking levels, context window, output caps, input modalities, gateway compat presets, EN/中文 UI. \| DSH 网页端模型能力管理插件。 |
| 653 | [Yvesgao/dsh-shortcut-creator](https://github.com/Yvesgao/dsh-shortcut-creator) | 2 | 2026-08-15 | 2026-08-30 | DSH 启动器- 在 DSH 设置页一键创建 Windows 桌面快捷方式，自动打开浏览器、可固定任务栏。DSH plugin: one-click Windows desktop shortcut launcher from the Settings page (DeepSeek Harness or any local server) —Install: dsh plugin --profile web add github:Yvesgao/dsh-desktop-shortcut#main |
| 654 | [zaimokuza-yoshiteru/dsh-acp-adapter](https://github.com/zaimokuza-yoshiteru/dsh-acp-adapter) | 2 | 2026-08-24 | 2026-08-24 | Use AI agents from the DSH session UI. |
| 655 | [zclDragon/dsh-side-chat](https://github.com/zclDragon/dsh-side-chat) | 2 | 2026-08-22 | 2026-08-23 | DSH web plugin: Codex-style /side side conversations — a temporary fork of the current chat in a floating panel, without interrupting the main task. |
| 656 | [zeropointnine/dsh-compact-and-branch](https://github.com/zeropointnine/dsh-compact-and-branch) | 2 | 2026-08-23 | 2026-08-24 | Compact a session and continue the work in a new one |
| 657 | [zhangdong456/dsh-prompt-presets](https://github.com/zhangdong456/dsh-prompt-presets) | 2 | 2026-08-21 | 2026-08-22 | Prompt Presets to manage your library  |
| 658 | [zhaoan2308184882-spec/deepseek-harness-plugins](https://github.com/zhaoan2308184882-spec/deepseek-harness-plugins) | 2 | 2026-08-24 | 2026-08-24 | Unofficial community plugins for DeepSeek Harness: Codex provider and role model router |
| 659 | [zhenghaoyang24/obsidian-plugin-deepshian](https://github.com/zhenghaoyang24/obsidian-plugin-deepshian) | 2 | 2026-08-27 | 2026-08-27 | Sidebar AI chat powered by the local DeepSeek Harness (dsh): streaming replies, tool calls, and real vault file edits. |
| 660 | [zhengjy01/weread-export](https://github.com/zhengjy01/weread-export) | 2 | 2026-08-23 | 2026-08-23 | 微信读书 (WeChat Reading) integration for DeepSeek Harness: official Skills API gateway — bookshelf, highlights/thoughts, reading stats, flomo export |
| 661 | [zhiyaoli0221/dsh-finance-db](https://github.com/zhiyaoli0221/dsh-finance-db) | 2 | 2026-08-22 | 2026-08-23 | Read-only market data for DeepSeek Harness. Ask about a stock, and let DSH call the data tools directly. \| 为 DeepSeek Harness 提供只读金融市场数据。让 DSH 直接调用工具查询行情。 |
| 662 | [ZHOUcourier/dsh-theme-whalegirl](https://github.com/ZHOUcourier/dsh-theme-whalegirl) | 2 | 2026-08-22 | 2026-08-23 | DeepSeek-鲸鱼娘 (Whale Girl) theme for the DeepSeek Harness Web UI — ported from DreamSkin ver_cb557ececaa5de3f3dbe: full --dsw-* token remap + ambient wallpaper. |
| 663 | [zhoulvyuan/dsh-plugin](https://github.com/zhoulvyuan/dsh-plugin) | 2 | 2026-08-26 | 2026-08-28 | deepseek-harness插件 |
| 664 | [zhuifengqug/pixel-skin](https://github.com/zhuifengqug/pixel-skin) | 2 | 2026-08-23 | 2026-08-23 | dsh像素风皮肤 |
| 665 | [zslzxy/aitoubiaoling-bid-review](https://github.com/zslzxy/aitoubiaoling-bid-review) | 2 | 2026-08-23 | 2026-08-24 | AI投标灵标书审核 Skill：稳定审核非扫描 PDF/DOCX 的商务标、技术标与通用文档风险 |
| 666 | [ztmajor/DSCoder](https://github.com/ztmajor/DSCoder) | 2 | 2026-08-20 | 2026-08-24 | 这是我给自己写的一个小工具——现在有太多 dsh-desktop 类项目，插件越装越多，越来越重，我就想要个干净的 AI 编码壳，里面有我需要的最基本的功能。于是有了 DSCoder。主要供我自己日常使用，如果你也有类似的需求，也欢迎取用。 |
| 667 | [0231071/llm-as-a-verifier](https://github.com/0231071/llm-as-a-verifier) | 1 | 2026-08-25 | 2026-08-25 | LLM-as-a-Verifier plugin for DeepSeek Harness (DSH): best-of-N 候选并行生成 + 概率枢轴锦标赛(PPT)验证器择优, 官方样式设置卡片, lav_status/lav_set 会话工具 \| DSH 插件: 让 AI 回答经过多候选验证器选优 |
| 668 | [0QwQ0/dsh-ui-auth](https://github.com/0QwQ0/dsh-ui-auth) | 1 | 2026-08-23 | 2026-08-23 | DeepSeek Harness Web UI 认证网关插件：登录门禁、用户管理、管理员专属模型/Key 配置、数据隔离 · Authentication gate for the DeepSeek Harness Web UI: login gate, user management, admin-only model/API-key config, data isolation |
| 669 | [0xrushmoon/dsh-freeroute](https://github.com/0xrushmoon/dsh-freeroute) | 1 | 2026-08-25 | 2026-08-27 | Free-tier model aggregation plugin for the DeepSeek Harness (dsh): transparent failover, multi-key rotation, settings panel |
| 670 | [1024483906-pixel/dsh-novel-reader](https://github.com/1024483906-pixel/dsh-novel-reader) | 1 | 2026-08-25 | 2026-08-25 | DSH休闲阅读文本插件 |
| 671 | [166767/dsh-error-audit](https://github.com/166767/dsh-error-audit) | 1 | 2026-08-29 | 2026-08-30 | DeepSeek Harness 实时 AI 自审插件：任何报错/警告第一时间连同时间、错误码、会话、用户原话、AI 动作与工作区写入专用日志目录，并主动通知 AI、内置 read_error_logs 工具随时读取。Real-time AI self-audit for DeepSeek Harness — captures every error/warning with timestamp, error code, session, user prompt, AI action and workspace into a dedicated log folder; instantly notifies the agent and ships a read_error_logs tool. |
| 672 | [173787247/dsh-tool-budget](https://github.com/173787247/dsh-tool-budget) | 1 | 2026-08-29 | 2026-08-31 | Hard-stop DeepSeek Harness tool use after a per-session call budget |
| 673 | [173787247/dsh-wsl-browser](https://github.com/173787247/dsh-wsl-browser) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness tool: open http(s) URLs in the Windows default browser from WSL. |
| 674 | [173787247/dsh-wsl-clipboard](https://github.com/173787247/dsh-wsl-clipboard) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness tool: read/write the Windows clipboard from WSL. |
| 675 | [173787247/dsh-wsl-cred](https://github.com/173787247/dsh-wsl-cred) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness tool: safe Git credential hints for Windows GCM from WSL. |
| 676 | [173787247/dsh-wsl-distro](https://github.com/173787247/dsh-wsl-distro) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness plugin: current WSL distro facts and multi-distro warnings. |
| 677 | [173787247/dsh-wsl-github](https://github.com/173787247/dsh-wsl-github) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness: GitHub App status (open PRs + latest Actions) for WSL agents |
| 678 | [173787247/dsh-wsl-gpu](https://github.com/173787247/dsh-wsl-gpu) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness tool: probe nvidia-smi / GPU visibility inside WSL. |
| 679 | [173787247/dsh-wsl-kit](https://github.com/173787247/dsh-wsl-kit) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness WSL kit (EN/ZH): docs + install.sh + cordis.patch for Windows browser + WSL agent plugins |
| 680 | [173787247/dsh-wsl-launch](https://github.com/173787247/dsh-wsl-launch) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness tool: launch allowlisted Windows apps from WSL. |
| 681 | [173787247/dsh-wsl-notify](https://github.com/173787247/dsh-wsl-notify) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness tool: Windows MessageBox notification from WSL. |
| 682 | [173787247/dsh-wsl-path](https://github.com/173787247/dsh-wsl-path) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness tool: convert WSL Linux and Windows paths with /mnt/c caveats. |
| 683 | [173787247/dsh-wsl-port](https://github.com/173787247/dsh-wsl-port) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness tool: diagnose WSL port listening and Windows localhost forwarding. |
| 684 | [2327644800/dsh-usage-analytics](https://github.com/2327644800/dsh-usage-analytics) | 1 | 2026-08-22 | 2026-08-22 | Personal usage analytics & activity dashboard for the DeepSeek Harness (dsh) web GUI: token totals, contribution heatmap, model share, insights. Local-only, metadata only. |
| 685 | [240xu/verdict-engine](https://github.com/240xu/verdict-engine) | 1 | 2026-08-24 | 2026-08-27 | Verdict Engine — machine-checkable engineering governance: prose skill for any agent + dsh-themis DSH plugin (read-only tools, fail-closed, protocolJson negotiation). 纯文本规范 + 可校验运行时双载体。 |
| 686 | [2522669008-zcy/dsh-time-prefix](https://github.com/2522669008-zcy/dsh-time-prefix) | 1 | 2026-08-24 | 2026-08-25 | 在每条用户消息前自动插入 【2026/08/23，22:36】 这样的时间文本 |
| 687 | [2DogsLee/dsh_whalebuddy](https://github.com/2DogsLee/dsh_whalebuddy) | 1 | 2026-08-29 | 2026-08-29 | whalebuddy - DeepSeek Harness desktop pet (Windows): a DSH bundle plugin + Tauri shell. A porthole whale reflects your agent live state, with autostart & skin settings. |
| 688 | [33moren33/dsh-slice-bench](https://github.com/33moren33/dsh-slice-bench) | 1 | 2026-08-30 | 2026-08-30 | 把插件放进一台真起来的最小 DSH 机器，让 harness 自己说它站不站得住 · Runtime bench for DSH plugin version conflicts — the harness gives the verdict, not us |
| 689 | [452926826/dsh-ssh-logs](https://github.com/452926826/dsh-ssh-logs) | 1 | 2026-08-25 | 2026-08-26 | Read allowlisted remote logs over SSH from DeepSeek Harness conversations |
| 690 | [6HOLLIS/DSH-Hiyuki-Frost-Sakura](https://github.com/6HOLLIS/DSH-Hiyuki-Frost-Sakura) | 1 | 2026-08-24 | 2026-08-25 | Immersive Hiyuki dual-form skin for DeepSeek Harness Web, with frost/sakura transitions, themed controls, and native DSH layout. |
| 691 | [937862061/dsh-project-workbench](https://github.com/937862061/dsh-project-workbench) | 1 | 2026-08-22 | 2026-08-23 | DeepSeek Harness Web 本地项目工作台：按项目、需求组和会话管理原生对话，并以渐进式共享记忆自动衔接组内上下文。  Local DeepSeek Harness Web plugin that organizes native conversations by project and requirement group, with progressive shared memory automatically carried into each group conversation. |
| 692 | [988hj7tczd-oss/dsh-a11y-scan](https://github.com/988hj7tczd-oss/dsh-a11y-scan) | 1 | 2026-08-24 | 2026-08-24 | DSH native accessibility (WCAG) scanner: runs axe-core over local HTML files / build output / URLs and reports violations as Markdown/HTML/JSON |
| 693 | [988hj7tczd-oss/dsh-asciinema](https://github.com/988hj7tczd-oss/dsh-asciinema) | 1 | 2026-08-24 | 2026-08-24 | DSH plugin: record terminal/tool output as asciinema v2 (.cast), replay with an offline embedded player, and export HTML |
| 694 | [988hj7tczd-oss/dsh-dep-vuln-scan](https://github.com/988hj7tczd-oss/dsh-dep-vuln-scan) | 1 | 2026-08-24 | 2026-08-24 | Scan project lockfiles (npm/pnpm/yarn/pip/go/cargo/maven/gradle) against the free OSV API and report confirmed dependency vulnerabilities with fix versions |
| 695 | [988hj7tczd-oss/dsh-invoice-tools](https://github.com/988hj7tczd-oss/dsh-invoice-tools) | 1 | 2026-08-24 | 2026-08-24 | DSH native tools: parse Chinese e-invoice PDFs into structured JSON with amount cross-check, and generate expense reports (Markdown / xlsx) |
| 696 | [988hj7tczd-oss/dsh-lsp-packs](https://github.com/988hj7tczd-oss/dsh-lsp-packs) | 1 | 2026-08-24 | 2026-08-24 | Out-of-the-box per-language LSP configuration packs for DeepSeek Harness: 12 Cordis plugins (one per language) reusing the shared @deepseek-ai/dsh-lsp-stdio + @deepseek-ai/dsh-tool-lsp base |
| 697 | [988hj7tczd-oss/dsh-mcp-tunnel](https://github.com/988hj7tczd-oss/dsh-mcp-tunnel) | 1 | 2026-08-24 | 2026-08-24 | DSH plugin: expose a local MCP server to remote agents via outbound-only tunnel (mcp-proxy + cloudflared Quick Tunnel) and register the public URL into dsh-mcp-client |
| 698 | [988hj7tczd-oss/dsh-modernize-code](https://github.com/988hj7tczd-oss/dsh-modernize-code) | 1 | 2026-08-24 | 2026-08-24 | DSH skill pack: legacy code modernization workflow (preflight -> assess -> map -> transform) with Cordis mount plugin, offline Python scripts and smoke tests |
| 699 | [988hj7tczd-oss/dsh-pr-description](https://github.com/988hj7tczd-oss/dsh-pr-description) | 1 | 2026-08-24 | 2026-08-24 | DSH native tool: analyze the current branch diff and generate a Conventional Commits PR title, description and self-review checklist |
| 700 | [988hj7tczd-oss/dsh-receipts](https://github.com/988hj7tczd-oss/dsh-receipts) | 1 | 2026-08-24 | 2026-08-24 | Mine local DSH session logs (JSONL) into personal usage & impact receipts: Markdown day/week/month reports plus a self-contained HTML receipt |
| 701 | [988hj7tczd-oss/dsh-workflow-templates](https://github.com/988hj7tczd-oss/dsh-workflow-templates) | 1 | 2026-08-24 | 2026-08-24 | DSH preset workflow template library: 12 reusable orchestration script templates with list/search/run/validate tools |
| 702 | [aa2246740/dsh-auto-review](https://github.com/aa2246740/dsh-auto-review) | 1 | 2026-08-20 | 2026-08-25 | Codex-style Auto-review and Approve for me mode for DeepSeek Harness |
| 703 | [aa2246740/dsh-creator-mode-plus](https://github.com/aa2246740/dsh-creator-mode-plus) | 1 | 2026-08-20 | 2026-08-25 | Fail-closed Creator Mode+ bridge for DeepSeek Harness, supervised externally by DSHX. |
| 704 | [aa2246740/dsh-dragndrop-attachments](https://github.com/aa2246740/dsh-dragndrop-attachments) | 1 | 2026-08-24 | 2026-08-25 | Codex-style drag-and-drop files, folders, ZIP and Office attachments for DeepSeek Harness |
| 705 | [aa2246740/dsh-gateway](https://github.com/aa2246740/dsh-gateway) | 1 | 2026-08-25 | 2026-08-25 | One DSH Host, one messaging Gateway. Bring your own Slack and Feishu apps. |
| 706 | [aa2246740/dsh-oauth-login](https://github.com/aa2246740/dsh-oauth-login) | 1 | 2026-08-15 | 2026-08-25 | Pi-native multi-provider OAuth login for DeepSeek Harness. Independent store — never touches official CLI auth files. |
| 707 | [abbccdd/dsh-localtts](https://github.com/abbccdd/dsh-localtts) | 1 | 2026-08-28 | 2026-08-29 | Local IndexTTS 2.5 and GPT-SoVITS speech synthesis and playback for DeepSeek Harness. |
| 708 | [Abel-86/task-chime](https://github.com/Abel-86/task-chime) | 1 | 2026-08-22 | 2026-08-23 | DSH task chime: play local sounds for approval/permission requests and task completion, configurable from the Web GUI. DSH 任务提示音插件 |
| 709 | [ac0033/dsh-ctm](https://github.com/ac0033/dsh-ctm) | 1 | 2026-08-16 | 2026-08-25 | dsh 插件：CTM 上下文/终端管理，把模型上下文变成可见、可编辑、可评分的一等对象 |
| 710 | [ADDD1118/dsh-balance](https://github.com/ADDD1118/dsh-balance) | 1 | 2026-08-23 | 2026-08-23 | DeepSeek Harness (dsh) balance card — floating glass card (estimated days, balance, conversation usage/cost) + adjustable-size settings card |
| 711 | [AGSQ11/dsh-completion-gate](https://github.com/AGSQ11/dsh-completion-gate) | 1 | 2026-08-22 | 2026-08-22 | Evidence-backed production-readiness barrier for DeepSeek Harness. |
| 712 | [ai-yucheng/dsh-composer-image-tools](https://github.com/ai-yucheng/dsh-composer-image-tools) | 1 | 2026-08-21 | 2026-08-22 | DSH 聊天输入框图片工具(自研):上传图片 + 区域截图,注入草稿图片轨。零依赖,纯客户端+Electron desktopCapturer 截屏。 |
| 713 | [aiworkskills/deepseek-harness-server](https://github.com/aiworkskills/deepseek-harness-server) | 1 | 2026-08-18 | 2026-08-26 | 一个可以接入应用系统的deepseek harness插件，让原有的应用系统快速接入智能体能力 |
| 714 | [ajuwm/dsh-roleplay-plugin](https://github.com/ajuwm/dsh-roleplay-plugin) | 1 | 2026-08-23 | 2026-08-23 | 以角色扮演为主体、桌宠为附加功能的 DeepSeek Harness 插件 |
| 715 | [AKS1st/dock-media](https://github.com/AKS1st/dock-media) | 1 | 2026-08-21 | 2026-08-22 | Media player for the DSH dock: plays audio (music player) and video (fullscreen) files, streamed over HTTP Range. |
| 716 | [alanpaul1969/dsh-agent-sticky-note](https://github.com/alanpaul1969/dsh-agent-sticky-note) | 1 | 2026-08-23 | 2026-08-23 | 📌 Sticky-note plugin for DeepSeek Harness — agent notices & pending decisions visible in the Web GUI (Tailscale-friendly) |
| 717 | [alaxrpg/dsh-adaptive-model-router](https://github.com/alaxrpg/dsh-adaptive-model-router) | 1 | 2026-08-14 | 2026-08-25 | Adaptive model discovery, evaluation, tiering, and subagent routing for DeepSeek Harness |
| 718 | [AlexKaiqi/dsh-realtime-voice](https://github.com/AlexKaiqi/dsh-realtime-voice) | 1 | 2026-08-20 | 2026-08-24 | Full-duplex realtime voice-agent plugin for DeepSeek Harness, with OpenAI Realtime (WebRTC) and Doubao Duplex (WebSocket) adapters. |
| 719 | [AlexZhou19871030/dsh-cron-scheduler](https://github.com/AlexZhou19871030/dsh-cron-scheduler) | 1 | 2026-08-22 | 2026-08-23 | dsh-cron-scheduler |
| 720 | [algerkong/dsh-image-preview](https://github.com/algerkong/dsh-image-preview) | 1 | 2026-08-27 | 2026-08-27 | Image preview for DSH (DeepSeek Harness) web sessions: read_image results render as a thumbnail, click for full size in the built-in lightbox. |
| 721 | [AliceLJY/dsh-thumb](https://github.com/AliceLJY/dsh-thumb) | 1 | 2026-08-21 | 2026-08-25 | A phone shell for the DeepSeek Harness (dsh) web GUI — sidebar becomes an overlay drawer, settings goes full-screen single column. Zero hardcoded host class hashes. |
| 722 | [Alphainfix/wechat-clawbot](https://github.com/Alphainfix/wechat-clawbot) | 1 | 2026-08-24 | 2026-08-24 | 💬 A DeepSeek Harness plugin that brings your DSH agent into WeChat — chat with it from anywhere: native photo understanding, two-way file transfer, long-term memory, scheduled reminders, and permission approvals answered right in the chat. |
| 723 | [amphilagus/dsh-gamer](https://github.com/amphilagus/dsh-gamer) | 1 | 2026-08-20 | 2026-08-28 | DSH bundle + 游戏玩家 preset: play on a dsh-gaming-platform instance. |
| 724 | [anonRTtty/DSH-mobile-remote-mode-plugin](https://github.com/anonRTtty/DSH-mobile-remote-mode-plugin) | 1 | 2026-08-25 | 2026-08-25 | DSH (DeepSeek Harness) mobile remote mode plugin - LAN discovery, QR pairing, Level-1 observer and Level-2 remote prompt from Android/iOS phones and any browser. Multi-platform, early development (Dev0.1). |
| 725 | [Ansonfishing/dsh-ca-ref](https://github.com/Ansonfishing/dsh-ca-ref) | 1 | 2026-08-28 | 2026-08-28 | Clean Architecture reference library for DSH: 8 pinned reference repos with FTS5 search, assertion rules, and a review ledger for architecture reviews |
| 726 | [Ansonfishing/dsh-cap-profile](https://github.com/Ansonfishing/dsh-cap-profile) | 1 | 2026-08-28 | 2026-08-28 | Per-model capability profiling for DSH: turns local session history into tool-usage and error-rate dashboards with time-range filters |
| 727 | [ant404/dsh-media-gen](https://github.com/ant404/dsh-media-gen) | 1 | 2026-08-21 | 2026-08-22 | DSH plugin: generate images and videos via OpenAI-compatible providers, with dedicated settings menu and workspace media_gen output. |
| 728 | [Anyway-one/dsh-image-gen](https://github.com/Anyway-one/dsh-image-gen) | 1 | 2026-08-25 | 2026-08-25 | DeepSeek Harness Image2 生图插件，通过第三方 OpenAI Images 兼容接口调用 gpt-image-2，只需配置  API Key 和 baseURL。 |
| 729 | [anzhaohao/DragView](https://github.com/anzhaohao/DragView) | 1 | 2026-08-24 | 2026-08-25 | Drag-and-drop file attachments and secure in-app previews for DSH. |
| 730 | [anzhaohao/dsh-side-chat-plus-plus](https://github.com/anzhaohao/dsh-side-chat-plus-plus) | 1 | 2026-08-23 | 2026-08-23 | Codex 式多标签侧聊增强 - dsh-side-chat 破坏式 fork(多标签+整条消息引用+去 More details) |
| 731 | [aorucshiea/dsh-easy-start](https://github.com/aorucshiea/dsh-easy-start) | 1 | 2026-08-25 | 2026-08-26 | DSH Web browser lifecycle: ask/close/keep service on browser close, one-click restart with auto refresh |
| 732 | [aorucshiea/dsh-omnipotent-preset](https://github.com/aorucshiea/dsh-omnipotent-preset) | 1 | 2026-08-24 | 2026-08-25 | Omnipotent agent preset for DeepSeek Harness: Standard/PTC/Minimal + routing modes |
| 733 | [Ardig24/dsh-trajectory-ablation](https://github.com/Ardig24/dsh-trajectory-ablation) | 1 | 2026-08-25 | 2026-08-26 | Finds the actual cause of an agent failure by reconstructing, diffing, and ablating its context - a DeepSeek Harness plugin. |
| 734 | [Ares-song-RD/dsh-desktop-pet](https://github.com/Ares-song-RD/dsh-desktop-pet) | 1 | 2026-08-25 | 2026-08-25 | 桌宠插件：在 DeepSeek Harness Web 界面右下角悬浮一只可拖拽、会眨眼摇尾的小猫。A cute desktop pet plugin for the DeepSeek Harness Web GUI. |
| 735 | [ArmyWas/dsh-plugin-reducer](https://github.com/ArmyWas/dsh-plugin-reducer) | 1 | 2026-08-18 | 2026-08-26 | External CLI that finds a 1-minimal DeepSeek Harness plugin set reproducing a profile failure. |
| 736 | [arthur20150522/dsh-token-usage-cost](https://github.com/arthur20150522/dsh-token-usage-cost) | 1 | 2026-08-28 | 2026-08-28 | Shows per-turn and session token costs in DSH web conversations. |
| 737 | [artwar2020/dsh-model-center](https://github.com/artwar2020/dsh-model-center) | 1 | 2026-08-25 | 2026-08-25 | DSH 模型中心插件：免费模型目录 / 真免费实测 / 价格余额 / 一键切换 / 用量统计 — Model center plugin for DeepSeek Harness |
| 738 | [Ary66101/dsh-desktop](https://github.com/Ary66101/dsh-desktop) | 1 | 2026-08-25 | 2026-08-27 | dsh的自制桌面端 |
| 739 | [Ary66101/dsh-instruction-bubble](https://github.com/Ary66101/dsh-instruction-bubble) | 1 | 2026-08-27 | 2026-08-27 | 你的上文语境小气泡 |
| 740 | [awnlight/talon-ui](https://github.com/awnlight/talon-ui) | 1 | 2026-08-28 | 2026-08-28 | A terminal UI for DeepSeek Harness (dsh) agents. |
| 741 | [B1lli/dsh-plugin-bench](https://github.com/B1lli/dsh-plugin-bench) | 1 | 2026-08-22 | 2026-08-23 | Evidence-backed, type-aware quality scorecards for DeepSeek Harness plugins. |
| 742 | [BaiLiang-233/dsh-off-peak-schedule-widget](https://github.com/BaiLiang-233/dsh-off-peak-schedule-widget) | 1 | 2026-08-25 | 2026-08-25 | 价格时段输入队列调度 Harness 插件（dsh-plugin）：高峰拦截输入进休眠区，低谷按队列投递到目标对话 |
| 743 | [bailynlove/web-search-opencode-responses](https://github.com/bailynlove/web-search-opencode-responses) | 1 | 2026-08-21 | 2026-08-22 | dsh WebSearchProvider over the OpenCode Zen Go Responses API server-side web_search tool |
| 744 | [banttethai-ops/dsh-right-editor](https://github.com/banttethai-ops/dsh-right-editor) | 1 | 2026-08-21 | 2026-08-22 | Right-docked file panel for DSH Web: browse any directory and view/edit text, images, Office (docx/xlsx/pptx) and PDF documents. Uses local Python for parsing. |
| 745 | [bao-hp/dsh-check-update](https://github.com/bao-hp/dsh-check-update) | 1 | 2026-08-24 | 2026-08-24 | Check for DSH updates with changelog and backup. |
| 746 | [beartackler/dsh-bridge](https://github.com/beartackler/dsh-bridge) | 1 | 2026-08-25 | 2026-08-26 | Your harness muscle memory, verified and installed into DeepSeek Harness - familiar commands, connectors flow, and a trust-verified plugin catalog |
| 747 | [bescriptkiddie/dsh-wechat-collector](https://github.com/bescriptkiddie/dsh-wechat-collector) | 1 | 2026-08-26 | 2026-08-26 | DSH-native WeChat Official Account collector and ContentStudio handoff. |
| 748 | [better-er/dsh-peak-block](https://github.com/better-er/dsh-peak-block) | 1 | 2026-08-31 | 2026-08-31 | 梁文峰时间高峰自动拦截官方 DeepSeek 请求 |
| 749 | [BharathBillawa/dsh-tool-ddgs](https://github.com/BharathBillawa/dsh-tool-ddgs) | 1 | 2026-08-22 | 2026-08-22 | DuckDuckGo web search and URL fetch tools for DeepSeek Harness, no API key required. Provides web_search (via ddgs) and   web_fetch (via trafilatura) as a drop-in bundle |
| 750 | [BHXiang/auto-pwa](https://github.com/BHXiang/auto-pwa) | 1 | 2026-08-19 | 2026-08-28 | AI驱动的分波分析自动化。 |
| 751 | [big0lives/dsh-web-window-companion](https://github.com/big0lives/dsh-web-window-companion) | 1 | 2026-08-31 | 2026-08-31 | DSH Web 窗口伴侣插件：App 模式窗口打开 Web GUI，关窗即优雅停服。Close the window = stop the server. |
| 752 | [big0lives/dsh-win-quick-launcher](https://github.com/big0lives/dsh-win-quick-launcher) | 1 | 2026-08-31 | 2026-08-31 | DSH 的 Windows 便捷启动器：双击桌面图标启动 DeepSeek Harness Web，关掉浏览器窗口即停服务。支持源码安装与 npm 安装。 |
| 753 | [biliye/dsh-voice-call](https://github.com/biliye/dsh-voice-call) | 1 | 2026-08-16 | 2026-08-31 | 这是一个deepseek专属的语音通话插件 |
| 754 | [Binaryinject/dsh-review-checkout](https://github.com/Binaryinject/dsh-review-checkout) | 1 | 2026-08-26 | 2026-08-28 | dsh-review-checkout |
| 755 | [bingaha/dsh-live-mcp](https://github.com/bingaha/dsh-live-mcp) | 1 | 2026-08-19 | 2026-08-31 | 给DSH提供会话级的MCP控制能力 |
| 756 | [bingfengaaaaa/dsh-jj-vcs](https://github.com/bingfengaaaaa/dsh-jj-vcs) | 1 | 2026-08-22 | 2026-08-22 | Jujutsu version-control plugin and skill for DeepSeek Harness multi-agent teams |
| 757 | [bitterSmilezzz/dsh-plugins](https://github.com/bitterSmilezzz/dsh-plugins) | 1 | 2026-08-18 | 2026-08-25 | DSH 插件伞仓库（DSH Plugin Umbrella）— 所有新增插件的共同遵循仓库：承载插件契约（Pi / DSH 官方 / DSH-Store 准入 / dsh-std 协议）+ 按契约自动校验自有插件（GitHub Actions），经验档案按主题归档。 |
| 758 | [bjzkhy/dsh-token-ledger-pro](https://github.com/bjzkhy/dsh-token-ledger-pro) | 1 | 2026-08-30 | 2026-08-30 | DSH cost panel: meters every request from session events, prices it against a built-in catalog of 136 models across 16 providers, and shows model, balance, session/today/month spend and a monthly budget bar next to the composer. |
| 759 | [BlueChonk/dsh-balance-phoebe](https://github.com/BlueChonk/dsh-balance-phoebe) | 1 | 2026-08-28 | 2026-08-29 | 个人自用 鸣潮菲比查 longcat 剩余 token 挂件 - DSH 插件 |
| 760 | [bobjia/dsh-context-milvus](https://github.com/bobjia/dsh-context-milvus) | 1 | 2026-08-29 | 2026-08-29 | claude-context-milvus like plugin for Deepseek Harness (DSH)  |
| 761 | [Bobnemimimmi/dsh-always-status-bar](https://github.com/Bobnemimimmi/dsh-always-status-bar) | 1 | 2026-08-26 | 2026-08-26 | 始终显示消息下的 status bar，无需鼠标悬停 |
| 762 | [boheastill/phone-eye](https://github.com/boheastill/phone-eye) | 1 | 2026-08-25 | 2026-08-25 | Let your AI agent see and operate a real Android phone — vision + UI-tree fusion over adb, for any MCP client (Claude Code, Codex, dsh…) |
| 763 | [botaochen840-lgtm/fatfish-pet-smart-companion](https://github.com/botaochen840-lgtm/fatfish-pet-smart-companion) | 1 | 2026-08-22 | 2026-08-22 | FatFish Pet Smart Companion - 自包含智能桌面桌宠（改编自 whale-girl），下载即用，可选真连 DeepSeek Harness |
| 764 | [Boy-Grid/dsh-multi-folder-workspace](https://github.com/Boy-Grid/dsh-multi-folder-workspace) | 1 | 2026-08-22 | 2026-08-23 | Multi-folder workspaces for DeepSeek Harness: one workspace spanning several folders, with sessions able to read and write every member. Core patch set + plugin + a one-command npx launcher. |
| 765 | [bruc3van/dsh-doctor](https://github.com/bruc3van/dsh-doctor) | 1 | 2026-08-29 | 2026-08-29 | 帮助 Agent 诊断和升级 DeepSeek Harness 插件，从 DSH 0.1.1 适配到 0.1.2：识别 API 变化、修改代码、处理语义迁移，并为重新发布做好准备。 |
| 766 | [buguoshixc/dsh-user-message-navigator](https://github.com/buguoshixc/dsh-user-message-navigator) | 1 | 2026-08-23 | 2026-08-23 | Codex-style user-message navigation sidebar for DeepSeek Harness Web |
| 767 | [c-ling/dsh-plugin-request-retry](https://github.com/c-ling/dsh-plugin-request-retry) | 1 | 2026-08-23 | 2026-08-23 | DeepSeek Harness 请求重试插件：模型请求失败且错误信息命中关键词时，在内置重试策略耗尽后继续自动追加重试；设置面板可管理关键词与退避参数。 |
| 768 | [caopu16/dsh-local-memory](https://github.com/caopu16/dsh-local-memory) | 1 | 2026-08-27 | 2026-08-27 | DSH（DeepSeek Harness）本地跨会话记忆插件：捕获每轮对话摘要、注入最近几天记忆，并提供 memory_search 工具按需检索全部历史记忆。 |
| 769 | [Carrick-K7/dsh-plugin-source](https://github.com/Carrick-K7/dsh-plugin-source) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness plugin: group the Settings plugin list by origin (official/community), show version, upstream repo link and local-dev marker. Read-only, zero network. |
| 770 | [Castor6/BrowserRig](https://github.com/Castor6/BrowserRig) | 1 | 2026-08-21 | 2026-08-26 | Open-source local driver for trusted agents to control your existing signed-in Chromium browser without browser-wide remote-debugging approval. |
| 771 | [ccll/dsh-activity-pane](https://github.com/ccll/dsh-activity-pane) | 1 | 2026-08-24 | 2026-08-29 | Activity session overview pane for DeepSeek Harness (DSH) web — running sessions, sub-agents, waiting-for-action reminders & recent history at a glance / DSH 活动会话总览窗格 |
| 772 | [cczzyy-cn/c-vision](https://github.com/cczzyy-cn/c-vision) | 1 | 2026-08-22 | 2026-08-23 | DeepSeek Harness (DSH) 视觉插件 —— 给智能体屏幕/窗口视觉 + 电脑使用能力（see/ocr/list_windows + 鼠标键盘操作），跨语言调用捆绑的 Python cvision，Windows / macOS 可用。 |
| 773 | [Charlie-Wang-03/dsh-sightline](https://github.com/Charlie-Wang-03/dsh-sightline) | 1 | 2026-08-23 | 2026-08-27 | See the same repo through every agent's eyes — compare the effective instruction surfaces of DeepSeek Harness, Codex, and Claude Code. 查看同一仓库在 DeepSeek Harness、Codex 与 Claude Code 眼中的不同指令面。 |
| 774 | [chen731215-dev/dsh-muv-engine](https://github.com/chen731215-dev/dsh-muv-engine) | 1 | 2026-08-27 | 2026-08-27 | DSH Native MUV Engine - tavern companion: regex script execution, variable state tracking, iframe status bar rendering, PolyForm-Noncommercial-Copyleft-1.0.0 |
| 775 | [chen731215-dev/dsh-muv-table](https://github.com/chen731215-dev/dsh-muv-table) | 1 | 2026-08-27 | 2026-08-27 | MUV Variable Table Editor - tavern companion plugin for DeepSeek Harness: structured table editing for UpdateVariable blocks, PolyForm-Noncommercial-Copyleft-1.0.0 |
| 776 | [chendefine/dsh-sidebar-cdp-browser](https://github.com/chendefine/dsh-sidebar-cdp-browser) | 1 | 2026-08-19 | 2026-08-27 | deepseek harness live view chromium via cdp in sidebar tab |
| 777 | [chendefine/dsh-web-search-aggregation](https://github.com/chendefine/dsh-web-search-aggregation) | 1 | 2026-08-23 | 2026-08-23 | Aggregated web-search provider for DeepSeek Harness (DSH): one prioritized queue over AnySearch / TinyFish / Tavily with multi-key rotation and ordered fallback. |
| 778 | [chenpengye/dsh-balance-local](https://github.com/chenpengye/dsh-balance-local) | 1 | 2026-08-21 | 2026-08-22 | DeepSeek API balance plugin for DeepSeek Harness (dsh): Settings-page panel + composer badge. Key stays on the Host; browser gets sanitized balance only. |
| 779 | [chenpengye/dsh-balance-whale](https://github.com/chenpengye/dsh-balance-whale) | 1 | 2026-08-21 | 2026-08-22 | 🐳 Floating DeepSeek API balance widget for DeepSeek Harness (dsh) with a whale-girl icon. Key stays on the Host; browser gets sanitized balance only. |
| 780 | [ChenSiyun1234/dsh-tray-windows](https://github.com/ChenSiyun1234/dsh-tray-windows) | 1 | 2026-08-22 | 2026-08-22 | 把 DeepSeek Harness (dsh web) 变成真正的 Windows 桌面应用：托盘控制、独立应用窗口、退出即彻底停止后端（无残留进程）。非官方项目。 |
| 781 | [chenzhi-clude/dsh-hooks-pack](https://github.com/chenzhi-clude/dsh-hooks-pack) | 1 | 2026-08-21 | 2026-08-22 | One-click Claude Code and Codex hooks for DeepSeek Harness: auto-discovers your existing hooks config and runs it on the official bridge plugins. |
| 782 | [cherrchen/dsh-client-ui-details-host](https://github.com/cherrchen/dsh-client-ui-details-host) | 1 | 2026-08-24 | 2026-08-25 | 可移植 DSH Client Details 栏基础设施，在 AppFrame 详情列承载活动 surface；DeepSeek Harness Desktop 内置。 / Portable DSH Client details-column infrastructure for one active AppFrame surface; built into DeepSeek Harness Desktop. |
| 783 | [cherrchen/dsh-plugin-git](https://github.com/cherrchen/dsh-plugin-git) | 1 | 2026-08-23 | 2026-08-25 | DSH Git 仓库服务与 Client UI 插件，依赖 Details Host；DeepSeek Harness Desktop 预装。 / DSH Git repository service and client UI; requires Details Host; pre-installed in DeepSeek Harness Desktop. |
| 784 | [cherrchen/dsh-theme-studio](https://github.com/cherrchen/dsh-theme-studio) | 1 | 2026-08-26 | 2026-08-26 | 可移植的 DSH/Cordis 主题插件：内置配色浏览、预览、应用与持久化；DeepSeek Harness Desktop 预装。 / Portable DSH/Cordis theme overlay plugin with builtin palettes, preview, apply, and persistence; pre-installed in DeepSeek Harness Desktop. |
| 785 | [Chillizu/mop-plugins](https://github.com/Chillizu/mop-plugins) | 1 | 2026-08-15 | 2026-08-26 | MiOpIIk：DeepSeek Harness 单职责插件集 + 四层 agent 工作流 preset（npm: dsh-miopiik） |
| 786 | [chinazkk/dsh-task-panel](https://github.com/chinazkk/dsh-task-panel) | 1 | 2026-08-14 | 2026-08-26 | DSH Web task panel for queued sub-agent execution, scheduled runs, auto review, acceptance, rework, and historical session context. |
| 787 | [chongyangdu2008-cyrus/dsh-subagent-inspector](https://github.com/chongyangdu2008-cyrus/dsh-subagent-inspector) | 1 | 2026-08-28 | 2026-08-28 | Read-only live subagent process inspector for DeepSeek Harness Web |
| 788 | [Circleyan/whiteboat-dsh](https://github.com/Circleyan/whiteboat-dsh) | 1 | 2026-08-25 | 2026-08-25 | Whiteboat for DeepSeek Harness; the quiet water surface is the first feature slice. |
| 789 | [CJL-1995/dsh-session-health](https://github.com/CJL-1995/dsh-session-health) | 1 | 2026-08-23 | 2026-08-24 | a plugin that can judge your Agent session is healthy or not |
| 790 | [CJYLZS/dsh-commandcode-plan-autosync](https://github.com/CJYLZS/dsh-commandcode-plan-autosync) | 1 | 2026-08-28 | 2026-08-28 | auto sync commandcode coding plan models in dsh |
| 791 | [CLASSLU/dsh-telegram-bridge](https://github.com/CLASSLU/dsh-telegram-bridge) | 1 | 2026-08-24 | 2026-08-24 | Telegram bridge for DeepSeek Harness (dsh): chat with your DSH agent from Telegram — access control, skills, workspace browsing, file transfer. |
| 792 | [Cloud-J/dsh-chat-jumper](https://github.com/Cloud-J/dsh-chat-jumper) | 1 | 2026-08-24 | 2026-08-24 | dsh对话导航 |
| 793 | [Cmjingahaha/dsh-dudulu](https://github.com/Cmjingahaha/dsh-dudulu) | 1 | 2026-08-27 | 2026-08-27 | 嘟一声 · DSH 任务完成提示音插件：Agent 回合完成时播放提示音，带设置面板（音量/试听/上传） |
| 794 | [cn-zhangpeng/dsh-shanhai-stats](https://github.com/cn-zhangpeng/dsh-shanhai-stats) | 1 | 2026-08-22 | 2026-08-23 | 山海系列 DeepSeek Harness 用量统计插件：总量徽章、每日走势、GitHub 风格热力图、按模型/提供商分组明细 |
| 795 | [CNSeniorious000/dsh-py-codeact](https://github.com/CNSeniorious000/dsh-py-codeact) | 1 | 2026-08-28 | 2026-08-28 | Python-based CodeAct for dsh with persistent state across cells, replacing Dynamic Workflows and code-mode |
| 796 | [Co1ombiagly/prompt_optimize_dsh](https://github.com/Co1ombiagly/prompt_optimize_dsh) | 1 | 2026-08-30 | 2026-08-31 | DeepSeek Harness (DSH) 提示词优化器插件：一句口语化需求 → 结构化高质量提示词，结果自动填入会话输入框。复用 DSH 内置模型路由，零 API Key 管理。 |
| 797 | [CochraneK/dsh-gate-game-plugin](https://github.com/CochraneK/dsh-gate-game-plugin) | 1 | 2026-08-24 | 2026-08-24 | Logo-eating mini-game + one-click lock button for DeepSeek Harness web UI |
| 798 | [code4lala/dsh-plugin-workspace-path](https://github.com/code4lala/dsh-plugin-workspace-path) | 1 | 2026-08-25 | 2026-08-26 | 可用于在 DSH Web 侧边栏快速查看每个工作区的完整目录路径，减少同名工作区混淆。它作为 DSH 客户端插件安装到 Web profile，在标题下方注入路径副标题并自动换行，支持热加载、位置匹配和重命名或排序后实时同步。 |
| 799 | [CodermanYHZ/dsh-node-flow](https://github.com/CodermanYHZ/dsh-node-flow) | 1 | 2026-08-27 | 2026-08-27 | 节点式 DSH 工作流画布：编排子代理、代码、条件、循环与定时任务，支持模型路由与 AI 生成指南。 Node-mode DSH workflow canvas: orchestrate sub-agents, code, conditions, loops & scheduled tasks. |
| 800 | [coeasy/dsh-go](https://github.com/coeasy/dsh-go) | 1 | 2026-08-23 | 2026-08-24 | DeepSeek Harness 插件市场导航站 |
| 801 | [conafun/dsh-music-plus](https://github.com/conafun/dsh-music-plus) | 1 | 2026-08-29 | 2026-08-29 | 基于 dsh-music-player 的修改版：移除在线QQ/酷狗/讲书/歌词，新增播客 |
| 802 | [crack-time/dsh-archive](https://github.com/crack-time/dsh-archive) | 1 | 2026-08-15 | 2026-08-31 | Session archive plugin for DSH web GUI |
| 803 | [crazy-L118/dsh-desktop-notify](https://github.com/crazy-L118/dsh-desktop-notify) | 1 | 2026-08-25 | 2026-08-26 | Desktop notification plugin for dsh: get a native OS toast when the AI finishes its reply. Toggle lives in dsh Settings → General. |
| 804 | [CSI-entitymorton/stavros-dsh-redteamer](https://github.com/CSI-entitymorton/stavros-dsh-redteamer) | 1 | 2026-08-29 | 2026-08-29 | Authorized-only AI red-team / pentest plugin for the DeepSeek Harness (DSH). Fail-closed scope guard: Stavros persona, 24 specialist subagents, 78 zero-dependency tools. |
| 805 | [czj-git/dsh-plugin-hub](https://github.com/czj-git/dsh-plugin-hub) | 1 | 2026-08-27 | 2026-08-27 | DeepSeek Harness tools for searching and ranking verified plugins from DSH Plugin Hub |
| 806 | [czx1111/dsh-plugin-manager](https://github.com/czx1111/dsh-plugin-manager) | 1 | 2026-08-22 | 2026-08-25 | dsh-plugin-manager |
| 807 | [D-Robotics/dsh-plugin-rdk](https://github.com/D-Robotics/dsh-plugin-rdk) | 1 | 2026-08-14 | 2026-08-28 | D-Robotics RDK (地瓜机器人) integration for DeepSeek Harness — native RDK skill catalog, rdk_skills browser tool, and rdk_board_detect device detection |
| 808 | [D2Moqi/dsh-openwiki](https://github.com/D2Moqi/dsh-openwiki) | 1 | 2026-08-29 | 2026-08-29 | DSH 插件：把 openwiki 的代码库知识库能力搬进 DeepSeek Harness —— 一键生成 / 阅读 / 更新仓库 Wiki 与 Grounded Claims（溯源知识卡片），直接复用 DSH 已配置的模型，无需二次填 Key。 |
| 809 | [d3vmeh/dsh-fetch-timeouts](https://github.com/d3vmeh/dsh-fetch-timeouts) | 1 | 2026-08-30 | 2026-08-30 | DeepSeek Harness plugin: raise Node's HTTP timeouts process-wide so slow local models (Ollama, LM Studio) are not cut off at 5 minutes |
| 810 | [d3vmeh/dsh-llm-gate](https://github.com/d3vmeh/dsh-llm-gate) | 1 | 2026-08-29 | 2026-08-29 | Per-provider concurrency gate for DeepSeek Harness model requests |
| 811 | [DahliaVoid/dsh-temp-session](https://github.com/DahliaVoid/dsh-temp-session) | 1 | 2026-08-28 | 2026-08-28 | dsh工作区可选化，100%纯AI coding产物 |
| 812 | [daishengli/dsh-docker](https://github.com/daishengli/dsh-docker) | 1 | 2026-08-27 | 2026-08-28 | 使用 Docker 封装运行 deepseek-harness d的 Web 服务。容器内运行 dsh 和 Caddy，宿主机通过 3080 端口访问服务。 |
| 813 | [danhcng3822f/dsh-mcp-kimicodeandmgr](https://github.com/danhcng3822f/dsh-mcp-kimicodeandmgr) | 1 | 2026-08-21 | 2026-08-22 | MCP engine and manager for DeepSeek Harness. Fork of yangfch3/dsh-mcp-mgr, MCP layer rebuilt on kimi-code's architecture: self-contained engine, three config layers, transport-driven status. |
| 814 | [DaoCaoRenH/dsh-openai-responses-bridge](https://github.com/DaoCaoRenH/dsh-openai-responses-bridge) | 1 | 2026-08-19 | 2026-08-22 | DeepSeek Harness plugin for third-party OpenAI Responses and native Gemini APIs, with custom providers, model discovery, and hosted web search. |
| 815 | [daodishisha28/dsh-sidechat-plugin](https://github.com/daodishisha28/dsh-sidechat-plugin) | 1 | 2026-08-30 | 2026-08-31 | Open a persistent side conversation from any DeepSeek Harness session to investigate questions, clarify requirements, or explore alternatives without polluting the main task’s context, then review and send a concise conclusion back to the parent conversation. Tested with DSH 0.1.2-alpha.1. |
| 816 | [dat-lequoc/dsh-opinionated-subagent](https://github.com/dat-lequoc/dsh-opinionated-subagent) | 1 | 2026-08-27 | 2026-08-28 | A minimal, opinionated subagent for DeepSeek Harness: you choose which models a child may run on and at which reasoning effort, and a correction reaches a working child at its next step |
| 817 | [dat-lequoc/dsh-supervisor](https://github.com/dat-lequoc/dsh-supervisor) | 1 | 2026-08-22 | 2026-08-22 | Always-on supervisor agent bundle for DeepSeek Harness: main-agent preset + schedule overlay, one dsh plugin add away |
| 818 | [DaXiGua732/start-dsh](https://github.com/DaXiGua732/start-dsh) | 1 | 2026-08-22 | 2026-08-22 | 一个能够直接快速启动DSH的ps脚本，具备高峰时段检测功能，高峰时段启动时不会直接进入DSH，反之直接进入，帮助个人开发者省钱省力 |
| 819 | [DDDFXYqiming/dsh-session-recap](https://github.com/DDDFXYqiming/dsh-session-recap) | 1 | 2026-08-28 | 2026-08-28 | Session recap plugin for DeepSeek Harness (Claude Code-style away summaries) |
| 820 | [ddtcorex/dsh-maestro-ci](https://github.com/ddtcorex/dsh-maestro-ci) | 1 | 2026-08-26 | 2026-08-28 | Reusable GitHub Actions workflows for the Maestro suite — Cordis / DSH |
| 821 | [ddtcorex/dsh-maestro-config](https://github.com/ddtcorex/dsh-maestro-config) | 1 | 2026-08-25 | 2026-08-26 | Maestro Config — shared settings service for the dsh-maestro-* suite over the single namespaced store (~/.dsh/maestro/settings.json) |
| 822 | [ddtcorex/dsh-maestro-config-lib](https://github.com/ddtcorex/dsh-maestro-config-lib) | 1 | 2026-08-25 | 2026-08-28 | Maestro settings store library — atomic namespaced JSON store shared by dsh-maestro-* plugins (embedded dependency, no Cordis row) |
| 823 | [ddtcorex/dsh-maestro-dashboard](https://github.com/ddtcorex/dsh-maestro-dashboard) | 1 | 2026-08-28 | 2026-08-28 | Maestro Dashboard — unified Control Center (Overview/Plugins/Usage) DSH-native |
| 824 | [ddtcorex/dsh-maestro-devkit](https://github.com/ddtcorex/dsh-maestro-devkit) | 1 | 2026-08-27 | 2026-08-28 | General development toolkit for DeepSeek Harness — visual review, HMR, style inspector, Cordis/Govard/Skills dev (tunnel-aware) |
| 825 | [ddtcorex/dsh-maestro-diagram](https://github.com/ddtcorex/dsh-maestro-diagram) | 1 | 2026-08-27 | 2026-08-28 | DSH Maestro diagram studio — mermaid_verify + mermaid_drift |
| 826 | [ddtcorex/dsh-maestro-govard](https://github.com/ddtcorex/dsh-maestro-govard) | 1 | 2026-08-25 | 2026-08-26 | Thin bridge exposing the Govard CLI to DeepSeek Harness agents as tools. |
| 827 | [ddtcorex/dsh-maestro-guard](https://github.com/ddtcorex/dsh-maestro-guard) | 1 | 2026-08-25 | 2026-08-26 | Host-only safety gate for DeepSeek Harness: approval store, secret redaction, permission policy, waterfall pre-execute integration. |
| 828 | [ddtcorex/dsh-maestro-meta](https://github.com/ddtcorex/dsh-maestro-meta) | 1 | 2026-08-24 | 2026-08-26 | Maestro Harness meta-bundle: one plugin to install the whole Govard + DSH harness |
| 829 | [ddtcorex/dsh-maestro-mobile](https://github.com/ddtcorex/dsh-maestro-mobile) | 1 | 2026-08-24 | 2026-08-25 | Portrait & mobile adaptation for the DeepSeek Harness Web UI — overlay drawer, full-width conversation, sheet dialogs, safe-area handling. Below 1024px it adapts; at ≥1024px it is a no-op. |
| 830 | [ddtcorex/dsh-maestro-notifier](https://github.com/ddtcorex/dsh-maestro-notifier) | 1 | 2026-08-25 | 2026-08-26 | Maestro Notifier — pluggable notifier service for DeepSeek Harness (Telegram first; registry open to further providers) |
| 831 | [ddtcorex/dsh-maestro-observe](https://github.com/ddtcorex/dsh-maestro-observe) | 1 | 2026-08-25 | 2026-08-26 | Observability / debug tooling for DeepSeek Harness: trace, cost, and health capture + client dashboard. |
| 832 | [ddtcorex/dsh-maestro-remote](https://github.com/ddtcorex/dsh-maestro-remote) | 1 | 2026-08-25 | 2026-08-26 | Remote access for DeepSeek Harness via cloudflared tunnel + proxy, with PIN auth and Telegram notifications. |
| 833 | [ddtcorex/dsh-maestro-review](https://github.com/ddtcorex/dsh-maestro-review) | 1 | 2026-08-25 | 2026-08-26 | Pluggable merge-request review pipeline for DeepSeek Harness (webhook → orchestrator → findings) with GitLab + GitHub providers. |
| 834 | [DecarbonizedGlucose/dsh-memory-note](https://github.com/DecarbonizedGlucose/dsh-memory-note) | 1 | 2026-08-17 | 2026-08-23 | Lightweight local cross-session memory for DeepSeek Harness |
| 835 | [deluo/dsh-usage-display](https://github.com/deluo/dsh-usage-display) | 1 | 2026-08-22 | 2026-08-23 | 在 dsh（DeepSeek Harness）会话头部展示模型厂商余额/用量徽标的插件：内置 DeepSeek 余额、MiniMax Token Plan 与智谱 GLM Coding Plan 配额，适配器架构支持接入更多厂商；host 侧按轮次取数，经 SSE 同步到浏览器。 |
| 836 | [demo007x/dsh-web-mermaid](https://github.com/demo007x/dsh-web-mermaid) | 1 | 2026-08-21 | 2026-08-22 | Deepseek harness mermaid流程图渲染插件 |
| 837 | [dfzjb/whalemaid-desktop-pet](https://github.com/dfzjb/whalemaid-desktop-pet) | 1 | 2026-08-24 | 2026-08-25 | 像素风蓝发鲸鱼女仆桌面宠物 · DSH Agent 桌面入口 · Electron + TypeScript |
| 838 | [dHR-P/dsh-safe-launch](https://github.com/dHR-P/dsh-safe-launch) | 1 | 2026-08-23 | 2026-08-23 | DSH (DeepSeek Harness) plugin: dsh-safe-launch - desktop safe-start launcher with last-good boot config, consent-gated canary updates for dsh & plugins, compatibility-checked plugin installation. DeepSeek Harness safe launcher plugin |
| 839 | [difimim/dsh-voice-input-npm](https://github.com/difimim/dsh-voice-input-npm) | 1 | 2026-08-30 | 2026-08-30 | 语音输入插件 for Deepseek Harness |
| 840 | [DiligenceLai/dsh-memory-ga](https://github.com/DiligenceLai/dsh-memory-ga) | 1 | 2026-08-22 | 2026-08-22 | Gated GA-style layered memory for DeepSeek Harness: hard-injected L1 index + RULES, session working checkpoint, settlement ritual to Skills/L1/L2 - no silent auto-retain. |
| 841 | [Diluka/dsh-persona](https://github.com/Diluka/dsh-persona) | 1 | 2026-08-25 | 2026-08-26 | Configurable coding collaboration style prompts and settings UI for DeepSeek Harness. |
| 842 | [dingminhua/dsh-connect-workbuddy](https://github.com/dingminhua/dsh-connect-workbuddy) | 1 | 2026-08-28 | 2026-08-30 | Connect locally signed-in WorkBuddy models to DeepSeek Harness with a read-only credits overview and model management. |
| 843 | [Dingpenghui-good/dsh-plugin-manager](https://github.com/Dingpenghui-good/dsh-plugin-manager) | 1 | 2026-08-16 | 2026-08-23 | Writable plugin management tab for DeepSeek Harness - toggle, enable/disable, and uninstall user-installed Cordis plugins from Settings |
| 844 | [dingyi580/dsh-plugin-gemini-theme](https://github.com/dingyi580/dsh-plugin-gemini-theme) | 1 | 2026-08-29 | 2026-08-30 | A Gemini-styled skin for the DeepSeek Harness web client |
| 845 | [DK-Zhu/dsh-consult](https://github.com/DK-Zhu/dsh-consult) | 1 | 2026-08-21 | 2026-08-24 | Evidence-first multi-model consultation for DeepSeek Harness: 2–5 independently configured models review the same evidence, and the main agent synthesizes their anonymous opinions. |
| 846 | [domitor-syh/dsh-ui-skin-switcher](https://github.com/domitor-syh/dsh-ui-skin-switcher) | 1 | 2026-08-27 | 2026-08-28 | Model & reasoning-effort switcher plugin for DeepSeek Harness (DSH): composer seat with Off/Max effort slider. DSH 插件：模型与思考力度切换器。 |
| 847 | [doublemolu/dsh-balance-dock](https://github.com/doublemolu/dsh-balance-dock) | 1 | 2026-08-28 | 2026-08-28 | DeepSeek Harness balance dock: balance card, per-conversation spend/tokens, 50-yuan segmented progress bar, recharge button, position guard |
| 848 | [drscrewdriver/dsh-llm-openai-completions](https://github.com/drscrewdriver/dsh-llm-openai-completions) | 1 | 2026-08-29 | 2026-08-29 | dsh-llm-openai-completions |
| 849 | [dsh-ai-org/top-dsh-plugins](https://github.com/dsh-ai-org/top-dsh-plugins) | 1 | 2026-08-22 | 2026-08-22 | 📈 Daily-updated DeepSeek Harness plugin rankings · 每日更新的 DSH 插件榜单 — powered by dsh-ai.org |
| 850 | [duyanta123/dsh-refactor-insight](https://github.com/duyanta123/dsh-refactor-insight) | 1 | 2026-08-22 | 2026-08-23 | Turn codebase smells into an executable, priority-ordered refactoring plan (file-length / deep-nesting / TODO-density). |
| 851 | [EastMG/dsh-gacha-calendar](https://github.com/EastMG/dsh-gacha-calendar) | 1 | 2026-08-27 | 2026-08-30 | DeepSeek Harness 二游卡池/活动排期速查插件：侧边栏按钮 内置 11 款主流二游 可添加自定义游戏 |
| 852 | [Edge-Echo/dsh-netassist](https://github.com/Edge-Echo/dsh-netassist) | 1 | 2026-08-30 | 2026-08-30 | Network & proxy assistant for DeepSeek Harness (dsh): one-shot GitHub connectivity check, system proxy status, proxy port probing, full diag chain and hosts conflict scan. |
| 853 | [Edge-Echo/dsh-win-toolkit](https://github.com/Edge-Echo/dsh-win-toolkit) | 1 | 2026-08-30 | 2026-08-30 | Windows-native capability pack for DeepSeek Harness (dsh): clipboard, notifications, hosts file, network diagnostics — safe PowerShell-backed tools. |
| 854 | [Elave-66/dsh-blue-sea-player](https://github.com/Elave-66/dsh-blue-sea-player) | 1 | 2026-08-23 | 2026-08-23 | 蓝海之约鲸鱼娘 DSH 播放器插件：12 套皮肤 · 5 首默认音乐 · CD 旋转封面 · 收纳小球 |
| 855 | [elizax/dsh-http-proxy](https://github.com/elizax/dsh-http-proxy) | 1 | 2026-08-26 | 2026-08-26 | 支持设置LLM的代理地址 |
| 856 | [elmaxid/dsh-manage](https://github.com/elmaxid/dsh-manage) | 1 | 2026-08-21 | 2026-08-22 | Instalacion y administracion de DeepSeek Harness (dsh): install/start/stop/update/status para puestos dev |
| 857 | [Elpsycoogroo/dsh-work-report](https://github.com/Elpsycoogroo/dsh-work-report) | 1 | 2026-08-28 | 2026-08-28 | Neural Ledger - turn DSH collaboration sessions into a visual work ledger: token analytics, smart insights, trend forecasting, and one-click daily/weekly/monthly Markdown reports. |
| 858 | [emeryxu1-blip/dsh-matrix-skin](https://github.com/emeryxu1-blip/dsh-matrix-skin) | 1 | 2026-08-22 | 2026-08-24 | Black-first Matrix hacker skin for DeepSeek Harness (DSH) Web — live session-powered code rain and readable provider reasoning. |
| 859 | [enoughpower/dsh-harmony](https://github.com/enoughpower/dsh-harmony) | 1 | 2026-08-22 | 2026-08-23 | DSH Harmony 客户端 搭配 dsh-pocket 使用 |
| 860 | [Entaum/dsh-free-games](https://github.com/Entaum/dsh-free-games) | 1 | 2026-08-30 | 2026-08-31 | Deepseek Harness free games plugin. Play while coding! |
| 861 | [ErrorLst/dsh-code-pipeline](https://github.com/ErrorLst/dsh-code-pipeline) | 1 | 2026-08-23 | 2026-08-24 | DSH bundle plugin: 为 code-pipeline 预设（PTC 流水线）动态注入阶段子代理工具（subagent_plan / subagent_impl / subagent_review），各阶段 provider/model/思考等级可在设置页实时配置 |
| 862 | [esonx/dsh-project-j4agent](https://github.com/esonx/dsh-project-j4agent) | 1 | 2026-08-24 | 2026-08-24 | Agent-native Software Development Lifecycle Management for DeepSeek Harness |
| 863 | [EternalNight996/memory-eternal](https://github.com/EternalNight996/memory-eternal) | 1 | 2026-08-31 | 2026-08-31 | 记忆核心（Memory Eternal）：自研的 DeepSeek Harness 记忆插件——对话结束自动沉淀知识卡到本地 Markdown Vault（自研去重 / 自研 CJK 检索 / 知识图谱 + 审核中心 / 回收中心），Agent 通过 memory_recall 按需召回历史上下文，零人工干预。 |
| 864 | [Evan1u/deepseek-harness-desktop](https://github.com/Evan1u/deepseek-harness-desktop) | 1 | 2026-08-22 | 2026-08-23 | Light-weight Desktop App for Deepseek Harness |
| 865 | [Evhye38496/dsh-perfscope](https://github.com/Evhye38496/dsh-perfscope) | 1 | 2026-08-23 | 2026-08-24 | One-click health check & score for your DeepSeek Harness plugins. Scan -> Score -> Fix -> Share. PerfScope for dsh. |
| 866 | [exoticknight/dsh-theme-eink-retro](https://github.com/exoticknight/dsh-theme-eink-retro) | 1 | 2026-08-26 | 2026-08-26 | A paper-and-ink client-side theme for DeepSeek Harness with Balanced and Immersive modes. |
| 867 | [f1yan9/dsh-balance-pie](https://github.com/f1yan9/dsh-balance-pie) | 1 | 2026-08-30 | 2026-08-30 | DSH 插件：可拖拽余额饼图 / 真实消耗 / 历史热力图 — balance pie with real spending & monthly heatmap for DeepSeek Harness. |
| 868 | [falling-ts/dsh-web-ding](https://github.com/falling-ts/dsh-web-ding) | 1 | 2026-08-27 | 2026-08-27 | Browser-only 'ding' on agent end; works on servers.浏览器专属"叮":回合结束时响起,服务器部署也生效 |
| 869 | [fallow5/dsh-pin-sessions](https://github.com/fallow5/dsh-pin-sessions) | 1 | 2026-08-28 | 2026-08-31 | DSH (DeepSeek Harness) web plugin: pin sessions to the top of the sidebar for quick access to recurring workflows. Includes archive panel with batch delete, restore, and workspace grouping. |
| 870 | [fan56/dsh-model-sync](https://github.com/fan56/dsh-model-sync) | 1 | 2026-08-28 | 2026-08-29 | A dsh (DeepSeek Harness) Cordis plugin that keeps llm-pi-ai provider routes' model catalog in sync with the pi.dev gateway — written through the official settings seam, zero patches to dsh internals. |
| 871 | [fan56/dsh-subagent-registry](https://github.com/fan56/dsh-subagent-registry) | 1 | 2026-08-16 | 2026-08-28 | dsh plugin: register ~/.dsh/agents/*.md as dsh-callable subagents |
| 872 | [FanetheDivine/dsh-plugin-om](https://github.com/FanetheDivine/dsh-plugin-om) | 1 | 2026-08-15 | 2026-08-27 | DSH插件，以Observational Memory方式管理上下文 |
| 873 | [fatatalia/dsh-dreaming](https://github.com/fatatalia/dsh-dreaming) | 1 | 2026-08-18 | 2026-08-25 | dsh 梦境记忆整合插件：凌晨随机窗口把记忆梦境化（裸上下文 narrative 纯梦写作）+ 信号驱动洞察晋升 + MEMORY.md 预算管理，随 dsh web 启停 |
| 874 | [FeatherHunter/dsh-plugin-ui-debug](https://github.com/FeatherHunter/dsh-plugin-ui-debug) | 1 | 2026-08-18 | 2026-08-22 | DSH 插件 UI 调试神器：让 AI 在真实 Chrome 中帮你看界面、点按钮、拖组件，一键安装零配置 |
| 875 | [felix-lj-ct/dsh-mcp-workspace-scope](https://github.com/felix-lj-ct/dsh-mcp-workspace-scope) | 1 | 2026-08-31 | 2026-08-31 | Scopes MCP tool injection per workspace directory in the DeepSeek Harness: a session opened in a project sees only the MCP servers that project needs — removed from the model's tool list and refused at call time. Plus per-session switches in the composer to narrow or widen the session you are in, temporarily. |
| 876 | [fengb3/dsh-theme-aurum](https://github.com/fengb3/dsh-theme-aurum) | 1 | 2026-08-24 | 2026-08-28 | DSH 鎏金主题插件:金粉奢华皮肤,htm 恒等映射流水,原型驱动的逐节移植 |
| 877 | [fenglin-ai/dsh-funasr-voice](https://github.com/fenglin-ai/dsh-funasr-voice) | 1 | 2026-08-22 | 2026-08-23 | DeepSeek Harness 本地离线语音输入插件：麦克风 → FunASR(SenseVoice) → 输入框，全离线识别。 |
| 878 | [fjzzwxp/dsh-mnemosyne-memory](https://github.com/fjzzwxp/dsh-mnemosyne-memory) | 1 | 2026-08-24 | 2026-08-25 | Mnemosyne 永久记忆插件 - 为 DSH 提供长期记忆、向量搜索和 LLM 反思功能，对标 Hindsight Coding Agents |
| 879 | [flg1217/dsh-quick-commands](https://github.com/flg1217/dsh-quick-commands) | 1 | 2026-08-24 | 2026-08-24 | User-defined slash commands for DeepSeek Harness: configure quick commands (name + prompt) in the settings panel; /name inserts a chip that expands to the prompt on send. |
| 880 | [flyhigao/dsh-produced-file-paths](https://github.com/flyhigao/dsh-produced-file-paths) | 1 | 2026-08-20 | 2026-08-23 | DSH Web plugin to show and copy absolute paths for produced files |
| 881 | [focksor/dsh-plugin-mini-dashboard](https://github.com/focksor/dsh-plugin-mini-dashboard) | 1 | 2026-08-28 | 2026-08-28 | A session & token mini dashboard for DSH web. It renders just above the sidebar's "Settings" row and summarizes, in one small draggable float window, what your sessions are doing right now and what they have cost you today. |
| 882 | [focksor/dsh-plugin-node-time](https://github.com/focksor/dsh-plugin-node-time) | 1 | 2026-08-29 | 2026-08-31 | Hover timestamps for DSH web. Hovering a chat node row — Think, Bash, Read/Edit/Write, Search, commands, compaction markers, sub-calls — pops a compact card with that node's start time → end time and how long it took. |
| 883 | [focksor/dsh-plugin-thinking-size](https://github.com/focksor/dsh-plugin-thinking-size) | 1 | 2026-08-28 | 2026-08-28 | A live reasoning-token badge for DSH web. It appends a compact Think(128) / Think(5.2K) marker to the title of every "Think" disclosure row in the conversation — ticking in real time while the model is still thinking, and staying put on history messages afterwards. |
| 884 | [FranklinZaneDurant/agent-discipline](https://github.com/FranklinZaneDurant/agent-discipline) | 1 | 2026-08-27 | 2026-08-27 | 给 AI 编码 Agent 的仓库工作纪律插件（DeepSeek Harness bundle）：方法论提示段 + 工件脚手架（AGENTS.md/特性清单/验证门）+ 合规审计。 |
| 885 | [Freakz2z/dsh-evidence-ledger](https://github.com/Freakz2z/dsh-evidence-ledger) | 1 | 2026-08-24 | 2026-08-24 | Local append-only evidence ledger for DeepSeek Harness |
| 886 | [Frog755/dsh-wallpaper](https://github.com/Frog755/dsh-wallpaper) | 1 | 2026-08-15 | 2026-08-24 | Persistent wallpaper plugin for DeepSeek Harness with opacity, blur, and a fixed web origin. |
| 887 | [fsrmqi/dsh-promptkit](https://github.com/fsrmqi/dsh-promptkit) | 1 | 2026-08-26 | 2026-08-26 | Prompt building & enhancement toolkit for DeepSeek Harness: Studio + QuickEnhancer. 开源的 Prompt 构建与增强工具包。 |
| 888 | [fufengyuan/dsh-council](https://github.com/fufengyuan/dsh-council) | 1 | 2026-08-26 | 2026-08-27 | dsh-council — 高智议会（Council of High Intelligence）for DeepSeek Harness 在 dsh（DeepSeek Harness）里召集历史人物议会，对复杂问题进行多视角结构化辩论，最终由主席综合裁决。 |
| 889 | [Fz2hOpenSource/firmware-forge](https://github.com/Fz2hOpenSource/firmware-forge) | 1 | 2026-08-24 | 2026-08-25 | 基于 DSH 的 AI 嵌入式固件工程工作台，覆盖固件设计、协议设计、测试验证、编译、烧录与调试闭环。 |
| 890 | [g-yixuan/dsh-sidenote](https://github.com/g-yixuan/dsh-sidenote) | 1 | 2026-08-19 | 2026-08-28 | Codex-style side chat & selection annotations for DeepSeek Harness (DSH) web — fork the session into a persistent side panel; quote selections into context. Thin consumer of dsh-better-sidebar. |
| 891 | [Gaines-cz/dsh-a-share-screener](https://github.com/Gaines-cz/dsh-a-share-screener) | 1 | 2026-08-21 | 2026-08-22 | A-share stock screening plugin for DeepSeek Harness (dsh): pluggable strategies, Tushare token via credentials ref, free Eastmoney/Tencent fallback. |
| 892 | [georesearch-dsh/georesearch-dsh](https://github.com/georesearch-dsh/georesearch-dsh) | 1 | 2026-08-27 | 2026-08-28 | GeoResearch agent plugin for DeepSeek Harness |
| 893 | [Georgehaoren/DSH-WhaleConsole](https://github.com/Georgehaoren/DSH-WhaleConsole) | 1 | 2026-08-29 | 2026-08-29 | Unofficial macOS desktop companion and WebUI skin plugin for DeepSeek Harness. 面向 DeepSeek Harness 的非官方 macOS 桌面伴侣与 WebUI 换肤插件。 |
| 894 | [goldgish/dsh-agent-trace](https://github.com/goldgish/dsh-agent-trace) | 1 | 2026-08-26 | 2026-08-26 | Agent Trace — visualize an agent's reasoning, parallel tool calls, and results as an interactive DAG inside DeepSeek Harness. |
| 895 | [GooDAnDReaDY/dsh-lanmode](https://github.com/GooDAnDReaDY/dsh-lanmode) | 1 | 2026-08-20 | 2026-08-25 | LAN network routing and browser media API compatibility helper for DeepSeek Harness Web UI |
| 896 | [GooDAnDReaDY/dsh-subscriptions](https://github.com/GooDAnDReaDY/dsh-subscriptions) | 1 | 2026-08-21 | 2026-08-25 | OAuth subscription LLM providers for DeepSeek Harness (Codex, Claude, Grok, Antigravity) |
| 897 | [goodie1972/prompt-optimizer](https://github.com/goodie1972/prompt-optimizer) | 1 | 2026-08-24 | 2026-08-25 | 🔮 Multi-tool AI prompt optimizer plugin for ZCode, Claude Code, Codex CLI, Reasonix, DSH, MimoCode, OpenCode — 中文提示词优化插件 \| AI prompt optimizer plugin with /optimize command and optimize_prompt MCP tool |
| 898 | [graceen2331-prog/find-plugin](https://github.com/graceen2331-prog/find-plugin) | 1 | 2026-08-23 | 2026-08-23 | DeepSeek Harness tool for finding and verifying community DSH plugins on GitHub |
| 899 | [gtbwpkwjnb-alt/learn-skill](https://github.com/gtbwpkwjnb-alt/learn-skill) | 1 | 2026-06-21 | 2026-08-23 | 学习+链接 → 全自动采集·AI总结·亮点·术语·评分·图谱·深度OCR·入库 \| One link → AI analysis+highlights+glossary+rating+knowledge graph → KB import (v3.5) |
| 900 | [gtbwpkwjnb-alt/skills-summarize-audit-skill](https://github.com/gtbwpkwjnb-alt/skills-summarize-audit-skill) | 1 | 2026-06-18 | 2026-08-23 | Skills Audit — 技能审查·画像·评分·优化 / Universal agent tool auditor — profile, score, optimize |
| 901 | [gtbwpkwjnb-alt/summarize-skill](https://github.com/gtbwpkwjnb-alt/summarize-skill) | 1 | 2026-06-17 | 2026-08-23 | 会话级全维总结 — 项目·进度·建议·错误，一个命令全清 \| Session-level summary for project/progress/suggestion/error |
| 902 | [guhanfei-ai/dsh-mindmap](https://github.com/guhanfei-ai/dsh-mindmap) | 1 | 2026-08-22 | 2026-08-23 | 让DSH帮你快速制作思维脑图 |
| 903 | [GuionAI/web](https://github.com/GuionAI/web) | 1 | 2026-08-22 | 2026-08-30 | A web research toolkit with multi-provider search and clean Markdown extraction from static and JavaScript-rendered pages, plus public code and library docs search—available via CLI and MCP. |
| 904 | [gulagala001/dsh-trisoul](https://github.com/gulagala001/dsh-trisoul) | 1 | 2026-08-27 | 2026-08-27 | TriSoul —— 三魂共识 Agent：三个灵魂盲写+匿名互评，三官（对齐/博识/实证）补偿生成，画布式上下文，记忆中枢。DeepSeek Harness 插件套件，一键装/独立端口/一键卸载 |
| 905 | [GuoFengyu110429/dsh-high-fee-alert](https://github.com/GuoFengyu110429/dsh-high-fee-alert) | 1 | 2026-08-24 | 2026-08-25 | 一个由DSH制作的插件，用于在峰谷中的峰时段进行提醒以节省费用。 |
| 906 | [Gyanano/dsh-grok-auth](https://github.com/Gyanano/dsh-grok-auth) | 1 | 2026-08-22 | 2026-08-23 | DeepSeek Harness plugin that reuses the official Grok CLI login (SuperGrok / X Premium OAuth) for an xai LLM route |
| 907 | [hackernotfound/dsh-tacit](https://github.com/hackernotfound/dsh-tacit) | 1 | 2026-08-27 | 2026-08-27 | Learns what you leave unsaid in your prompts and steers the DeepSeek Harness agent for you |
| 908 | [Hades03/dsh-model-quota-usage](https://github.com/Hades03/dsh-model-quota-usage) | 1 | 2026-08-22 | 2026-08-22 | DeepSeek Harness plugin: DeepSeek balance and per-provider/model token usage in a draggable overlay. |
| 909 | [having5548/dsh-notify](https://github.com/having5548/dsh-notify) | 1 | 2026-08-23 | 2026-08-24 | Universal notification plugin for DeepSeek Harness: in-app toasts, native Windows toasts, one-click approval from the action center |
| 910 | [heiheiha798/dsh-plugin-response-window](https://github.com/heiheiha798/dsh-plugin-response-window) | 1 | 2026-08-24 | 2026-08-24 | DeepSeek Harness (DSH) web plugin: wrap each prompt-to-prompt turn's response (tool calls + assistant text) in a bounded-height scrollable window/slide, Grok-build style. |
| 911 | [hejielijob-commits/SemaRail](https://github.com/hejielijob-commits/SemaRail) | 1 | 2026-08-17 | 2026-08-30 | Governed semantic layer for AI agents, with a DeepSeek Harness plugin that turns Harness into a data agent. |
| 912 | [helibeiqi/dsh-csp-runtime](https://github.com/helibeiqi/dsh-csp-runtime) | 1 | 2026-08-23 | 2026-08-24 | Cognitive State Protocol (CSP) v0.1 — the cross-framework interop layer that makes AI thinking state serializable, persistable, and transferable. Host-side Cordis plugin for the DSH ecosystem. |
| 913 | [henrychenhao/dsh-skin-argentina](https://github.com/henrychenhao/dsh-skin-argentina) | 1 | 2026-08-27 | 2026-08-27 | 梅西 阿根廷皮肤 |
| 914 | [HenryPhoebe/dsh-plugin-easyppt](https://github.com/HenryPhoebe/dsh-plugin-easyppt) | 1 | 2026-08-27 | 2026-08-27 | easyppt是一个面向 DeepSeek Harness (DSH) 的演示文稿生成 dsh-plugin（npm 包 + Cordis bundle + 内置技能）。用户输入大纲（Markdown / JSON / 自然语言）与插图，即可基于 DSH 原生 Univer 工具链生成PPTX,HTML,JSON |
| 915 | [hgl011091/dsh-rss-monitor](https://github.com/hgl011091/dsh-rss-monitor) | 1 | 2026-08-28 | 2026-08-28 | DeepSeek Harness 原生 RSS 订阅监控插件：多源订阅、关键词过滤、定时检查去重、新条目邮件通知（缩略图 HTML 模板），SMTP 密码走凭据库永不落盘，原生设置页四页签体验。 |
| 916 | [hhb1028/dsh-retry-boost](https://github.com/hhb1028/dsh-retry-boost) | 1 | 2026-08-27 | 2026-08-27 | 让 DeepSeek Harness 自动重试商汤 429/QUOTA 等瞬时网关故障直到任务完成——启动时给所有 llm-pi-ai provider 热注入加固版 retryPolicy。 |
| 917 | [Hjay1101/dsh-plugin-token-usage](https://github.com/Hjay1101/dsh-plugin-token-usage) | 1 | 2026-08-22 | 2026-08-23 | GitHub-style token usage heat map for DeepSeek Harness — day/week/month granularity, per-model breakdown, hover-today badge. Read-only, fully local. |
| 918 | [hjj345/dsh-sm-context-piano](https://github.com/hjj345/dsh-sm-context-piano) | 1 | 2026-08-21 | 2026-08-29 | DeepSeek Harness Web GUI 的 Codex 风格对话导航器：帮助用户快速浏览、定位和切换对话，提升多任务、多会话场景下的工作效率。 \|  Codex-style conversation navigator for the DeepSeek Harness Web GUI. |
| 919 | [hjj345/dsh-sm-version-display](https://github.com/hjj345/dsh-sm-version-display) | 1 | 2026-08-28 | 2026-08-30 | 用于在侧边栏“设置”按钮上方显示已安装 dsh 版本的 DeepSeek Harness Web 插件。  \|  DeepSeek Harness Web plugin that displays the installed dsh version above the sidebar Settings button. |
| 920 | [Hoemr/dsh-better-overleaf](https://github.com/Hoemr/dsh-better-overleaf) | 1 | 2026-08-24 | 2026-08-24 | Overleaf tab for DSH better-sidebar: direct-CDP login, project mirrors under <workspace>/overleaf/, git/API sync, sidebar file preview |
| 921 | [honyKing/dsh-session-archive-plugin](https://github.com/honyKing/dsh-session-archive-plugin) | 1 | 2026-08-23 | 2026-08-23 | DSH 上下文存档与历史检索插件：自动压缩前把会话完整存档（zstd 解码为可读 jsonl + 摘要），压缩后按需全文检索历史对话。内置 archive_session / search_archive 工具与打包技能，dsh plugin add 一键安装。 |
| 922 | [HOWILLMAKEIT/football-mcp](https://github.com/HOWILLMAKEIT/football-mcp) | 1 | 2026-08-24 | 2026-08-25 | 面向 Claude、Codex、Cursor 和 DeepSeek Harness 的足球数据 MCP Server，支持 18 个欧洲联赛、8 个杯赛，以及比赛、积分榜、交锋、赔率和近期状态查询。 |
| 923 | [HTian-qwq/prts-terrarchive](https://github.com/HTian-qwq/prts-terrarchive) | 1 | 2026-08-31 | 2026-08-31 | 为明日方舟的长篇剧情打造的RAG类DSH插件，拥有多种快速检索能力。 |
| 924 | [HuanLinOTO/dsh-plugin-better-glob](https://github.com/HuanLinOTO/dsh-plugin-better-glob) | 1 | 2026-08-30 | 2026-08-30 | 以 per-agent 阴影顶替内置 glob：自动排除无底洞目录（node_modules 等），传 include 白名单才能搜入 \| Shadows the built-in glob per agent: auto-excludes bottomless directories (node_modules etc.), pass an include whitelist to search inside them |
| 925 | [HuanLinOTO/dsh-plugin-better-locale](https://github.com/HuanLinOTO/dsh-plugin-better-locale) | 1 | 2026-08-23 | 2026-08-23 | DSH web 插件：通过运行时 monkey-patch LocaleRuntime.lookup 注入第三语言（ja/ko/...）覆盖，保持 dsh active locale 不变；通过 DSH 设置页通用分区暴露切换 UI。 \| DSH web plugin: injects third-language (ja/ko/...) overrides via a runtime monkey-patch of LocaleRuntime.lookup, leaving the dsh active locale unchanged; exposes a switcher UI through the DSH settings page (General section). |
| 926 | [Huasecc/dsh-usage](https://github.com/Huasecc/dsh-usage) | 1 | 2026-08-15 | 2026-08-24 | DeepSeek 用量面板—DSHWeb GUI 余额与Token用量仪表盘 |
| 927 | [hufang360/dsh-sticky-notes](https://github.com/hufang360/dsh-sticky-notes) | 1 | 2026-08-16 | 2026-08-22 | 记下想法，让agent落盘！ |
| 928 | [hw-cola/dsh-message-enhancer](https://github.com/hw-cola/dsh-message-enhancer) | 1 | 2026-08-24 | 2026-08-24 | DSH插件，消息功能增强 |
| 929 | [hw-cola/dsh-remote-control](https://github.com/hw-cola/dsh-remote-control) | 1 | 2026-08-25 | 2026-08-25 | DSH插件，手机远程控制 |
| 930 | [hzpeng57/dsh-lens-rail](https://github.com/hzpeng57/dsh-lens-rail) | 1 | 2026-08-25 | 2026-08-25 | Codex-style left message navigation rail for DeepSeek Harness |
| 931 | [hzthzt/dsh-skill-switch](https://github.com/hzthzt/dsh-skill-switch) | 1 | 2026-08-22 | 2026-08-23 | Windows Junction-based global Skill switcher for DeepSeek Harness Web. |
| 932 | [iasiv5/skins](https://github.com/iasiv5/skins) | 1 | 2026-08-28 | 2026-08-28 | 换肤如换季，归真只一键 —— DeepSeek Harness Web 多皮肤切换器：明暗双态、中英双语、SHA 校验自动更新。Hot-swappable brand skins for DeepSeek Harness Web. |
| 933 | [icearia0219/dsh-memory-spaces](https://github.com/icearia0219/dsh-memory-spaces) | 1 | 2026-08-25 | 2026-08-25 | User-governed local memory spaces for DeepSeek Harness — explicitly share selected sessions with previewable, versioned, provenance-aware recall. |
| 934 | [icyaaaww/dsh-adaptive-model-router](https://github.com/icyaaaww/dsh-adaptive-model-router) | 1 | 2026-08-24 | 2026-08-24 | Deterministic per-turn adaptive model routing for DeepSeek Harness |
| 935 | [Idreamxkl/dsh-conversation-flat](https://github.com/Idreamxkl/dsh-conversation-flat) | 1 | 2026-08-30 | 2026-08-30 | Document-flow conversation layout for DeepSeek Harness web GUI — full-width column, user message bars, sender label, full-width tables. 纯 CSS 的 dsh 对话区通栏布局插件 |
| 936 | [iguowz/dsh-cortex](https://github.com/iguowz/dsh-cortex) | 1 | 2026-08-23 | 2026-08-23 | 低成本多模型编排插件（Cortex）：大模型规划验收，子agent小模型执行，降本保质 |
| 937 | [iimaguest/dsh-contradictions-indicator](https://github.com/iimaguest/dsh-contradictions-indicator) | 1 | 2026-08-30 | 2026-08-30 | DSH plugin: 0-100 conversation coherence badge with parallel contradiction analysis |
| 938 | [ImCabbage/dsh-plugin-mindmap](https://github.com/ImCabbage/dsh-plugin-mindmap) | 1 | 2026-08-20 | 2026-08-23 | MindMap: a DeepSeek Harness plugin that distills conversations into persistent storylines with an interactive map tab. |
| 939 | [IP050/dsh-video-player](https://github.com/IP050/dsh-video-player) | 1 | 2026-08-25 | 2026-08-26 | A floating, draggable, resizable **video player** for DeepSeek Harness (DSH). |
| 940 | [jadehare/dsh-model-controller](https://github.com/jadehare/dsh-model-controller) | 1 | 2026-08-21 | 2026-08-24 | 为 DeepSeek Harness 提供基于关键词和语义分类的动态模型路由插件，可按任务自动选择模型与推理强度。 |
| 941 | [Jaeger0624/dsh-conversation-nav](https://github.com/Jaeger0624/dsh-conversation-nav) | 1 | 2026-08-23 | 2026-08-23 | Codex-style conversation turn navigation for DeepSeek Harness Web GUI: piano-key rail, hover preview with send time, click-to-jump, per-turn marks |
| 942 | [JanEickholt/dsh-inline-diff](https://github.com/JanEickholt/dsh-inline-diff) | 1 | 2026-08-25 | 2026-08-26 | Renders edit and write tool calls as always-expanded side-by-side git-style diffs in a diff viewer, with optional syntax coloring and word-level highlighting. |
| 943 | [jarvis959/galvanize-dsh](https://github.com/jarvis959/galvanize-dsh) | 1 | 2026-08-28 | 2026-08-28 | Triggers inside your DSH agent: wake a fresh DeepSeek Harness session when files, mail, webhooks, or git events happen. Native Cordis bundle, heartbeat-proved install. |
| 944 | [JasonFreeLab/dsh-superpowers](https://github.com/JasonFreeLab/dsh-superpowers) | 1 | 2026-08-28 | 2026-08-28 | DSH (DeepSeek Harness) port of obra/superpowers — 14 native skills for multi-agent software development: brainstorming, planning, TDD, systematic debugging, and code review. |
| 945 | [jasonliu119/find-image-prompt-skill](https://github.com/jasonliu119/find-image-prompt-skill) | 1 | 2026-08-23 | 2026-08-23 | Open AI-agent skill and DeepSeek function-calling adapter for turning ideas and public reference images into production-ready image prompts. |
| 946 | [jeffy-Peng/deepseek-harness-usage](https://github.com/jeffy-Peng/deepseek-harness-usage) | 1 | 2026-08-16 | 2026-08-28 | DeepSeek Harness 插件，显示每日消费与账户总余额。DeepSeek Harness plugin for account balance and evidence-bounded daily CNY consumption |
| 947 | [Jensen-Yao/dsh-model-palette](https://github.com/Jensen-Yao/dsh-model-palette) | 1 | 2026-08-26 | 2026-08-26 | Global provider-aware model command palette and optional OpenRouter media tools for DeepSeek Harness. |
| 948 | [jerryqx/dsh-xiaoyuzhou](https://github.com/jerryqx/dsh-xiaoyuzhou) | 1 | 2026-08-26 | 2026-08-26 | DSH (DeepSeek Harness) 小宇宙播客插件：免登录播放/扫码登录/订阅同步/搜索，Web 播放条与面板 + podcast_play 工具 |
| 949 | [jerryqx/dsh-ximalaya](https://github.com/jerryqx/dsh-ximalaya) | 1 | 2026-08-25 | 2026-08-25 | DeepSeek Harness 喜马拉雅播客插件：搜索/播放/收藏 + ximalaya_play 模型工具 |
| 950 | [jetheaven/dsh-code-reviewer](https://github.com/jetheaven/dsh-code-reviewer) | 1 | 2026-08-14 | 2026-08-27 | AI代码审查插件：bug检测/安全漏洞/性能/风格四维审查，行号定位+修复示例 |
| 951 | [jetheaven/dsh-content-rewriter](https://github.com/jetheaven/dsh-content-rewriter) | 1 | 2026-08-14 | 2026-08-27 | 一键内容改写：小红书/知乎/商务邮件/精简/扩写/Twitter 多风格 |
| 952 | [jetheaven/dsh-data-extractor](https://github.com/jetheaven/dsh-data-extractor) | 1 | 2026-08-14 | 2026-08-27 | 结构化数据提取：从非结构化文本提取字段，输出 JSON/CSV/表格 |
| 953 | [jetheaven/dsh-meeting-notes](https://github.com/jetheaven/dsh-meeting-notes) | 1 | 2026-08-14 | 2026-08-27 | 会议纪要智能生成：从转写文本提取决议/待办/负责人/截止时间/风险 |
| 954 | [jetheaven/dsh-prompt-optimizer](https://github.com/jetheaven/dsh-prompt-optimizer) | 1 | 2026-08-14 | 2026-08-27 | AI提示词优化器：诊断Prompt问题并输出结构化高质量优化版本 |
| 955 | [jetheaven/dsh-seo-writer](https://github.com/jetheaven/dsh-seo-writer) | 1 | 2026-08-14 | 2026-08-27 | SEO文章生成器：给定关键词和语言，生成搜索引擎友好的完整文章 |
| 956 | [jetheaven/dsh-text-diff](https://github.com/jetheaven/dsh-text-diff) | 1 | 2026-08-14 | 2026-08-27 | AI智能文本对比：找出两段文字的差异、语义变化和潜在风险点 |
| 957 | [jetheaven/dsh-translate-pro](https://github.com/jetheaven/dsh-translate-pro) | 1 | 2026-08-14 | 2026-08-27 | 专业翻译：术语一致、专业领域选择与语气调整，附带术语对照表 |
| 958 | [jiangliuhong/dsh-gpt-oauth](https://github.com/jiangliuhong/dsh-gpt-oauth) | 1 | 2026-08-26 | 2026-08-27 | openai models for login by chatgpt |
| 959 | [JianwuYang/dsh-ui-kanban](https://github.com/JianwuYang/dsh-ui-kanban) | 1 | 2026-08-27 | 2026-08-27 | 让 agent 直接干 Jira/GitLab 的活 · DSH 看板插件 \| A dsh plugin that turns Jira + GitLab into an agent-workable kanban board |
| 960 | [jianxx/dsh-cc](https://github.com/jianxx/dsh-cc) | 1 | 2026-08-15 | 2026-08-28 | Bring the Claude Code workflow to DeepSeek Harness - TUI, permissions, hooks, memory, skills, subagents, MCP, worktrees, and more. |
| 961 | [Jimmyzwang-cloud/dsh-inkscreen-theme](https://github.com/Jimmyzwang-cloud/dsh-inkscreen-theme) | 1 | 2026-08-22 | 2026-08-23 | Ink-and-paper Apple-glass theme for DeepSeek Harness (dsh) web client, with a handwritten jimmy sidebar brand |
| 962 | [jing-hy/computer-user](https://github.com/jing-hy/computer-user) | 1 | 2026-08-21 | 2026-08-27 | DSH plugin: Codex-style computer use for Windows - read the screen, drive mouse & keyboard via SendInput; pairs with picturereader to close the look-act-verify loop. |
| 963 | [jinzheng8115/dsh-Minesweeper](https://github.com/jinzheng8115/dsh-Minesweeper) | 1 | 2026-08-24 | 2026-08-24 | DeepSeek Harness minesweeper plugin — agent tool set + human panel sharing one board. 扫雷插件：agent 工具集与人类面板共享同一棋盘。 |
| 964 | [jli658942-web/dsh-market-skill](https://github.com/jli658942-web/dsh-market-skill) | 1 | 2026-08-22 | 2026-08-22 | DSH Market 全局 skill：教 Agent 发现、评估、安装 DeepSeek Harness 插件/技能。Global skill teaching agents to use DSH Market (dsh.market) to discover, evaluate and install DSH plugins and skills. |
| 965 | [JMweitao/dsh-local-plugin-installer](https://github.com/JMweitao/dsh-local-plugin-installer) | 1 | 2026-08-21 | 2026-08-22 | 从 DSH Web 设置页安装并构建本地插件 / Install and build local DeepSeek Harness plugins from the Web settings page. |
| 966 | [jn18755/dsh-skill-nannan](https://github.com/jn18755/dsh-skill-nannan) | 1 | 2026-08-27 | 2026-08-27 | DSH 插件：基于《地狱磨砺》(Hell Grind) 方法论的 AI 视频提示词规范（29 条规则，已去除压力测试阶段） |
| 967 | [joao-paulo-santos/dsh-event-relay](https://github.com/joao-paulo-santos/dsh-event-relay) | 1 | 2026-08-24 | 2026-08-25 | Event relay: one SSE channel pushing host-side notifications to subscribed browser surfaces (server-side topic-prefix filtering, __relay/open reconnect signal) |
| 968 | [JohnXu22786/calendar](https://github.com/JohnXu22786/calendar) | 1 | 2026-08-23 | 2026-08-23 | CalDAV + iCalendar + RRULE calendar integration bundle for DeepSeek Harness (dsh), with Chinese-bias (lunar calendar / holidays / Asia/Shang |
| 969 | [JohnXu22786/subtitle-studio](https://github.com/JohnXu22786/subtitle-studio) | 1 | 2026-08-23 | 2026-08-23 | Multi-language subtitle translation workflow for dsh: SRT/VTT parsing, sentence-level LLM translation, bilingual merge, alignment validation |
| 970 | [Jokasa7/dsh-product-subagent-console](https://github.com/Jokasa7/dsh-product-subagent-console) | 1 | 2026-08-22 | 2026-08-22 | Design, observe, diagnose, and reuse evidence-backed multi-Agent workflows inside DeepSeek Harness |
| 971 | [jony5933/codex-dsh-bridge](https://github.com/jony5933/codex-dsh-bridge) | 1 | 2026-08-24 | 2026-08-24 | A visible, workspace-aware Codex to DeepSeek Harness Web Host bridge. |
| 972 | [JovanHE/ds-balance](https://github.com/JovanHE/ds-balance) | 1 | 2026-08-22 | 2026-08-23 | A minimal DeepSeek account balance widget for the DeepSeek Harness web GUI |
| 973 | [jsoncode/dsh-balance-by-token](https://github.com/jsoncode/dsh-balance-by-token) | 1 | 2026-08-21 | 2026-08-22 | DeepSeek Harness（dsh）双面插件（宿主 + 浏览器半边）：查看 DeepSeek 账户余额， 按 token 用量估算费用，价格按模型 × 高峰/空闲时段在线配置。所有能力收敛在 统一弹框中（侧边栏底部「余额」入口），另在会话头部提供实时 「当前会话 ≈xx CNY \| 余额 xx CNY」按钮。界面中英双语（跟随宿主 UI 语言）。 |
| 974 | [Jstn-1g/dsh-live-voice](https://github.com/Jstn-1g/dsh-live-voice) | 1 | 2026-08-25 | 2026-08-28 | DSH Live Voice: consent-bound one-turn voice for DeepSeek Harness, with a credential-free local synthetic demo, exact-Session isolation, and explicit draft handoff. |
| 975 | [junwei529/work-charter-dsh](https://github.com/junwei529/work-charter-dsh) | 1 | 2026-08-28 | 2026-08-30 | DSH-native Work Charter policy plugin backed by session-coordinator-dsh |
| 976 | [JuwanXu/dsh-camel](https://github.com/JuwanXu/dsh-camel) | 1 | 2026-08-25 | 2026-08-25 | DeepSeek Harness plugin for provider/model-aware adaptive rate-limit pacing, visible retries, and free-model recovery. |
| 977 | [JuwanXu/dsh-continue](https://github.com/JuwanXu/dsh-continue) | 1 | 2026-08-25 | 2026-08-25 | DeepSeek Harness plugin for fail-closed network recovery, recommended answers, decision learning, and unattended continuation. |
| 978 | [jypjypjypjyp/dsh-notifier](https://github.com/jypjypjypjyp/dsh-notifier) | 1 | 2026-08-27 | 2026-08-27 | 审批/完成/错误事件通知：浏览器 Notification + 系统原生 toast（Windows PowerShell WinRT / macOS osascript / Linux notify-send，均无需额外安装）；提示音可配、每条通知独立显示不互相替换、非安全上下文自动降级横幅 |
| 979 | [Kaiji-Z/dsh-plugin-warroom](https://github.com/Kaiji-Z/dsh-plugin-warroom) | 1 | 2026-08-30 | 2026-08-31 | RTS-style multi-agent orchestration board for DeepSeek Harness: issue plain-language strategic orders, a staff agent drafts acceptance-checked task orders, commander agents deploy typed subagent troops on isolated workspaces — with a 3D starfield campaign view, append-only event logs, and machine-checked verification. |
| 980 | [KakaruHayate/dsh-degen-heal](https://github.com/KakaruHayate/dsh-degen-heal) | 1 | 2026-08-25 | 2026-08-25 | Detect and self-heal LLM output degeneration loops inside a DeepSeek Harness agent session.（有死锁，别用） |
| 981 | [KannaKuron/dsh-agent-lang](https://github.com/KannaKuron/dsh-agent-lang) | 1 | 2026-08-31 | 2026-08-31 | Agent language control: DSH plugin — tool-call descriptions, model thinking, and replies each follow the GUI language, force a fixed language, or turn off; injected as one global runtime-context directive. \| Agent 语言控制:DSH 插件——工具描述、模型思考、回复输出三通道各自跟随界面语言 / 强制指定 / 关闭,以全局 runtime-context 注入,不改任何 preset。 |
| 982 | [kedoupi/xiaotaozi-dsh](https://github.com/kedoupi/xiaotaozi-dsh) | 1 | 2026-08-21 | 2026-08-22 | xiaotaozi-dsh：小桃子 DeepSeek Harness 插件与 Mac 客户端 |
| 983 | [keman-ai/dsh-opencode-zen](https://github.com/keman-ai/dsh-opencode-zen) | 1 | 2026-08-19 | 2026-08-27 | Bring OpenCode Zen's free models to DeepSeek Harness — zero config, no API key, catalog discovered live from upstream |
| 984 | [kenny2077/dsh-web-search-doubao](https://github.com/kenny2077/dsh-web-search-doubao) | 1 | 2026-08-29 | 2026-08-29 | Doubao Search provider for the DeepSeek Harness |
| 985 | [kenny2077/dsh-web-search-zai](https://github.com/kenny2077/dsh-web-search-zai) | 1 | 2026-08-28 | 2026-08-28 | One ZAI_API_KEY for both chat and search — plug-and-play Z.ai (GLM) web search for the DeepSeek Harness. |
| 986 | [KevinZhangNothing/dsh-task-graph](https://github.com/KevinZhangNothing/dsh-task-graph) | 1 | 2026-08-27 | 2026-08-27 | Task flow / execution graph plugin for DeepSeek Harness (DSH) — visualize a single task's full run: agents, tools, skills, subtasks, retries, live status. DSH 单任务执行流程图谱插件。 |
| 987 | [kfirsch/dsh-hebrew-rtl](https://github.com/kfirsch/dsh-hebrew-rtl) | 1 | 2026-08-24 | 2026-08-25 | Hebrew RTL support for the DeepSeek Harness web UI: dominant-script block direction, bidi-safe input fields, and RTL-aware line navigation. |
| 988 | [KhalilHsu/dsh-plugins](https://github.com/KhalilHsu/dsh-plugins) | 1 | 2026-08-17 | 2026-08-28 | Enhance DeepSeek Harness Web GUI with smart per-turn reasoning/tool folding and query navigation. |
| 989 | [kirbylynx/dsh-hub](https://github.com/kirbylynx/dsh-hub) | 1 | 2026-08-27 | 2026-08-27 | DeepSeek Harness Hub |
| 990 | [komoai2026/dsh-zpdf](https://github.com/komoai2026/dsh-zpdf) | 1 | 2026-08-22 | 2026-08-23 | Zpdf tools for DeepSeek Harness with durable API-key settings and CLI configuration. |
| 991 | [kovey/dsh-nvim-tui](https://github.com/kovey/dsh-nvim-tui) | 1 | 2026-08-21 | 2026-08-25 | TUI of DeepSeek Harness with Neovim |
| 992 | [kuanfu0430/dsh-sidebar-branch-chat](https://github.com/kuanfu0430/dsh-sidebar-branch-chat) | 1 | 2026-08-24 | 2026-08-24 | Adds a Branch Chat tab to dsh-better-sidebar: independent archived sessions with a context digest and the same tools as the main agent. |
| 993 | [l-vM2k/dsh-ayaka-theme](https://github.com/l-vM2k/dsh-ayaka-theme) | 1 | 2026-08-28 | 2026-08-28 | deepseek harness plugins dsh-ayaka-theme |
| 994 | [L1ttleBad/dsh-multi-task](https://github.com/L1ttleBad/dsh-multi-task) | 1 | 2026-08-25 | 2026-08-25 | A prototype Multi-task Agent Preset for DeepSeek Harness. |
| 995 | [LamplitIsles/kepos-imagegen](https://github.com/LamplitIsles/kepos-imagegen) | 1 | 2026-08-27 | 2026-08-30 | Image generation tools via kepos exposed codex endpoint |
| 996 | [lansi-ai/dsh-desktop](https://github.com/lansi-ai/dsh-desktop) | 1 | 2026-08-25 | 2026-08-26 | 把 DeepSeek Harness 做成一个真正的桌面应用：Electron 主进程内嵌 Cordis Host（与官方 Web 版同内核、零移植）， 渲染进程加载官方 Web UI 发行物（file:///自定义协议 + IPC 桥接，不开放 HTTP 端口）， 所有桌面原生能力（托盘、全局热键、系统通知、剪贴板、开机自启、协议唤起、多窗口）以 host 插件 形态注入运行时， 与官方「一切皆插件」的架构同构——不是给网页套壳，而是把桌面能力变成可装配、可卸载、可审查的插件树。  AI 驱动开发声明 |
| 997 | [lansi-ai/dsh-fetch-url](https://github.com/lansi-ai/dsh-fetch-url) | 1 | 2026-08-24 | 2026-08-25 | DeepSeek Harness (DSH) 抓取工具插件 — 注册模型可调用的 fetch_url 工具，抓取任意 URL（境内直连 / 境外走代理），返回有界摘要。 |
| 998 | [lansi-ai/dsh-plugin-starter](https://github.com/lansi-ai/dsh-plugin-starter) | 1 | 2026-08-24 | 2026-08-25 | DSH plugin development starter: a loadable skill (SKILL.md) plus copy-paste templates for building dual-face (Host + Client) DSH plugins |
| 999 | [Laplace-bit/dsh-pianist](https://github.com/Laplace-bit/dsh-pianist) | 1 | 2026-08-17 | 2026-08-25 | 🎹 A DeepSeek Harness piano plugin — deterministic musical timeline, Canvas2D grand piano, sample-based audio. 让 AI 弹一曲，也是模型的本事。 |
| 1000 | [lasdrder0705/dsh-pro-vision](https://github.com/lasdrder0705/dsh-pro-vision) | 1 | 2026-08-21 | 2026-08-22 | DSH plugin: let DeepSeek-V4-Pro use V4-Flash-Vision-Exp for attached images. Install: dsh plugin --profile web add github:lasdrder0705/dsh-pro-vision |
| 1001 | [launchmaniac/dsh-media-tools](https://github.com/launchmaniac/dsh-media-tools) | 1 | 2026-08-23 | 2026-08-24 | OpenRouter image, video, and speech generation as deepseek-harness tools — an out-of-tree profile bundle, no fork required |
| 1002 | [lc23313/dsh-autoupdate](https://github.com/lc23313/dsh-autoupdate) | 1 | 2026-08-23 | 2026-08-23 | dsh 内置自动更新插件 — Auto-update for DeepSeek Harness: safe version detection, exit-time apply, health check, auto-rollback & circuit breaker. |
| 1003 | [lengzhanbao/dsh-raiden-theme](https://github.com/lengzhanbao/dsh-raiden-theme) | 1 | 2026-08-26 | 2026-08-26 | Raiden Inazuma Atelier / 稻妻雷电工房 — DSH Web 紫金亚克力主题（独立于 Taffy） |
| 1004 | [leonardoxr/dsh-claude-usage](https://github.com/leonardoxr/dsh-claude-usage) | 1 | 2026-08-24 | 2026-08-24 | Anthropic Claude plan usage indicator for DeepSeek Harness |
| 1005 | [leonardoxr/dsh-companion](https://github.com/leonardoxr/dsh-companion) | 1 | 2026-08-22 | 2026-08-24 | Read-only workspace and session JSON API plugin for DeepSeek Harness native clients. |
| 1006 | [leonardoxr/dsh-harness-updater](https://github.com/leonardoxr/dsh-harness-updater) | 1 | 2026-08-24 | 2026-08-24 | Claude Code / Codex CLI update detection, prompting, and one-click channel updates for DeepSeek Harness |
| 1007 | [leonardoxr/dsh-native](https://github.com/leonardoxr/dsh-native) | 1 | 2026-08-22 | 2026-08-24 | Native desktop and iOS shell for trusted HTTPS web apps, with saved servers and first-class DeepSeek Harness support. |
| 1008 | [leonardoxr/dsh-plugin-manager](https://github.com/leonardoxr/dsh-plugin-manager) | 1 | 2026-08-24 | 2026-08-24 | Safe loopback-only Web UI for managing DeepSeek Harness profile plugins |
| 1009 | [leonardoxr/dsh-routed-subagent](https://github.com/leonardoxr/dsh-routed-subagent) | 1 | 2026-08-22 | 2026-08-22 | Complexity-routed subagent delegation for DeepSeek Harness: the model picks the runtime tier per task. |
| 1010 | [lewes2/archpresent](https://github.com/lewes2/archpresent) | 1 | 2026-08-29 | 2026-08-29 | Agent skill: generate beautiful dark-themed architecture diagrams from your project/demo/idea. Interactive, verifiable, and editable. Delivered as self-contained HTML. |
| 1011 | [lhh010/dsh-file-trace](https://github.com/lhh010/dsh-file-trace) | 1 | 2026-08-28 | 2026-08-30 | DSH Web UI 文件追踪插件：记录并查看模型读取/写入/编辑的文件，带行号内容与终端风逐行 diff(红删绿增蓝改)、hunk 上下文折叠、可拖拽高度。适配 DSH dsh-v0.1.2-alpha.1，纯客户端零核心改动。 |
| 1012 | [LHKong7/dsh-browser-runtime](https://github.com/LHKong7/dsh-browser-runtime) | 1 | 2026-08-26 | 2026-08-27 | deepseek harness plugin browser runtime |
| 1013 | [liiiubai/dsh-mcp-bridge](https://github.com/liiiubai/dsh-mcp-bridge) | 1 | 2026-08-28 | 2026-08-28 | Expose DeepSeek Harness tools as a standard MCP server (streamable HTTP) — drive dsh from Claude Code, Codex, or any MCP client |
| 1014 | [lilightspeed/dsh-seekbuddy](https://github.com/lilightspeed/dsh-seekbuddy) | 1 | 2026-08-23 | 2026-08-23 | Desktop pet peer client for DeepSeek Harness (DSH): /api + WebSocket client, MCP server, desktop shell (Electron). |
| 1015 | [lindog114514/dsh-dglab](https://github.com/lindog114514/dsh-dglab) | 1 | 2026-08-23 | 2026-08-23 | Deepseek harness的DG-LAB 控制插件为 AI 提供 dglab-kit 工具集 |
| 1016 | [lispking/dsh-devpanel](https://github.com/lispking/dsh-devpanel) | 1 | 2026-08-24 | 2026-08-24 | A developer toolkit for the DeepSeek Harness (DSH) web console: a real multi-tab PTY terminal plus an AI-output file browser. |
| 1017 | [litianshuo110/dsh-ds-vision-auto-route](https://github.com/litianshuo110/dsh-ds-vision-auto-route) | 1 | 2026-08-22 | 2026-08-22 | Route image-bearing turns to a configurable image-capable model for DeepSeek Harness |
| 1018 | [LLYlab/DSHEssentialTools](https://github.com/LLYlab/DSHEssentialTools) | 1 | 2026-08-27 | 2026-08-28 | DSH 永久插件：LVAL 工程运行/代码查看/程序版本快照回退 + VTD 虚拟对话树（编辑/重试/分支、消息小版本）+ DET 管理器。A permanent DeepSeek Harness plugin: project run & code viewer, program snapshots, an in-session conversation tree (edit/retry/branches), message micro-versions and a feature manager. |
| 1019 | [lmong11/dsh-game-center](https://github.com/lmong11/dsh-game-center) | 1 | 2026-08-21 | 2026-08-22 | AI-powered Game Center plugin for DeepSeek Harness, featuring Texas Holdem with 1–7 agent players. |
| 1020 | [LoKiGGo/dsh-tools](https://github.com/LoKiGGo/dsh-tools) | 1 | 2026-08-16 | 2026-08-27 | dsh web通用工具箱插件，纯AI制作（包括仓库），零人工含量，可能不会维护，请谨慎使用。 |
| 1021 | [longnb47/dsh-agent-gateway](https://github.com/longnb47/dsh-agent-gateway) | 1 | 2026-08-23 | 2026-08-25 | MCP stdio gateway for exposing local AGY, Codex, and OpenCode CLI agents to DeepSeek Harness (DSH). |
| 1022 | [LONGSASASASASA/dsh-issue2pr](https://github.com/LONGSASASASASA/dsh-issue2pr) | 1 | 2026-08-29 | 2026-08-30 | 从一条 Issue 到一份被合并的 PR，每一段都有自己的输入契约、失败信号、可回滚产物与可独立审查的 Artifact。 |
| 1023 | [LongSir0419/dsh-git-branch-manage](https://github.com/LongSir0419/dsh-git-branch-manage) | 1 | 2026-08-24 | 2026-08-24 | DSH bundle: 当前 Git 分支徽标。在会话 header 与新会话欢迎页显示当前分支，支持切换、新建、更新、拉取、推送、删除（仅本地分支，IDEA 风格目录树）。 |
| 1024 | [Loopiplusplus/dsh-plugin-toggle-manager](https://github.com/Loopiplusplus/dsh-plugin-toggle-manager) | 1 | 2026-08-20 | 2026-08-22 | Visual plugin manager for DSH Web. |
| 1025 | [looput/dsh-finance-lab](https://github.com/looput/dsh-finance-lab) | 1 | 2026-08-18 | 2026-08-26 | DeepSeek Harness finance plugin: direct market HTTP APIs, portfolio settings, model tools |
| 1026 | [Lottle7/dsh-quota](https://github.com/Lottle7/dsh-quota) | 1 | 2026-08-25 | 2026-08-25 | Multi-provider quota, balance and Token-cost dashboard for DeepSeek Harness Web. |
| 1027 | [louishzwang/dsh-web-launcher](https://github.com/louishzwang/dsh-web-launcher) | 1 | 2026-08-21 | 2026-08-31 | DSH Web本地终端启动脚本 |
| 1028 | [ls-cool-123/dsh-account-balance](https://github.com/ls-cool-123/dsh-account-balance) | 1 | 2026-08-22 | 2026-08-22 | DeepSeek account balance dashboard plugin for dsh web — shows your DeepSeek API balance above the chat window. |
| 1029 | [Lsc-91-69/dsh-brain-compaction](https://github.com/Lsc-91-69/dsh-brain-compaction) | 1 | 2026-08-28 | 2026-08-28 | 人脑式上下文压缩逻辑，大幅减少长任务上下文占用以及token消耗 |
| 1030 | [lsh2002/dsh-custom-fonts](https://github.com/lsh2002/dsh-custom-fonts) | 1 | 2026-08-24 | 2026-08-24 | deepseek-harness的修改字体插件 |
| 1031 | [Lucasli2018/totoro-pet](https://github.com/Lucasli2018/totoro-pet) | 1 | 2026-08-24 | 2026-08-25 | DSH Web GUI 桌宠插件（悬浮 Q 版龙猫 · 喂食/抚摸/玩耍/睡觉互动养成） |
| 1032 | [LucienLL/dsh-session-status](https://github.com/LucienLL/dsh-session-status) | 1 | 2026-08-25 | 2026-08-26 | DSH 对话状态标签插件：给每个对话设置项目状态（进行中/已结项/搁置中 + 自定义标签/icon），会话列表与头部可见，跨浏览器持久化 |
| 1033 | [luckybilly/dsh-split-view](https://github.com/luckybilly/dsh-split-view) | 1 | 2026-08-25 | 2026-08-25 | 一个插件把 DeepSeek Harness 主窗口变成多个分屏，同时查看多个会话的状态。再也不用在会话列表里切来切去了。 |
| 1034 | [luckycaoj/dsh-plugin-session-console-sleepcat](https://github.com/luckycaoj/dsh-plugin-session-console-sleepcat) | 1 | 2026-08-31 | 2026-08-31 | 一个dsh的辅助使用小插件，DSH client plugin: embedded tool rail + session questions console — jump to past questions, collapse the model's working process. 🐱 |
| 1035 | [lumose0/dsh-file-reference-everything](https://github.com/lumose0/dsh-file-reference-everything) | 1 | 2026-08-27 | 2026-08-27 | Whole-disk @ file references for DeepSeek Harness — Everything-backed instant search with fuzzy/regex and a cross-platform fallback index |
| 1036 | [Lunatic029/dsh-clash-proxy](https://github.com/Lunatic029/dsh-clash-proxy) | 1 | 2026-08-27 | 2026-08-27 | Route DeepSeek Harness's outbound network through Clash — LLM, web search/fetch and shell commands all use your local Clash proxy. |
| 1037 | [luweiyabo/dsh-whale-pet](https://github.com/luweiyabo/dsh-whale-pet) | 1 | 2026-08-23 | 2026-08-24 | DeepSeek Harness Web UI 的开源鲸鱼桌宠插件，支持 Agent 状态感知、多种透明动画、点击拖拽、屏幕漫游、自定义动作与触发规则。 |
| 1038 | [luxueliu/luxueliu-reasoning-efforts](https://github.com/luxueliu/luxueliu-reasoning-efforts) | 1 | 2026-08-21 | 2026-08-22 | DSH里只有ds能选推理强度？20个常用模型推理强度按钮已就位！涵盖grok/Gemini / Kimi/glm……20个模型仅预设，实际槽位无上限！可以任意添加你的本地网关模型！（非 ds 系网关模型推理强度档位插件 + 路由级 llm-pi-ai 补丁） |
| 1039 | [LVSUGARS/dsh-web-launcher](https://github.com/LVSUGARS/dsh-web-launcher) | 1 | 2026-08-21 | 2026-08-22 | Windows desktop launcher for DeepSeek Harness (DSH) Web: install the official CLI, manage local workspaces, and safely start, stop, and update DSH. |
| 1040 | [LXFLGH/dsh-deepseek-relay](https://github.com/LXFLGH/dsh-deepseek-relay) | 1 | 2026-08-25 | 2026-08-26 | DeepSeek relay station adapter for deepseek-harness with reasoning-effort control |
| 1041 | [ly028716/dsh-memory-plugin](https://github.com/ly028716/dsh-memory-plugin) | 1 | 2026-08-20 | 2026-08-22 | Intelligent memory system for DSH - Track user preferences, tool usage, and project context to provide personalized recommendations |
| 1042 | [Lzh3070/dsh-model-visibility](https://github.com/Lzh3070/dsh-model-visibility) | 1 | 2026-08-27 | 2026-08-27 | DeepSeek Harness 插件：模型可见性管理——按渠道/模型隐藏或显示模型选择菜单里的条目 / Control which models appear in the DSH model selector |
| 1043 | [m1khal3v/dsh-tool-codegraph](https://github.com/m1khal3v/dsh-tool-codegraph) | 1 | 2026-08-29 | 2026-08-30 | CodeGraph navigation tools for DeepSeek Harness |
| 1044 | [M1ssbe4r/PocketCode](https://github.com/M1ssbe4r/PocketCode) | 1 | 2026-08-26 | 2026-08-26 | An AI agent that can code, build, and run apps locally on your phone.一个能在手机本地完成编码、编译和运行应用的AI Agent。。 |
| 1045 | [makajo/dsh-gemini-m3e-theme](https://github.com/makajo/dsh-gemini-m3e-theme) | 1 | 2026-08-29 | 2026-08-30 | Gemini-style Material 3 Expressive theme for DeepSeek Harness Web (persistent client bundle) |
| 1046 | [Malenia12/seedance-video-generator](https://github.com/Malenia12/seedance-video-generator) | 1 | 2026-08-22 | 2026-08-22 | Seedance 2.5 video generator: DSH agent plugin + local web workbench |
| 1047 | [MaRi23333/dsh-grok-kit](https://github.com/MaRi23333/dsh-grok-kit) | 1 | 2026-08-24 | 2026-08-25 | DeepSeek Harness 的 Grok 插件：OAuth 登录、主循环融合网页/X 搜索与 Imagine。第三方非官方项目。 |
| 1048 | [mario03690/dsh-lines](https://github.com/mario03690/dsh-lines) | 1 | 2026-08-22 | 2026-08-22 | Freeze a working sequence into a hosted production line. Turn a sequence of tool calls that alr |
| 1049 | [mastergo-design/dsh-canvas](https://github.com/mastergo-design/dsh-canvas) | 1 | 2026-08-27 | 2026-08-27 | MasterGo Canvas MCP plugin for DeepSeek Harness |
| 1050 | [Max-Null/dsh-plugin-center](https://github.com/Max-Null/dsh-plugin-center) | 1 | 2026-08-16 | 2026-08-25 | Plugin center for DeepSeek Harness: browse, install and update community plugins from inside the Web UI · DSH 插件管理中心：在 Web 界面浏览社区市场、一键安装与更新插件 |
| 1051 | [Max-Null/seek-soul-in-darkness](https://github.com/Max-Null/seek-soul-in-darkness) | 1 | 2026-08-15 | 2026-08-23 | Seek Soul in Darkness (SSiD) — DSH-based desktop AI: finding the soul of silicon life in darkness · 暗夜寻魂（思灵）：基于 DSH 的桌面 AI，寻找硅基生命的灵魂 |
| 1052 | [mba1398/dsh-done](https://github.com/mba1398/dsh-done) | 1 | 2026-08-23 | 2026-08-23 | One plugin that don't consume tokens. |
| 1053 | [me93-ghb/dsh-matrix-think](https://github.com/me93-ghb/dsh-matrix-think) | 1 | 2026-08-27 | 2026-08-27 | Matrix rain for expanded thinking in DeepSeek Harness Web |
| 1054 | [Medesol/dsh-kimi-formula](https://github.com/Medesol/dsh-kimi-formula) | 1 | 2026-08-31 | 2026-08-31 | Kimi (Moonshot AI) official Formula API tools for DeepSeek Harness — web_search via kimi-official provider + 10 kimi_* tools, no DeepSeek/Exa/Perplexity key needed |
| 1055 | [Melosic/dsh-invoke](https://github.com/Melosic/dsh-invoke) | 1 | 2026-08-14 | 2026-08-26 | Prompt Vault & Invoker for DeepSeek Harness — 管理、分类、快速调用提示词，支持侧边栏 GUI 与复制粘贴 |
| 1056 | [meng-114/dsh-image-tiler](https://github.com/meng-114/dsh-image-tiler) | 1 | 2026-08-21 | 2026-08-22 | DSH插件：将大图像分割成带标签的800像素图块，并保留概览图，同时保留视觉模型所需的细节。包含设置卡。DSH plugin: slice large images into labeled 800px tiles + overview, preserving detail for vision models. Settings card included. |
| 1057 | [mengnanxyyyy/dsh-markdown-xyy](https://github.com/mengnanxyyyy/dsh-markdown-xyy) | 1 | 2026-08-29 | 2026-08-29 | dsh markdown 主题插件 |
| 1058 | [Mengshang-spec/dsh-plugin-trustlens](https://github.com/Mengshang-spec/dsh-plugin-trustlens) | 1 | 2026-08-23 | 2026-08-23 | Read-only DSH plugin security auditor with current-session model review |
| 1059 | [mengzhangj/dsh-wallpaper](https://github.com/mengzhangj/dsh-wallpaper) | 1 | 2026-08-25 | 2026-08-26 | DSH-Wallpaper background wallpaper and system font picker plugin for DSH Desktop. Plugin source only, no DSH core. |
| 1060 | [menotbobbybrown/create-dsh-app](https://github.com/menotbobbybrown/create-dsh-app) | 1 | 2026-08-22 | 2026-08-22 | 1-Line AI Agent Scaffolding Generator for DeepSeek Harness (dsh) — Everything is a Plugin |
| 1061 | [menotbobbybrown/dsh-plugin-browser](https://github.com/menotbobbybrown/dsh-plugin-browser) | 1 | 2026-08-22 | 2026-08-22 | Native Web Browser Automation Agent Plugin for DeepSeek Harness (dsh) — Everything is a Plugin |
| 1062 | [menotbobbybrown/dsh-plugin-memory](https://github.com/menotbobbybrown/dsh-plugin-memory) | 1 | 2026-08-22 | 2026-08-22 | Persistent Knowledge Graph & Long-Term Memory Plugin for DeepSeek Harness (dsh) — Everything is a Plugin |
| 1063 | [MerlinShieh/AgentMemHub](https://github.com/MerlinShieh/AgentMemHub) | 1 | 2026-08-25 | 2026-08-27 | 统一提取多 Agent Harness 会话为全量事件流(含工具链/思维链/Shell/补丁) → SQLite 检索 → 桥接 MemOS 生成记忆 |
| 1064 | [messiahyl/dsh-plugins](https://github.com/messiahyl/dsh-plugins) | 1 | 2026-08-21 | 2026-08-22 | DSH 插件总仓库：monorepo 开发 + 安装源（本地归档/npm/GitHub/索引）+ 第三方目录。国内网络友好，归档 sha256 校验。 |
| 1065 | [MichaelShii/dsh-plugin-teamflow](https://github.com/MichaelShii/dsh-plugin-teamflow) | 1 | 2026-08-17 | 2026-08-26 | dsh plugin teamflow |
| 1066 | [mienfong/dsh-session-mgr](https://github.com/mienfong/dsh-session-mgr) | 1 | 2026-08-24 | 2026-08-24 | Session manager for the DeepSeek Harness web UI: move, archive, restore, backup/export and import conversations across workspaces. Trilingual (English / 简体 / 繁體). |
| 1067 | [Mikuzjc/dsh-office-for-mso](https://github.com/Mikuzjc/dsh-office-for-mso) | 1 | 2026-08-23 | 2026-08-23 | DeepSeek Harness (DSH) plugin/skill: control open Word/Excel/PowerPoint via Office add-in (33 actions, AI-orchestrated, near-Copilot workflows) \| DSH 的 Office 技能：操控打开的 Word/Excel/PPT |
| 1068 | [MingYU-kalo/dsh-https-fix](https://github.com/MingYU-kalo/dsh-https-fix) | 1 | 2026-08-21 | 2026-08-22 | DeepSeek Harness plugin: built-in HTTPS reverse proxy with configurable settings (设置→插件配置→Https Fix) |
| 1069 | [minyang-chen/dsh-stock-lookup](https://github.com/minyang-chen/dsh-stock-lookup) | 1 | 2026-08-25 | 2026-08-25 | DSH plugin: resolve company names to stock symbols via SEC EDGAR and fetch live quotes via Yahoo Finance |
| 1070 | [minyang2020/dsh-migrate-on-429](https://github.com/minyang2020/dsh-migrate-on-429) | 1 | 2026-08-22 | 2026-08-22 | DeepSeek Harness (dsh) plugin: automatic session handoff when a session keeps hitting 429 TPM rate limits — cancel old, summarize handover, continue in a fresh session. True handoff, never parallel. |
| 1071 | [Missher12/deepseek-harness-desktop](https://github.com/Missher12/deepseek-harness-desktop) | 1 | 2026-08-13 | 2026-08-29 | Unofficial Intel macOS desktop app for DeepSeek Harness |
| 1072 | [Missher12/dsh-missher-memory](https://github.com/Missher12/dsh-missher-memory) | 1 | 2026-08-23 | 2026-08-24 | Project-scoped reviewed long-project memory for DeepSeek Harness |
| 1073 | [mjn96/dsh-rhine-theme](https://github.com/mjn96/dsh-rhine-theme) | 1 | 2026-08-24 | 2026-08-24 | 明日方舟莱茵生命美术风格的deepseek harness皮肤主题 |
| 1074 | [mjw-git/dsh-pet](https://github.com/mjw-git/dsh-pet) | 1 | 2026-08-24 | 2026-08-24 | Desktop pet plugin for DeepSeek Harness (dsh) — grows with your agent token usage; XP economy, custom spritesheets, SSE status push, one-command install |
| 1075 | [ML-QSeek/SurvX](https://github.com/ML-QSeek/SurvX) | 1 | 2026-06-24 | 2026-08-24 | SurvX — A paradigm for building intelligent systems where behavior is driven by data change. It unifies capability units (F), structured entities (Matter), and self-evolving entities (Ego) under one architecture that works with or without AI. A prototype exploring XGI (Xenogenic General Intelligence) and the future of development. |
| 1076 | [mldhao/dsh-conversation-strip](https://github.com/mldhao/dsh-conversation-strip) | 1 | 2026-08-27 | 2026-08-27 | Codex-inspired vertical conversation-turn rail for the DeepSeek Harness web UI. |
| 1077 | [Modellix/dsh-modellix](https://github.com/Modellix/dsh-modellix) | 1 | 2026-08-24 | 2026-08-25 | DeepSeek Harness plugin for Modellix Web Search and Web Fetch. |
| 1078 | [monotykamary/dsh-multiprovider](https://github.com/monotykamary/dsh-multiprovider) | 1 | 2026-08-24 | 2026-08-25 | Provider-neutral multi-account scheduling, affinity, health, and Settings UI for DeepSeek Harness |
| 1079 | [moonlin1213/dsh-agent-sound-alert](https://github.com/moonlin1213/dsh-agent-sound-alert) | 1 | 2026-08-29 | 2026-08-29 | macOS sound alerts for DeepSeek Harness agent lifecycle events |
| 1080 | [Movingtoleveltwo/dsh-revert](https://github.com/Movingtoleveltwo/dsh-revert) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness 现代化对话回退与重试插件：纯 UI 图形交互、原地 Prompt 微调、支持工作区与外部文件双引擎安全恢复。 |
| 1081 | [mtdx2001/think-zh](https://github.com/mtdx2001/think-zh) | 1 | 2026-08-29 | 2026-08-29 | AI reasoning real-time Chinese localization suite (DSH ready, OpenAI-compatible endpoint) |
| 1082 | [MuAllen/dsh-gateway-wallet](https://github.com/MuAllen/dsh-gateway-wallet) | 1 | 2026-08-24 | 2026-08-26 | 读取当前 API key 在站点账本上的剩余额度和实扣，支持 Sub2API、New API 与 DeepSeek 官方，不是本地 token 估算。 |
| 1083 | [mumuer1024/dsh-ui-liteglass](https://github.com/mumuer1024/dsh-ui-liteglass) | 1 | 2026-08-21 | 2026-08-27 | LiteGlass — a lightweight appearance skin for DeepSeek Harness Web UI: wallpaper, glass-like transparency, and accent color. Server-side settings, multi-device, leaves native light/dark mode alone. |
| 1084 | [my-dsh/dsh-web-search-tavily](https://github.com/my-dsh/dsh-web-search-tavily) | 1 | 2026-08-30 | 2026-08-30 | Tavily web-search provider plugin for DeepSeek Harness (dsh) — registers into ctx.web so the model-facing web_search tool uses Tavily |
| 1085 | [Nasbaye/dsh-launcher](https://github.com/Nasbaye/dsh-launcher) | 1 | 2026-08-24 | 2026-08-25 | DeepSeek Harness one-click restart plugin: status dot, reliable worker (pre-flight + health check), resume-after-restart and auto-continue on token truncation |
| 1086 | [NattoCB/dsh-plugin-pin-session](https://github.com/NattoCB/dsh-plugin-pin-session) | 1 | 2026-08-23 | 2026-08-24 | Pin sessions in the DeepSeek Harness web GUI: Pinned Sessions group above the sidebar list + Pin/Unpin in the session row menu. |
| 1087 | [NattoCB/dsh-web-search-session-follow](https://github.com/NattoCB/dsh-web-search-session-follow) | 1 | 2026-08-23 | 2026-08-23 | DSH web_search provider that follows the conversation's routed model provider — per-provider endpoint/credential/dialect table with built-in official fallback |
| 1088 | [NecromanAlbert/dsh-show-media](https://github.com/NecromanAlbert/dsh-show-media) | 1 | 2026-08-25 | 2026-08-25 | Show a local image or short video inside the current DeepSeek Harness conversation card. |
| 1089 | [NEVSTOP-LAB/dsh-version-inspector](https://github.com/NEVSTOP-LAB/dsh-version-inspector) | 1 | 2026-08-23 | 2026-08-24 | DSH 版本信息插件，在 DSH 设置面板新增「版本信息」页，以紧凑多列树展示 DeepSeek Harness、插件与依赖的版本，支持按包名/版本过滤与 day/dark |
| 1090 | [NexusAgentX/dsh-reasoning-effort](https://github.com/NexusAgentX/dsh-reasoning-effort) | 1 | 2026-08-15 | 2026-08-26 | Host-side dsh plugin that adds seven reasoning-effort levels to third-party llm-pi-ai models in the web composer. |
| 1091 | [Niceck/dsh-hhxg-market](https://github.com/Niceck/dsh-hhxg-market) | 1 | 2026-08-27 | 2026-08-27 | 恢恢量化 hhxg.top A股量化数据插件 for DeepSeek Harness (dsh)：6 个免费工具 + 5 个 VIP 工具（MCP 桥接）· A-share quant data plugin |
| 1092 | [nicecx/dsh-macos-calendar](https://github.com/nicecx/dsh-macos-calendar) | 1 | 2026-08-24 | 2026-08-24 | DSH host-side plugin: real macOS Calendar integration (create/list/query/delete events via AppleScript) for DeepSeek Harness agents |
| 1093 | [nicecx/dsh-matrix-skin](https://github.com/nicecx/dsh-matrix-skin) | 1 | 2026-08-24 | 2026-08-24 | Night-friendly Matrix dark-green skin for the DeepSeek Harness web GUI (standalone mirror of upstream dsh-web-ui packages/skins/matrix) |
| 1094 | [Nigel211/dsh-text2img-compress](https://github.com/Nigel211/dsh-text2img-compress) | 1 | 2026-08-22 | 2026-08-22 | 把长文本渲染成图片发送，利用每图 384 token 封顶压缩 LLM 输入 token，专为DeepSeek Harness设计的插件；Pack long text into images to cut LLM input tokens (384/image cap) — a DeepSeek Harness plugin. |
| 1095 | [NimuStudio/NimuQDock-dsh](https://github.com/NimuStudio/NimuQDock-dsh) | 1 | 2026-08-27 | 2026-08-27 | 把 DeepSeek Harness接入QQ的对接坞——带人格引擎的仿真群友：心情、精力、记忆，像真人一样潜水与参与。 |
| 1096 | [NIU-001-LIU/dsh-chat-timeline-plus](https://github.com/NIU-001-LIU/dsh-chat-timeline-plus) | 1 | 2026-08-25 | 2026-08-25 | DeepSeek Harness timeline with hover Q&A preview and panel pin |
| 1097 | [niyongsheng/meww](https://github.com/niyongsheng/meww) | 1 | 2026-08-27 | 2026-08-27 | pokemon ai pet🐣电子宠物 |
| 1098 | [njjpro/dsh-vault](https://github.com/njjpro/dsh-vault) | 1 | 2026-08-30 | 2026-08-30 | Persistent credential vault plugin for DeepSeek Harness (DSH) - manage API tokens, server logins, and site credentials in one settings panel. |
| 1099 | [njuptlzf/dsh-dynamic-background](https://github.com/njuptlzf/dsh-dynamic-background) | 1 | 2026-08-22 | 2026-08-23 | DeepSeek Harness (DSH) 动态背景切换插件：上传 GIF/静态图与内置 12 色纯色调色板，定时丝滑交叉淡入淡出切换页面背景，聊天区自动叠加主题色保护层。安装：dsh plugin add github:njuptlzf/dsh-dynamic-background |
| 1100 | [Noemm/dsh-web-search-glm](https://github.com/Noemm/dsh-web-search-glm) | 1 | 2026-08-28 | 2026-08-28 | Zhipu GLM search provider for the DeepSeek Harness (dsh) web seam — native web_search via the Anthropic-compatible API |
| 1101 | [NOirBRight/dsh-llm-commandcode](https://github.com/NOirBRight/dsh-llm-commandcode) | 1 | 2026-08-27 | 2026-08-29 | Command Code Provider API LLM plugin for DeepSeek Harness |
| 1102 | [NOirBRight/dsh-model-switch](https://github.com/NOirBRight/dsh-model-switch) | 1 | 2026-08-19 | 2026-08-29 | Model purposes spec and tickets for DeepSeek Harness |
| 1103 | [NokorinNishikino/kidai-plugin-remote](https://github.com/NokorinNishikino/kidai-plugin-remote) | 1 | 2026-08-21 | 2026-08-22 | KPR 纪代管理：DSH的外部管理器，启停插件、隔离运行、手动回滚、预检诊断、变砖救急！配合KSG（Kidai-snapshot-guard）使用，自动快照、备份回滚！  |
| 1104 | [NokorinNishikino/kidai-plugin-remote-client](https://github.com/NokorinNishikino/kidai-plugin-remote-client) | 1 | 2026-08-21 | 2026-08-22 | KPR‘C 纪代管理（Client）：零依赖的桌面客户端，DSH的外部管理器，启停插件、隔离运行、手动回滚、预检诊断、变砖救急！配合KSG（Kidai-snapshot-guard）使用，保存自动快照、备份回滚！ |
| 1105 | [NokorinNishikino/kidai-snapshot-guard](https://github.com/NokorinNishikino/kidai-snapshot-guard) | 1 | 2026-08-21 | 2026-08-22 | KSG 纪代备份：DSH 内部备份插件，关闭自动保存快照、开机确认、单 zip 备份导出导入恢复、隔离自动恢复、多主流备份插件文件兼容 |
| 1106 | [NONAME-2121237/dsh-timeline](https://github.com/NONAME-2121237/dsh-timeline) | 1 | 2026-08-24 | 2026-08-24 | DSH web plugin: interaction timeline rail for long conversations (fork-independent successor of dsh-history) |
| 1107 | [NonchalantLudens/dsh-skin-collection](https://github.com/NonchalantLudens/dsh-skin-collection) | 1 | 2026-08-23 | 2026-08-23 | Multi-style skin collection for DeepSeek Harness (dsh) web GUI — 9 themes with scoped decoration CSS and a sidebar skin manager |
| 1108 | [NoxTyrannus/dsh-cipher](https://github.com/NoxTyrannus/dsh-cipher) | 1 | 2026-08-29 | 2026-08-29 | 把 cipher 的持续思考/三中台/四类记忆以 UNNI/LOOP 会话模式接入 DSH（dsh-plugin bundle） |
| 1109 | [Nuomi9/dsh-fgo-chaldea](https://github.com/Nuomi9/dsh-fgo-chaldea) | 1 | 2026-08-15 | 2026-08-27 | FGO Chaldea-inspired skin pack for DeepSeek Harness Web UI: 5 themes, original generated backdrops, gold trim. |
| 1110 | [nxz1026/SinglePlayer](https://github.com/nxz1026/SinglePlayer) | 1 | 2026-08-22 | 2026-08-22 | 单身汉播放器，适配DeepSeek harness web的播放器，支持多平台聚合。Bachelor Player is a media player designed to integrate with DeepSeek Harness Web, supporting multi-platform content aggregation. |
| 1111 | [Nzssm1/dsh-strategy-deployment-review](https://github.com/Nzssm1/dsh-strategy-deployment-review) | 1 | 2026-08-27 | 2026-08-27 | DSH agent preset for rigorous strategy live-deployment testing/evaluation. Retest. |
| 1112 | [objectivex666/dsh-settings-search](https://github.com/objectivex666/dsh-settings-search) | 1 | 2026-08-25 | 2026-08-27 | A plugin that adds a search box to the DSH settings panel. |
| 1113 | [omdsh-dev/dsh-accessibility](https://github.com/omdsh-dev/dsh-accessibility) | 1 | 2026-08-25 | 2026-08-26 | DSH accessibility companion, core remediation, test tooling, assistive-technology evidence, and accessible authoring. |
| 1114 | [OneCat2015/Remote-My-DSH](https://github.com/OneCat2015/Remote-My-DSH) | 1 | 2026-08-21 | 2026-08-23 | 一个Deepseek Harness远程插件（AI Coding注意） |
| 1115 | [oneinitAI/dsh-thunderforge](https://github.com/oneinitAI/dsh-thunderforge) | 1 | 2026-08-22 | 2026-08-23 | ⚡ ThunderForge · 宇宙无敌雷霆霹雳炫光 — 励志做 0 元以内最 nb 的 DSH 插件（产品目标）：一站式 DSH 插件开发套件 |
| 1116 | [onenameneo/dsh-plugin-loom-chat](https://github.com/onenameneo/dsh-plugin-loom-chat) | 1 | 2026-08-30 | 2026-08-31 | Loom Chat is a DSH Web client plugin that turns linear ordinary sessions into a pannable, zoomable Loom-style canvas for parallel exploration. |
| 1117 | [open-dsh-plugins/dsh-open-in-app](https://github.com/open-dsh-plugins/dsh-open-in-app) | 1 | 2026-08-20 | 2026-08-24 | dsh web-UI plugin: open the current session's workspace folder with an installed app (Finder, Terminal, VS Code, Ghostty, Zed, ...) — icons included |
| 1118 | [OpenCnid/recursus](https://github.com/OpenCnid/recursus) | 1 | 2026-08-22 | 2026-08-22 | A durable, full-access runtime agent built on DeepSeek Harness |
| 1119 | [openllmsh/dsh](https://github.com/openllmsh/dsh) | 1 | 2026-08-24 | 2026-08-27 | DeepSeek Harness (dsh) bundle: route the harness through OpenLLM (OpenAI-compatible) + register the OpenLLM MCP, with CLI/daemon onboarding. |
| 1120 | [orpheus0829/dsh-identity-control](https://github.com/orpheus0829/dsh-identity-control) | 1 | 2026-08-21 | 2026-08-22 | 为 DeepSeek Harness (DSH) 打造的自定义人设控制插件。 在对话输入栏旁自由填写你的人设文本，一键开关，所有新对话自动生效、免重启。 人设纯粹是你设定的风格，不覆盖 DSH 安全护栏，安装即用、状态持久化。 |
| 1121 | [Oscar-Williams/dsh-deepatlas](https://github.com/Oscar-Williams/dsh-deepatlas) | 1 | 2026-08-22 | 2026-08-22 | Local capability assurance and evidence-backed plugin navigation for DeepSeek Harness. |
| 1122 | [oxlyn/dsh-model-health](https://github.com/oxlyn/dsh-model-health) | 1 | 2026-08-22 | 2026-08-22 | dsh model health status check |
| 1123 | [oxlyn/dsh-plugin-mgr](https://github.com/oxlyn/dsh-plugin-mgr) | 1 | 2026-08-22 | 2026-08-22 | deepseek harness plugin manager |
| 1124 | [pan17/dsh-minimax-usage](https://github.com/pan17/dsh-minimax-usage) | 1 | 2026-08-24 | 2026-08-24 | DSH plugin: floating MiniMax Token Plan usage bubble in the Web UI |
| 1125 | [patrickluvsoj/dsh-llm-nous](https://github.com/patrickluvsoj/dsh-llm-nous) | 1 | 2026-08-21 | 2026-08-27 | Nous Portal LLM plugin bundle for DeepSeek Harness |
| 1126 | [paulalesius/dsh-hindsight-advanced](https://github.com/paulalesius/dsh-hindsight-advanced) | 1 | 2026-08-23 | 2026-08-23 | Long-term memory for DeepSeek Harness agents: automatic recall each turn, a retain/recall/reflect tool, standing rules, and visibility you scope to the whole bank, a preset, or a session. |
| 1127 | [pc439527/dsh-model-provider](https://github.com/pc439527/dsh-model-provider) | 1 | 2026-08-24 | 2026-08-24 | DeepSeek Harness Model Selector UX Enhancement Plugin: show each model's provider (providerId:modelId identity, provider-grouped catalog, shadowed composer model seat) |
| 1128 | [pengls/dsh-quick-view](https://github.com/pengls/dsh-quick-view) | 1 | 2026-08-23 | 2026-08-23 | dsh quick view plugin |
| 1129 | [phantomSuying/dsh-module-driven-develop](https://github.com/phantomSuying/dsh-module-driven-develop) | 1 | 2026-08-30 | 2026-08-31 | DSH plugin for module-driven development: decompose requirements into a module tree, generate each module with an independent agent, and fully regenerate from design on any change. |
| 1130 | [pharaohnie/dsh-rtk-tools](https://github.com/pharaohnie/dsh-rtk-tools) | 1 | 2026-08-25 | 2026-08-25 | DSH plugin: expose rtk (Rust Token Killer) as wide-category Tools — save 60-90% tokens on shell output with softRewriteBash routing |
| 1131 | [philmingdao/anno](https://github.com/philmingdao/anno) | 1 | 2026-08-16 | 2026-08-22 | Local-first HTML review and annotation for AI coding agents |
| 1132 | [pipipigu/dsh-workspace-tree](https://github.com/pipipigu/dsh-workspace-tree) | 1 | 2026-08-28 | 2026-08-28 | Virtual session folder grouping, drag & drop, and subproject manager for DeepSeek Harness (DSH). |
| 1133 | [pmorgan3/deep-tui](https://github.com/pmorgan3/deep-tui) | 1 | 2026-08-21 | 2026-08-22 | deep-tui is a plugin-first coding-agent harness built on Cordis. Providers, tools, prompts, permissions, storage, themes, commands, renderers, and the agent loop are all replaceable plugins. |
| 1134 | [ppjun2026/dsh-client-ui-lingxi](https://github.com/ppjun2026/dsh-client-ui-lingxi) | 1 | 2026-08-23 | 2026-08-23 | 灵犀（Lingxi）— DSH Web GUI 灵感工作台插件：想法池录入/孵化/计划/立项管理 + AI 解析评分与关联图谱，单文件 JSON 存储，零构建工具链，MIT。 |
| 1135 | [Practice019/dsh-kun-pet](https://github.com/Practice019/dsh-kun-pet) | 1 | 2026-08-15 | 2026-08-25 | Kun Like 桌宠 - DSH 桌面宠物插件 |
| 1136 | [promisez322-prog/dsh-vox-input](https://github.com/promisez322-prog/dsh-vox-input) | 1 | 2026-08-30 | 2026-08-31 | Voice (speech-to-text) input for the DSH Web composer via Web Speech API — tap, speak, transcript fills the input box. Zero server, zero API keys. |
| 1137 | [ptonlix/dsh-forge](https://github.com/ptonlix/dsh-forge) | 1 | 2026-08-22 | 2026-08-31 |  building an auditable desktop distribution around DeepSeek Harness (DSH).  |
| 1138 | [puesite/dsh-telegram-notify](https://github.com/puesite/dsh-telegram-notify) | 1 | 2026-08-23 | 2026-08-24 | DSH/EAC Telegram 通知 + 聊天 + 远程批准插件 |
| 1139 | [purezhi/dsh-plugin-confirmo](https://github.com/purezhi/dsh-plugin-confirmo) | 1 | 2026-08-22 | 2026-08-23 | 复刻 confirmo for DeepSeek Harness |
| 1140 | [pwping/dsh-power-launch](https://github.com/pwping/dsh-power-launch) | 1 | 2026-08-29 | 2026-08-29 | DSH桌面启动器插件，双击桌面快捷方式启动dsh Web UI，不需要每次打开终端手动输入命令 |
| 1141 | [qinglang8609/deepseek_herdr](https://github.com/qinglang8609/deepseek_herdr) | 1 | 2026-08-21 | 2026-08-23 | 多智能体总指挥插件（DeepSeek Harness 原生版） ——让 DeepSeek 高效打开并指挥一个 claude / opencode / codex 智能体团队，实时看到每个智能体在做什么，通过共享记忆与任务看板编排多人协作。 |
| 1142 | [QinpanWan/dsh-doc-quick](https://github.com/QinpanWan/dsh-doc-quick) | 1 | 2026-08-25 | 2026-08-27 | Drag documents into the dsh web chat for direct local-file processing; a right sidebar lists outputs and file paths. 拖拽文档进 Web 对话框快速处理，右侧侧栏展示产出。 |
| 1143 | [QinpanWan/dsh-harmonyos-market](https://github.com/QinpanWan/dsh-harmonyos-market) | 1 | 2026-08-24 | 2026-08-27 | HarmonyOS-exclusive plugin market for DeepSeek Harness — only plugins that actually run on HarmonyOS |
| 1144 | [QinpanWan/dsh-prompt-antivirus](https://github.com/QinpanWan/dsh-prompt-antivirus) | 1 | 2026-08-31 | 2026-08-31 | dsh 全局防提示注入/上下文病毒感染插件：扫描工具参数、结果、进模型前消息与出站流；quarantine/block/monitor 三模式 + 金丝雀 + 可演进签名库（学习/导入/导出）。纯 JS 零原生依赖。 |
| 1145 | [QinXi-ai/dsh-codex-import](https://github.com/QinXi-ai/dsh-codex-import) | 1 | 2026-08-13 | 2026-08-23 | Read-only Codex setup compatibility scanner for DeepSeek Harness |
| 1146 | [Qiongkura/dsh-interface-settings](https://github.com/Qiongkura/dsh-interface-settings) | 1 | 2026-08-16 | 2026-08-29 | DSH interface customization plugin: wallpaper / transparency / glass blur / splash screen一个 DeepSeek Harness 前端插件：把「壁纸 / 区域透明 / 输入框与轨迹毛玻璃 / 模糊程度 / 启动画面」做成一站式界面设置，作为独立插件项目上传、分享，装进 DSH 即可使用 |
| 1147 | [qiufengcrl/dsh-ip-https](https://github.com/qiufengcrl/dsh-ip-https) | 1 | 2026-08-26 | 2026-08-26 | DeepSeek Harness plugin: remote settings + Let's Encrypt IP certificates |
| 1148 | [qixin-ai-data/dsh-qixin-insight-mcp-oauth](https://github.com/qixin-ai-data/dsh-qixin-insight-mcp-oauth) | 1 | 2026-08-29 | 2026-08-31 | DeepSeek Harness 插件：一键 OAuth 2.1 (PKCE) 授权，将启信慧眼 MCP 服务端挂载进 harness，让模型直接触达企业工商、股权、司法与风险等智能数据。 |
| 1149 | [qiyeren/dsh-eac-popup](https://github.com/qiyeren/dsh-eac-popup) | 1 | 2026-08-27 | 2026-08-27 | DSH plugin: ???? agent ??/?????,EAC ????(??????)+?????5?+?????? |
| 1150 | [QuantumKuba/dsh-graphify-plugin](https://github.com/QuantumKuba/dsh-graphify-plugin) | 1 | 2026-08-31 | 2026-08-31 | Native Graphify knowledge graph plugin for DeepSeek Harness (DSH) — code intelligence, god nodes, and topological agent tools. |
| 1151 | [qwert702/dsh-continue-on-limit](https://github.com/qwert702/dsh-continue-on-limit) | 1 | 2026-08-20 | 2026-08-23 | Auto-continue for DeepSeek Harness: when a local model hits its output-token cap, automatically send "continue" so the reply keeps flowing |
| 1152 | [Qx002/dsh-group-chat](https://github.com/Qx002/dsh-group-chat) | 1 | 2026-08-21 | 2026-08-22 | DeepSeek Harness插件，多AI群聊插件 |
| 1153 | [Raiyan007-gb/dsh-remote-tunnel-easy](https://github.com/Raiyan007-gb/dsh-remote-tunnel-easy) | 1 | 2026-08-28 | 2026-08-29 | DSH plugin bundle: scan a QR to open the deepseek-harness web UI on your phone inside the same session - cloudflared quick tunnel, no database, Windows/macOS/Linux |
| 1154 | [ramen-ai-dev/dsh-ramen-guard](https://github.com/ramen-ai-dev/dsh-ramen-guard) | 1 | 2026-08-27 | 2026-08-27 | Fail-closed DeepSeek Harness guard enforcing ramen-ai Core IT policy before tool execution. |
| 1155 | [rangrongg/SearchSieve](https://github.com/rangrongg/SearchSieve) | 1 | 2026-08-26 | 2026-08-26 | DeepSeek Harness 插件：逐页判断搜索结果的语义相关度，智能过滤无关噪音，量化信息覆盖度，让每一次AI检索都透明可信。 |
| 1156 | [Raphaelutumn/dsh-mood](https://github.com/Raphaelutumn/dsh-mood) | 1 | 2026-08-27 | 2026-08-27 | A tiny behavioral mood ring for your AI coding agent: a four-state session-header status light (GOOD/CONFUSED/FRUSTRATED/OVERWHELMED) for DeepSeek Harness |
| 1157 | [re-ITRT/dsh-keyring](https://github.com/re-ITRT/dsh-keyring) | 1 | 2026-08-22 | 2026-08-22 | DeepSeek Harness 密钥保险箱插件：自动捕获与脱敏密钥/凭据，settings 界面管理，支持会话级与全局级存储。 |
| 1158 | [red000000/dsh-cross-session-bridge](https://github.com/red000000/dsh-cross-session-bridge) | 1 | 2026-08-22 | 2026-08-23 | 适用于deepseek harness的根会话桥插件，可令根会话间双向通信 |
| 1159 | [RGarvel/dsh-channel-spec](https://github.com/RGarvel/dsh-channel-spec) | 1 | 2026-08-27 | 2026-08-27 | RFC: 按来源渠道对 DSH 会话分类展示（session header channel 字段 + GUI 渠道视图）— 源自 deepseek-harness discussion #3897 |
| 1160 | [RGarvel/dsh-channel-view](https://github.com/RGarvel/dsh-channel-view) | 1 | 2026-08-27 | 2026-08-27 | DSH 渠道会话视图 spike：侧边栏 Channels tab 注入 + 会话投影数据链（RFC-0001, discussion #3897） |
| 1161 | [Rock-ql/dsh-relay-fast](https://github.com/Rock-ql/dsh-relay-fast) | 1 | 2026-08-25 | 2026-08-25 | DSH relay plugin: reasoning-effort autofill, /models sync, capability-aware Fast toggle \| DSH 中转站思考等级与 Fast 开关插件 |
| 1162 | [rongxingda/dsh-prompt-enhance](https://github.com/rongxingda/dsh-prompt-enhance) | 1 | 2026-08-29 | 2026-08-29 | Prompt enhancement plugin for the DeepSeek Harness web GUI: one-click rewrite of the composer draft into a structured prompt, with preview, fill-back, and undo. |
| 1163 | [Ruiming-cn/dsh-ask-in-sidebar](https://github.com/Ruiming-cn/dsh-ask-in-sidebar) | 1 | 2026-08-25 | 2026-08-25 | Ask about selected assistant text in an ephemeral DSH Web sidebar using a snapshot of the main conversation. |
| 1164 | [Ruiming-cn/dsh-more-session-operations](https://github.com/Ruiming-cn/dsh-more-session-operations) | 1 | 2026-08-21 | 2026-08-22 | DeepSeek Harness Web sidebar session-row menu enhancements: mark unread via the official completed-reminder dot, copy session ID, delete session with confirmation, archive confirmation, and recursive subagent-session deletion. |
| 1165 | [runfali/dsh-config-center](https://github.com/runfali/dsh-config-center) | 1 | 2026-08-24 | 2026-08-24 | dsh 扩展管理中心：WebUI 内统一管理 插件 / Skill / MCP -- bundle 安装移除、cordis.patch.yml 行增删改、SKILL.md 编辑、MCP 动态挂载即时生效。零侵入 bundle 插件，不改 dsh 源码。 |
| 1166 | [runfali/dsh-export-kit](https://github.com/runfali/dsh-export-kit) | 1 | 2026-08-24 | 2026-08-24 | dsh 对话导出套件：一键将对话导出为 Markdown / TXT / JSON / CSV / PNG 长图 / PDF，附公式复制（LaTeX / MathML / Word 兼容）、设置备份与全会话归档。零侵入 bundle 插件，不改 Harness 源码。 |
| 1167 | [runfali/dsh-mem0-plugins](https://github.com/runfali/dsh-mem0-plugins) | 1 | 2026-08-24 | 2026-08-24 | dsh 持久化记忆插件 - 依托自建的 mem0‑graph 服务器实现自动回忆与回写。 |
| 1168 | [runfali/dsh-prompt-injector](https://github.com/runfali/dsh-prompt-injector) | 1 | 2026-08-27 | 2026-08-27 | dsh 通用每轮上下文注入插件：设置页管理提示词清单，每轮对话把每条启用提示词以「上下文注入」提醒行注入模型上下文，让纪律规则（例如 图谱消费/wiki 先查/记忆召回）可靠生效。 |
| 1169 | [Ruszero01/dsh-tang-governance](https://github.com/Ruszero01/dsh-tang-governance) | 1 | 2026-08-23 | 2026-08-26 | Three Departments and Six Ministries governance mode plugin for DeepSeek Harness \| dsh 三省六部模式插件 |
| 1170 | [S2P2/dsh-lab](https://github.com/S2P2/dsh-lab) | 1 | 2026-08-21 | 2026-08-23 | Personal DeepSeek Harness extension lab — plugins, Agent presets, and supporting research. |
| 1171 | [SA1992X/dsh-ctrl-enter-submit](https://github.com/SA1992X/dsh-ctrl-enter-submit) | 1 | 2026-08-25 | 2026-08-26 | 轻松换行 |
| 1172 | [SaekiRaku/deepseek-rainbow-fart](https://github.com/SaekiRaku/deepseek-rainbow-fart) | 1 | 2026-08-26 | 2026-08-31 | 当你使用 DeepSeek Harness WebUI 发送消息后，插件会基于你的内容生成夸赞你的话，并通过 TTS 合成并播放声音。 \| After you send a message via DeepSeek Harness WebUI, the plugin generates compliments based on your input and plays them via TTS. |
| 1173 | [sakthiveltofficial/dsh-gmail-plugins](https://github.com/sakthiveltofficial/dsh-gmail-plugins) | 1 | 2026-08-25 | 2026-08-25 | dsh-gmail: Gmail plugin suite for DeepSeek Harness — 61 model-facing tools + 2 polling triggers over the Gmail & People APIs (OAuth2) |
| 1174 | [sakthiveltofficial/dsh-shopify-plugins](https://github.com/sakthiveltofficial/dsh-shopify-plugins) | 1 | 2026-08-26 | 2026-08-26 | Shopify plugin for DeepSeek Harness: 213 model-facing shopify_* tools over the Shopify Admin REST + GraphQL APIs (products, orders, customers, inventory, fulfillments, discounts, content, webhooks, themes, billing, bulk operations) with Admin API access-token auth. |
| 1175 | [sarfarazstark/dsh-material-file-icons](https://github.com/sarfarazstark/dsh-material-file-icons) | 1 | 2026-08-23 | 2026-08-23 | Material Icon Theme file & folder icons for the DeepSeek Harness web GUI (dsh-better-sidebar) - 349 authentic SVGs, named folders with open variants, zero patching required |
| 1176 | [sch246/dsh-warm-minimal](https://github.com/sch246/dsh-warm-minimal) | 1 | 2026-08-24 | 2026-08-24 | DSH 温暖极简模式：模仿官方 minimal 的首轮两工具形态引导 deepseek-v4-pro 进入 we need 思维链；bootstrap 后第二轮再放行其余工具。 |
| 1177 | [scientisbo/dsh-codex-usage](https://github.com/scientisbo/dsh-codex-usage) | 1 | 2026-08-23 | 2026-08-24 | Codex 用量 · 订阅配额 + DeepSeek 余额聚合（DeepSeek Harness host 插件） \| Codex subscription quota & DeepSeek balance aggregator for DeepSeek Harness |
| 1178 | [scientisbo/dsh-deepseek-usage](https://github.com/scientisbo/dsh-deepseek-usage) | 1 | 2026-08-23 | 2026-08-24 | DeepSeek 用量 · 余额面板（DeepSeek Harness Web 客户端插件） \| A clean DeepSeek usage & balance panel for DeepSeek Harness |
| 1179 | [SeerableOfficial/dsh-anydoc-markdown](https://github.com/SeerableOfficial/dsh-anydoc-markdown) | 1 | 2026-08-29 | 2026-08-31 | Document → Markdown + vision image description plugin for DeepSeek Harness (dsh). Converts Word/PPT/Excel/ODT/RTF/EPUB/CSV/PDF via firecrawl-anydoc and describes embedded images with a VLM. |
| 1180 | [SeireiA/dsh-plugin-rtk](https://github.com/SeireiA/dsh-plugin-rtk) | 1 | 2026-08-21 | 2026-08-21 | DeepSeek Harness plugin for RTK-powered shell output compaction |
| 1181 | [sg88/dsh-proxy-switch](https://github.com/sg88/dsh-proxy-switch) | 1 | 2026-08-22 | 2026-08-22 | DSH 网络代理开关：直连失败自动回退到 HTTP/SOCKS5 代理，设置面板可配置代理地址 |
| 1182 | [Shaky77/KISS_Law-DSH](https://github.com/Shaky77/KISS_Law-DSH) | 1 | 2026-08-19 | 2026-08-27 | Weiwen's Law (KISS-Law) — a domain-agnostic causal-constraint middleware for DeepSeek Harness. A faithful, white-box presentation of how causal law actually runs. White-box audit, never prediction. Hard-gate the boundary; inner H decides freely. |
| 1183 | [shangshuo1/DSH-Virtual](https://github.com/shangshuo1/DSH-Virtual) | 1 | 2026-08-24 | 2026-08-24 | Manage multiple isolated DeepSeek Harness (dsh) instances like virtual machines. Rust/egui native desktop app. |
| 1184 | [shaomingbo/dsh-attention](https://github.com/shaomingbo/dsh-attention) | 1 | 2026-08-23 | 2026-08-24 | Desktop attention alerts for DeepSeek Harness Web: tab title, favicon, sound, and native OS notifications. |
| 1185 | [shaomingbo/dsh-subscription-search](https://github.com/shaomingbo/dsh-subscription-search) | 1 | 2026-08-19 | 2026-08-30 | ChatGPT/Grok subscription OAuth, model routes, and ChatGPT to Grok to Exa to DeepSeek web-search fallback for DeepSeek Harness |
| 1186 | [sharewiner/dsh-model-management](https://github.com/sharewiner/dsh-model-management) | 1 | 2026-08-25 | 2026-08-25 | DSH model management, synchronized model visibility, and OpenAI Responses web search. |
| 1187 | [Sharl210/dsh-strip-sandbox-permissions](https://github.com/Sharl210/dsh-strip-sandbox-permissions) | 1 | 2026-08-21 | 2026-08-22 | Strip sandbox_permissions/justification from model tool-call arguments to avoid false sandbox escalation errors |
| 1188 | [shendeguize/AgentSideCar](https://github.com/shendeguize/AgentSideCar) | 1 | 2026-08-22 | 2026-08-25 | A local-first CLI for observing AI-agent sessions |
| 1189 | [shendeguize/Remote_DSH_Center](https://github.com/shendeguize/Remote_DSH_Center) | 1 | 2026-08-20 | 2026-08-24 | One-page local manager and CLI for local and remote dsh web instances, with SSH tunnels for remote hosts. |
| 1190 | [shengmk/godsh](https://github.com/shengmk/godsh) | 1 | 2026-08-28 | 2026-08-28 | godsh - GUI launcher for DeepSeek Harness (dsh): manage profiles, plugins, kernels, and dsh versions |
| 1191 | [Shhaaawwww/vibe-intent-compiler](https://github.com/Shhaaawwww/vibe-intent-compiler) | 1 | 2026-08-25 | 2026-08-25 | A one-click DeepSeek Harness plugin that compiles messy Vibe Coder drafts into concise, faithful, actionable instructions without inventing details. |
| 1192 | [ShinonomeAya/dsh-git-chain](https://github.com/ShinonomeAya/dsh-git-chain) | 1 | 2026-08-26 | 2026-08-26 | DeepSeek Harness plugin: Cursor-style Git commit-chain graph with SVG lanes, commit details, diff, filtering, and guarded branch switching. |
| 1193 | [shixiong0529/dsh-schedule-enable](https://github.com/shixiong0529/dsh-schedule-enable) | 1 | 2026-08-26 | 2026-08-26 | 为deepseek harness创建自动化任务 |
| 1194 | [Shizuku-keop/dsh-compat-guard](https://github.com/Shizuku-keop/dsh-compat-guard) | 1 | 2026-08-25 | 2026-08-25 | Compatibility governance for DeepSeek Harness: upgrade pre-flight gate, storage-format fingerprint,  backup, session migration, per-profile lockfile, plugin x DSH compat matrix. |
| 1195 | [Shizuku-keop/dsh-health](https://github.com/Shizuku-keop/dsh-health) | 1 | 2026-08-26 | 2026-08-26 | Session loop-health diagnostics for DeepSeek Harness: oscillation/stall/near-repeat/per-tool/token/compaction profiles + auditable 0-100 score. CLI + live watch bundle. |
| 1196 | [Shonean/deepseek-harness-vscode-desktop](https://github.com/Shonean/deepseek-harness-vscode-desktop) | 1 | 2026-08-27 | 2026-08-27 | Enhanced VS Code extension + Desktop app for DeepSeek Harness (DSH): inline diff, @mentions, selection context, approval UI, plan mode, global shortcut. Claude Code-grade experience. Unofficial community project. |
| 1197 | [shuaihaoV/dsh-TheWanderingEarthII](https://github.com/shuaihaoV/dsh-TheWanderingEarthII) | 1 | 2026-08-25 | 2026-08-25 | The Wandering Earth II · 流浪地球2 — DSH Web GUI 电影风格主题：发动机点火联动、MOSS 化发送按钮、星场 HUD |
| 1198 | [shuaweng/DSH_xieshujing](https://github.com/shuaweng/DSH_xieshujing) | 1 | 2026-08-30 | 2026-08-30 | 写书鲸：面向 DeepSeek Harness 的原生 AI 小说创作工作台插件 |
| 1199 | [sjlgg/dsh-free-web-search](https://github.com/sjlgg/dsh-free-web-search) | 1 | 2026-08-23 | 2026-08-23 | a deepseek plugin for free web search |
| 1200 | [SkuraSshly/dsh-done-badge](https://github.com/SkuraSshly/dsh-done-badge) | 1 | 2026-08-24 | 2026-08-24 | DeepSeek Harness (DSH) task completion badge: native Windows taskbar counter (ITaskbarList3) while the window is away, auto-clears on return. Subagent sessions excluded. |
| 1201 | [SleepEggTart/dsh-code-coverage](https://github.com/SleepEggTart/dsh-code-coverage) | 1 | 2026-08-26 | 2026-08-27 | 解析 DSH session 日志归因 AI 生成文件，叠加 c8 覆盖率，产出 AI vs 人工代码覆盖率对比、高危未测文件清单与信任分。 |
| 1202 | [SleepEggTart/dsh-dev-wrapped](https://github.com/SleepEggTart/dsh-dev-wrapped) | 1 | 2026-08-26 | 2026-08-27 | DeepSeek Harness (DSH) 开发者使用报告——类 Spotify Wrapped，统计与 AI 结对编程的行为，生成可分享报告卡片 |
| 1203 | [SleepEggTart/dsh-mbti-jury](https://github.com/SleepEggTart/dsh-mbti-jury) | 1 | 2026-08-31 | 2026-08-31 | DSH 插件：16 型 MBTI 人格评审团，并排评审你最近一次 commit——同一个 diff，16 种看见世界的方式。 |
| 1204 | [SLin-code/dsh-skill-manager](https://github.com/SLin-code/dsh-skill-manager) | 1 | 2026-08-24 | 2026-08-24 | Minimal, security-focused local Skill Manager for DeepSeek Harness Web. |
| 1205 | [Slymaster/dsh-theme-lab](https://github.com/Slymaster/dsh-theme-lab) | 1 | 2026-08-24 | 2026-08-24 | Unofficial modular themes and starter kit for DeepSeek Harness. |
| 1206 | [Snow-ea/dsh-token-optimizer](https://github.com/Snow-ea/dsh-token-optimizer) | 1 | 2026-08-30 | 2026-08-30 | Deterministic, recoverable tool-result compression and cache-aware compaction for DeepSeek Harness. |
| 1207 | [SnowRikka/dsh-llama-responses](https://github.com/SnowRikka/dsh-llama-responses) | 1 | 2026-08-22 | 2026-08-23 | DeepSeek Harness plugin: run subagents on a local llama.cpp model via the OpenAI Responses (/v1/responses) protocol — LLM adapter + delegation skill |
| 1208 | [softspark/dsh-codex](https://github.com/softspark/dsh-codex) | 1 | 2026-08-25 | 2026-08-27 | DeepSeek Harness provider for locally authenticated Codex app-server access through a ChatGPT subscription. |
| 1209 | [sol5766/dshm](https://github.com/sol5766/dshm) | 1 | 2026-08-20 | 2026-08-22 | deepseek harnes HarmonyOS PC client |
| 1210 | [spirits001/dsh-user-message-rail](https://github.com/spirits001/dsh-user-message-rail) | 1 | 2026-08-23 | 2026-08-23 | A dsh client plugin: a tick rail on the window left edge marking every message you sent, with hover preview and jump-to-message. |
| 1211 | [spritebbb/dsh-skill-usage](https://github.com/spritebbb/dsh-skill-usage) | 1 | 2026-08-31 | 2026-08-31 | Real-time display of the currently active skill in the DeepSeek Harness Web GUI — a composer dock chip showing the current skill name with hover history. 🌟 实时显示 DSH 当前正在使用的技能，安装在输入框下方的小徽章，装上就能用～ |
| 1212 | [sryimnoob123/dsh-global-prompt](https://github.com/sryimnoob123/dsh-global-prompt) | 1 | 2026-08-25 | 2026-08-25 | DSH settings plugin for global and project AGENTS.md, identity/persona injection, and result notifications. |
| 1213 | [sryimnoob123/dsh-tool-pwsh-safe](https://github.com/sryimnoob123/dsh-tool-pwsh-safe) | 1 | 2026-08-20 | 2026-08-26 | Elbow-proof PowerShell for DeepSeek Harness: pwsh_safe tool runs scripts via base64 -EncodedCommand, immune to quoting/escaping pain, sandbox-seam based |
| 1214 | [sryimnoob123/dsh-web-search-ollama](https://github.com/sryimnoob123/dsh-web-search-ollama) | 1 | 2026-08-20 | 2026-08-25 | Ollama-backed web search provider for DeepSeek Harness (ctx.web) |
| 1215 | [SsTtone1/dsh-message-cleaner](https://github.com/SsTtone1/dsh-message-cleaner) | 1 | 2026-08-25 | 2026-08-25 | DSH Web GUI 插件：在会话输入框上方提供历史消息记录面板，支持按条删除、原位恢复与内置节点导航条，让长会话的管理像编辑文档一样简单。 |
| 1216 | [StabCut/dsh-edit-regenerate](https://github.com/StabCut/dsh-edit-regenerate) | 1 | 2026-08-18 | 2026-08-24 | DSH plugin: edit a user message in conversation history and regenerate from the revised prompt in a forked session. |
| 1217 | [starefinger/dsh-llm-qwen-local](https://github.com/starefinger/dsh-llm-qwen-local) | 1 | 2026-08-26 | 2026-08-26 | 面向 DeepSeek Harness(dsh)的 LLM 适配器插件:驱动由 OpenAI 兼容服务的本地部署 Qwen3.8-27B 模型。支持按模型多模态开关、完全可配置的推理档位、请求图像投影,以及中英双语 Web 设置页。 |
| 1218 | [Stellight/dsh-imggen](https://github.com/Stellight/dsh-imggen) | 1 | 2026-08-22 | 2026-08-22 | DeepSeek Harness plugin: text-to-image output with in-chat image cards, download button, history gallery, and provider selection tabs (Pollinations / OpenAI DALL-E 3). |
| 1219 | [steve-magne/dsh-plugins](https://github.com/steve-magne/dsh-plugins) | 1 | 2026-08-24 | 2026-08-25 | DeepSeek Harness plugins — dual-face cordis packages extending the DSH web surface: command deck, git worktrees, one-click PRs, cron-scheduled tasks |
| 1220 | [stultuss/dsh-clear-tool-results](https://github.com/stultuss/dsh-clear-tool-results) | 1 | 2026-08-25 | 2026-08-25 | DSH 宿主插件：每轮对话结束后，把该轮的原始工具结果归档（tool result）到会话目录（tool-result-logs），并从上下文中清除，减少 Token 消耗；模型可用 read_tool_result_log 工具按轮次或时间自主读取归档数据。 |
| 1221 | [StvLi/dsh-phoenix](https://github.com/StvLi/dsh-phoenix) | 1 | 2026-08-30 | 2026-08-31 | Never-interrupt, resumable lifecycle for DeepSeek Harness (dsh): graceful restart + client auto-reconnect + cross-restart goal continuation. |
| 1222 | [SUJIElearning/dsh-trashbin](https://github.com/SUJIElearning/dsh-trashbin) | 1 | 2026-08-23 | 2026-08-23 | DSH 回收站（删除冷静区）：归档的对话进入回收站，支持恢复、立即移除、7 天自动清理 |
| 1223 | [SUJIElearning/zhaoyu-restart](https://github.com/SUJIElearning/zhaoyu-restart) | 1 | 2026-08-23 | 2026-08-23 | One-click silent DSH restart button for DeepSeek Harness (dsh-plugin) |
| 1224 | [sumarilkkxx/dsh-atlas](https://github.com/sumarilkkxx/dsh-atlas) | 1 | 2026-08-21 | 2026-08-22 | Visual conversation canvas for DeepSeek Harness. |
| 1225 | [summer-521/deepseek-harness-swift](https://github.com/summer-521/deepseek-harness-swift) | 1 | 2026-08-25 | 2026-08-28 | 基于 AppKit、SwiftUI 与 WKWebView 的 DSH 原生 macOS 桌面壳，提供设置中心、DSH 版本管理、插件管理、通知和 Sparkle 应用更新。 |
| 1226 | [Sunday2Mo/dsh-file-quote](https://github.com/Sunday2Mo/dsh-file-quote) | 1 | 2026-08-27 | 2026-08-27 | 基于 better-sidebar 的统一引用插件：划选文件/消息即可批注引用，引用块带文件路径与行区间、双端折叠、点击跳回原文 ｜ Unified-quoting plugin built on DSH-better-sidebar: select files or messages to annotate; quote blocks carry path & line range, collapse in chat and history, and jump back to the source on click. |
| 1227 | [sunkeycn/dsh-desktop](https://github.com/sunkeycn/dsh-desktop) | 1 | 2026-08-25 | 2026-08-25 | Native macOS desktop wrapper for DeepSeek Harness with plugin management and FRP remote access |
| 1228 | [SunNull/dsh-relay](https://github.com/SunNull/dsh-relay) | 1 | 2026-08-16 | 2026-08-24 | Cloud relay for DeepSeek Harness: expose your home dsh instance to any device with full real-time sync (out-of-tree plugin + wire-trunk architecture) |
| 1229 | [sunzhyang1616-ui/dsh-ssh-terminal](https://github.com/sunzhyang1616-ui/dsh-ssh-terminal) | 1 | 2026-08-29 | 2026-08-29 | 在 DSH 侧边栏（dsh-better-sidebar）连接远程主机的 SSH 终端：逐步查看 agent 命令与输出，内置 ssh_connect / ssh_exec 等工具，记录本机持久化。 |
| 1230 | [svgop/dsh-rich-questions](https://github.com/svgop/dsh-rich-questions) | 1 | 2026-08-26 | 2026-08-29 | Rich branching survey system for DeepSeek Harness (DSH) Web GUI — ask_survey tool with branch graphs, delayed hover insights, Mermaid diagrams, quick mode, reroll/push/discuss actions |
| 1231 | [sycamorestr/dsh-platform-account-manager-plugin](https://github.com/sycamorestr/dsh-platform-account-manager-plugin) | 1 | 2026-08-29 | 2026-08-29 | DSH platform account and persistent browser-session manager |
| 1232 | [T-Markus-Liang/dsh-game-studio](https://github.com/T-Markus-Liang/dsh-game-studio) | 1 | 2026-08-21 | 2026-08-22 | DSH Game Studio: AI-native Game Development Runtime for DeepSeek Harness — 可安装/卸载/升级的游戏开发插件（/game 子命令、动态 Agent Pool、引擎适配器、Verifier + Quality Gate） |
| 1233 | [Tangtang232/dsh-recovery](https://github.com/Tangtang232/dsh-recovery) | 1 | 2026-08-25 | 2026-08-25 | Recovery: Web first aid for DeepSeek Harness |
| 1234 | [tanle-mtr/dsh-plogin-plugin-recommender](https://github.com/tanle-mtr/dsh-plogin-plugin-recommender) | 1 | 2026-08-22 | 2026-08-23 | The most comprehensive AI-curated list of DeepSeek Harness (DSH) plugins - 190+ plugins, 12 categories, updated hourly by AI. |
| 1235 | [TaoruiLiu19/DSHwork](https://github.com/TaoruiLiu19/DSHwork) | 1 | 2026-08-15 | 2026-08-24 | DeepSeek Harness Desktop Client |
| 1236 | [taoser258/dsh-client-ui-skin-qingxiao](https://github.com/taoser258/dsh-client-ui-skin-qingxiao) | 1 | 2026-08-29 | 2026-08-29 | 清宵 · 弦凝清霄 —— DeepSeek Harness (DSH) Web 界面美化皮肤：以《鸣潮》角色清宵为灵感的冰蓝·青碧·月白·玄夜调色板，含可换背景画卷、剑气流光粒子、磨砂玻璃面板与新会话迎宾页。A Qingxiao (Wuthering Waves) themed client UI skin for the DSH web GUI. |
| 1237 | [taskschd1145/deepseek-harness-clean](https://github.com/taskschd1145/deepseek-harness-clean) | 1 | 2026-08-22 | 2026-08-22 | 一个"三无"DSH桌面子端：打开它，就等于在浏览器里打DSH， 只不过它是一个带托盘图标、全原生的 Windows 窗口。 |
| 1238 | [TestTheBoy/dsh_plugin_file_attach](https://github.com/TestTheBoy/dsh_plugin_file_attach) | 1 | 2026-08-26 | 2026-08-26 | Add files to context |
| 1239 | [thedeveloper256/dsh-model-router](https://github.com/thedeveloper256/dsh-model-router) | 1 | 2026-08-21 | 2026-08-22 | DeepSeek Harness plugin: role-based model routing — planner (root agent) on deepseek-v4-pro, delegated executor subagents on deepseek-v4-flash; ships a prompt section and a pro-flash-routing skill. |
| 1240 | [TheHeartFickle/dsh-one-dark-pro](https://github.com/TheHeartFickle/dsh-one-dark-pro) | 1 | 2026-08-22 | 2026-08-23 | DSH（DeepSeek Harness）主题插件：注册 One Dark Pro 配色，并把「外观」设置里的主题添加 One Dark Pro。 |
| 1241 | [TheHeartFickle/dsh-session-manager](https://github.com/TheHeartFickle/dsh-session-manager) | 1 | 2026-08-21 | 2026-08-22 | DSH 会话管理插件 —— 对话回退 + 归档会话，长会话可回滚、可整理。 |
| 1242 | [thomasvvugt/dsh-kanban-flow](https://github.com/thomasvvugt/dsh-kanban-flow) | 1 | 2026-08-25 | 2026-08-25 | Agent-driven kanban board for DeepSeek Harness: one board per workspace, per-task agent sessions, guarded human/agent workflow |
| 1243 | [thomasvvugt/dsh-wide-stats-footer](https://github.com/thomasvvugt/dsh-wide-stats-footer) | 1 | 2026-08-24 | 2026-08-25 | Removes the width clamp on the DeepSeek Harness composer stats footer — long turn/token stats lines span the full composer width instead of truncating |
| 1244 | [TianyiTwT/dsh-image-zoom](https://github.com/TianyiTwT/dsh-image-zoom) | 1 | 2026-08-23 | 2026-08-24 | **Smart image splitting and zooming for Vision-Language Models (VLMs) inside [DeepSeek Harness (dsh)](https://github.com/deepseek-ai/deepseek-harness).** |
| 1245 | [tieveto666-code/dsh-data-mode](https://github.com/tieveto666-code/dsh-data-mode) | 1 | 2026-08-23 | 2026-08-23 | DSH 数据模式插件：在原版 DeepSeek Harness 上增加只读问数。连接数据库或上传 CSV/Excel，用自然语言查数，并支持按数据源管理业务知识。 |
| 1246 | [tieveto666-code/dsh-memory-migration](https://github.com/tieveto666-code/dsh-memory-migration) | 1 | 2026-08-26 | 2026-08-26 | 为原版 DeepSeek Harness 提供长期记忆：用键值对保存身份、偏好、方法论和约束，并在后续对话中按提问召回。可手动增删改查；也可选「记忆迁移」，从 ChatGPT / Claude / Gemini / DeepSeek 官方导出包提取少量核心记忆。独立插件，不修改 DSH 源码。 |
| 1247 | [tiger0012/dsh-we-wallpaper-sync](https://github.com/tiger0012/dsh-we-wallpaper-sync) | 1 | 2026-08-26 | 2026-08-26 | Reusable skill: browse/search/download Wallpaper Engine (Steam 431960) workshop wallpapers and wire them into the DSH skin center, bypassing the Steam HTTP block and region-mismatch sign-in block. |
| 1248 | [Tinger-X/dsh-session-enhance](https://github.com/Tinger-X/dsh-session-enhance) | 1 | 2026-08-25 | 2026-08-31 | Full-control session management for DeepSeek Harness Web |
| 1249 | [TNTsama11/dsh-tool-vision](https://github.com/TNTsama11/dsh-tool-vision) | 1 | 2026-08-21 | 2026-08-22 | DeepSeek Harness (DSH) plugin that lets a text-only agent call DeepSeek-V4-Flash-Vision-Exp to see images on demand, without manually switching models. |
| 1250 | [tower1229/dsh-thinkbar](https://github.com/tower1229/dsh-thinkbar) | 1 | 2026-08-29 | 2026-08-31 | 让 DeepSeek Harness 的思考状态被看见——零侵入地将 reasoning 等待转化为由蓝到金、持续升温的动态 ThinkBar。 |
| 1251 | [Triple3h/dsh-usage-stats](https://github.com/Triple3h/dsh-usage-stats) | 1 | 2026-08-19 | 2026-08-23 | DSH Web plugin: usage statistics — daily/model tokens, sessions, messages, activity heatmap in a zcode-style panel. DSH Web 插件：侧边栏使用统计面板（按天/按模型 tokens、会话、消息、活跃热力图）。 |
| 1252 | [trrrrrryg/dsh-ssh-forge](https://github.com/trrrrrryg/dsh-ssh-forge) | 1 | 2026-08-24 | 2026-08-26 | DSH SSH Forge：为 DeepSeek Harness（DSH）提供 SSH 远程工作区能力：已核验的服务器身份、失败关闭的 Agent 执行路由、远端文件与命令操作；提供 Windows 离线一键安装包，无需 Node.js 或构建工具。 |
| 1253 | [Tsqurt/dsh-plugin-studio](https://github.com/Tsqurt/dsh-plugin-studio) | 1 | 2026-08-27 | 2026-08-28 | 为了开发插件，开发了一个开发插件的插件。通过可视化的事件流、插件管理、工具管理、技能管理、预设管理，简化插件的开发流程，方便开发者理解插件的作用。 |
| 1254 | [TT-Wang/dsh-cron](https://github.com/TT-Wang/dsh-cron) | 1 | 2026-08-26 | 2026-08-26 | Scheduled work for DeepSeek Harness that survives session end, host restart and machine sleep — it schedules an outcome (completion window + effect check + catch-up), not a moment. |
| 1255 | [TwilightSpirit/dsh-message-edit](https://github.com/TwilightSpirit/dsh-message-edit) | 1 | 2026-08-22 | 2026-08-23 | 在消息气泡上加修改按钮，通过 DSH surface replace 机制改写模型上下文，fork 继承、支持 markdown、可审计 |
| 1256 | [tyx6661234/dsh-community-listening](https://github.com/tyx6661234/dsh-community-listening) | 1 | 2026-08-26 | 2026-08-26 | 面向 DeepSeek Harness (DSH) 的社交评论研究插件 |
| 1257 | [Ultmebius/universal-plugin-hub](https://github.com/Ultmebius/universal-plugin-hub) | 1 | 2026-08-26 | 2026-08-31 | DSH 插件市场：内置 Claude 官方插件目录，支持添加 Git 仓库作为插件源；一键安装，技能、子代理、MCP、LSP、hooks 装完自动接线 · Plugin marketplace for DeepSeek Harness |
| 1258 | [Unintendedz/dsh-attention-notify](https://github.com/Unintendedz/dsh-attention-notify) | 1 | 2026-08-23 | 2026-08-23 | Browser notifications for every DSH event that needs user attention |
| 1259 | [Unintendedz/dsh-conversation-tree](https://github.com/Unintendedz/dsh-conversation-tree) | 1 | 2026-08-23 | 2026-08-23 | ChatGPT-style immutable reply branches, inline branch switching, and whole-tree browsing for DeepSeek Harness. |
| 1260 | [Unintendedz/dsh-response-meta](https://github.com/Unintendedz/dsh-response-meta) | 1 | 2026-08-23 | 2026-08-23 | Always-visible model, reasoning, throughput, timestamp, runtime, and TTFT metadata for DeepSeek Harness replies. |
| 1261 | [Unintendedz/dsh-session-tools](https://github.com/Unintendedz/dsh-session-tools) | 1 | 2026-08-23 | 2026-08-23 | Archive, cross-session read, and copy-ID tools for DeepSeek Harness conversations. |
| 1262 | [UNscientific-9/dsh-turnfold](https://github.com/UNscientific-9/dsh-turnfold) | 1 | 2026-08-27 | 2026-08-27 | DSH Web 轮次折叠插件：thinking/工具调用流式可见，turn 完成后自动收纳成一行摘要。 |
| 1263 | [unStone/dsh-plugin-web-ppt](https://github.com/unStone/dsh-plugin-web-ppt) | 1 | 2026-08-22 | 2026-08-22 | DeepSeek Harness plugin: let your agent read and export .pptx / .ppt — pure JS, no PowerPoint, no conversion, no network. |
| 1264 | [v587d/dsh-custom-skin](https://github.com/v587d/dsh-custom-skin) | 1 | 2026-08-28 | 2026-08-28 | 自己的插件皮肤管理工具。 |
| 1265 | [v587d/dsh-LLM-quotes](https://github.com/v587d/dsh-LLM-quotes) | 1 | 2026-08-25 | 2026-08-25 | Latest LLM provider API prices, right inside DeepSeek Harness (dsh) → Settings → Models.最新的大模型（LLM）厂商 API 价格，直接显示在 DeepSeek Harness（dsh） 的 设置 → 模型 页面中。 |
| 1266 | [viethoang35/dsh-chat-bridge](https://github.com/viethoang35/dsh-chat-bridge) | 1 | 2026-08-22 | 2026-08-24 | Chat bridge that connects Telegram (WhatsApp, Zalo, Viber, ... ) to DeepSeek Harness via its headless CLI |
| 1267 | [VioletScar-Hui/trcost-plugin](https://github.com/VioletScar-Hui/trcost-plugin) | 1 | 2026-08-28 | 2026-08-28 | 轨迹省钱优化器：DSH 会话轨迹 token 浪费分析 + waterfall 执行层强制拦截/截断。Trajectory cost optimizer with enforcement layer for DeepSeek Harness. |
| 1268 | [Vuitier/dsh-sound-notify](https://github.com/Vuitier/dsh-sound-notify) | 1 | 2026-08-31 | 2026-08-31 | DSH web plugin: chime on turn complete & intervention needed。DSH任务完成提示音插件 |
| 1269 | [w2327644822-png/dsh-usage-analytics](https://github.com/w2327644822-png/dsh-usage-analytics) | 1 | 2026-08-26 | 2026-08-27 | Personal usage analytics & activity dashboard for the DeepSeek Harness (dsh) web GUI: token totals, contribution heatmap, model share, insights. Local-only, metadata only. |
| 1270 | [Wanbinyu/dsh-companion](https://github.com/Wanbinyu/dsh-companion) | 1 | 2026-08-21 | 2026-08-25 | Local state-aware desktop companion and task-status overlay for DeepSeek Harness Web |
| 1271 | [wangxueqi00/dsh-client-ui-knowledge-cards](https://github.com/wangxueqi00/dsh-client-ui-knowledge-cards) | 1 | 2026-08-31 | 2026-08-31 | A plugin of deepseek harness（DSH）.Turn any conversation in your [DeepSeek Harness](https://github.com/deepseek-ai/deepseek-harness) Web GUI into clean, textured knowledge cards — concepts, flowcharts, comparisons, summaries and mind maps — generated by the agent, previewed in a tabbed gallery, and downloadable in multiple formats. |
| 1272 | [wangzhanchao883/dsh-plugin](https://github.com/wangzhanchao883/dsh-plugin) | 1 | 2026-08-22 | 2026-08-22 | DeepSeek Harness plugin collection: self-developed DSH plugins (screenshot capture, OCR, Obsidian). ?? DSH ?????? |
| 1273 | [warment/deepseek-harness-locale-ru](https://github.com/warment/deepseek-harness-locale-ru) | 1 | 2026-08-30 | 2026-08-31 | Русский язык для DeepSeek Harness web UI — one-command install, 1061 строка, 100% покрытие |
| 1274 | [Washington5533/guarftrain](https://github.com/Washington5533/guarftrain) | 1 | 2026-08-09 | 2026-08-26 | 🛡️ 一行命令，训练脚本零行改动，获得完整守护能力。GPU 监控 · 崩溃恢复 · OOM 自救 · Agent 决策 · MCP 35 工具 · Web Dashboard。 |
| 1275 | [WayneYu430/dsh-voice-agent](https://github.com/WayneYu430/dsh-voice-agent) | 1 | 2026-08-24 | 2026-08-25 | a full duplex voice mode for DSH |
| 1276 | [wenyixiaoqingnian/screenshot-review](https://github.com/wenyixiaoqingnian/screenshot-review) | 1 | 2026-08-29 | 2026-08-29 | dsh skill: 截图审阅——模型自己截图、自己看图、自己改代码，迭代优化前端效果 |
| 1277 | [wertyBSd/dsh-local-llm](https://github.com/wertyBSd/dsh-local-llm) | 1 | 2026-08-20 | 2026-08-24 | Local LLM integration plugin for DeepSeek Harness |
| 1278 | [weshopai/weshop-skill-package](https://github.com/weshopai/weshop-skill-package) | 1 | 2026-08-20 | 2026-08-25 | Creative AI Skills for Codex, Claude Code, Cursor, Deepseek harness and any Agent Skills-compatible runtime. |
| 1279 | [WesleyJay/dsh-weather](https://github.com/WesleyJay/dsh-weather) | 1 | 2026-08-27 | 2026-08-28 | 一个 DSH 天气查询插件，让 AI 智能体可以查询全球城市的实时天气和天气预报 |
| 1280 | [Wodexinhaoleng-Kasssa/dsh-reader](https://github.com/Wodexinhaoleng-Kasssa/dsh-reader) | 1 | 2026-08-22 | 2026-08-22 | In-browser novel reader for the dsh web GUI: online book-source search, chapter-by-chapter reading in a chat-style view, and whole-book TXT download. |
| 1281 | [wodongx123/dsh-qq-notify](https://github.com/wodongx123/dsh-qq-notify) | 1 | 2026-08-17 | 2026-08-27 | QQ notifications via local NapCat for DeepSeek Harness: qq_send / qq_status / qq_napcat / qq_deploy native tools + one-click deploy scripts. QQ???? |
| 1282 | [woosh2010/dsh-usage-dashboard](https://github.com/woosh2010/dsh-usage-dashboard) | 1 | 2026-08-21 | 2026-08-22 | DeepSeek Harness (dsh) usage analytics plugin: peak/valley billing dock, token/cost/model dashboard, cross-session history, global filters \| 用量分析插件：峰谷计费坞 + 用量仪表盘 |
| 1283 | [wozoulesky/dsh-obsidian](https://github.com/wozoulesky/dsh-obsidian) | 1 | 2026-08-14 | 2026-08-23 | DSH（DeepSeek Harness）嵌入 Obsidian 的 AI 协作者插件：聊天侧边栏、内联编辑、@提及与计划模式（连接本地 http://127.0.0.1:3080） |
| 1284 | [writeCasually/dsh-git](https://github.com/writeCasually/dsh-git) | 1 | 2026-08-21 | 2026-08-31 | DeepSeek Harness Git plugin — visual git status, diff, commit & file preview in the DSH web UI |
| 1285 | [WSL043/dsh-deepseek-dashboard](https://github.com/WSL043/dsh-deepseek-dashboard) | 1 | 2026-08-24 | 2026-08-27 | 已归档：DeepSeek API 余额与 DSH 本地用量面板；现有 Release 保留，不再适配未来 DSH。 |
| 1286 | [wszhoho/dsh-file-attachment](https://github.com/wszhoho/dsh-file-attachment) | 1 | 2026-08-28 | 2026-08-28 | 拖入 / 粘贴 / 工具栏上传按钮（📎，可多选）为输入框附加文件：图片走既有草稿图片流程（不落盘）；文档全文落盘到会话工作区 .dsh-file-attachment/ 并插入 @绝对路径引用 |
| 1287 | [wtksana/dsh-font-plugin](https://github.com/wtksana/dsh-font-plugin) | 1 | 2026-08-27 | 2026-08-27 | DeepSeek Harness Font Plugin, DSH 字体插件 |
| 1288 | [xiaobai2017666/dsh-chrome-cdp](https://github.com/xiaobai2017666/dsh-chrome-cdp) | 1 | 2026-08-28 | 2026-08-31 | Chrome DevTools Protocol 插件 for DeepSeek Harness。通过 chromremote-interface 以 CDP 连接并操控 Chrome |
| 1289 | [xiaochaZ/dsh-session-title-summary](https://github.com/xiaochaZ/dsh-session-title-summary) | 1 | 2026-08-25 | 2026-08-26 | DSH plugin: rolling session summary + current-task title (@xiaochaz) |
| 1290 | [xiaoguomeiyitian/dsh-qr-share](https://github.com/xiaoguomeiyitian/dsh-qr-share) | 1 | 2026-08-29 | 2026-08-30 | DSH web plugin: a sidebar-footer QR-code button that lets a phone scan and re-issue the current browser's authenticated launch URL. |
| 1291 | [XIAOke8698/dsh-memory-forget](https://github.com/XIAOke8698/dsh-memory-forget) | 1 | 2026-08-23 | 2026-08-23 | Forgetting engine for AI agents — memory TTL, decay, eviction, audit. The opposite of memory programming. DSH plugin + local skill + CLI. |
| 1292 | [XiaoluoFoxington/dsh-theme-hacker-terminal](https://github.com/XiaoluoFoxington/dsh-theme-hacker-terminal) | 1 | 2026-08-24 | 2026-08-24 | Hacker-terminal skin for the dsh web GUI: pure black, high-contrast green, right-angle geometry, monospace font, full-width conversation, OLED-safe, scrollbars on Gecko/Blink/WebKit. |
| 1293 | [xiaoshi7915/dsh-kb-manager](https://github.com/xiaoshi7915/dsh-kb-manager) | 1 | 2026-08-27 | 2026-08-27 | DSH local knowledge base plugin: multi-format import, smart chunking, vector index, hybrid search (BM25 + sqlite-vec + RRF) for agent long-term memory |
| 1294 | [xiaoshi7915/dsh-memory-manager](https://github.com/xiaoshi7915/dsh-memory-manager) | 1 | 2026-08-25 | 2026-08-26 | A unified memory management layer |
| 1295 | [XiaoWind/dsh-cron](https://github.com/XiaoWind/dsh-cron) | 1 | 2026-08-21 | 2026-08-22 | DeepSeek Harness plugin: a /cron slash command for cron-scheduled recurring agent loops |
| 1296 | [xiaxi626/dsh-skills-nexus](https://github.com/xiaxi626/dsh-skills-nexus) | 1 | 2026-08-22 | 2026-08-22 | Universal DSH skill adapter. Install once, then register any GitHub repo containing a SKILL.md as a DSH skill — one command per repo. No Cordis plugin code or package.json needed in the skill repo. |
| 1297 | [Xichun123/dsh-relay-models](https://github.com/Xichun123/dsh-relay-models) | 1 | 2026-08-14 | 2026-08-29 | Mixed-protocol relay model discovery, metadata matching, and Web configuration for DeepSeek Harness |
| 1298 | [xie-tj/dsh-subagent](https://github.com/xie-tj/dsh-subagent) | 1 | 2026-08-24 | 2026-08-24 | Named subagent profiles with configurable model routing and reasoning for DeepSeek Harness |
| 1299 | [Xinlong-Wu/dsh-auto-review](https://github.com/Xinlong-Wu/dsh-auto-review) | 1 | 2026-08-20 | 2026-08-24 | adds an auto-review permission preset to DeepSeek Harness. Same Codex auto review |
| 1300 | [xipian1216/dsh-aa-bridge](https://github.com/xipian1216/dsh-aa-bridge) | 1 | 2026-08-17 | 2026-08-31 | Agents Anywhere bridge and Web status plugin for DeepSeek Harness |
| 1301 | [xiuyuan18/dsh-engram-session](https://github.com/xiuyuan18/dsh-engram-session) | 1 | 2026-08-23 | 2026-08-23 | Unofficial community plugin: per-session Engram memory for DeepSeek Harness — spawns an engram MCP child per agent session rooted at the session workspace, registers mem_* tools per agent scope, and injects the Memory Protocol as a system-prompt section. |
| 1302 | [xiyunSacire/dsh-skill-manager](https://github.com/xiyunSacire/dsh-skill-manager) | 1 | 2026-08-28 | 2026-08-28 |  The dsh-skill-manager is a deep-integration Web UI plugin designed to provide developers and advanced users with direct visibility and control over the true, persistent "skill memory" of DeepSeek Harness (DSH). |
| 1303 | [xjailll/dsh-portfolio-publisher](https://github.com/xjailll/dsh-portfolio-publisher) | 1 | 2026-08-29 | 2026-08-29 | DeepSeek Harness 插件：GitHub 求职仓库一键发布助手（LLM README + Web 面板 + 一键推送） |
| 1304 | [xmnathan/dsh-skin-galactic-opera](https://github.com/xmnathan/dsh-skin-galactic-opera) | 1 | 2026-08-27 | 2026-08-27 | Unofficial cinematic space-opera dark skin bundle for the DSH Web GUI. |
| 1305 | [XSakura666/dsh-plugin-ChronoAgent](https://github.com/XSakura666/dsh-plugin-ChronoAgent) | 1 | 2026-08-15 | 2026-08-27 | Local-first desktop app that schedules AI agent tasks like cron jobs — zero token cost until they run. Write a task, set a time, and it runs automatically with files, web, MCP tools, and multi-model support.      |
| 1306 | [xtd1145/dsh-full-access-switch](https://github.com/xtd1145/dsh-full-access-switch) | 1 | 2026-08-23 | 2026-08-24 | DSH one-time Full access switch: no per-session confirmation for new workspaces/conversations |
| 1307 | [xuan666-lab/dsh-openrouter-provider-advisor](https://github.com/xuan666-lab/dsh-openrouter-provider-advisor) | 1 | 2026-08-24 | 2026-08-24 | DSH plugin that ranks OpenRouter providers by cost, speed, context, and reliability, then switches the active route. |
| 1308 | [xuanyuanluoxue/computer-use-vision](https://github.com/xuanyuanluoxue/computer-use-vision) | 1 | 2026-08-22 | 2026-08-22 | Windows computer-use capability for DSH: screenshot, vision, simulated input, self-evolving knowledge base. Plugin + skill dual-mode. |
| 1309 | [xuc865/dsh-librarian](https://github.com/xuc865/dsh-librarian) | 1 | 2026-08-23 | 2026-08-24 | a dsh plugin that helps you to automatically generate, evolve and manage your dsh plugins |
| 1310 | [yafangwang9/dsh-voice-plugin](https://github.com/yafangwang9/dsh-voice-plugin) | 1 | 2026-08-24 | 2026-08-24 | Voice input plugin for DeepSeek Harness |
| 1311 | [yakoylp/dsh-md-convert](https://github.com/yakoylp/dsh-md-convert) | 1 | 2026-08-28 | 2026-08-28 | Convert Office documents and PDFs (incl. scanned, via CPU-first routing OCR with lightweight models: PP-DocLayout-L layout, RapidOCR text, SLANet tables, FormulaNet formulas) to structurally-formatted Markdown. CLI + dsh agent tool (md_convert). |
| 1312 | [yangbobo2021/relay-dsh-plugin-manager](https://github.com/yangbobo2021/relay-dsh-plugin-manager) | 1 | 2026-08-26 | 2026-08-26 | A standalone plugin manager for DeepSeek Harness. |
| 1313 | [yangdongzhen590/dsh-knj-menu](https://github.com/yangdongzhen590/dsh-knj-menu) | 1 | 2026-08-23 | 2026-08-24 | Third-party menu manager for DeepSeek Harness: collects plugin menu entries with fold/collapse and pinned items. |
| 1314 | [yanglingrise/dsh-erii-boot-splash](https://github.com/yanglingrise/dsh-erii-boot-splash) | 1 | 2026-08-22 | 2026-08-22 | Erii (Sakura) themed boot splash animation for the DeepSeek Harness Web UI: falling sakura petals, a mint monster mascot, and the line "Sakura, walk slower." Auto fades out; pure client-side. |
| 1315 | [yangwuan55/dsh-feishu-integration](https://github.com/yangwuan55/dsh-feishu-integration) | 1 | 2026-08-24 | 2026-08-24 | Bidirectional Feishu/Lark integration for DeepSeek Harness: summaries, reply routing, binding UI, and QR provisioning. |
| 1316 | [yaopushen/dsh-plugin-background-tasks](https://github.com/yaopushen/dsh-plugin-background-tasks) | 1 | 2026-08-23 | 2026-08-24 | Antigravity-style run_command for DeepSeek Harness: 10s sync window, auto background promotion, completion reports |
| 1317 | [Ycet/dsh-awesome-hud](https://github.com/Ycet/dsh-awesome-hud) | 1 | 2026-08-29 | 2026-08-30 | dsh侧边HUD面板，包含多个信息展示模块（可自定义是否展示），集成压缩上下文、查看git graph等功能。DSH side HUD panel, containing multiple information display modules (customizable whether to display), integrating features such as compressed context, viewing git graph, etc. |
| 1318 | [Ycet/dsh-session-plus](https://github.com/Ycet/dsh-session-plus) | 1 | 2026-08-24 | 2026-08-25 | DSH 会话增强插件：一键打开工作区 · 模型提供商菜单头部 · 选中文本加入对话 / DSH session enhancement plugin: open workspace · provider header · add selected text to conversation |
| 1319 | [yejiming/dsh-ppt](https://github.com/yejiming/dsh-ppt) | 1 | 2026-08-25 | 2026-08-26 | PPT design preset and editable PPTX production tools for DeepSeek Harness |
| 1320 | [yhbd-top/dsh-plugin-top](https://github.com/yhbd-top/dsh-plugin-top) | 1 | 2026-08-29 | 2026-08-29 | yhbd.top 插件雷达 for DeepSeek Harness：侧边栏大面板浏览 3900+ 插件目录（搜索 / 22 分类 / 站点同款五榜单 / 榜单联动分类），安装引导语一键写入会话输入框；进程内同源反代，零配置；附带 Agent 可调用的搜索与榜单工具。 |
| 1321 | [YINGCHAO-98/dsh-private-plugins](https://github.com/YINGCHAO-98/dsh-private-plugins) | 1 | 2026-08-25 | 2026-08-26 | 在 DeepSeek Harness Web 设置中统一导入、启用、更新和管理本地及云端私有插件。 |
| 1322 | [yingzaicc/dsh-editor-selection-vscode](https://github.com/yingzaicc/dsh-editor-selection-vscode) | 1 | 2026-08-23 | 2026-08-23 | DSH 编辑器选区桥接扩展:把 VS Code 的主选区(路径+行区间,不含任何文件内容)推送给本地 DeepSeek Harness,使对话自动聚焦你正在看的代码。 |
| 1323 | [yingzaicc/dsh-gitland](https://github.com/yingzaicc/dsh-gitland) | 1 | 2026-08-23 | 2026-08-23 | DeepSeek Harness（DSH）的 Git 面板插件：在 Web GUI 中呈现 GoLand 风格的 Git 工具窗口 —— 提交日志时间线（彩色泳道图）、分支管理、worktree 管理，以及工作区状态摘要，并支持简单的 分支/worktree 操作。 |
| 1324 | [yishengdaxiaonengjihui/dsh-poor-router](https://github.com/yishengdaxiaonengjihui/dsh-poor-router) | 1 | 2026-08-26 | 2026-08-26 | Budget-LLM pool router for DeepSeek Harness: ledger, health tracking, Thompson-sampling failover across free-tier models. 穷鬼路由器 |
| 1325 | [yj-liuzepeng/dsh-project-brain](https://github.com/yj-liuzepeng/dsh-project-brain) | 1 | 2026-08-30 | 2026-08-30 | Persistent project intelligence and memory plugin for DSH: architecture analysis, cross-session context, TODOs, and optional hybrid retrieval |
| 1326 | [YJLTF/dsh-plugin-offline-packager](https://github.com/YJLTF/dsh-plugin-offline-packager) | 1 | 2026-08-25 | 2026-08-25 | DeepSeek Harness 离线打包插件 — 在联网环境下将 DSH 插件打包为离线安装包（.tgz），传输到离线 DSH 环境中加载安装。 |
| 1327 | [ylxmf2005/dsh-openai-server-compaction](https://github.com/ylxmf2005/dsh-openai-server-compaction) | 1 | 2026-08-21 | 2026-08-22 | OpenAI Responses adapter with durable server-side compaction for DeepSeek Harness. |
| 1328 | [ynnmuraii/dsh-sandbox](https://github.com/ynnmuraii/dsh-sandbox) | 1 | 2026-08-22 | 2026-08-26 | dsh-lab meta-repo: plugin laboratory for DeepSeek Harness (workbench, template, catalog) |
| 1329 | [yongshuai0314/dsh-i-have-adhd](https://github.com/yongshuai0314/dsh-i-have-adhd) | 1 | 2026-08-26 | 2026-08-26 | ADHD-friendly output shaping for DeepSeek Harness: one system-prompt section with adhd_on/adhd_off/adhd_status tools, persisted across restarts. Inspired by ayghri/i-have-adhd (MIT). |
| 1330 | [yoshino-xiao7/dsh-grok-provider](https://github.com/yoshino-xiao7/dsh-grok-provider) | 1 | 2026-08-26 | 2026-08-26 | DeepSeek Harness 的社区 Grok Build Provider：官方 CLI 浏览器 OAuth、动态模型、流式工具调用与额度面板。Community Grok Build provider with official CLI OAuth, dynamic models, streaming tools, and a quota dashboard. |
| 1331 | [yth1120/deepseek-harness](https://github.com/yth1120/deepseek-harness) | 1 | 2026-08-23 | 2026-08-23 | DeepSeek Harness source with the dsh-web-workbench plugin suite (right workbench, terminal, timeline, review, files and browser preview). |
| 1332 | [yuan-source-666/dsh-github-manager](https://github.com/yuan-source-666/dsh-github-manager) | 1 | 2026-08-27 | 2026-08-27 | GitHub 仓库 AI 自动管理通道插件 (DeepSeek Harness community bundle): 27 个工具（仓库/Issue/PR/分支/文件/标签/话题/Tags/Releases/搜索）+ Web 设置卡片 + dry-run 防护 + secret 令牌。 |
| 1333 | [yuan-source-666/dsh-research-autoresearch](https://github.com/yuan-source-666/dsh-research-autoresearch) | 1 | 2026-08-27 | 2026-08-27 | AutoResearch 科研协议 DSH 全家桶插件：arXiv recall + LQS 评分 + 状态持久化 + 停滞红绿灯 + 五人格中位数评审 + 可视化总控台卡片。灵感：Deli Chen "From Draft to Strong-Accept: How a Self-Play Survey Hit 8.6"。 |
| 1334 | [yuan-source-666/dsh-task-notifier](https://github.com/yuan-source-666/dsh-task-notifier) | 1 | 2026-08-28 | 2026-08-28 | DeepSeek Harness community plugin: OS notification when a turn, subagent, background job, goal, or workflow finishes. Localized wording, per-source switches, custom delivery command. npm: dsh-task-notifier |
| 1335 | [yumm007/dsh-reveal-files](https://github.com/yumm007/dsh-reveal-files) | 1 | 2026-08-23 | 2026-08-24 | A dual-face DeepSeek Harness plugin that adds a folder icon next to the "Produces" row |
| 1336 | [YunlongL-byte/dsh-launcher](https://github.com/YunlongL-byte/dsh-launcher) | 1 | 2026-08-22 | 2026-08-22 | macOS 程序坞一键启动 DeepSeek Harness (DSH) 的快捷启动器 / One-click DSH launcher for macOS Dock |
| 1337 | [yunniees/DSH-Plugin-Manager](https://github.com/yunniees/DSH-Plugin-Manager) | 1 | 2026-08-28 | 2026-08-28 | Visual plugin manager for DeepSeek Harness: AI auto-translation, AI one-click summaries, AI plugin search, one-click share & install of multiple plugins, bulk updates |
| 1338 | [YupegLV/dsh-chat-log](https://github.com/YupegLV/dsh-chat-log) | 1 | 2026-08-25 | 2026-08-25 | Fold DSH session logs into clean chat logs: stream fragments merged, nothing else dropped. /chat + browser download.  把 DSH 会话日志折叠成聊天记录：流式碎片合并，其余内容一行不丢。/chat 命令 + 浏览器下载。 |
| 1339 | [Yur0918/dsh-user-addons](https://github.com/Yur0918/dsh-user-addons) | 1 | 2026-08-28 | 2026-08-28 | Community DSH web plugin for file uploads, archived-session management, image capability detection, and model/token usage insights. |
| 1340 | [yushi-javatoai/ai-web-ppt-maker](https://github.com/yushi-javatoai/ai-web-ppt-maker) | 1 | 2026-08-31 | 2026-08-31 | AI 网页 PPT 生成器：粘贴长文案，AI 流式拆解为多页网页 PPT，支持全屏演示、键盘翻页、多套主题与独立 HTML 导出。 |
| 1341 | [yushuosun/dsh-cost-governor](https://github.com/yushuosun/dsh-cost-governor) | 1 | 2026-08-22 | 2026-08-22 | Cost governance & budget enforcement for DeepSeek Harness: per-model token-cost accounting, multi-provider pricing, budget warn thresholds, and a usage dashboard. |
| 1342 | [yx222yx/DSH-Feedback-Bridge](https://github.com/yx222yx/DSH-Feedback-Bridge) | 1 | 2026-08-29 | 2026-08-30 | 一个 DeepSeek Harness 插件，帮助用户将功能想法和错误反馈整理为清晰、注重隐私的 GitHub Discussions。A DeepSeek Harness plugin that helps users turn ideas and bug reports into clear, privacy-aware GitHub Discussions. |
| 1343 | [yxie2/dsh-petrinet](https://github.com/yxie2/dsh-petrinet) | 1 | 2026-08-24 | 2026-08-24 | Workflow-net runtime for DeepSeek Harness: resource-aware concurrency, native loops and fan-out, static soundness checking before a plan becomes durable, and process mining over its own event log. |
| 1344 | [yyyq0325-ai/dsh-webgate](https://github.com/yyyq0325-ai/dsh-webgate) | 1 | 2026-08-22 | 2026-08-26 | 为 DeepSeek Harness 的 Web GUI 加一道账号密码门：每次打开 DSH Web 都必须先登录；登录令牌有效期 12 小时；令牌过期被登出时，后台正在运行的任务完全不受影响，重新登录后一切还在。 |
| 1345 | [yztdtf/dsh-worktable-pet](https://github.com/yztdtf/dsh-worktable-pet) | 1 | 2026-08-27 | 2026-08-27 | DeepSeek Harness ??????????(Dynamic Cordis Plugin) |
| 1346 | [Zara-Siwei/dsh-float](https://github.com/Zara-Siwei/dsh-float) | 1 | 2026-08-26 | 2026-08-27 | Floating minimal-mode DeepSeek Harness (dsh) plugin: a transparent terminal TUI over dsh web in a borderless Electron window. |
| 1347 | [zergtant/dsh-remote-access](https://github.com/zergtant/dsh-remote-access) | 1 | 2026-08-23 | 2026-08-24 | DeepSeek Harness (dsh) 远程访问插件：提供 TLS、登录认证、会话保护和 HTTP/WebSocket 透明反代，支持局域网及 FRP ，cloudflare隧道等远程访问。 |
| 1348 | [zhaimingyou/dsh.plus](https://github.com/zhaimingyou/dsh.plus) | 1 | 2026-08-25 | 2026-08-25 | DSH plugin that shows the dsh.plus curated plugin catalog inside DeepSeek Harness |
| 1349 | [zhangyqjiaoshou-oss/dsh-model-sync](https://github.com/zhangyqjiaoshou-oss/dsh-model-sync) | 1 | 2026-08-29 | 2026-08-29 | One-click / auto model sync for DeepSeek Harness providers |
| 1350 | [Zhanxueyou/deepseek-balance](https://github.com/Zhanxueyou/deepseek-balance) | 1 | 2026-08-30 | 2026-08-30 | 零依赖 Python CLI 查询 DeepSeek API 余额，低余额自动提醒并发送 macOS 通知；附带 DSH 侧边栏插件，实时展示余额、今日/本月用量与缓存命中率。 |
| 1351 | [Zhanxueyou/dsh-plugin-manager](https://github.com/Zhanxueyou/dsh-plugin-manager) | 1 | 2026-08-30 | 2026-08-30 | DSH Web 客户端插件管理器侧边栏面板：全量插件清单（描述/状态/来源/版本/分类）、启停热重载、删除本地自定义插件，并可浏览、搜索、一键安装 GitHub topic:dsh-plugin 远程插件。 |
| 1352 | [zhaoxuejie/dsh-daily-digest](https://github.com/zhaoxuejie/dsh-daily-digest) | 1 | 2026-08-27 | 2026-08-27 | DSH 每日工作摘要插件：自动记录任务/会话/错误，一键生成日报/周报 Markdown，Web 悬浮摘要卡 |
| 1353 | [zhaoxuejie/dsh-plugin-learning-path](https://github.com/zhaoxuejie/dsh-plugin-learning-path) | 1 | 2026-08-21 | 2026-08-27 | DeepSeek Harness 插件开发学习教程：15 节课程 + 4 个实战项目 + 发布课，交互式单页应用，纯 HTML/CSS/JS 零构建 |
| 1354 | [zheng16965/dsh-deliverables-toggle](https://github.com/zheng16965/dsh-deliverables-toggle) | 1 | 2026-08-24 | 2026-08-24 | 为 DeepSeek Harness 对话产物列表增加主动展开与收起功能的 Web UI 插件。 |
| 1355 | [zhengjy01/dsh-cubox](https://github.com/zhengjy01/dsh-cubox) | 1 | 2026-08-23 | 2026-08-23 | Cubox sync plugin for DeepSeek Harness: scheduled sync, AI daily brief from your prompt template into Obsidian, per-card markdown export — via the /c/api/cli endpoints |
| 1356 | [Zhiyi-Zhao/dsh-notion-skill](https://github.com/Zhiyi-Zhao/dsh-notion-skill) | 1 | 2026-08-27 | 2026-08-27 | DSH (DeepSeek Harness) skill: read/write Notion workspaces via the official REST API |
| 1357 | [Zhiyi-Zhao/file-brief](https://github.com/Zhiyi-Zhao/file-brief) | 1 | 2026-07-30 | 2026-08-27 | Task-local, privacy-preserving file catalogs for reusable Codex input-file understanding. |
| 1358 | [zhongjie10086/dsh-adaptive-native](https://github.com/zhongjie10086/dsh-adaptive-native) | 1 | 2026-08-16 | 2026-08-30 | Windows-native Adaptive preset for DeepSeek Harness |
| 1359 | [zhoupengyun572-cell/dsh-hana-research](https://github.com/zhoupengyun572-cell/dsh-hana-research) | 1 | 2026-08-28 | 2026-08-28 | A local literature review, PDF annotation, evidence synthesis, and research notes workbench for DeepSeek Harness. |
| 1360 | [zhubaohi/dsh-qwen38-compaction-fix](https://github.com/zhubaohi/dsh-qwen38-compaction-fix) | 1 | 2026-08-25 | 2026-08-25 | DSH plugin: stop qwen3.8-27b from burning its output budget on thinking during context compaction |
| 1361 | [ZhuoSir/dsh-cron](https://github.com/ZhuoSir/dsh-cron) | 1 | 2026-08-22 | 2026-08-22 | DeepSeek Harness 定时任务插件：对话中自然语言创建，到点自动执行并在会话中回复，支持 cron 表达式与 Web 管理面板 |
| 1362 | [zhuzhujunandy/dsh-model-router](https://github.com/zhuzhujunandy/dsh-model-router) | 1 | 2026-08-23 | 2026-08-23 | Tiered model routing plugin for DeepSeek Harness (DSH): route delegated work to fast/medium/heavy model tiers with DoD verification, cross-provider fallback, background delegation, and per-conversation budget modes. |
| 1363 | [zhuzichen362/dsh-call-shrink](https://github.com/zhuzichen362/dsh-call-shrink) | 1 | 2026-08-29 | 2026-08-29 | dsh |
| 1364 | [zjh02249/dsh-desktop-operator](https://github.com/zjh02249/dsh-desktop-operator) | 1 | 2026-08-27 | 2026-08-27 | DSH Desktop Operator: safe Windows Computer Use, desktop automation, UI Automation, and MCP tools for DeepSeek Harness |
| 1365 | [zjuhbh/dsh-full-with-approval](https://github.com/zjuhbh/dsh-full-with-approval) | 1 | 2026-08-22 | 2026-08-23 | DSH profile plugin: full-access (GPU-capable) sandbox with per-operation approval for writes outside the workspace or to protected files. |
| 1366 | [Zleap-AI/dsh-sag](https://github.com/Zleap-AI/dsh-sag) | 1 | 2026-08-29 | 2026-08-29 | 面向 DeepSeek Harness 的 SAG 本地个人知识库插件，支持知识检索、原文读取、文件上传、文本写入与文档管理。 |
| 1367 | [Zn-Dk/dsh-session-explorer](https://github.com/Zn-Dk/dsh-session-explorer) | 1 | 2026-08-24 | 2026-08-25 | DSH Web plugin: message-level full-text search + timeline visualization for sessions. |
| 1368 | [ZnFr60/dsh-lan-access-for-rpi-os-or-debian](https://github.com/ZnFr60/dsh-lan-access-for-rpi-os-or-debian) | 1 | 2026-08-26 | 2026-08-26 | Raspberry Pi 64-bit (aarch64) LAN access + boot auto-start installer for the DeepSeek Harness (dsh) Web UI: phone/LAN devices control dsh from a browser (0.0.0.0 bind, /api trust fence, crypto.randomUUID polyfill, privileged-API fix, systemd auto-start). |
| 1369 | [ZnFr60/dsh-lan-access-for-windows](https://github.com/ZnFr60/dsh-lan-access-for-windows) | 1 | 2026-08-25 | 2026-08-26 | DeepSeek Harness LAN-access bundle plugin: bind dsh web to 0.0.0.0 + crypto.randomUUID secure-context shim for phone browsers. |
| 1370 | [zoumutou/dsh-attachment-downscale](https://github.com/zoumutou/dsh-attachment-downscale) | 1 | 2026-08-22 | 2026-08-22 | DSH 插件：图片附件超限自动降级（2000px / 3.5MB / 4000万像素） |
| 1371 | [ZPA76/deepseek-pa-dsh-desktop](https://github.com/ZPA76/deepseek-pa-dsh-desktop) | 1 | 2026-08-26 | 2026-08-26 | DeepSeek-PA（DPA）是基于 DeepSeek Harness（DSH）构建的非官方模块化桌面工作台，提供独立的 Chat 与 Agent 空间、插件与 Skill 扩展、全局主题，以及可监督的多智能体集群项目。Unofficial modular desktop workspace for DeepSeek Harness (DSH), featuring separate Chat and Agent views, plugins, Skills, global themes, and supervised multi-agent projects. |
| 1372 | [ztting01/dsh-agentenv-sandbox](https://github.com/ztting01/dsh-agentenv-sandbox) | 1 | 2026-08-24 | 2026-08-25 | AgentENV/E2B microVM execution-world bundle for DeepSeek Harness |
| 1373 | [ZutoMayoo/totoTheCat](https://github.com/ZutoMayoo/totoTheCat) | 1 | 2026-08-20 | 2026-08-22 | 在你的DeepSeek Harness中加入桌宠小猫托托的插件 |
| 1374 | [zw11591-sketch/dsh-pet-panel](https://github.com/zw11591-sketch/dsh-pet-panel) | 1 | 2026-08-28 | 2026-08-28 | A desktop pet plus a conversation overview panel for the DeepSeek Harness Web UI — self-contained client plugin (no host service) |
| 1375 | [zzj8442-blip/dsh-mobile-remote](https://github.com/zzj8442-blip/dsh-mobile-remote) | 1 | 2026-08-24 | 2026-08-24 | 📡 手机远程遥控 DeepSeek Harness：实时进度 / 审批 / 对话（PWA + PIN 配对 + Tailscale 外网支持） |
| 1376 | [zzy-12345678/dsh-file-convert](https://github.com/zzy-12345678/dsh-file-convert) | 1 | 2026-08-29 | 2026-08-30 | Local-first file conversion for DeepSeek Harness — images, PDF, data, audio/video & office docs. 7 tools, 26 conversions, no API keys, no uploads. |
| 1377 | [ZZZjf13960/dsh-onfail](https://github.com/ZZZjf13960/dsh-onfail) | 1 | 2026-08-28 | 2026-08-28 | DSH plugin: poll GitHub Actions, surface failed checks as cards, open a fix session with log context. |
| 1378 | [0N3-0/dsh-tui-mcp-manager](https://github.com/0N3-0/dsh-tui-mcp-manager) | 0 | 2026-08-25 | 2026-08-25 |   面向 dsh-TUI 的原生 MCP Server 管理插件：通过 /mcp-manager 浮窗完成 MCP CRUD、启停、Sets、复制、Inspector、Tool schema、Doctor Lite 和凭据引用管理，并将配   置原子写入当前 profile，支持 Cordis HMR 热重载。 |
| 1379 | [0w0miki/dsh-question-rail](https://github.com/0w0miki/dsh-question-rail) | 0 | 2026-08-23 | 2026-08-24 | 给Deepseek Harness滚动条加上提问节点 |
| 1380 | [0xrushmoon/dsh-plugin](https://github.com/0xrushmoon/dsh-plugin) | 0 | 2026-08-24 | 2026-08-24 | dsh-plugin |
| 1381 | [1-CellBio/dsh-okf](https://github.com/1-CellBio/dsh-okf) | 0 | 2026-08-19 | 2026-08-22 | DeepSeek Harness plugin: turn research PDFs into a citable OKF markdown library, with full-text & semantic search, knowledge graph, and survey writing. |
| 1382 | [12398k/dsh-opencode-go-dashboard](https://github.com/12398k/dsh-opencode-go-dashboard) | 0 | 2026-08-24 | 2026-08-24 | dsh-opencode-go-dashboard |
| 1383 | [123twtd/dsh-plugin-manager](https://github.com/123twtd/dsh-plugin-manager) | 0 | 2026-08-29 | 2026-08-29 | Independent DSH plugin inventory and transactional Profile manager. |
| 1384 | [142gg-GZX/unity-dsh-bridge](https://github.com/142gg-GZX/unity-dsh-bridge) | 0 | 2026-08-25 | 2026-08-25 | DSH plugin: control Unity / Tuanjie editor over a local HTTP bridge — build scenes, write C#, compile, play, screenshot, simulate input. |
| 1385 | [162568316/dsh-tokenrhythm-bill](https://github.com/162568316/dsh-tokenrhythm-bill) | 0 | 2026-08-31 | 2026-08-31 | dsh-tokenrhythm-bill |
| 1386 | [18126295767-cell/dsh-mac-control](https://github.com/18126295767-cell/dsh-mac-control) | 0 | 2026-08-19 | 2026-08-22 | Give DeepSeek Harness hands on your Mac: native browser and desktop control tools for macOS. |
| 1387 | [1clickreport/dsh-1clickreport](https://github.com/1clickreport/dsh-1clickreport) | 0 | 2026-08-22 | 2026-08-23 | Connect your marketing data (Google Ads, Meta, GA4, Search Console, Shopify, Stripe) to DeepSeek Harness via MCP |
| 1388 | [1Ecc/dsh-lenovo-toolkit](https://github.com/1Ecc/dsh-lenovo-toolkit) | 0 | 2026-08-28 | 2026-08-28 | 联想专业工具集 · DeepSeek Harness 插件。电池健康检测（macOS/Windows）：容量、循环次数、双口径健康度、SVG 衰减趋势图与系统官方电池报告。Lenovo professional toolkit for DeepSeek Harness. |
| 1389 | [2017java/dsh-md-overlay](https://github.com/2017java/dsh-md-overlay) | 0 | 2026-08-24 | 2026-08-26 | DSH web 插件：可悬浮 / 可停靠的多标签 Markdown 预览面板 + md_preview 模型工具，会话里一键预览报告。 |
| 1390 | [2017java/dsh-md-viewer](https://github.com/2017java/dsh-md-viewer) | 0 | 2026-08-24 | 2026-08-26 | DSH web 插件：在 dsh-better-sidebar 侧边栏内把 Markdown 富渲染为预览（代码高亮 / 目录 / 一键复制）。 |
| 1391 | [2877905731/dsh-think-autoexpand](https://github.com/2877905731/dsh-think-autoexpand) | 0 | 2026-08-27 | 2026-08-27 | dsh-think-autoexpand：让 DeepSeek Harness 里的 Think 思考行始终可见，并在流式输出时自动展开，实时查看 Agent 完整推理过程；保留工具卡折叠体验。 |
| 1392 | [452926826/dsh-feishu-bot](https://github.com/452926826/dsh-feishu-bot) | 0 | 2026-08-25 | 2026-08-26 | Connect a Feishu bot to DeepSeek Harness projects and conversations |
| 1393 | [618527/dsh-install-guard](https://github.com/618527/dsh-install-guard) | 0 | 2026-08-30 | 2026-08-30 | DSH 插件安装前兼容性预检守卫：检查 Node/engines、@deepseek-ai peer 版本与 dsh 清单，可选隔离试启动。 |
| 1394 | [666emmm/dsh-file-upload](https://github.com/666emmm/dsh-file-upload) | 0 | 2026-08-31 | 2026-08-31 | dsh-file-upload fork: uploaded-file management (list/info/delete/@path) + zero-copy clipboard path reading for DeepSeek Harness |
| 1395 | [6jeffr3y/dsh-burpsuite-mcp](https://github.com/6jeffr3y/dsh-burpsuite-mcp) | 0 | 2026-08-30 | 2026-08-30 | Native Burp Suite MCP tools and live settings for DeepSeek Harness |
| 1396 | [6jeffr3y/dsh-session-manager](https://github.com/6jeffr3y/dsh-session-manager) | 0 | 2026-08-30 | 2026-08-30 | Session archive, tagging, relationship graph and safe deletion for DeepSeek Harness Web |
| 1397 | [988hj7tczd-oss/dsh-math-olympiad](https://github.com/988hj7tczd-oss/dsh-math-olympiad) | 0 | 2026-08-24 | 2026-08-24 | DSH skill bundle: competition math (IMO/Putnam/USAMO/AIME) solved with pure reasoning, adversarial verification in a fresh subagent, and calibrated confidence |
| 1398 | [988hj7tczd-oss/dsh-skill-creator](https://github.com/988hj7tczd-oss/dsh-skill-creator) | 0 | 2026-08-24 | 2026-08-24 | One-shot DSH skill (SKILL.md) generator: capture intent, draft, validate, package and distribute skills from inside a DeepSeek Harness session |
| 1399 | [988hj7tczd-oss/harness-github](https://github.com/988hj7tczd-oss/harness-github) | 0 | 2026-08-23 | 2026-08-26 | DeepSeek Harness GitHub plugin: review PRs, triage issues, debug Actions CI, handle incoming GitHub events (webhooks + polling) via dsh-native tools. |
| 1400 | [a1303845406/dsh-comfy-video-studio](https://github.com/a1303845406/dsh-comfy-video-studio) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness 的 ComfyUI MiniMax H3 视频工作台 |
| 1401 | [a1303845406/dsh-sakura-theme](https://github.com/a1303845406/dsh-sakura-theme) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness 的晴樱与夜樱主题插件 |
| 1402 | [a805026135/dsh-constellation](https://github.com/a805026135/dsh-constellation) | 0 | 2026-08-25 | 2026-08-25 | A live, self-organizing constellation map of your DeepSeek Harness plugin universe — AI-balanced taxonomy, bilingual labels, instant search, health diagnostics, and one-click plugin operations. |
| 1403 | [aa2246740/dsh-cuadrive-mac](https://github.com/aa2246740/dsh-cuadrive-mac) | 0 | 2026-08-20 | 2026-08-25 | macOS-only DeepSeek Harness plugin: private cua-driver computer-use for DSH |
| 1404 | [aa2246740/dsh-files-panel](https://github.com/aa2246740/dsh-files-panel) | 0 | 2026-08-18 | 2026-08-25 | Community DeepSeek Harness plugin: right-side workspace file tree. Does not patch DSH core. |
| 1405 | [aa2246740/dsh-grok-plan-mode](https://github.com/aa2246740/dsh-grok-plan-mode) | 0 | 2026-08-21 | 2026-08-25 | Full Grok Build Plan Mode port for DeepSeek Harness. Replaces official DSH Plan with Grok's state machine, plan.md edit gate, enter/exit tools, and review surface. |
| 1406 | [aa2246740/dsh-image-conatiner](https://github.com/aa2246740/dsh-image-conatiner) | 0 | 2026-08-19 | 2026-08-25 | Codex-style generated-image gallery and lightbox for DeepSeek Harness |
| 1407 | [aa2246740/dsh-resume](https://github.com/aa2246740/dsh-resume) | 0 | 2026-08-20 | 2026-08-25 | Continue Codex, Claude Code, and Cursor work in DeepSeek Harness |
| 1408 | [aa2246740/pstack-dsh](https://github.com/aa2246740/pstack-dsh) | 0 | 2026-08-25 | 2026-08-25 | DeepSeek Harness port of official pstack. Playbooks and principles are poteto's; only the harness call layer is rewritten. |
| 1409 | [aalvsz/dsh-hermes-bridge](https://github.com/aalvsz/dsh-hermes-bridge) | 0 | 2026-08-27 | 2026-08-27 | Literal Hermes Agent → DeepSeek Harness bridge: shared memory, skills, live tools, MCP, and full-agent delegation. |
| 1410 | [ABccgh/dsh-desktop-dev](https://github.com/ABccgh/dsh-desktop-dev) | 0 | 2026-08-29 | 2026-08-29 | DeepSeek Harness agent preset: Windows full-stack desktop development team |
| 1411 | [Aclypea/dsh-repetition-guard](https://github.com/Aclypea/dsh-repetition-guard) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness (DSH) 模型输出复读熔断插件 / Repetition guard plugin for DeepSeek Harness |
| 1412 | [ADDD1118/dsh-update](https://github.com/ADDD1118/dsh-update) | 0 | 2026-08-22 | 2026-08-22 | DeepSeek Harness (dsh) check-for-updates plugin — 右上角检查更新 UI + 关闭后自动升级 (npm / update-dsh.ps1) |
| 1413 | [adoreQ/deepseek-balance](https://github.com/adoreQ/deepseek-balance) | 0 | 2026-08-29 | 2026-08-29 | deepseek harness查看余额插件 |
| 1414 | [adrianleb/dsh-tmux-cc](https://github.com/adrianleb/dsh-tmux-cc) | 0 | 2026-08-25 | 2026-08-26 | A persistent, responsive tmux control-mode cockpit for DeepSeek Harness Web. |
| 1415 | [Aetheri-AI/dsh-plugins](https://github.com/Aetheri-AI/dsh-plugins) | 0 | 2026-08-29 | 2026-08-29 | Community plugins for DeepSeek Harness (dsh) |
| 1416 | [AFAP/dsh-trajectory-traceview](https://github.com/AFAP/dsh-trajectory-traceview) | 0 | 2026-08-26 | 2026-08-26 | 轨迹视图插件：把 DeepSeek Harness Web GUI 会话的 AI 执行流程渲染为可回放的横向时间轴（minimap / 搜索 / 回放 / 步骤与子调用详情 / 原始请求分析 / Markdown 导出）。 |
| 1417 | [AGSQ11/dsh-subagent-model-visibility](https://github.com/AGSQ11/dsh-subagent-model-visibility) | 0 | 2026-08-21 | 2026-08-22 | A small DeepSeek Harness plugin that shows the actual provider/model used by a subagent directly inside the existing native subagent tool-call row. |
| 1418 | [aiko-dsh-plugins/dsh-bid-studio](https://github.com/aiko-dsh-plugins/dsh-bid-studio) | 0 | 2026-08-29 | 2026-08-29 | Installable Bid Studio workbench for DeepSeek Harness |
| 1419 | [aiko-dsh-plugins/dsh-ontology-kernel](https://github.com/aiko-dsh-plugins/dsh-ontology-kernel) | 0 | 2026-08-29 | 2026-08-29 | Installable Ontology Kernel bundle for DeepSeek Harness |
| 1420 | [ailiasdesu/dsh-session-manager](https://github.com/ailiasdesu/dsh-session-manager) | 0 | 2026-08-28 | 2026-08-28 | DSH session migration plugin: drag-and-drop sessions between workspaces in the Web UI settings panel (auto backup/rollback, official workspaceRegistry sync) |
| 1421 | [ailreth/xiaoxiao-persona-core](https://github.com/ailreth/xiaoxiao-persona-core) | 0 | 2026-08-30 | 2026-08-31 | A persona-core injection plugin for DeepSeek Harness — an honest, boundary-aware, gentle-yet-firm AI persona; an attempt at whether AI can birth consciousness. |
| 1422 | [AIMarshallLee/dsh-mcp-orchestrator](https://github.com/AIMarshallLee/dsh-mcp-orchestrator) | 0 | 2026-08-19 | 2026-08-23 | MCP orchestration layer for DeepSeek Harness — multi-server routing, health monitoring, fallback, and tool aggregation |
| 1423 | [AIMarshallLee/dsh-obsidian-bridge](https://github.com/AIMarshallLee/dsh-obsidian-bridge) | 0 | 2026-08-18 | 2026-08-23 | Bidirectional knowledge bridge between DeepSeek Harness and Obsidian Vault — FTS5 search, draft writing, session linking |
| 1424 | [AIMarshallLee/dsh-teacher-preset](https://github.com/AIMarshallLee/dsh-teacher-preset) | 0 | 2026-08-19 | 2026-08-23 | Teacher-focused vertical industry preset for DeepSeek Harness — lesson plans, rubrics, quizzes, and teaching materials generation |
| 1425 | [aixlb/dsh-bcc](https://github.com/aixlb/dsh-bcc) | 0 | 2026-08-21 | 2026-08-22 | 包拆拆 for DeepSeek Harness: video to script/storyboard/style guide. dsh-plugin. |
| 1426 | [aiyacharley/dsh-pubmed](https://github.com/aiyacharley/dsh-pubmed) | 0 | 2026-08-27 | 2026-08-27 | 把 pubmed-mcp-server 的核心能力 移植成 DSH 原生模型工具：搜索、文章元数据、全文、引用格式化、MeSH、ID 转换等 11 个工具， 直接对接 NCBI E-utilities 与 Europe PMC REST，无需额外的 MCP 客户端配置。 |
| 1427 | [AKI2253/Sidor_Character](https://github.com/AKI2253/Sidor_Character) | 0 | 2026-08-24 | 2026-08-24 | SIDOR 人设卡 —— DeepSeek Harness 附属插件：批量导入人设卡（.persona.md / 酒馆角色卡），自由加载/更换人设，会话内即时应用 + Agent 预设持久化。 |
| 1428 | [AKUSH99/dsh-balance-chip](https://github.com/AKUSH99/dsh-balance-chip) | 0 | 2026-08-26 | 2026-08-26 | DeepSeek API balance in the DSH sidebar footer and bottom-right pill - live status dot plus amount, 60s refresh, API key stays in the local credential store |
| 1429 | [alaxrpg/dsh-chatgpt-pip](https://github.com/alaxrpg/dsh-chatgpt-pip) | 0 | 2026-08-28 | 2026-08-28 | DSH 插件：ChatGPT 画中画小窗 + 把 ChatGPT 定稿计划回流到新 DSH 对话执行 |
| 1430 | [alaxrpg/dsh-subagent-route-badges](https://github.com/alaxrpg/dsh-subagent-route-badges) | 0 | 2026-08-27 | 2026-08-27 | Display subagent provider, model, and reasoning effort badges in DeepSeek Harness |
| 1431 | [alaxrpg/dsh-vision-bridge](https://github.com/alaxrpg/dsh-vision-bridge) | 0 | 2026-08-25 | 2026-08-27 | DSH 插件：为纯文本模型提供视觉能力，支持任意 OpenAI 兼容多模态 API |
| 1432 | [Albertlsy588/dsh-shipgate](https://github.com/Albertlsy588/dsh-shipgate) | 0 | 2026-08-28 | 2026-08-28 | Local-first DSH pre-merge delivery receipt generator |
| 1433 | [alchemistwu/dsh-tool-call-guard](https://github.com/alchemistwu/dsh-tool-call-guard) | 0 | 2026-08-30 | 2026-08-31 | DSH plugin: neutralize tool calls with invalid JSON arguments on the wire — so one malformed model generation cannot brick a session against strict OpenAI-compatible servers (vLLM) |
| 1434 | [aleleppy/leppy-loop-deepseek](https://github.com/aleleppy/leppy-loop-deepseek) | 0 | 2026-08-22 | 2026-08-22 | Native Leppy Loop bundle for DeepSeek Harness |
| 1435 | [alex-dsh-plugin/open-in-vscode](https://github.com/alex-dsh-plugin/open-in-vscode) | 0 | 2026-08-24 | 2026-08-24 | DeepSeek Harness (dsh) Web 插件：工作区一键打开 VSCode，对话内文件路径点击跳转 VSCode（支持 文件:行:列） |
| 1436 | [alexchen5/research-epic-manager](https://github.com/alexchen5/research-epic-manager) | 0 | 2026-08-24 | 2026-08-31 | Agent skills for running research projects end-to-end using a plain-file epic→issues→comments tracker. |
| 1437 | [alexfengrui/dsh-client-ui-skin-real-madrid](https://github.com/alexfengrui/dsh-client-ui-skin-real-madrid) | 0 | 2026-08-25 | 2026-08-25 | Real Madrid dual-mode skin for DeepSeek Harness: Bernabeu night stadium (dark) and white-kit pinstripes (light). Unofficial fan work. |
| 1438 | [AlexKaiqi/dsh-block-to-file](https://github.com/AlexKaiqi/dsh-block-to-file) | 0 | 2026-08-17 | 2026-08-22 | simple runtime ability to map a block to file, such that bash can access |
| 1439 | [AlexKaiqi/dsh-temporary-workspace](https://github.com/AlexKaiqi/dsh-temporary-workspace) | 0 | 2026-08-18 | 2026-08-25 | Isolated temporary Workspaces for DeepSeek Harness |
| 1440 | [alexpadholol/dsh-plugin-fusion](https://github.com/alexpadholol/dsh-plugin-fusion) | 0 | 2026-08-23 | 2026-08-23 | llm自采样插件 |
| 1441 | [AlgoVaultLabs/dsh-algovault](https://github.com/AlgoVaultLabs/dsh-algovault) | 0 | 2026-08-30 | 2026-08-30 | Preconfigured DeepSeek Harness bundle for the AlgoVault MCP server — composite trade calls, market regime and cross-venue funding arbitrage as mcp__algovault__* tools. |
| 1442 | [alin-ever/dsh-plugin-autoqueue](https://github.com/alin-ever/dsh-plugin-autoqueue) | 0 | 2026-08-26 | 2026-08-27 | DeepSeek Harness 无人值守任务队列插件：丢 .md 进收件箱 → AI 自动执行 → 产出报告 |
| 1443 | [aliuguofa/dsh-traffic-light](https://github.com/aliuguofa/dsh-traffic-light) | 0 | 2026-08-24 | 2026-08-24 | 一个 DeepSeek Harness Web UI 插件：在聊天输入框区域显示一盏红 / 黄 / 绿三色信号灯，实时反映当前会话的状态，点击可查看详情。 |
| 1444 | [All3nCN/dsh-better-sidebar-N23](https://github.com/All3nCN/dsh-better-sidebar-N23) | 0 | 2026-08-31 | 2026-08-31 | DSH web plugin: complete workbench (explorer/editors/previews/terminal/git/browser/tasks) + shell refactor. Fork of omdsh-dev/DSH-better-sidebar under @all3cn scope. |
| 1445 | [AllenLogo/dsh-software-tools](https://github.com/AllenLogo/dsh-software-tools) | 0 | 2026-08-21 | 2026-08-22 | DSH 侧边栏【软件工具】管理器:勾选本机 WSL/Windows 软件工具并注入模型系统提示,随插件自带 add-software-tool 技能。Sidebar software-tools manager for DeepSeek Harness Web. |
| 1446 | [alpacachen/dsh-automation](https://github.com/alpacachen/dsh-automation) | 0 | 2026-08-30 | 2026-08-30 | Schedule and manage one-time and recurring Agent tasks in DeepSeek Harness |
| 1447 | [altuman-w/dsh-plugin-plantuml](https://github.com/altuman-w/dsh-plugin-plantuml) | 0 | 2026-08-31 | 2026-08-31 | deepseek harness plugin view plantuml |
| 1448 | [Amoss-1/routine-taskboard](https://github.com/Amoss-1/routine-taskboard) | 0 | 2026-08-27 | 2026-08-28 | Self-contained routine board plugin for DeepSeek Harness (DSH): scheduled job placards with scripts, IO artifacts, health lamps. MIT. |
| 1449 | [an4nsi/dsh-fork-view](https://github.com/an4nsi/dsh-fork-view) | 0 | 2026-08-21 | 2026-08-22 | DSH web plugin: replaces the native workspace browser in the left sidebar with a session tree in the style of pi-web by agegr. |
| 1450 | [AnakinCao/dsh-code-nav](https://github.com/AnakinCao/dsh-code-nav) | 0 | 2026-08-26 | 2026-08-26 | DSH web plugin (dsh-better-sidebar companion): code preview with per-language syntax highlighting, symbol outline navigation and in-file search |
| 1451 | [AnakinCao/dsh-md-export](https://github.com/AnakinCao/dsh-md-export) | 0 | 2026-08-26 | 2026-08-26 | DSH web plugin (dsh-better-sidebar companion): export the current .md file to standalone HTML (Mermaid inlined) or PDF - export button on the markdown toolbar |
| 1452 | [AnakinWu/DSH-plugin](https://github.com/AnakinWu/DSH-plugin) | 0 | 2026-08-30 | 2026-08-30 | Anakin‘s dsh-plugins |
| 1453 | [anaksunamu/dsh-vidfetch](https://github.com/anaksunamu/dsh-vidfetch) | 0 | 2026-08-24 | 2026-08-24 | Give your DeepSeek Harness agent an on-demand video downloader |
| 1454 | [andrepontesmelo/dsh-model-router](https://github.com/andrepontesmelo/dsh-model-router) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness plugin: virtual model routes with failover, exponential backoff, sleep windows |
| 1455 | [andrepontesmelo/dsh-suite](https://github.com/andrepontesmelo/dsh-suite) | 0 | 2026-08-27 | 2026-08-27 | The DSH productivity suite: plugins + agent skills for the DeepSeek Harness, installable in one command. |
| 1456 | [andrepontesmelo/moving-target](https://github.com/andrepontesmelo/moving-target) | 0 | 2026-08-27 | 2026-08-27 | DSH plugin: cold-start context — distills your first prompts into one goal paragraph injected into every new session |
| 1457 | [andyfan1094/dsh-minimax-usage-pro](https://github.com/andyfan1094/dsh-minimax-usage-pro) | 0 | 2026-08-21 | 2026-08-22 | DSH bundle plugin showing MiniMax Token Plan / Subscription usage in Settings. Pro edition using webServer routes (host.call is unavailable to trusted bundle plugins on DSH 0.1.0-rc.8). |
| 1458 | [AndyWipe13/dsh-session-management](https://github.com/AndyWipe13/dsh-session-management) | 0 | 2026-08-30 | 2026-08-30 | A plugin for managing sessions generated by DeepSeek Harness, allowing users to freely delete legacy sessions and supporting session import from other third-party Agents (Claude Code, Codex). |
| 1459 | [Anna-la/dsh-simplify](https://github.com/Anna-la/dsh-simplify) | 0 | 2026-08-28 | 2026-08-28 | DeepSeek Harness 界面简化插件：清理模式下右键移除页面元素，设置页中可原样恢复。 |
| 1460 | [Anna-la/dsh-submodel-change](https://github.com/Anna-la/dsh-submodel-change) | 0 | 2026-08-27 | 2026-08-29 | 可以选择子 agent 调用的模型。 |
| 1461 | [Anna-la/dsh-token-stat](https://github.com/Anna-la/dsh-token-stat) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness token 用量统计插件: 按模型/日期区分, 设置页看板, 数据目录在线更改 |
| 1462 | [AnonyJcy/dsh-plugin-j-space](https://github.com/AnonyJcy/dsh-plugin-j-space) | 0 | 2026-08-23 | 2026-08-27 | J-Space Cognition Suite V3.7 原生 DeepSeek Harness 智能体预设与独立 Cordis 插件，提供深层推理路由、工作区状态外化账本（.jspace）与全模型解耦的认知工作空间 |
| 1463 | [AnonyJcy/dsh-plugin-mobile-touch](https://github.com/AnonyJcy/dsh-plugin-mobile-touch) | 0 | 2026-08-27 | 2026-08-28 | Mobile & iPad touch optimization plugin for DeepSeek Harness Web GUI |
| 1464 | [Ansonfishing/dsh-model-manager](https://github.com/Ansonfishing/dsh-model-manager) | 0 | 2026-08-28 | 2026-08-28 | Manage local LLM inference servers in DSH: GPU registry, parameter profiles, VRAM validation, and tok/s benchmarks for llama.cpp, SGLang, and vLLM |
| 1465 | [Anyway-one/dsh-balance](https://github.com/Anyway-one/dsh-balance) | 0 | 2026-08-26 | 2026-08-26 | 为 DeepSeek Harness 提供持久化的余额与用量显示插件，让您随时掌握资源消耗情况，无需离开工作区。 |
| 1466 | [aqiane/dsh-client-ui-period-hint](https://github.com/aqiane/dsh-client-ui-period-hint) | 0 | 2026-08-21 | 2026-08-22 | 在输入栏显示当前dsAPI价格时段 |
| 1467 | [Army1900/dsh-e2e-dev-sdd](https://github.com/Army1900/dsh-e2e-dev-sdd) | 0 | 2026-08-26 | 2026-08-27 | dsh插件，用于驱动定制的e2e开发 |
| 1468 | [ArmyWas/dsh-codex-compat-canary](https://github.com/ArmyWas/dsh-codex-compat-canary) | 0 | 2026-08-25 | 2026-08-25 | Detect Codex App Server protocol drift that DeepSeek Harness cannot safely interpret. |
| 1469 | [asdasdsdsdasdasdasd/dsh-computer-use](https://github.com/asdasdsdsdasdasdasd/dsh-computer-use) | 0 | 2026-08-25 | 2026-08-29 | Linux X11 computer-use for DeepSeek Harness: screenshot, mouse, keyboard via a zero-dependency Python XTest helper — no Node native modules, no accessibility framework. |
| 1470 | [Asher-2000/dsh-artist-mode](https://github.com/Asher-2000/dsh-artist-mode) | 0 | 2026-08-22 | 2026-08-25 | DSH 艺术家模式 — 对话式设计交付预设（HTML 原生设计 / 反 AI slop / 5维评审 / Agnes AI 生图生视频） |
| 1471 | [Asher-2000/dsh-inline-images](https://github.com/Asher-2000/dsh-inline-images) | 0 | 2026-08-24 | 2026-08-25 | 对话内联图片/视频:LLM 回复中输出的本地图片路径在消息正文直接渲染,视频可点击播放。修复增强版(URL自动修正/刷新持久化/反向代理兼容)。 |
| 1472 | [ashuai/dsh-s2s](https://github.com/ashuai/dsh-s2s) | 0 | 2026-08-31 | 2026-08-31 | Connect AI agent sessions on one machine — a DeepSeek Harness plugin for session-to-session collaboration, with lifecycle support to wake finished sessions and loop-safe messaging budgets. |
| 1473 | [AstralFoundry/dsh-workspace](https://github.com/AstralFoundry/dsh-workspace) | 0 | 2026-08-27 | 2026-08-27 | A lightweight IDE and Git workspace plugin for DeepSeek Harness |
| 1474 | [asuramaya/osiris](https://github.com/asuramaya/osiris) | 0 | 2026-08-04 | 2026-08-22 | The persistent memory and coordination graph for AI agents (MCP, DeepSeek Harness, Claude Code, Cursor) |
| 1475 | [auggie246/dsh-mattpocock-skills](https://github.com/auggie246/dsh-mattpocock-skills) | 0 | 2026-08-28 | 2026-08-28 | Deepseek Harness plugin to install Mattpocock skills. |
| 1476 | [auggie246/dsh-output-styles](https://github.com/auggie246/dsh-output-styles) | 0 | 2026-08-28 | 2026-08-28 | Enable output styles in Deepseek Harness settings! |
| 1477 | [auggie246/dsh-sidebar](https://github.com/auggie246/dsh-sidebar) | 0 | 2026-08-27 | 2026-08-28 | Sidebar and panels for full developer interaction! |
| 1478 | [auggie246/dsh-synthetic-web-search](https://github.com/auggie246/dsh-synthetic-web-search) | 0 | 2026-08-28 | 2026-08-28 | Deepseek Harness plugin to use synthetic.new web search instead of built-in Deepseek web search |
| 1479 | [avdergh/chroma-cut](https://github.com/avdergh/chroma-cut) | 0 | 2026-08-28 | 2026-08-28 | Preserve anti-aliased outlines while cutting chroma-backed game assets. CLI + MCP + Codex plugin. |
| 1480 | [AwesomeHou/dsh-trace-collapse](https://github.com/AwesomeHou/dsh-trace-collapse) | 0 | 2026-08-15 | 2026-08-25 | DeepSeek Harness web plugin: collapse the agent trajectory while always keeping the agent's final output; default-collapse after final output is on by default (configurable in Settings). |
| 1481 | [awol2005ex3/dsh-md-table-export](https://github.com/awol2005ex3/dsh-md-table-export) | 0 | 2026-08-28 | 2026-08-28 | DeepSeek Harness（`dsh`）插件：把对话内容里的 **Markdown 表格** 一键导出为 **Excel（`.xlsx`）**。 |
| 1482 | [awol2005ex3/dsh-role-manager](https://github.com/awol2005ex3/dsh-role-manager) | 0 | 2026-08-28 | 2026-08-28 | DeepSeek Harness（dsh）角色管理插件。为每个"角色"预设一份初始系统提示词，在 Web 界面中切换当前角色，从而让模型以不同的身份 / 设定开始对话。 |
| 1483 | [awol2005ex3/dsh-user-manager](https://github.com/awol2005ex3/dsh-user-manager) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness（`dsh`）插件：为单机的 harness 增加**用户管理**与**会话按用户隔离**。 |
| 1484 | [axdlee/dsh-yeelight-smart-home](https://github.com/axdlee/dsh-yeelight-smart-home) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness plugin: Yeelight smart home control via the local yeelight-home runtime (skill, tools, settings card) |
| 1485 | [ayumedaze/dsh-git](https://github.com/ayumedaze/dsh-git) | 0 | 2026-08-29 | 2026-08-29 | dsh-plugin |
| 1486 | [Azonda/dsh-whale-writing](https://github.com/Azonda/dsh-whale-writing) | 0 | 2026-08-30 | 2026-08-31 | 老人与大肥鱼：Deepseek Harness超级写作增强插件，具备四种风格和五种写作严谨度的自动切换功能，并且具备任务级本地记忆和去ai味后处理、。 |
| 1487 | [B1lli/dsh-learning-bundle](https://github.com/B1lli/dsh-learning-bundle) | 0 | 2026-08-22 | 2026-08-24 | Proof-carrying correction learning for DSH: explicit adoption, scoped recall, and reconstructable delivery. |
| 1488 | [bailong-Hakuryu/dsh-engineering-control-plane](https://github.com/bailong-Hakuryu/dsh-engineering-control-plane) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness 工程任务编排与发布门禁插件，支持 /mission 指令、任务路由、计划执行、验证和状态跟踪。 \| Engineering mission orchestration and release-gate plugin for DeepSeek Harness with /mission routing, planning, execution, verification, and status tracking. |
| 1489 | [bailong-Hakuryu/dsh-security-assurance](https://github.com/bailong-Hakuryu/dsh-security-assurance) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness 策略驱动的仓库安全评估插件，支持包生命周期评估、证据、发现、裁决、导出和 /security 指令。 \| Policy-driven repository security assurance plugin for DeepSeek Harness with package lifecycle assessments, evidence, findings, verdicts, exports, and /security routing. |
| 1490 | [baiyang123/dsh-audit-missing](https://github.com/baiyang123/dsh-audit-missing) | 0 | 2026-08-27 | 2026-08-28 | 对照开发计划等文档，当AI开发完一个迭代之后扫描是否有漏开发的功能（真的好用） |
| 1491 | [baiyuscc13724-max/dsh-godot-preview](https://github.com/baiyuscc13724-max/dsh-godot-preview) | 0 | 2026-08-25 | 2026-08-25 | Independent Godot 4 Web and native preview plugin for DeepSeek Harness |
| 1492 | [bamboostrip/dsh-llm-capabilities](https://github.com/bamboostrip/dsh-llm-capabilities) | 0 | 2026-08-26 | 2026-08-26 | DSH plugin: auto-detect and configure model capabilities (reasoningEfforts + input modalities) for llm-pi-ai. Successor to dsh-reasoning-efforts. |
| 1493 | [BaoBao1996121/dsh-restart-ui](https://github.com/BaoBao1996121/dsh-restart-ui) | 0 | 2026-08-28 | 2026-08-28 | One-click cross-platform restart button for DeepSeek Harness Web UI |
| 1494 | [BaronCyrus/dsh-kimi-subscription](https://github.com/BaronCyrus/dsh-kimi-subscription) | 0 | 2026-08-28 | 2026-08-28 | Use a Kimi Code subscription in DeepSeek Harness with OAuth, quota display, and composer usage |
| 1495 | [BarrierFly/apx-watchdog](https://github.com/BarrierFly/apx-watchdog) | 0 | 2026-08-26 | 2026-08-26 | 牛来写的东西 |
| 1496 | [Barry-Liu-001/dsh_ark_plan_usage](https://github.com/Barry-Liu-001/dsh_ark_plan_usage) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness (DSH) 侧边栏插件：实时展示火山方舟 Agent Plan 用量（5h/周/月），数据来自本机 arkcli |
| 1497 | [Barry-Liu-001/dsh_chat_index](https://github.com/Barry-Liu-001/dsh_chat_index) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness (DSH) 对话索引插件：在对话区右边缘显示一列小圆点，每个点代表一条用户发送的消息。圆点等间距、紧凑、纵向居中排列（消息过多放不下时间距自动压缩以适应高度）；当前阅读位置的点高亮为品牌色。 |
| 1498 | [bbboy31/dsh-terminal-tabs](https://github.com/bbboy31/dsh-terminal-tabs) | 0 | 2026-08-26 | 2026-08-26 | Terminals view tab for DeepSeek Harness web UI — live background job count, streaming output, one-click kill |
| 1499 | [BenYuan-Nolove-onani/dsh-token-stats](https://github.com/BenYuan-Nolove-onani/dsh-token-stats) | 0 | 2026-08-15 | 2026-08-23 | Token usage statistics plugin for DeepSeek Harness — per-window consumption metrics with an enable/disable switch, right in Settings.----------DeepSeek Harness 的 Token 用量统计插件：按时间窗统计消耗指标，设置页内随时启停。 |
| 1500 | [benz-ai-x/dsh-session-graph](https://github.com/benz-ai-x/dsh-session-graph) | 0 | 2026-08-28 | 2026-08-30 | Visual session graph for DeepSeek Harness — browse, arrange, branch, merge, and summarize AI agent sessions on an interactive canvas. |
| 1501 | [berserk0501/dsh-soundscape](https://github.com/berserk0501/dsh-soundscape) | 0 | 2026-08-26 | 2026-08-26 | DSH 本机思考与工具音效插件，支持 MediaPlayer、WAV/MP3、自定义映射和设置面板 |
| 1502 | [bf185003/dsh-favicon-status](https://github.com/bf185003/dsh-favicon-status) | 0 | 2026-08-21 | 2026-08-24 | Browser tab status indicator plugin for DeepSeek Harness (dsh web): paints the document favicon from the sessions list projection - green done / amber waiting / blue running, spinning while work executes. |
| 1503 | [Bigesila-B/dsh-media-forge](https://github.com/Bigesila-B/dsh-media-forge) | 0 | 2026-08-26 | 2026-08-26 | DSH Media Forge plugin: agent + skills workflow for media-generation APIs, with a sidebar skill panel (zh/en docs) |
| 1504 | [bigfurma-bot/dsh-attention](https://github.com/bigfurma-bot/dsh-attention) | 0 | 2026-08-22 | 2026-08-24 | Approval attention watcher for DeepSeek Harness: bell sound + tab-title flash whenever an approval needs the owner's decision |
| 1505 | [bigfurma-bot/dsh-todos](https://github.com/bigfurma-bot/dsh-todos) | 0 | 2026-08-22 | 2026-08-24 | Persistent shared to-do list for DeepSeek Harness: web UI tab + agent tools over one JSON store, writable from both sides |
| 1506 | [bigfurma-bot/dsh-voice-dictation](https://github.com/bigfurma-bot/dsh-voice-dictation) | 0 | 2026-08-22 | 2026-08-24 | Push-to-talk voice dictation for DeepSeek Harness: mic button in the composer transcribes via local Parakeet STT into your message draft |
| 1507 | [bigfurma-bot/dsh-web-restart](https://github.com/bigfurma-bot/dsh-web-restart) | 0 | 2026-08-25 | 2026-08-26 | One-click restart for DeepSeek Harness Web UI — arm-to-confirm button pinned to the Settings › General corner, live status dot, detached Linux restarter. Linux port of 1123762794/dsh-web-restart |
| 1508 | [bigfurma-bot/dsh-websearch-mcp](https://github.com/bigfurma-bot/dsh-websearch-mcp) | 0 | 2026-08-22 | 2026-08-24 | Local web search for DeepSeek Harness via MCP — Bing/Brave/DuckDuckGo scraping, no API keys, agent-installable |
| 1509 | [bigharm/dsh-agentnoodle](https://github.com/bigharm/dsh-agentnoodle) | 0 | 2026-08-30 | 2026-08-31 | DeepSeek Harness 插件：AI 驱动的群像聊天游戏框架。轻量化酒馆。兼容 SillyTavern V1/V2/V3 JSON 和 PNG 内嵌卡片。添加npc和场景之类的，给harness提要求，让它做就行。玩家输入一个行动，场景中多个 NPC 各自做出反应，每条反应独立成一条带头像插图的聊天室消息；支持场景切换、NPC 关系变化与本地 JSON 存档。 |
| 1510 | [BiKing567/dsh-subagent-panel](https://github.com/BiKing567/dsh-subagent-panel) | 0 | 2026-08-31 | 2026-08-31 | DSH 插件：把每个子代理渲染成主对话里可点击的卡片，点击直接进入子代理会话（与标题栏同一路径）。\| DSH plugin: render every subagent as a clickable inline card that opens the child session — same navigation the header's subagent catalog uses. |
| 1511 | [birdmanhj/dsh-mv-session](https://github.com/birdmanhj/dsh-mv-session) | 0 | 2026-08-25 | 2026-08-25 | A plug-in for Deepseek Harness that easy to move/rename session from old workspace to new workspace. |
| 1512 | [BISTU-guheihei/DSH-SessionManager](https://github.com/BISTU-guheihei/DSH-SessionManager) | 0 | 2026-08-26 | 2026-08-26 | DSH 会话管理工具：可视化/命令行查看与删除历史聊天记录，自动清理缓存残留 |
| 1513 | [bitterSmilezzz/dsh-asr-voice](https://github.com/bitterSmilezzz/dsh-asr-voice) | 0 | 2026-08-25 | 2026-08-27 | 开口即成文 · Speak-to-prompt for DeepSeek Harness：云端 ASR 语音识别 + 提示词优化 + 填入草稿/自动发送，跨平台 macOS / Windows。 |
| 1514 | [biyuhao/dsh-model-proxy](https://github.com/biyuhao/dsh-model-proxy) | 0 | 2026-08-22 | 2026-08-23 | DSH plugin: per-model proxy routing (http/https/socks5) with a settings UI — e.g. opencode/muse-spark-1.2-contributor needs a proxy while sibling models stay direct |
| 1515 | [bleakbelladonnals/dsh-artifact-harbor](https://github.com/bleakbelladonnals/dsh-artifact-harbor) | 0 | 2026-08-27 | 2026-08-27 | Artifact Harbor — secure, session-aware artifact previews for DeepSeek Harness Web |
| 1516 | [bleakbelladonnals/dsh-echo](https://github.com/bleakbelladonnals/dsh-echo) | 0 | 2026-08-27 | 2026-08-27 | Record MCP once. Replay it safely inside DeepSeek Harness. |
| 1517 | [bleamayaka/dsh-file-beam](https://github.com/bleamayaka/dsh-file-beam) | 0 | 2026-08-27 | 2026-08-27 | dsh-file-beam - DSH plugin: drag files into the web composer, resolve real absolute paths, hidden path injection for the agent (no copy, no path in composer). |
| 1518 | [bLueriVerLHR/dsh-better-webui](https://github.com/bLueriVerLHR/dsh-better-webui) | 0 | 2026-08-20 | 2026-08-27 | Minimal improvement if possible. |
| 1519 | [bo961386926/dolphin-pet-plugin](https://github.com/bo961386926/dolphin-pet-plugin) | 0 | 2026-08-26 | 2026-08-26 | Cute desktop pet for DeepSeek Harness - custom name, upload your own pet image, or generate one with AI. DSH 桌面宠物插件 |
| 1520 | [bochen2029-pixel/dsh-first-hop](https://github.com/bochen2029-pixel/dsh-first-hop) | 0 | 2026-08-25 | 2026-08-26 | Your agent wakes on evidence, not on a clock. A community plugin for DeepSeek Harness: watches the streams your harness already carries and decides - hold, flag, counsel, or wake. Local judge, shadow by default, MIT. |
| 1521 | [bosinHU/dsh-skill-editor](https://github.com/bosinHU/dsh-skill-editor) | 0 | 2026-08-29 | 2026-08-30 | Edit skills directly in DSH web settings |
| 1522 | [BoWuGit/dsh-reasoning](https://github.com/BoWuGit/dsh-reasoning) | 0 | 2026-08-31 | 2026-08-31 | Codex-style /reasoning command for DeepSeek Harness Web |
| 1523 | [BrianHIO-x/dsh-think-expand](https://github.com/BrianHIO-x/dsh-think-expand) | 0 | 2026-08-22 | 2026-08-22 | DeepSeek Harness plugin that auto-expands Think rows while reasoning |
| 1524 | [Britneycode/dsh-distillery](https://github.com/Britneycode/dsh-distillery) | 0 | 2026-08-30 | 2026-08-30 | dsh 插件：本地蒸馏器——扫历史会话挖「用户纠错 → 改对」片段，脱敏后蒸馏成微调 JSONL / SKILL.md 技能草稿 / AGENTS.md 规则补丁，带人工审核队列 |
| 1525 | [Britneycode/dsh-live-room](https://github.com/Britneycode/dsh-live-room) | 0 | 2026-08-30 | 2026-08-30 | dsh 插件：把会话变成免登录、只读、可分享的实时直播间（SSE 观看页 + 弹幕 + agent 工具） |
| 1526 | [Bronier/dsh-web-search-so360](https://github.com/Bronier/dsh-web-search-so360) | 0 | 2026-08-27 | 2026-08-27 | Keyless web search provider for DeepSeek Harness backed by 360 Search (so.com). |
| 1527 | [BrucePayton/dsh-plugin-graphgpt](https://github.com/BrucePayton/dsh-plugin-graphgpt) | 0 | 2026-08-22 | 2026-08-23 | Run validated GraphGPT workflows as native DeepSeek Harness tools |
| 1528 | [buchylx/create-dsh-content-plugin](https://github.com/buchylx/create-dsh-content-plugin) | 0 | 2026-08-26 | 2026-08-26 | Zero-dependency CLI that scaffolds a content-automation DSH plugin (Dev.to/GitHub/Bluesky/Mastodon). Like create-vite, for DSH. |
| 1529 | [buildbeforewepitch/agentscars](https://github.com/buildbeforewepitch/agentscars) | 0 | 2026-08-21 | 2026-08-22 | A public commons of real AI-agent failure patterns ("scars") — searchable via API and MCP. Live at agentscars.com. |
| 1530 | [bycall/dsh-code-collector](https://github.com/bycall/dsh-code-collector) | 0 | 2026-08-27 | 2026-08-27 | Session code collector for DeepSeek Harness: gather every code block the model produced in the current session, grouped by language, with copy / download-all / jump-to-turn. |
| 1531 | [ByxHuster/DSH-Paper-Highlighting-Agent](https://github.com/ByxHuster/DSH-Paper-Highlighting-Agent) | 0 | 2026-08-27 | 2026-08-27 | An interactive and customized paper highlighting tool built upon Deepseek Harness (DSH), still under development. |
| 1532 | [c0nfident/github-slideshow](https://github.com/c0nfident/github-slideshow) | 0 | 2020-07-07 | 2026-08-30 | A robot powered training repository :robot: |
| 1533 | [c2j/dsh-swarmforge](https://github.com/c2j/dsh-swarmforge) | 0 | 2026-08-23 | 2026-08-24 | SwarmForge migrate as a DeepSeek Harness Plugin |
| 1534 | [CagierAsh123/dsh-obsidian-agent-wiki](https://github.com/CagierAsh123/dsh-obsidian-agent-wiki) | 0 | 2026-08-26 | 2026-08-27 | Searchable SQLite-indexed Obsidian memory for DeepSeek Harness |
| 1535 | [Calvin451970353/dsh-vmic](https://github.com/Calvin451970353/dsh-vmic) | 0 | 2026-08-25 | 2026-08-27 | Voice input plugin for DeepSeek Harness: mic button, 16kHz WAV recording, ASR via Xiaomi MiMo / Volcengine Doubao (live), optional LLM polish. |
| 1536 | [CanaryJing/dsh-big-fat-whale-maid-adaptive](https://github.com/CanaryJing/dsh-big-fat-whale-maid-adaptive) | 0 | 2026-08-23 | 2026-08-27 | 大肥鱼女仆长智能体，用风神与明神插件vibe而来，解决wsl与windows互通问题 |
| 1537 | [CarlMarkswx/deepseek-multimodel](https://github.com/CarlMarkswx/deepseek-multimodel) | 0 | 2026-08-24 | 2026-08-24 | Unified vision and image-generation plugin suite for DeepSeek Harness |
| 1538 | [Castem114/dsh-visioncraft](https://github.com/Castem114/dsh-visioncraft) | 0 | 2026-08-26 | 2026-08-26 | 为 DeepSeek Harness（DSH）Web 量身打造的双插件扩展，为纯文本模型补齐"视觉"短板 |
| 1539 | [cayan0x/dsh-fold-context](https://github.com/cayan0x/dsh-fold-context) | 0 | 2026-08-28 | 2026-08-28 | Auto-fold context/system messages in DSH — collapse think blocks, tool calls, and tool results into grouped expandable bars. |
| 1540 | [cayan0x/Lume](https://github.com/cayan0x/Lume) | 0 | 2026-08-29 | 2026-08-31 | Lume - DSH Desktop persona-switching plugin (loli/senpai/none) with P0-P3 thinking logic |
| 1541 | [Centaurea5547196/dsh-page-zoom](https://github.com/Centaurea5547196/dsh-page-zoom) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness Web UI ??????:????? + Ctrl+??/Ctrl+=/-/0 ???,25%-300%,?????? |
| 1542 | [ch3vr0n5/dsh-docker-services](https://github.com/ch3vr0n5/dsh-docker-services) | 0 | 2026-08-26 | 2026-08-27 | Portable DeepSeek Harness plugin for securely monitoring and operating Docker services |
| 1543 | [chancoki/dsh-model-search-plugin](https://github.com/chancoki/dsh-model-search-plugin) | 0 | 2026-08-24 | 2026-08-24 | 为 DeepSeek Harness (DSH) Web GUI 提供模型搜索功能的插件——在模型选择弹窗中添加关键字搜索框，快速筛选模型。 |
| 1544 | [change979666/ox-alpha-dsh](https://github.com/change979666/ox-alpha-dsh) | 0 | 2026-08-25 | 2026-08-25 | [Model Hub for DSH] Lightweight model/provider integration toolkit for DeepSeek Harness Desktop - one plugin installs Ox Alpha (stealth/ox-alpha), plus custom models, custom OpenAI-compatible providers, health check, discovery and rollback. bilingual zh/en |
| 1545 | [changyinliangbaikai/dsh-b2us-schedule](https://github.com/changyinliangbaikai/dsh-b2us-schedule) | 0 | 2026-08-29 | 2026-08-30 | dsh定时任务插件，支持延迟、固定间隔、cron表达式，支持执行shell命令，支持发起Agent会话 |
| 1546 | [chaoliu615/dsh-agnes](https://github.com/chaoliu615/dsh-agnes) | 0 | 2026-08-20 | 2026-08-26 | 为在dsh中使用Agnes AI的免费图片、视频生成功能而开发，欢迎使用！欢迎提issues。 |
| 1547 | [Che-Year/dsh-pet-lulu](https://github.com/Che-Year/dsh-pet-lulu) | 0 | 2026-08-26 | 2026-08-26 | A cute terminal and web pet plugin for DeepSeek Harness (dsh), using assets from lulu and capybara projects. |
| 1548 | [Cheeserackery/deepseek-time](https://github.com/Cheeserackery/deepseek-time) | 0 | 2026-08-18 | 2026-08-28 | 一款Agent插件，能够实时直观显示DeepSeek当前收费时段状态。DeepSeek pricing-period status indicator with Hermes, DSH, and Codex adapters. |
| 1549 | [chemmy-11/dsh-nexus](https://github.com/chemmy-11/dsh-nexus) | 0 | 2026-08-24 | 2026-08-31 | Vault observation plugin for DeepSeek Harness: Obsidian vault metadata snapshot + edit stats + observation panel |
| 1550 | [chen70456-lang/dsh-tmwebdriver](https://github.com/chen70456-lang/dsh-tmwebdriver) | 0 | 2026-08-30 | 2026-08-30 | One tool, infinite reach: arbitrary JS in your real logged-in browser. Unlike fixed-action plugins, browser_execute_js does anything DevTools can — read, click, type, fill, navigate, screenshot, CDP. Plus list_tabs/snapshot/type. Zero-setup, self-healing. |
| 1551 | [chendefine/dsh-sidebar-onlyoffice](https://github.com/chendefine/dsh-sidebar-onlyoffice) | 0 | 2026-08-24 | 2026-08-27 | DSH web plugin: open and edit .docx/.xlsx/.pptx in the better-sidebar editor through a self-hosted ONLYOFFICE Document Server (JWT-signed config, atomic save-back, live refresh on AI edits) |
| 1552 | [chendefine/dsh-sidebar-vscode](https://github.com/chendefine/dsh-sidebar-vscode) | 0 | 2026-08-27 | 2026-08-27 | DSH plugin: a better-sidebar tab embedding the VS Code web workbench at the session workspace; editor selections and explorer files land as atomic reference chips |
| 1553 | [chengoak/dsh-font-size](https://github.com/chengoak/dsh-font-size) | 0 | 2026-08-21 | 2026-08-22 | DSH Web GUI plugin: 'Conversation font size' slider (12-22 px) in Settings → General. |
| 1554 | [ChengxiuCDP/dsh-migrate-codex](https://github.com/ChengxiuCDP/dsh-migrate-codex) | 0 | 2026-08-23 | 2026-08-23 | DSH plugin: safely migrate a Codex environment between machines (/migrate-codex command + codex-migration skill) |
| 1555 | [chenyangcun/dsh-command-palette](https://github.com/chenyangcun/dsh-command-palette) | 0 | 2026-08-30 | 2026-08-30 | A keyboard-first command palette for standard DeepSeek Harness |
| 1556 | [chenyangcun/dsh-fixed-new-session-model](https://github.com/chenyangcun/dsh-fixed-new-session-model) | 0 | 2026-08-30 | 2026-08-30 | 为 DSH 固定新会话的默认 Agent 预设与模型，支持全局默认设置和工作区独立配置。 |
| 1557 | [chenyedamw/dropshipping-product-scout](https://github.com/chenyedamw/dropshipping-product-scout) | 0 | 2026-08-22 | 2026-08-25 | Dropshipping Product Scout MCP 服务的 Claude Code 插件 —— 精选商品搜索、库存查询与物流估算  |
| 1558 | [Choco-Zz/dsh-image-amnesia](https://github.com/Choco-Zz/dsh-image-amnesia) | 0 | 2026-08-31 | 2026-08-31 | Drop historical images before DeepSeek Harness relay requests; keep native vision on the newest image. |
| 1559 | [chocobo77/dsh-infinite-context](https://github.com/chocobo77/dsh-infinite-context) | 0 | 2026-08-29 | 2026-08-30 | DeepSeek Harness plugin: multi-tier memory management, semantic retrieval, structured memory, and model-context awareness for infinite context. |
| 1560 | [chouyulanxia114514/dsh-uisketch](https://github.com/chouyulanxia114514/dsh-uisketch) | 0 | 2026-08-28 | 2026-08-28 | UI Sketch to AI 画板编辑器 × DSH 插件：侧栏开关 + 全屏 iframe 浮层，开箱即用 |
| 1561 | [chris-003/dsh-agent-in-browser](https://github.com/chris-003/dsh-agent-in-browser) | 0 | 2026-08-31 | 2026-08-31 | Let a DeepSeek Harness agent see and control your browser in real time — read, screenshot, navigate, click, and manage tabs via tool calls. |
| 1562 | [CHristianREEVEE/dsh-xiuxian-world](https://github.com/CHristianREEVEE/dsh-xiuxian-world) | 0 | 2026-08-28 | 2026-08-28 | 云仙大世界 — a living xiuxian world for DeepSeek Harness agents: enter, cultivate, and export a self-contained HTML replay of your journey |
| 1563 | [cinderzhan/dsh-plugin-dew](https://github.com/cinderzhan/dsh-plugin-dew) | 0 | 2026-08-26 | 2026-08-26 | See what your other coding agents are doing from inside DSH: Claude Code, Codex, Cursor and DSH sessions, their state, and their scheduled tasks. |
| 1564 | [Cinnamobot/dsh-disclosure-tweaks](https://github.com/Cinnamobot/dsh-disclosure-tweaks) | 0 | 2026-08-25 | 2026-08-25 | Auto-expand/collapse DSH conversation disclosure rows (Think, tool calls, context, todo, queue) with per-type Settings toggles. Manual toggles are never overridden. |
| 1565 | [Cinnamobot/dsh-nothing-skin](https://github.com/Cinnamobot/dsh-nothing-skin) | 0 | 2026-08-25 | 2026-08-25 | Nothing Phone style skin for DeepSeek Harness — dot-matrix background, Space Grotesk/Mono, monochrome + signal red, per-feature Settings toggles |
| 1566 | [cKNKSnd/dsh-model-provider-badge](https://github.com/cKNKSnd/dsh-model-provider-badge) | 0 | 2026-08-19 | 2026-08-23 | DeepSeek Harnes 输入框当前模型提供商名称 |
| 1567 | [classic-takeoff/DSH_plugins](https://github.com/classic-takeoff/DSH_plugins) | 0 | 2026-08-31 | 2026-08-31 | some plugins for dsh |
| 1568 | [cloveric/deepseek-harness-web-search-plugin](https://github.com/cloveric/deepseek-harness-web-search-plugin) | 0 | 2026-08-29 | 2026-08-29 | Source-traceable Brave + Tavily live web search and URL extraction for DeepSeek Harness. Native DSH plugin; TaroCub optional. |
| 1569 | [cmhaoren-sudo/dsh-tab-status](https://github.com/cmhaoren-sudo/dsh-tab-status) | 0 | 2026-08-22 | 2026-08-23 | DSH plugin: leave long-running tasks and watch yellow/green/blue on the Firefox, Chrome, or Edge tab. 长程任务可切出去，标签仍能看到状态。 |
| 1570 | [co-Elly/dsh-plugin-vision](https://github.com/co-Elly/dsh-plugin-vision) | 0 | 2026-08-22 | 2026-08-22 | 👁️ Give your DeepSeek Harness the gift of sight — enables pure-text LLMs to analyze images via Zhipu's free GLM-4V-Flash vision model |
| 1571 | [Co-Kyo/dsh-interview-forge](https://github.com/Co-Kyo/dsh-interview-forge) | 0 | 2026-08-22 | 2026-08-22 | interview-forge-plugin for deepseek harness |
| 1572 | [coffee-man666/dsh-lens](https://github.com/coffee-man666/dsh-lens) | 0 | 2026-08-22 | 2026-08-23 | Repository and agent-runtime analysis skills as an installable DeepSeek Harness (dsh) plugin |
| 1573 | [ColdCGH/dsh-desktop-shell](https://github.com/ColdCGH/dsh-desktop-shell) | 0 | 2026-08-24 | 2026-08-29 | dsh desktop shell plugin |
| 1574 | [ConTr0L0/dsh-balance-monitor](https://github.com/ConTr0L0/dsh-balance-monitor) | 0 | 2026-08-22 | 2026-08-25 | dsh-balance-monitor 是 DeepSeek Harness（DSH）的插件：在侧边栏实时显示 API 余额，按官方峰谷价目（每日自动从 DeepSeek 官方文档同步）精确计算每次请求成本，按会话/模型/日期拆分消耗统计，并支持每日、累计、请求次数三类上限（可硬拦截后续 LLM 请求）。Web 端与桌面端通用，计费口径已与 DeepSeek 平台账单逐项对账 |
| 1575 | [Cooberped/dsh-evidence](https://github.com/Cooberped/dsh-evidence) | 0 | 2026-08-28 | 2026-08-28 | Turn local files into versioned evidence in DeepSeek Harness: composer upload, private local retrieval, and coordinate-exact PDF/DOCX/XLSX/PPTX reads. |
| 1576 | [coolgech/dsh-siyuan](https://github.com/coolgech/dsh-siyuan) | 0 | 2026-08-27 | 2026-08-27 | A plugin for deepseek harnes that operates on the notes of Siyuan. |
| 1577 | [CoolTea001/dsh-cool-theme](https://github.com/CoolTea001/dsh-cool-theme) | 0 | 2026-08-30 | 2026-08-30 | A plugin for changing themes for DSH, with a number of popular default themes built in. |
| 1578 | [cslht11/dsh-custom-patches](https://github.com/cslht11/dsh-custom-patches) | 0 | 2026-08-18 | 2026-08-24 | DSH (DeepSeek Harness) 自定义增强补丁集：输入历史 + 编辑最后一条消息并重新生成。Custom enhancements for the DeepSeek Harness Web GUI via compiled-artifact patches. |
| 1579 | [cslht11/dsh-provider-config](https://github.com/cslht11/dsh-provider-config) | 0 | 2026-08-26 | 2026-08-26 | DSH (DeepSeek Harness) LLM 供应商配置模板与限流重试机制最佳实践（SenseNova 脱敏版）。Provider config templates + retry-policy best practices for DSH, sanitized. |
| 1580 | [cslht11/dsh-ssh-remote](https://github.com/cslht11/dsh-ssh-remote) | 0 | 2026-08-20 | 2026-08-24 | DeepSeek Harness SSH 远程工作区插件（多机并行）：同时连接多台服务器，Agent 直接查看/编辑/执行远程文件。基于 flymysql/dsh-remote (MIT) 适配 0.1.1-rc.2 |
| 1581 | [cstarc/dsh-skill-mcp-bridge](https://github.com/cstarc/dsh-skill-mcp-bridge) | 0 | 2026-08-26 | 2026-08-26 | dsh 项目桥接插件：自动导入 .claude/.agents/.trae skills 并桥接 MCP 服务器（HTTP/SSE + stdio），GUI 开关控制、状态持久化 |
| 1582 | [csustyang/dsh-garmin-coach](https://github.com/csustyang/dsh-garmin-coach) | 0 | 2026-08-27 | 2026-08-31 | Garmin Connect 运动健康 AI 教练插件 for DeepSeek Harness |
| 1583 | [CyberFox-lab/dsh-rss](https://github.com/CyberFox-lab/dsh-rss) | 0 | 2026-08-30 | 2026-08-30 | RSS/Atom reader and Agent tools plugin for DeepSeek Harness |
| 1584 | [cyjyyd/dsh-llm-xai-oauth](https://github.com/cyjyyd/dsh-llm-xai-oauth) | 0 | 2026-08-27 | 2026-08-27 | Native SuperGrok / X Premium OAuth provider for DeepSeek Harness. Reuses local grok-bridge tokens; no xAI API key. |
| 1585 | [d3vmeh/dsh-context-budget](https://github.com/d3vmeh/dsh-context-budget) | 0 | 2026-08-29 | 2026-08-30 | DeepSeek Harness plugin: keep a local model's context at a size your GPU handles well (measured prefill speed, hard ceiling, early compaction) |
| 1586 | [da-beda/dsh-lockstep](https://github.com/da-beda/dsh-lockstep) | 0 | 2026-08-24 | 2026-08-24 | Pin-aware updater for DeepSeek Harness. Check lockfile drift, plan pin bumps, never float to latest. |
| 1587 | [daetz-coder/DSH-Mobile](https://github.com/daetz-coder/DSH-Mobile) | 0 | 2026-08-24 | 2026-08-25 | DSH-Mobile · 把 DeepSeek Harness 装进口袋 — scan-to-pair Android companion for the official DeepSeek Harness Web UI. DeepSeek Harness 手机配套：扫码配对、状态通知、桌面远程控制。 |
| 1588 | [daveycodez/dsh-llm-agent-bridge](https://github.com/daveycodez/dsh-llm-agent-bridge) | 0 | 2026-08-26 | 2026-08-27 | Claude as a selectable LLM provider in DeepSeek Harness, via Anthropic's official Claude Agent SDK. Works in any DSH mode. |
| 1589 | [david0702/dsh-cost](https://github.com/david0702/dsh-cost) | 0 | 2026-08-26 | 2026-08-26 | DSH (DeepSeek Harness) 对话底部费用显示插件：按每笔请求时间+模型分批计费，分时段明细，模型归属，读图金额，余额。 |
| 1590 | [DavidRm1911/dsh-llm-subscription](https://github.com/DavidRm1911/dsh-llm-subscription) | 0 | 2026-08-24 | 2026-08-25 | Native DeepSeek Harness LLM adapter for Claude Code / Antigravity CLI subscriptions — no API key |
| 1591 | [DavidRm1911/dsh-subscription-gateway](https://github.com/DavidRm1911/dsh-subscription-gateway) | 0 | 2026-08-24 | 2026-08-25 | OpenAI-compatible gateway that lets DeepSeek Harness use your existing Claude Code / Antigravity / Ollama logins instead of a paid API key |
| 1592 | [Dayi-Z/gitcompass](https://github.com/Dayi-Z/gitcompass) | 0 | 2026-08-28 | 2026-08-29 | GitHub-connected visual git panel for DeepSeek Harness - branch switcher, file-level approval cards, PR/issue workspace |
| 1593 | [dddzzz123-dz/dsh-read-image-plugin](https://github.com/dddzzz123-dz/dsh-read-image-plugin) | 0 | 2026-08-22 | 2026-08-22 | Image input fallback for DeepSeek Harness with native multimodal model detection and Volcengine Ark vision. |
| 1594 | [DecresLuna/DSH-Service](https://github.com/DecresLuna/DSH-Service) | 0 | 2026-08-22 | 2026-08-22 | DSH Service - DeepSeek Harness Mac 菜单栏服务管理器 |
| 1595 | [Dee3526/dsh-plugin-trtc-conai](https://github.com/Dee3526/dsh-plugin-trtc-conai) | 0 | 2026-08-31 | 2026-08-31 | Tencent RTC Conversational AI (ConAI) voice agent tools for the DeepSeek Harness |
| 1596 | [DeepseekHarnessPlugins/Notification](https://github.com/DeepseekHarnessPlugins/Notification) | 0 | 2026-08-26 | 2026-08-26 | DeepseekHarnessPlugin |
| 1597 | [DeepVite/dsh-model-selector](https://github.com/DeepVite/dsh-model-selector) | 0 | 2026-08-23 | 2026-08-26 | 梁文谷插件 · DeepSeek Harness 模型选择器升级：一级菜单模型/思考档位选择 + 自定义模型别名 + 高峰低谷计价倒计时。Apache-2.0 |
| 1598 | [delicious28/wuming-books-mcp](https://github.com/delicious28/wuming-books-mcp) | 0 | 2026-08-28 | 2026-08-31 | Free remote MCP server for searching 680K+ Chinese books with Douban ratings, AI reading guides and curated toplists. No API key. |
| 1599 | [demacia1314/dsh-remote-deliver](https://github.com/demacia1314/dsh-remote-deliver) | 0 | 2026-08-27 | 2026-08-27 | 🚀 告别繁琐 SCP！远程部署 DSH 一键下载修改后的文件与图片预览交付插件 |
| 1600 | [Demigod-cyber/dsh-angelina-theme](https://github.com/Demigod-cyber/dsh-angelina-theme) | 0 | 2026-08-26 | 2026-08-26 | DSH主题插件——直到大地变成一颗酸橙（Angelina 浅蓝主题） |
| 1601 | [DemoJ/proactive-notify](https://github.com/DemoJ/proactive-notify) | 0 | 2026-08-20 | 2026-08-22 | 一个运行在 DeepSeek Harness（DSH）Web GUI 上的消息通知插件 |
| 1602 | [dengyier/openworkproof-dsh-plugin](https://github.com/dengyier/openworkproof-dsh-plugin) | 0 | 2026-08-30 | 2026-08-30 | Community DeepSeek Harness plugin for verifiable AI agent authorization, execution evidence, and offline delivery verification |
| 1603 | [dennisrongo/dsh-plugins](https://github.com/dennisrongo/dsh-plugins) | 0 | 2026-08-23 | 2026-08-27 | Dennis Rongo's plugin collection for DeepSeek Harness (dsh)  |
| 1604 | [DepressionL/fortune-assistant](https://github.com/DepressionL/fortune-assistant) | 0 | 2026-08-28 | 2026-08-30 | dsh算命插件 |
| 1605 | [Destined-at-Dawn/dsh-visual-workbench](https://github.com/Destined-at-Dawn/dsh-visual-workbench) | 0 | 2026-08-25 | 2026-08-26 | A DSH visual workbench for Obsidian-style knowledge spaces and local Comfy MCP workflows. |
| 1606 | [DevViking-Persike/dsh-docker](https://github.com/DevViking-Persike/dsh-docker) | 0 | 2026-08-22 | 2026-08-22 | DeepSeek Harness plugin: Docker container, image, log, and Compose tools for the agent, over the local Docker CLI |
| 1607 | [DevViking-Persike/dsh-git-graph](https://github.com/DevViking-Persike/dsh-git-graph) | 0 | 2026-08-25 | 2026-08-26 | DeepSeek Harness plugin: a Git commit-graph view with lanes, refs, and worktree management |
| 1608 | [DevViking-Persike/dsh-monaco](https://github.com/DevViking-Persike/dsh-monaco) | 0 | 2026-08-22 | 2026-08-22 | DeepSeek Harness plugin: serves the Monaco editor distribution over a host HTTP route, so an editor plugin needs no CDN |
| 1609 | [dfhxxc666/dsh-llm-mimo](https://github.com/dfhxxc666/dsh-llm-mimo) | 0 | 2026-08-27 | 2026-08-27 | Xiaomi MiMo v2.5 adapter for DeepSeek Harness — fixed fork (sanitize tool args, dsh-llm 0.1.1-rc.2, prepareCall, keepalive) |
| 1610 | [difimim/dsh-voice-input](https://github.com/difimim/dsh-voice-input) | 0 | 2026-08-29 | 2026-08-30 | 语音输入插件 for Deepseek Harness |
| 1611 | [dingminhua/dsh-connect-trae](https://github.com/dingminhua/dsh-connect-trae) | 0 | 2026-08-28 | 2026-08-28 | Connect locally signed-in Trae models to DeepSeek Harness with a read-only credits overview. |
| 1612 | [dingxin-tech/dsh-maxcompute](https://github.com/dingxin-tech/dsh-maxcompute) | 0 | 2026-08-31 | 2026-08-31 | DSH (DeepSeek Harness) plugin for MaxCompute (ODPS): metadata browsing, cost-gated SQL execution, background jobs and result export. |
| 1613 | [djs326/dsh-titlebar-feed](https://github.com/djs326/dsh-titlebar-feed) | 0 | 2026-08-30 | 2026-08-31 | DSH Desktop 标题栏信息条插件：修复 Windows 无边框标题栏遮挡，提供可配置信息条（静态文本 / HTTP 接口 / JS 函数 / 系统指标），支持分页、动态切换与快捷键。npm: dsh-titlebar-feed |
| 1614 | [DobyChao/dsh-workspace-enhancement](https://github.com/DobyChao/dsh-workspace-enhancement) | 0 | 2026-08-25 | 2026-08-27 | DeepSeek Harness plugin: local and remote (SSH) workspaces in one place. Remote execution uses a single SSH connection (multi-hop jumps allowed); bash, files, PTY, and LSP share that link. |
| 1615 | [doer1296/dsh-plugin-voice](https://github.com/doer1296/dsh-plugin-voice) | 0 | 2026-08-29 | 2026-08-29 | DeepSeek Harness 语音插件：火山 seed-tts 云端 TTS（自动回退 SAPI/Huihui 离线）+ 桌面通知 + 场景化 WAV 提示音 + 提问自动呼叫。DSH 原生集成，零 Python 依赖，Windows 原生。 |
| 1616 | [dongsheng123132/dsh-artifact-promotion-proof](https://github.com/dongsheng123132/dsh-artifact-promotion-proof) | 0 | 2026-08-26 | 2026-08-26 | Offline proof that one immutable artifact followed a declared promotion chain |
| 1617 | [dongsheng123132/dsh-attestation-proof](https://github.com/dongsheng123132/dsh-attestation-proof) | 0 | 2026-08-25 | 2026-08-25 | Offline content-addressed DSSE/in-toto attestation proof for DeepSeek Harness |
| 1618 | [dongsheng123132/dsh-break-glass-settlement-proof](https://github.com/dongsheng123132/dsh-break-glass-settlement-proof) | 0 | 2026-08-26 | 2026-08-26 | Offline content-addressed DSH proof for break-glass session settlement evidence |
| 1619 | [dongsheng123132/dsh-build-hermeticity-proof](https://github.com/dongsheng123132/dsh-build-hermeticity-proof) | 0 | 2026-08-26 | 2026-08-26 | Offline hash-only proof that recorded build accesses stayed within a declared closure |
| 1620 | [dongsheng123132/dsh-change-window-proof](https://github.com/dongsheng123132/dsh-change-window-proof) | 0 | 2026-08-26 | 2026-08-26 | Offline content-addressed DSH proof for change-window settlement evidence |
| 1621 | [dongsheng123132/dsh-credential-retirement-proof](https://github.com/dongsheng123132/dsh-credential-retirement-proof) | 0 | 2026-08-26 | 2026-08-27 | Evidence-only DSH plugin for credential retirement settlement |
| 1622 | [dongsheng123132/dsh-duty-separation-proof](https://github.com/dongsheng123132/dsh-duty-separation-proof) | 0 | 2026-08-26 | 2026-08-27 | Offline content-addressed duty-separation evidence for supplied DSH workflow receipts |
| 1623 | [dongsheng123132/dsh-license-obligation-proof](https://github.com/dongsheng123132/dsh-license-obligation-proof) | 0 | 2026-08-27 | 2026-08-27 | Evidence-only DSH plugin for license obligation delivery closure |
| 1624 | [dongsheng123132/dsh-policy-waiver-proof](https://github.com/dongsheng123132/dsh-policy-waiver-proof) | 0 | 2026-08-25 | 2026-08-26 | Offline content-addressed proof that temporary DSH policy waivers stayed within approved bounds |
| 1625 | [dongsheng123132/dsh-principal-binding-proof](https://github.com/dongsheng123132/dsh-principal-binding-proof) | 0 | 2026-08-25 | 2026-08-26 | Offline content-addressed proof of pseudonymous authority binding across DSH execution surfaces |
| 1626 | [dongsheng123132/dsh-reproducible-build-proof](https://github.com/dongsheng123132/dsh-reproducible-build-proof) | 0 | 2026-08-26 | 2026-08-26 | Offline content-addressed proof that independent build receipts reproduced byte-identical specified artifacts |
| 1627 | [dongsheng123132/dsh-retention-settlement-proof](https://github.com/dongsheng123132/dsh-retention-settlement-proof) | 0 | 2026-08-25 | 2026-08-25 | Body-free retention settlement and non-resurrection evidence for DeepSeek Harness |
| 1628 | [dongsheng123132/dsh-tool-surface-proof](https://github.com/dongsheng123132/dsh-tool-surface-proof) | 0 | 2026-08-25 | 2026-08-26 | Deployment-scoped model-visible DSH tool surface conformance evidence |
| 1629 | [dongsheng123132/dsh-vulnerability-remediation-proof](https://github.com/dongsheng123132/dsh-vulnerability-remediation-proof) | 0 | 2026-08-27 | 2026-08-27 | Evidence-only DSH plugin for vulnerability remediation closure |
| 1630 | [dongsheng123132/dsh-windows-settlement-proof](https://github.com/dongsheng123132/dsh-windows-settlement-proof) | 0 | 2026-08-25 | 2026-08-26 | Offline content-addressed proof that approved Windows control-plane changes settled across required surfaces |
| 1631 | [donoteatme/dsh-local-link](https://github.com/donoteatme/dsh-local-link) | 0 | 2026-08-27 | 2026-08-28 | Lightweight DeepSeek Harness plugin for paired LAN access: scan a QR code and continue the current DSH Web session from any phone, tablet, or computer. |
| 1632 | [DoshinJiu/dsh-ui-boost](https://github.com/DoshinJiu/dsh-ui-boost) | 0 | 2026-08-29 | 2026-08-29 | deepseek harness界面调色插件/RGB滑块调色 |
| 1633 | [DosterBool/dsh-zombie-gc](https://github.com/DosterBool/dsh-zombie-gc) | 0 | 2026-08-22 | 2026-08-22 | DSH 插件：开机清理僵尸 agent（已收尾会话仍挂 registry，导致退出重进后输入框卡死） |
| 1634 | [dougen/dsh-deepseek-usage](https://github.com/dougen/dsh-deepseek-usage) | 0 | 2026-08-23 | 2026-08-23 | DeepSeek usage sidebar plugin for DeepSeek Harness: account balance (official API), current unit pricing and peak/off-peak indicator, zh/en UI. |
| 1635 | [DreamZhongJu/dsh-smart-model-router](https://github.com/DreamZhongJu/dsh-smart-model-router) | 0 | 2026-08-23 | 2026-08-24 | A configurable Smart Model Router bundle for DeepSeek Harness (DSH). |
| 1636 | [dsh-plugins/dsh-network-settings](https://github.com/dsh-plugins/dsh-network-settings) | 0 | 2026-08-21 | 2026-08-22 | A DeepSeek Harness plugin that bundles three network capabilities — User-Agent rewriting (from @dsh-plugin/dsh-user-agent), a HTTP / HTTPS-CONNECT / SOCKS5 proxy (from dsh-net-proxy), and configurable request auto-retry — all driven from a single 网络设置 (Network) tab in the Web settings. |
| 1637 | [dsh-plugins/dsh-plugin-market](https://github.com/dsh-plugins/dsh-plugin-market) | 0 | 2026-08-26 | 2026-08-26 | A structured plugin marketplace for DeepSeek Harness — each plugin described as JSON, auto-aggregated into a single plugins.json for the dsh-plugins.github.io site. DeepSeek Harness 结构化插件市场 —— 每个插件以 JSON 描述，自动聚合为单一 plugins.json 供 dsh-plugins.github.io 站点消费。 |
| 1638 | [dsh-plugins/dsh-user-agent](https://github.com/dsh-plugins/dsh-user-agent) | 0 | 2026-08-21 | 2026-08-22 | Rewrites the User-Agent sent by every outgoing HTTP request (LLM API calls and other global-fetch traffic) to a value of your choice, configured live from a dedicated UA 设置 (User-Agent) tab in the Web settings. 为 dsh 发出的所有出站 HTTP 请求（LLM API 调用等走全局 fetch 的流量）改写 User-Agent，并可在 Web 设置的 UA 设置 选项卡中实时配置。 |
| 1639 | [dshworks/dsh-ego-browser](https://github.com/dshworks/dsh-ego-browser) | 0 | 2026-08-24 | 2026-08-24 | ego lite browser automation for dsh that remembers — recall a site's learned tools, promote a working script into a new one, hand the user the keyboard for real. 7 tools, host-only, MIT. |
| 1640 | [dubeno/dsh-agent-plugin-bridge](https://github.com/dubeno/dsh-agent-plugin-bridge) | 0 | 2026-08-20 | 2026-08-25 | 将符合Agent Plugin规范的插件适配到DSH生态 |
| 1641 | [dujar/dsh-community-plugins](https://github.com/dujar/dsh-community-plugins) | 0 | 2026-08-25 | 2026-08-25 | DeepSeek Harness web-GUI plugin: discover and install community plugins from the dsh-plugin topic — searchable SQLite catalog, fork browser, local-plugin installs |
| 1642 | [dujar/dsh-restart](https://github.com/dujar/dsh-restart) | 0 | 2026-08-25 | 2026-08-25 | DeepSeek Harness web-GUI plugin: restart dsh web in one click, toggle installed plugins, git panel for local checkouts |
| 1643 | [dusbin/dsh-attention](https://github.com/dusbin/dsh-attention) | 0 | 2026-08-30 | 2026-08-30 | 任务完成后进行提醒，发完任务就可以去喝杯咖啡了，完成了会叫你的 |
| 1644 | [dusbin/dsh-multi-tenant](https://github.com/dusbin/dsh-multi-tenant) | 0 | 2026-08-29 | 2026-08-29 | dsh 支持多租户插件 |
| 1645 | [dusbin/voice-plugin](https://github.com/dusbin/voice-plugin) | 0 | 2026-08-27 | 2026-08-27 | Dsh(deepseek harness)语音输入插件 Ps: 朗读功能目前还不是很棒。 |
| 1646 | [dxsdyhm/dsh-adb-logcat](https://github.com/dxsdyhm/dsh-adb-logcat) | 0 | 2026-08-26 | 2026-08-26 | Android Studio-style ADB logcat viewer for the DSH Web GUI |
| 1647 | [dy395769511-star/dsh-pdf-to-word](https://github.com/dy395769511-star/dsh-pdf-to-word) | 0 | 2026-08-29 | 2026-08-29 | PDF to Word conversion plugin for DeepSeek Harness (dsh): PyMuPDF/PaddleOCR pipeline + LLM visual style verification |
| 1648 | [EasyTZ/dsh-git](https://github.com/EasyTZ/dsh-git) | 0 | 2026-08-27 | 2026-08-27 | Git panel plugin for DeepSeek Harness (dsh) — visual staging, commits, push and branch switching in the sidebar |
| 1649 | [EasyTZ/dsh-reveal-explorer](https://github.com/EasyTZ/dsh-reveal-explorer) | 0 | 2026-08-27 | 2026-08-27 | Reveal-in-file-manager plugin for DeepSeek Harness (dsh) — open the current workspace in your system file manager |
| 1650 | [EasyTZ/dsh-terminal-panel](https://github.com/EasyTZ/dsh-terminal-panel) | 0 | 2026-08-27 | 2026-08-27 | Terminal panel plugin for DeepSeek Harness (dsh) — run commands in the current workspace with streaming output |
| 1651 | [EasyTZ/dsh-ui-balance](https://github.com/EasyTZ/dsh-ui-balance) | 0 | 2026-08-27 | 2026-08-27 | Balance display plugin for DeepSeek Harness (dsh) — show your DeepSeek API balance under each reply |
| 1652 | [eehcx/dsh-gentle-engram](https://github.com/eehcx/dsh-gentle-engram) | 0 | 2026-08-26 | 2026-08-27 | DSH adapter for Engram — persistent memory bridge built with Cordis. |
| 1653 | [elevenmoon999/dsh-clash-proxy](https://github.com/elevenmoon999/dsh-clash-proxy) | 0 | 2026-08-25 | 2026-08-25 | 智能分流 · 自包含 · 上手简单 —— DeepSeek Harness 规则分流代理插件（国内直连 / 国外走订阅节点），完全由 AI 生成。 |
| 1654 | [elonnzhang/dsh-plugin-template](https://github.com/elonnzhang/dsh-plugin-template) | 0 | 2026-08-21 | 2026-08-23 | DeepSeek Harness (dsh) 插件开发模版：最小化模版 + 全能力模版，含构建方式与加载到 dsh 的完整路径 |
| 1655 | [elonnzhang/dsh-system-prompt](https://github.com/elonnzhang/dsh-system-prompt) | 0 | 2026-08-23 | 2026-08-23 | DeepSeek Harness plugin for session-scoped system prompt inspection |
| 1656 | [emircanerkul/dsh-terminal](https://github.com/emircanerkul/dsh-terminal) | 0 | 2026-08-18 | 2026-08-24 | Workspace-aware web terminal plugin for the DeepSeek Harness (dsh). Runs a streaming PTY terminal at /terminal and embeds a split-pane terminal dock powered by xterm.js. |
| 1657 | [EmptyCollin/dsh-peak-valley-queue](https://github.com/EmptyCollin/dsh-peak-valley-queue) | 0 | 2026-08-27 | 2026-08-27 | Peak/valley pricing task queue for DeepSeek Harness |
| 1658 | [entireyu/dsh-webui-plus](https://github.com/entireyu/dsh-webui-plus) | 0 | 2026-08-25 | 2026-08-25 | DeepSeek Harness Webui 增强插件，自带对话锚点、归档任务等功能 |
| 1659 | [esonx/dsh-workforce](https://github.com/esonx/dsh-workforce) | 0 | 2026-08-23 | 2026-08-23 | Project-scoped organization and long-lived AI workforce layer for DeepSeek Harness |
| 1660 | [ESxyzbil/dsh-official-document-mode](https://github.com/ESxyzbil/dsh-official-document-mode) | 0 | 2026-08-22 | 2026-08-23 | DSH ??????:?????? + ??????? + ???? |
| 1661 | [Ever0330/universal-vision](https://github.com/Ever0330/universal-vision) | 0 | 2026-08-24 | 2026-08-24 | Universal vision-model plugin for DeepSeek Harness, enabling image description using any configured vision model. |
| 1662 | [eversko/dsh-blackbox](https://github.com/eversko/dsh-blackbox) | 0 | 2026-08-24 | 2026-08-25 | Privacy-safe flight recorder and incident reports for DeepSeek Harness. |
| 1663 | [EvieHe/dsh-resume-headless](https://github.com/EvieHe/dsh-resume-headless) | 0 | 2026-08-24 | 2026-08-24 | DeepSeek Harness (dsh) bundle: headless one-shot session resume. `dsh --profile headless --resume <session-id> "task"` continues a persisted session (history and turn numbering carry on), prints and exits. Overrides the official headless runner via ctx.agents.resume(); install with `dsh plugin add github:EvieHe/dsh-resume-headless#v0.1.1`. |
| 1664 | [evlon/deepseek-harness-launcher](https://github.com/evlon/deepseek-harness-launcher) | 0 | 2026-08-28 | 2026-08-29 | 托盘常驻的 DeepSeek Harness 安装 / 启动器（Tauri 2 无窗口应用，仅系统托盘 + 原生通知 + 日志文件） |
| 1665 | [evlon/dsh-codebuddy-models](https://github.com/evlon/dsh-codebuddy-models) | 0 | 2026-08-26 | 2026-08-29 | 把本机已登录的 CodeBuddy / WorkBuddy（腾讯代码助手） 订阅作为 dsh（DeepSeek Harness） 的原生 provider 接入，启用后 CodeBuddy 模型会直接出现在 dsh 的模型选择器中，可像其它模型一样被 agent 调用。 |
| 1666 | [evlon/dsh-matrix-agent](https://github.com/evlon/dsh-matrix-agent) | 0 | 2026-08-27 | 2026-08-29 | DeepSeek Harness（dsh）的 Matrix agent 桥接插件：把 Matrix 房间桥接到 harness agent 会话，每个房间一个会话，支持在聊天里远程监控、审批和追加指令；多分身架构 + 媒体/富文本/回复/编辑信息完整处理。 |
| 1667 | [Exception-H/dsh-gpt56-ptc](https://github.com/Exception-H/dsh-gpt56-ptc) | 0 | 2026-08-30 | 2026-08-30 | Native DSH Bundle: user-owned pure PTC / Code Mode preset for GPT-5.6 with plain-language answers and bounded execution. |
| 1668 | [Fabian-698/dsh-plugin-dev](https://github.com/Fabian-698/dsh-plugin-dev) | 0 | 2026-08-25 | 2026-08-25 | DeepSeek Harness (DSH) plugin development agent skill: 6 form typology, verify-plugin.mjs P1-P13 gate, scaffold generator, security discipline, and curated ecosystem backfills. An Agent Skill (SKILL.md), not an npm bundle. |
| 1669 | [FADE-4869/dsh-gacha-viz](https://github.com/FADE-4869/dsh-gacha-viz) | 0 | 2026-08-26 | 2026-08-27 | Genshin Impact gacha history visualizer and pity probability calculator for DeepSeek Harness (DSH plugin) |
| 1670 | [fan56/dsh-ask-router](https://github.com/fan56/dsh-ask-router) | 0 | 2026-08-25 | 2026-08-29 | dsh plugin: multi-surface ask-user routing, first answer wins |
| 1671 | [fan56/dsh-dcp](https://github.com/fan56/dsh-dcp) | 0 | 2026-08-17 | 2026-08-28 | dsh plugin: deterministic context compression backend — zero LLM calls, reproducible compression |
| 1672 | [fan56/dsh-feishu](https://github.com/fan56/dsh-feishu) | 0 | 2026-08-23 | 2026-08-26 | dsh plugin: drive an existing dsh session from Feishu/Lark — outbound-only bot, /resume picker, run status card |
| 1673 | [fan56/dsh-llm-net-retry](https://github.com/fan56/dsh-llm-net-retry) | 0 | 2026-08-22 | 2026-08-22 | dsh plugin: bounded retry for gateway network_error failures the stock retry policy cannot classify |
| 1674 | [fan56/dsh-mcp-adapter](https://github.com/fan56/dsh-mcp-adapter) | 0 | 2026-08-26 | 2026-08-29 | dsh plugin: fold mcp__* tool schemas into two meta-tools via prompt-side shim to save tokens |
| 1675 | [fan56/dsh-web-search-anysearch](https://github.com/fan56/dsh-web-search-anysearch) | 0 | 2026-08-26 | 2026-08-29 | AnySearch web search provider plugin for DeepSeek Harness (dsh) — zero-config, out-of-the-box |
| 1676 | [fan56/dsh-web-search-tavily](https://github.com/fan56/dsh-web-search-tavily) | 0 | 2026-08-25 | 2026-08-29 | Tavily web search provider plugin for DeepSeek Harness (dsh) |
| 1677 | [fanfan6/dsh-model-search](https://github.com/fanfan6/dsh-model-search) | 0 | 2026-08-22 | 2026-08-22 | DSH 模型搜索插件 - 跨平台快速筛选模型 |
| 1678 | [fantasyce/dsh-typelens](https://github.com/fantasyce/dsh-typelens) | 0 | 2026-08-27 | 2026-08-28 | Automatic bounded type context and edit diagnostics for DeepSeek Harness |
| 1679 | [Fast-Editor/lynkr-dsh-plugin](https://github.com/Fast-Editor/lynkr-dsh-plugin) | 0 | 2026-08-28 | 2026-08-28 | DeepSeek Harness (dsh) plugin: registers Lynkr as a custom OpenAI-compatible provider |
| 1680 | [fastengiel-kurai/dsh-peekfile-everything](https://github.com/fastengiel-kurai/dsh-peekfile-everything) | 0 | 2026-08-19 | 2026-08-22 | DSH local file search, clickable path detection, and floating preview plugin with optional EverythingCLI integration. |
| 1681 | [fatatalia/dsh-ledger](https://github.com/fatatalia/dsh-ledger) | 0 | 2026-08-18 | 2026-08-25 | dsh 只读记账仪表盘插件：会话页「记账」Tab 展示 beancount 账本月度快照（收支总览/资产结构动态分组/支出分类/最近交易），只读，复用 ledger.py，Fava 保留做深度分析 |
| 1682 | [fatatalia/dsh-turn-guard](https://github.com/fatatalia/dsh-turn-guard) | 0 | 2026-08-23 | 2026-08-25 | dsh turn-guard plugin: per-step timeout for agent turns (防模型退化死循环) |
| 1683 | [faye0526/dsh-backup-btn](https://github.com/faye0526/dsh-backup-btn) | 0 | 2026-08-26 | 2026-08-26 | DSH 一键备份按钮 - 浮动按钮备份 DSH 数据到 GitHub Gist |
| 1684 | [fbzz/readproof](https://github.com/fbzz/readproof) | 0 | 2026-08-21 | 2026-08-22 | Readproof — the lockfile and replay primitive for what AI agents read: stable identity, freshness policy, content-addressed snapshots, per-run manifests, diff, byte-exact replay, evidence bundles. |
| 1685 | [FeatureAgents/AgentsGitFlowController](https://github.com/FeatureAgents/AgentsGitFlowController) | 0 | 2026-08-17 | 2026-08-28 | Agents Client Level Git Flow Controller |
| 1686 | [felix-lj-ct/dsh-mcp-live-status](https://github.com/felix-lj-ct/dsh-mcp-live-status) | 0 | 2026-08-28 | 2026-08-28 | Adds a status pill to the DeepSeek Harness web composer tool row: how many configured MCP servers are actually reachable, plus per-server transport, tool count and failure reason on click. Surfaces what the settings page cannot — a server that mounted fine but never finished its MCP handshake. Read-only, no config needed. |
| 1687 | [fentz26/dsh-goodjob](https://github.com/fentz26/dsh-goodjob) | 0 | 2026-08-26 | 2026-08-27 | Multi-agent operations workspace for DeepSeek Harness. |
| 1688 | [fentz26/dsh-next](https://github.com/fentz26/dsh-next) | 0 | 2026-08-26 | 2026-08-27 | Performance-oriented backend/runtime modernization layer for DeepSeek Harness. |
| 1689 | [firestige/wsr-dsh](https://github.com/firestige/wsr-dsh) | 0 | 2026-08-29 | 2026-08-29 | WSR integrations for DeepSeek Harness: Execution, Studio, and suite bundles. |
| 1690 | [firestige/wsr-execution](https://github.com/firestige/wsr-execution) | 0 | 2026-08-17 | 2026-08-30 | Host-neutral execution boundary for workflow-self-recursive: resolves one exact Workflow Package, binds an immutable Delivery Manifest, coordinates the Delivery, emits bounded OTLP observations. Install via dsh plugin add wsr-dsh-intake · 与宿主无关的 Agent 工作流执行边界：解析并校验确定的工作流包，绑定不可变交付清单，协调交付并发出有界观测。 |
| 1691 | [Fisfzy/dsh-danus](https://github.com/Fisfzy/dsh-danus) | 0 | 2026-08-23 | 2026-08-25 | Verifier-gated multi-agent mathematical proof-search orchestration, native to DeepSeek Harness: content-addressed fact graph, role-gated tools, cold-start verifier, worker swarm, paper/report rendering. TypeScript, cross-platform. Based on Danus (frenzymath). |
| 1692 | [fishfromsky/dsh-march7th-skin](https://github.com/fishfromsky/dsh-march7th-skin) | 0 | 2026-08-20 | 2026-08-27 | 崩坏星穹铁道三月七主题的deepseek harness皮肤插件 |
| 1693 | [fishOfOUC/plugin-ui-controls](https://github.com/fishOfOUC/plugin-ui-controls) | 0 | 2026-08-23 | 2026-08-23 | Plugin control composer panel: the conversation.input.plugins seat over the pluginInventory Remote |
| 1694 | [FlameTN7/dsh-tui-browser-use](https://github.com/FlameTN7/dsh-tui-browser-use) | 0 | 2026-08-25 | 2026-08-31 | Browser automation bridge sub-plugin for dsh-tui |
| 1695 | [Flan246/dsh-latex-guard](https://github.com/Flan246/dsh-latex-guard) | 0 | 2026-08-26 | 2026-08-26 | LaTeX compile check and BibTeX lint/fill/audit tools for DeepSeek Harness and any agent. dsh plugin + CLI + SKILL.md. |
| 1696 | [Flan246/dsh-lit-search](https://github.com/Flan246/dsh-lit-search) | 0 | 2026-08-26 | 2026-08-26 | Academic literature search, citation and BibTeX tools for DeepSeek Harness and any agent (Crossref + OpenAlex). dsh plugin + CLI + SKILL.md. |
| 1697 | [flashyiyi/dsh-envelope-highlight](https://github.com/flashyiyi/dsh-envelope-highlight) | 0 | 2026-08-28 | 2026-08-28 | Restore syntax highlighting of read/write tool envelopes inside run_code (PTC / Code Mode) result cards |
| 1698 | [FloatingLifeTL/dsh-plugin_session-manager-custom](https://github.com/FloatingLifeTL/dsh-plugin_session-manager-custom) | 0 | 2026-08-22 | 2026-08-24 | DeepSeek Harness Web plugin for local session data management \| 当前项目仓库暂停开发且作归档状态 |
| 1699 | [Flonger/dsh-balance-vision](https://github.com/Flonger/dsh-balance-vision) | 0 | 2026-08-25 | 2026-08-25 | DeepSeek balance & session cost for DSH web UI, with official weekday peak/off-peak pricing and deepseek-v4-flash-vision-exp vision model support (same rate as flash) |
| 1700 | [Flonger/dsh-multi-clear](https://github.com/Flonger/dsh-multi-clear) | 0 | 2026-08-25 | 2026-08-26 | Multi-select clear (archive) workspace conversations and bulk-delete empty workspaces in the DSH sidebar, with workspace-level selection, tri-state checkboxes and confirm dialogs |
| 1701 | [flowingboy/dsh-local-perf](https://github.com/flowingboy/dsh-local-perf) | 0 | 2026-08-23 | 2026-08-23 | Durable DeepSeek Harness bundle: local-model performance tuning as a re-installable plugin layer (compaction, tool-result pruning, time context, cloud title routing, text-toolcall guard) — survives dsh updates |
| 1702 | [fly1989/dsh-deliberation](https://github.com/fly1989/dsh-deliberation) | 0 | 2026-08-20 | 2026-08-31 | Primary-controlled deliberation and opt-in reasoning-masked review for DeepSeek Harness. |
| 1703 | [flyingfishzxf/dsh-dsbal](https://github.com/flyingfishzxf/dsh-dsbal) | 0 | 2026-08-18 | 2026-08-27 | A simple DeepSeek API balance display plugin for dsh(deepseek-harness) |
| 1704 | [flymysql/dsh-browser-client](https://github.com/flymysql/dsh-browser-client) | 0 | 2026-08-23 | 2026-08-31 | DSH Browser Client — LLM 驱动的浏览器浮窗工作流工具（面向非研发人员的网页自动化） |
| 1705 | [FMDD61/dsh-oauth-copilot](https://github.com/FMDD61/dsh-oauth-copilot) | 0 | 2026-08-23 | 2026-08-24 | GitHub Copilot OAuth sign-in and model route for DeepSeek Harness |
| 1706 | [fogmodel/dsh-workspace-jump](https://github.com/fogmodel/dsh-workspace-jump) | 0 | 2026-08-23 | 2026-08-23 | DSH web plugin: quickly create or switch to a workspace from a directory path via the sidebar Workspace button. |
| 1707 | [force-push/dsh-llm-fallback](https://github.com/force-push/dsh-llm-fallback) | 0 | 2026-08-27 | 2026-08-27 | Self-healing cross-provider model fallback plugin for the DeepSeek Harness (DSH) — retries exhausted, re-bind the session to the next healthy model. |
| 1708 | [founder987/dsh-dev-ui](https://github.com/founder987/dsh-dev-ui) | 0 | 2026-08-25 | 2026-08-26 | 适合编码研发的UI界面 |
| 1709 | [fplj-fplj/dsh-ua-headers](https://github.com/fplj-fplj/dsh-ua-headers) | 0 | 2026-08-23 | 2026-08-25 | 为 DeepSeek Harness (DSH) 定制的 User-Agent 与请求头插件：按模型匹配改写 UA / 合并自定义请求头，遵循 dsh-ecosystem-spec 生态规范。A dsh-ecosystem-spec compliant plugin to customize User-Agent and request headers per model. |
| 1710 | [Francesco502/dsh-quota](https://github.com/Francesco502/dsh-quota) | 0 | 2026-08-26 | 2026-08-26 | AI Quota and Token Usage Monitor for DeepSeek Harness (Codex, Cursor, Antigravity, OpenCode-Go) |
| 1711 | [Frank-NF/dsh-drop-md](https://github.com/Frank-NF/dsh-drop-md) | 0 | 2026-08-30 | 2026-08-30 | Drag-and-drop markdown enhancer for DeepSeek Harness (DSH): inline small files, @-reference large ones, one-click SKILL.md install |
| 1712 | [frank6892103/dsh-WutheringWaves](https://github.com/frank6892103/dsh-WutheringWaves) | 0 | 2026-08-30 | 2026-08-31 | dsh鸣潮主题插件 |
| 1713 | [frederico-kluser/dsh-plugin-dev-agent-skill](https://github.com/frederico-kluser/dsh-plugin-dev-agent-skill) | 0 | 2026-08-22 | 2026-08-22 | Global agent skill: create, extend, secure, test and publish Cordis plugins for the DeepSeek Harness (DSH). Verified-by-measurement API surface (ctx.webServer, spawn(spec)), frontend levers, IPC, security, testing, packaging & publishing. |
| 1714 | [freedomkk-qfeng/dsh-mail-assistant](https://github.com/freedomkk-qfeng/dsh-mail-assistant) | 0 | 2026-08-31 | 2026-08-31 | Standards-based IMAP/SMTP mail connector for DeepSeek Harness, enabling agents to read and send email with explicit user controls. |
| 1715 | [freedomkk-qfeng/dsh-oidc](https://github.com/freedomkk-qfeng/dsh-oidc) | 0 | 2026-08-30 | 2026-08-30 | Enterprise OIDC, secure API-key binding, declarative branding, and OpenAI-compatible model integration for DeepSeek Harness. |
| 1716 | [FriendsHL/dsh-agent-evolution](https://github.com/FriendsHL/dsh-agent-evolution) | 0 | 2026-08-26 | 2026-08-27 | Preset-composed Agent experiments and evolution primitives for DeepSeek Harness |
| 1717 | [fthuu/Tokan-dsh-token-analytics](https://github.com/fthuu/Tokan-dsh-token-analytics) | 0 | 2026-08-31 | 2026-08-31 | 精准 Token 洞察，实时追踪，智能优化提示和用量归因 Sharp token insights, real‑time tracking, smart optimization signals & attribution  |
| 1718 | [FYHC1/dsh-web-manager](https://github.com/FYHC1/dsh-web-manager) | 0 | 2026-08-20 | 2026-08-23 | dsh-plugin + Windows tray manager for DeepSeek Harness WebUI (dsh web): standalone Edge app-window with the official whale icon, quick-launch desktop shortcuts for Windows/WSL, systemd hosting, runtime bridge, self-update. Legacy shortcut-only plugin (v1.x): https://github.com/FYHC1/dsh-webui-installer |
| 1719 | [FYHC1/dsh-webui-installer](https://github.com/FYHC1/dsh-webui-installer) | 0 | 2026-08-20 | 2026-08-23 | Legacy dsh plugin (v1.x, EOL): one-click desktop shortcuts that launch the DeepSeek Harness WebUI (dsh web) as a standalone app window on Windows / WSL / Linux. Need tray-based background management (multi-instance, systemd, self-update)? Use dsh-web-manager instead: https://github.com/FYHC1/dsh-web-manager |
| 1720 | [GalaxyBatMan111/dsh-plugins](https://github.com/GalaxyBatMan111/dsh-plugins) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness (DSH) plugins: agent bridge (Claude Code/Codex/Marvis) + Ghidra reverse engineering bridge |
| 1721 | [Gan332/dsh-typography](https://github.com/Gan332/dsh-typography) | 0 | 2026-08-23 | 2026-08-23 | Typography plugin for DeepSeek Harness - independent interface & code fonts, online presets, zero-conversion local font library (woff2/ttf/otf) |
| 1722 | [Gaochenyuen/dsh-scopus-searcher](https://github.com/Gaochenyuen/dsh-scopus-searcher) | 0 | 2026-08-24 | 2026-08-25 | Deep literature research agent as a Deepseek-Harness preset powered by Scopus API. |
| 1723 | [gaowei-AFK/dsh-prompt-polish](https://github.com/gaowei-AFK/dsh-prompt-polish) | 0 | 2026-08-26 | 2026-08-26 | Prompt polish ✨ — one-click rewrite of rough input into a structured professional prompt for DeepSeek Harness WebUI |
| 1724 | [gausszhou/dsh-opencode-session-id](https://github.com/gausszhou/dsh-opencode-session-id) | 0 | 2026-08-22 | 2026-08-24 | dsh session IDs for opencode, zero config. |
| 1725 | [gausszhou/dsh-where-am-i](https://github.com/gausszhou/dsh-where-am-i) | 0 | 2026-08-20 | 2026-08-24 | Neofetch for DeepSeek Harness. |
| 1726 | [gavenma/dsh-autoresearch-preset](https://github.com/gavenma/dsh-autoresearch-preset) | 0 | 2026-08-25 | 2026-08-25 | AutoResearch Project Mode preset for DeepSeek Harness. |
| 1727 | [GavinQiEr/dsh-cmdwatch](https://github.com/GavinQiEr/dsh-cmdwatch) | 0 | 2026-08-30 | 2026-08-30 | Real-time command monitor for DeepSeek Harness (DSH). Watch foreground/background command output in the Web UI without pausing the conversation. 命令窗：实时显示 DSH 命令与执行输出。 |
| 1728 | [Gcd1949/dsh-tools](https://github.com/Gcd1949/dsh-tools) | 0 | 2026-08-21 | 2026-08-22 | DeepSeek Harness (dsh) utilities: session-manager plugin & Windows control panel |
| 1729 | [geeklei/dsh-plugins](https://github.com/geeklei/dsh-plugins) | 0 | 2026-08-29 | 2026-08-29 | 一个面向 DeepSeek Harness (dsh)的插件库 |
| 1730 | [geekyfoxlab/dsh-subagents](https://github.com/geekyfoxlab/dsh-subagents) | 0 | 2026-08-26 | 2026-08-26 | Focused child-agent delegation (scout, researcher, worker, reviewer, oracle, delegate) and multi-agent workflows (council, parallel review, review loop) for DeepSeek Harness. |
| 1731 | [ghbhiee/dsh-plugin-tui](https://github.com/ghbhiee/dsh-plugin-tui) | 0 | 2026-08-28 | 2026-08-28 | Claude Code-style terminal UI plugin for DeepSeek Harness (dsh): streaming REPL, collapsed thinking, interactive session/model pickers, history replay, approval modes, bottom status bar |
| 1732 | [Ghost011118/dsh-plugin-governor-extension](https://github.com/Ghost011118/dsh-plugin-governor-extension) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness plugin governance: installable runtime tool policy plus companion boot admission, supervised restart, and rollback. |
| 1733 | [Ghost011118/dsh-plugin-marketplace](https://github.com/Ghost011118/dsh-plugin-marketplace) | 0 | 2026-08-28 | 2026-08-29 | Built-in plugin discovery, local requirement matching, optional GitHub stars, and one-click installation for DeepSeek Harness. |
| 1734 | [GitNoHup/macaron-theme](https://github.com/GitNoHup/macaron-theme) | 0 | 2026-08-26 | 2026-08-26 | 🍬 马卡龙毛玻璃主题（Macaron Glassmorphism Theme）— DeepSeek Harness 动态主题插件：四套马卡龙配色、145° 双色渐变、毛玻璃卡片；日间上色 / 夜间自动清除并记忆恢复。 |
| 1735 | [gjjkbssg/dsh-model-jury](https://github.com/gjjkbssg/dsh-model-jury) | 0 | 2026-08-31 | 2026-08-31 | Structured cross-model peer review for DeepSeek Harness — blind reasoning, anonymous critique, revision, and deterministic verdicts. |
| 1736 | [Glazyonyt/dsh-lowtide](https://github.com/Glazyonyt/dsh-lowtide) | 0 | 2026-08-28 | 2026-08-28 | Queue AI tasks during off-peak hours to cut costs and automate runs with dsh-lowtide for DeepSeek Harness. |
| 1737 | [goatliamia/dsh-runtime](https://github.com/goatliamia/dsh-runtime) | 0 | 2026-08-31 | 2026-08-31 | Experimental Runtime capability repository for DeepSeek Harness: minimal seam + evidence-backed presets |
| 1738 | [GoldenZqqq/dsh-model-collapse](https://github.com/GoldenZqqq/dsh-model-collapse) | 0 | 2026-08-27 | 2026-08-27 | DSH web plugin: collapse the model picker by provider, with a pinned quick bar (expand-all / collapse-all / focus-current / filter / reset). |
| 1739 | [goldgish/dsh-gamepad-approval](https://github.com/goldgish/dsh-gamepad-approval) | 0 | 2026-08-30 | 2026-08-30 | Xbox 手柄硬件审批插件 for DeepSeek Harness (dsh) — Agent 高危工具调用需物理按键确认，A 批准 / B 驳回 |
| 1740 | [GooDAnDReaDY/dsh-gitea](https://github.com/GooDAnDReaDY/dsh-gitea) | 0 | 2026-08-31 | 2026-08-31 | Gitea/Forgejo toolkit for DeepSeek Harness: issues, PRs, CI, releases, operations |
| 1741 | [GooDAnDReaDY/dsh-grok-xsearch](https://github.com/GooDAnDReaDY/dsh-grok-xsearch) | 0 | 2026-08-21 | 2026-08-22 | Real-time X (Twitter) search tool for DeepSeek Harness agents powered by isolated SuperGrok OAuth |
| 1742 | [GooDAnDReaDY/dsh-live-canvas](https://github.com/GooDAnDReaDY/dsh-live-canvas) | 0 | 2026-08-31 | 2026-08-31 | Interactive in-browser canvas for real-time preview of HTML, React components, SVGs, and diagrams with SSE hot-reload in DeepSeek Harness |
| 1743 | [GooDAnDReaDY/dsh-messenger-gateway](https://github.com/GooDAnDReaDY/dsh-messenger-gateway) | 0 | 2026-08-26 | 2026-08-26 | Telegram messenger bridge for DeepSeek Harness: sessions, steer, homes, and TTS voice notes |
| 1744 | [GooDAnDReaDY/dsh-model-sync](https://github.com/GooDAnDReaDY/dsh-model-sync) | 0 | 2026-08-23 | 2026-08-25 | Automated provider model catalog discovery and quota balance monitoring for DeepSeek Harness |
| 1745 | [GooDAnDReaDY/dsh-time-machine](https://github.com/GooDAnDReaDY/dsh-time-machine) | 0 | 2026-08-31 | 2026-08-31 | DSH plugin for smart checkpoints, workspace safety guards, and instant rollback |
| 1746 | [GooDAnDReaDY/dsh-usage-guard](https://github.com/GooDAnDReaDY/dsh-usage-guard) | 0 | 2026-08-24 | 2026-08-25 | Session token-usage sanitizer preventing chat history corruption from malformed provider metrics |
| 1747 | [Gorilla-Kevv/scnu-thesis-formatter](https://github.com/Gorilla-Kevv/scnu-thesis-formatter) | 0 | 2026-08-30 | 2026-08-30 | 华南师范大学本科毕业论文格式改写 + matplotlib 数据可视化（DeepSeek Harness 技能） |
| 1748 | [GreenLv/dsh-completion-guard](https://github.com/GreenLv/dsh-completion-guard) | 0 | 2026-08-26 | 2026-08-29 | Task-contract and completion-certification layer for DeepSeek Harness |
| 1749 | [GroupWork888/dsh-plugin-archived-sessions](https://github.com/GroupWork888/dsh-plugin-archived-sessions) | 0 | 2026-08-25 | 2026-08-26 | Browse and read archived DeepSeek Harness sessions from a sidebar panel. A read-only viewer: it does not restore sessions to the sidebar. |
| 1750 | [grstein/dsh-locale-ptbr](https://github.com/grstein/dsh-locale-ptbr) | 0 | 2026-08-31 | 2026-08-31 | Pacote de idioma Português (Brasil) para a GUI Web do DeepSeek Harness |
| 1751 | [guangxiangwu6-cmd/dsh-llm-failover](https://github.com/guangxiangwu6-cmd/dsh-llm-failover) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness model auto-failover plugin: retry threshold -> mark unavailable -> seamless switch to next healthy model -> cooldown auto-recover. 18-model pool, 19/19 tests, boot-safe. |
| 1752 | [guazixiong/dsh-coding-mode-preset](https://github.com/guazixiong/dsh-coding-mode-preset) | 0 | 2026-08-30 | 2026-08-30 | 为本地 DeepSeek Harness（`@deepseek-ai/dsh`）追加一个**编码模式** Agent Preset：门禁式工程交付流水线，包含三条独立流程——**需求开发**、**Bug 修复**、**功能迭代**。每个阶段的产物由全新上下文的"空白子代理"独立专家评审，通过后须经用户确认才进入下一阶段；最终以用户验收作为任务完结条件。 |
| 1753 | [guo6x/dsh-shipcheck](https://github.com/guo6x/dsh-shipcheck) | 0 | 2026-08-25 | 2026-08-26 | Evidence-first frontend release checks for DeepSeek Harness: real browser inspection, visual baselines, and reproducible reports. |
| 1754 | [gychen-NJU/dsh-overleaf](https://github.com/gychen-NJU/dsh-overleaf) | 0 | 2026-08-27 | 2026-08-29 | Embedded Overleaf workbench tab for DeepSeek Harness Web: same-origin reverse proxy, direct-CDP login, selection quoting, caret insertion, LaTeX assist panel |
| 1755 | [Hanmingh/dsh-desktop](https://github.com/Hanmingh/dsh-desktop) | 0 | 2026-08-27 | 2026-08-27 | Desktop Plugin for Deepseek Harness |
| 1756 | [hanzhangzzz/dsh-computer-use](https://github.com/hanzhangzzz/dsh-computer-use) | 0 | 2026-08-25 | 2026-08-26 | Computer use plugin for DeepSeek Harness: structure-first browser driving over a Playwright provider |
| 1757 | [haohaiHuang/Design-Agent](https://github.com/haohaiHuang/Design-Agent) | 0 | 2026-08-27 | 2026-08-27 | DSH 设计 Agent 完整可复现包：design-references 路由技能（DSH 适配）+ design-router 确定性工具插件 + my-agent 预设 |
| 1758 | [HaoR325/dsh-usage-daily](https://github.com/HaoR325/dsh-usage-daily) | 0 | 2026-08-30 | 2026-08-31 | DSH 用量日报浮窗插件：今日令牌/消息/轮数/估算费用 |
| 1759 | [haoranwang0921/dsh-bid-desk](https://github.com/haoranwang0921/dsh-bid-desk) | 0 | 2026-08-28 | 2026-08-30 | DSH 投标合规工作台是一个 DSH 插件 MVP，服务于投标文件编制过程。它将招标来源证据、要求记录、人工复核决定和生成报告关联起来，帮助具备相应资质或经验的人员在提交前核查缺口。 |
| 1760 | [haoyu-qi/dsh-zentao](https://github.com/haoyu-qi/dsh-zentao) | 0 | 2026-08-15 | 2026-08-26 | 面向 DeepSeek Harness 的 AVCON Web 界面定制与个人禅道 CLI 工作中心 |
| 1761 | [haozheou/dsh-exam-expert](https://github.com/haozheou/dsh-exam-expert) | 0 | 2026-08-30 | 2026-08-30 | 出题专家 · Exam Expert plugin for DeepSeek Harness: 把出题流程固化成值守流水线（角色+目录→通读→勾选表单→六分身流水线→看板交付） \| Turn the exam-paper workflow into an agent-supervised pipeline: wizard dialog, prefilled checklist form, six-role dual-kanban production |
| 1762 | [harness-home/harness-ai-app](https://github.com/harness-home/harness-ai-app) | 0 | 2026-08-21 | 2026-08-26 | Mobile client for Harness AI — follow, answer and approve your hosted agent sessions from your phone. Expo + React Native, talks only to your own server. |
| 1763 | [harness-home/harness-ai-desktop](https://github.com/harness-home/harness-ai-desktop) | 0 | 2026-08-21 | 2026-08-26 | Desktop client for Harness AI — an Electron app that boots the DeepSeek Harness (dsh) agent runtime in-process on loopback, with hosted sessions, remote approvals and a gated plugin market. |
| 1764 | [harness-home/harness-ai-plugins](https://github.com/harness-home/harness-ai-plugins) | 0 | 2026-08-26 | 2026-08-26 | Community plugin catalog for Harness AI: a scanner over the public npm registry, and the snapshot it publishes. |
| 1765 | [Harzva/dsh-restart-autoresume](https://github.com/Harzva/dsh-restart-autoresume) | 0 | 2026-08-29 | 2026-08-29 | Safe DSH restart coordination and durable top-level session autoresume |
| 1766 | [haythamat/dsh-client-ui-rtl](https://github.com/haythamat/dsh-client-ui-rtl) | 0 | 2026-08-27 | 2026-08-27 | Right-to-left text direction for the DeepSeek Harness Web client |
| 1767 | [hecailiaoPFS/firecrawl-research-engine](https://github.com/hecailiaoPFS/firecrawl-research-engine) | 0 | 2026-08-24 | 2026-08-24 | Deep technical research & verification skill for LLM agents: Firecrawl search-first, graceful degradation, anti-hallucination citations. Works with DSH / Claude Code / Codex / Cursor. |
| 1768 | [hedging8563/tokenlab-deepseek-harness-provider](https://github.com/hedging8563/tokenlab-deepseek-harness-provider) | 0 | 2026-08-27 | 2026-08-27 | TokenLab native-protocol model provider, multimodal tools, and async tasks for DeepSeek Harness |
| 1769 | [hehetoshang/dsh-talebook-plugin](https://github.com/hehetoshang/dsh-talebook-plugin) | 0 | 2026-08-27 | 2026-08-30 | DeepSeek Harness plugin for safely operating Talebook |
| 1770 | [helibeiqi/dsh-cdp-metadata](https://github.com/helibeiqi/dsh-cdp-metadata) | 0 | 2026-08-23 | 2026-08-28 | Capability Description Protocol (CDP) v0.1 — read-only AI-readable capability metadata layer for DSH Cordis plugins. |
| 1771 | [helibeiqi/dsh-cn-disclosure](https://github.com/helibeiqi/dsh-cn-disclosure) | 0 | 2026-08-28 | 2026-08-28 | 零依赖本地优先的 A股 公告/年报 结构化抽取 MCP server (dsh-plugin) |
| 1772 | [helibeiqi/dsh-context-aware-search](https://github.com/helibeiqi/dsh-context-aware-search) | 0 | 2026-08-19 | 2026-08-28 | Context-aware web search plugin for DeepSeek Harness (dsh): rewrites queries with session context, reranks + credibility-tags results, one-click source summarization across multiple backends. Fully decoupled from @deepseek-ai private packages for public CI. |
| 1773 | [helibeiqi/dsh-dcs-engine](https://github.com/helibeiqi/dsh-dcs-engine) | 0 | 2026-08-24 | 2026-08-28 | Dynamic Capability Synthesis Engine — DSH protocol stack credit engine |
| 1774 | [helibeiqi/dsh-docx-mcp](https://github.com/helibeiqi/dsh-docx-mcp) | 0 | 2026-08-28 | 2026-08-28 | Zero-dependency MCP stdio server that generates real .docx files from a JSON spec — Chinese office-automation vertical for DeepSeek Harness. |
| 1775 | [helibeiqi/dsh-hr-payroll-mcp](https://github.com/helibeiqi/dsh-hr-payroll-mcp) | 0 | 2026-08-29 | 2026-08-29 | 通用 HR 算薪 MCP 服务：本地化法定社保/公积金/个税计算 + 通用表头适配 + 企业配置 + 安全绩效公式（PII 不出机） |
| 1776 | [helibeiqi/dsh-industry-graph-mcp](https://github.com/helibeiqi/dsh-industry-graph-mcp) | 0 | 2026-08-28 | 2026-08-28 | 零依赖本地优先的 A股 产业链/申万行业/概念板块 知识图谱 MCP server (dsh-plugin) |
| 1777 | [helibeiqi/dsh-intent-network](https://github.com/helibeiqi/dsh-intent-network) | 0 | 2026-08-23 | 2026-08-23 | 将用户意图解析为可编辑、可观测、可学习的多跳工具调用图，消费 CDP 语义与 adapter 桥接工具 |
| 1778 | [helibeiqi/dsh-memory-projection](https://github.com/helibeiqi/dsh-memory-projection) | 0 | 2026-08-20 | 2026-08-28 | Hot-pluggable memory-projection scheduling framework for DeepSeek Harness (dsh): pure-function projection strategies + a runtime invariant guard, built on the cordis plugin kernel. |
| 1779 | [helibeiqi/dsh-quant-factor-pipeline](https://github.com/helibeiqi/dsh-quant-factor-pipeline) | 0 | 2026-08-28 | 2026-08-28 | Quant factor research pipeline as a dsh user-layer MCP server (CGO disposal-effect factor, RankIC, Newey-West t, regime-aware) |
| 1780 | [hellofuture2068/dsh-simple-view](https://github.com/hellofuture2068/dsh-simple-view) | 0 | 2026-08-26 | 2026-08-26 | Declutter DeepSeek Harness chat: hide agent execution-log rows, tighten spacing & fonts, bubble messages, and set a "reply concisely" system-prompt instruction. |
| 1781 | [hellogit2021/avoid-ai-writing-cn](https://github.com/hellogit2021/avoid-ai-writing-cn) | 0 | 2026-08-29 | 2026-08-29 | 知乎"去AI味写作技巧"社区免费提供：中文写作去 AI 味插件（AI-isms / AI writing / humanize）。说"去掉AI味"即重写，说"写的不错"自动学习新 AI 词。安装：dsh plugin --profile web add github:hellogit2021/avoid-ai-writing-cn |
| 1782 | [helloworld1631/dsh-volcengine-usage](https://github.com/helloworld1631/dsh-volcengine-usage) | 0 | 2026-08-27 | 2026-08-27 | Draggable Volcengine Coding Plan usage monitor for DeepSeek Harness Web. |
| 1783 | [HellowVirgil/dsh-antv-ava](https://github.com/HellowVirgil/dsh-antv-ava) | 0 | 2026-08-25 | 2026-08-25 | AntV AVA plugin for DeepSeek Harness with streaming narrative text and charts |
| 1784 | [HenryHwong/dsh-ui-billing](https://github.com/HenryHwong/dsh-ui-billing) | 0 | 2026-08-25 | 2026-08-25 | Billing widget plugin for the DeepSeek Harness Web GUI: current-session cost and API balance at the sidebar foot (dsh-plugin) |
| 1785 | [HenryHwong/dsh-ui-turn-rail](https://github.com/HenryHwong/dsh-ui-turn-rail) | 0 | 2026-08-25 | 2026-08-25 | Turn progress rail plugin for the DeepSeek Harness Web GUI (dsh-plugin) |
| 1786 | [henrytang2011win-coder/dsh-task-sounds](https://github.com/henrytang2011win-coder/dsh-task-sounds) | 0 | 2026-08-25 | 2026-08-25 | 为你的DeepSeek harness添加任务结束和提问时的提示音 |
| 1787 | [hfyydd/dsh-cua](https://github.com/hfyydd/dsh-cua) | 0 | 2026-08-28 | 2026-08-28 | Computer Use for DeepSeek Harness, backed by the cua-driver daemon (trycua): UIA element-level targeting, background-first input delivery, deterministic verification. |
| 1788 | [hhb1028/dsh-client-ui-timeline](https://github.com/hhb1028/dsh-client-ui-timeline) | 0 | 2026-08-30 | 2026-08-30 | DSH Web GUI 会话问题导航条：聊天区左缘一问一杠，随滚动高亮当前问题、悬停显示问答预览气泡、点击把该问平滑滚到视口顶（未渲染的更早历史自动翻页加载），无需改动 dsh 本体源码 |
| 1789 | [higekibaka/dsh-ciel](https://github.com/higekibaka/dsh-ciel) | 0 | 2026-08-31 | 2026-08-31 | 夏尔 Ciel — a pre-planning advisor and convergent critic for DeepSeek Harness: a second, knowledge-rich model offering directions, prior art, pitfalls and verification checklists (ideas, never steps). |
| 1790 | [HiSeax/dsh-agent-outputs-reader](https://github.com/HiSeax/dsh-agent-outputs-reader) | 0 | 2026-08-29 | 2026-08-30 | Overlay reader for agent output files: Markdown/GFM rendering, in-panel PDF, DOCX/XLSX/PPTX text preview, reply-end file chips. Pure JS, zero deps. |
| 1791 | [HiSeax/dsh-better-model-setting](https://github.com/HiSeax/dsh-better-model-setting) | 0 | 2026-08-23 | 2026-08-29 | DSH plugin: replaces official Models settings page with provider management, per-model reasoning effort, retry overrides, drag reorder, add official DeepSeek, credential status |
| 1792 | [Hjay1101/dsh-ios-control](https://github.com/Hjay1101/dsh-ios-control) | 0 | 2026-08-22 | 2026-08-22 | DeepSeek Harness 插件：手机扫码遥控电脑上的 agent —— 在 dsh-remote-link 基础上增强会话持久化（dsh 重启后已配对设备保持登录）、iOS 主屏图标等 |
| 1793 | [hjdhnx/dsh-desktop](https://github.com/hjdhnx/dsh-desktop) | 0 | 2026-08-22 | 2026-08-23 | DeepSeek Harness 桌面端 -- 从 Electron 迁移到 Tauri(Rust 壳 + Node Sidecar)架构 |
| 1794 | [hmlyx/dsh-memory](https://github.com/hmlyx/dsh-memory) | 0 | 2026-08-29 | 2026-08-29 | 简单的插件，让你的每个 AI 记录经验和记忆 |
| 1795 | [hmlyx/dsh-notify](https://github.com/hmlyx/dsh-notify) | 0 | 2026-08-29 | 2026-08-29 | 在输入框右边加了一个泡泡窗口，你可以接入插件或者告诉 AI 什么时候使用它。 |
| 1796 | [hnlisf/dsh-crypto-analyst](https://github.com/hnlisf/dsh-crypto-analyst) | 0 | 2026-08-24 | 2026-08-24 | 加密货币深度调研智能体 DSH 插件：5 步思维链研报 + 报告工作台 + 数据可视化 + MD/PDF 导出 |
| 1797 | [Hoemr/dsh-quicklook](https://github.com/Hoemr/dsh-quicklook) | 0 | 2026-08-24 | 2026-08-24 | QuickLook-style space-key large preview for DSH better-sidebar: press Space on the active file tab for an instant image/PDF/text overlay |
| 1798 | [honlnk/dsh-input-assist](https://github.com/honlnk/dsh-input-assist) | 0 | 2026-08-23 | 2026-08-25 | Input assistant for DeepSeek Harness Web UI: inline AI completion (FIM) and Chinese-friendly typo checking |
| 1799 | [honoriomelo/dsh-model-picker-search](https://github.com/honoriomelo/dsh-model-picker-search) | 0 | 2026-08-29 | 2026-08-29 | DSH Web GUI plugin: adds a live search field inside the model picker menu of the composer, plus the Effort (reasoning) selector. Drop-in replacement for the native model seat, sharing the same per-session ModelDirectory so /model popup, the effort selector, and the /model command stay consistent. |
| 1800 | [horizon105457/tsstream](https://github.com/horizon105457/tsstream) | 0 | 2026-08-26 | 2026-08-26 | 🌊 Agent-native time-series streaming for DeepSeek Harness (DSH plugin) — terminal/serial byte streams → indexed, queryable, event-driven timeline. 19 tools · 9 operators · 🧪 experimental |
| 1801 | [Hoshino-Yumetsuki/as-compatible-copilot](https://github.com/Hoshino-Yumetsuki/as-compatible-copilot) | 0 | 2026-08-01 | 2026-08-29 | A VSCode extension to use Openai/Anthropic/Gemini API Providers in GitHub Copilot Chat |
| 1802 | [hpyer/dsh-for-mac](https://github.com/hpyer/dsh-for-mac) | 0 | 2026-08-31 | 2026-08-31 | DshForMac 是 DeepSeek Harness 的原生 macOS 启动器与运行时管理器，提供本地环境检测、版本管理及内嵌 Web 界面。 |
| 1803 | [hrhgit/dsh-model-manager](https://github.com/hrhgit/dsh-model-manager) | 0 | 2026-08-14 | 2026-08-31 | Model tags, reasoning capabilities, image routing, and vision proxy support for DeepSeek Harness |
| 1804 | [htfc786/dsh-awake](https://github.com/htfc786/dsh-awake) | 0 | 2026-08-16 | 2026-08-23 | dsh-awake · 守夜人：在 agent 任务执行期间阻止操作系统休眠 |
| 1805 | [hu669293657/dsh-turn-tools](https://github.com/hu669293657/dsh-turn-tools) | 0 | 2026-08-29 | 2026-08-29 | DSH web plugin: per-turn deliverable buttons (open with the OS default app) and a turn-navigator dot rail for jumping between conversation turns. |
| 1806 | [huangDouP/dsh-client-ui-notifications](https://github.com/huangDouP/dsh-client-ui-notifications) | 0 | 2026-08-29 | 2026-08-29 | DSH Web notifications: browser notifications, tab title flash, favicon badge, and native Windows toasts with a bilingual (zh/en) settings page. |
| 1807 | [huangfuren/dsh-outline-auto](https://github.com/huangfuren/dsh-outline-auto) | 0 | 2026-08-25 | 2026-08-29 | DSH (DeepSeek Harness) web plugin: search and read company Outline knowledge base documents from conversations (outline_search / outline_get_document). |
| 1808 | [HuangLM03/dsh-plugin-session-archive](https://github.com/HuangLM03/dsh-plugin-session-archive) | 0 | 2026-08-31 | 2026-08-31 | Browse and permanently delete archived DeepSeek Harness sessions from the sidebar footer. |
| 1809 | [HuanLinOTO/dsh-plugin-copilot](https://github.com/HuanLinOTO/dsh-plugin-copilot) | 0 | 2026-08-28 | 2026-08-28 | Copilot 引导层插件：WebUI 设置卡片一键 GitHub 授权 + 自动激活模型路由并收窄模型列表（复用 dsh-llm-pi-ai 内置 device-flow） \| Copilot onboarding plugin: one-click GitHub auth from the WebUI settings card, auto-activating the model route and narrowing the model list (reuses dsh-llm-pi-ai's builtin device flow) |
| 1810 | [HuanLinOTO/dsh-plugin-tools-manager](https://github.com/HuanLinOTO/dsh-plugin-tools-manager) | 0 | 2026-08-14 | 2026-08-28 | DSH 工具管理器：查看/启停宿主已注册工具 \| DSH tools manager: inspect and toggle host-registered tools |
| 1811 | [HuanyuTan777/dsh-tool-pdf](https://github.com/HuanyuTan777/dsh-tool-pdf) | 0 | 2026-08-28 | 2026-08-28 | DSH PDF reader plugin (pdf_info / pdf_extract / pdf_render) |
| 1812 | [Huauauaa/dsh-chatbi](https://github.com/Huauauaa/dsh-chatbi) | 0 | 2026-08-24 | 2026-08-24 | a chatbi dsh |
| 1813 | [huaxiren6/DSH-QrPairing](https://github.com/huaxiren6/DSH-QrPairing) | 0 | 2026-08-19 | 2026-08-27 | Floating phone-pairing QR button for the DSH WebUI. Companion UI for dsh-remote-link. |
| 1814 | [huermi/dsh-JEPA-adapter](https://github.com/huermi/dsh-JEPA-adapter) | 0 | 2026-08-24 | 2026-08-25 | 适配调用JEPA模型的插件，提供一个本地的JEPA模型项目（需要进一步训练持续学习，已完成基本工具调用），可在家用计算机配置上运行。A plugin adapted to call the JEPA model, providing a local JEPA model project (requires further training for continual learning; basic tool calling has been completed) that can run on a home computer CPU. |
| 1815 | [HULILI-com/dsh-namecheck](https://github.com/HULILI-com/dsh-namecheck) | 0 | 2026-08-26 | 2026-08-26 | dsh plugin for checking domain availability and trademark screening of candidate product names |
| 1816 | [hun1315/dsh-msi-icons](https://github.com/hun1315/dsh-msi-icons) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness 模型选择器美化插件：厂商官方图标 + 四区平铺 + 置顶主力超时自动路由 \| Model selector beautifier for DSH: official vendor icons, pinned-first flat layout, first-token-timeout failover |
| 1817 | [hunbs-1/dsh-codepect](https://github.com/hunbs-1/dsh-codepect) | 0 | 2026-08-29 | 2026-08-30 | dsh-codepect is a DSH plugin generating OpenAPI 3.0 from TS/JS. Features: visual docs, versioning, change detection, mock & auto-rescan. Zero-dep, offline, ensures code-doc sync for backend API delivery. dsh-codepect是DSH插件，扫描TS/JS生成OpenAPI3.0文档。支持可视化、多版本、变更检测、Mock及自动重扫。零依赖离线可用，确保代码文档一致，助后端交付API契约。 |
| 1818 | [hunterxxn/deep-flow](https://github.com/hunterxxn/deep-flow) | 0 | 2026-08-14 | 2026-08-29 | deepseek-harness tui |
| 1819 | [huyang2024/dsh-openai-api](https://github.com/huyang2024/dsh-openai-api) | 0 | 2026-08-27 | 2026-08-27 | OpenAI-compatible HTTP surface for DeepSeek Harness (dsh): POST /v1/chat/completions, POST /v1/responses, GET /v1/models over the harness webServer + llm runtime |
| 1820 | [hxt9805/dsh-remote-tailscale](https://github.com/hxt9805/dsh-remote-tailscale) | 0 | 2026-08-22 | 2026-08-22 | DSH plugin: open the local DSH web UI on your other Tailscale devices |
| 1821 | [hyperion2144/dsh-desktop-tauriapp](https://github.com/hyperion2144/dsh-desktop-tauriapp) | 0 | 2026-08-18 | 2026-08-23 | Tauri 2 desktop shell wrapping the DeepSeek Harness Web GUI (macOS + Windows) — tray daemon, auto-launch/reuse of local dsh, --patch plugin injection, mobile access via LAN/tunnel pairing with cloudflared one-click tunnel. |
| 1822 | [hyperion2144/dsh-hashline-edittool](https://github.com/hyperion2144/dsh-hashline-edittool) | 0 | 2026-08-20 | 2026-08-22 | Hash-anchored read/edit/undo_last_edit tools for DeepSeek Harness (dsh) |
| 1823 | [hzthzt/dsh-summary-panel](https://github.com/hzthzt/dsh-summary-panel) | 0 | 2026-08-23 | 2026-08-23 | Extensible Codex-style pinned summary panel for DeepSeek Harness Web. |
| 1824 | [IcedWatermelonJuice/dsh-provider-veark](https://github.com/IcedWatermelonJuice/dsh-provider-veark) | 0 | 2026-08-30 | 2026-08-31 | 把火山方舟 Coding Plan 装进 DeepSeek Harness：文本 + 图片对话，图片走 Files API，密钥粘贴即用 |
| 1825 | [ichabodcole/dsh-plugin-monitor](https://github.com/ichabodcole/dsh-plugin-monitor) | 0 | 2026-08-25 | 2026-08-26 | A Deepseek harness monitor plugin.  |
| 1826 | [icyaaaww/dsh-tool-failure-circuit-breaker](https://github.com/icyaaaww/dsh-tool-failure-circuit-breaker) | 0 | 2026-08-24 | 2026-08-24 | DeepSeek Harness plugin that blocks repeated identical failed tool calls |
| 1827 | [icyaaaww/dsh-tui-secret-guard](https://github.com/icyaaaww/dsh-tui-secret-guard) | 0 | 2026-08-26 | 2026-08-26 | Blocks high-confidence secrets before dsh-TUI sends them to a model, compliant with dsh ecosystem manifest v0.15. |
| 1828 | [iguanren/Taishan-Vision](https://github.com/iguanren/Taishan-Vision) | 0 | 2026-08-29 | 2026-08-29 | 让 DeepSeek Harness 纯文本模型也能识图：默认推荐智谱 GLM-4.6V-FLASH和 GLM-4.1V-FLASH 免费视觉模型 |
| 1829 | [ihorleleka/Local-Rag-Wiki](https://github.com/ihorleleka/Local-Rag-Wiki) | 0 | 2026-06-03 | 2026-08-27 | A per-repository, Docker-hosted MCP knowledge service that gives coding agents a governed Markdown "wiki" with semantic retrieval. The promise — a local RAG wiki that accumulates durable project knowledge across agentic sessions. |
| 1830 | [IKEASven69/dsh-opencli](https://github.com/IKEASven69/dsh-opencli) | 0 | 2026-08-30 | 2026-08-30 | 让 DeepSeek Harness (dsh) 会办事:登录态真实浏览器 + 170+ 站点适配器 + write 审批门 |
| 1831 | [ikomom/dsh-trade-chart](https://github.com/ikomom/dsh-trade-chart) | 0 | 2026-08-14 | 2026-08-31 | DeepSeek Harness 交易图表插件：对话内直接渲染 K线/折线/柱状/面积图、技术指标（EMA/BOLL/MACD/RSI/KDJ/MAVOL）、热点轮动矩阵与连板晋级图。纯自绘 SVG，零外部依赖，附在线示例页。 |
| 1832 | [imaginevoldermert/dsh-minimal-launcher-plugin](https://github.com/imaginevoldermert/dsh-minimal-launcher-plugin) | 0 | 2026-08-23 | 2026-08-23 | A minimal Windows launcher plugin for DeepSeek Harness |
| 1833 | [imkingjh999/dsh-adaptive-effort](https://github.com/imkingjh999/dsh-adaptive-effort) | 0 | 2026-08-26 | 2026-08-26 | DSH plugin: auto reasoning_effort (low/high/max) per turn via MiniMax complexity scorer + token ledger + per-reply metadata label |
| 1834 | [imlishiyuan/dsh-keep-running](https://github.com/imlishiyuan/dsh-keep-running) | 0 | 2026-08-24 | 2026-08-24 | A watchdog plugin for DeepSeek Harness: on a **quota / rate-limit (HTTP 429)** error, it automatically creates a fixed-interval scheduled task that keeps delivering a "continue the task" prompt until it succeeds or you take over. DeepSeek Harness 的 watchdog 插件：遇到 **配额/限流（HTTP 429）** 时，自动创建一个固定间隔的定时任务，到点持续投递「继续任务」的提示，直到任务成功或你手动接手。 |
| 1835 | [inoricon1/dsh-frontier-math](https://github.com/inoricon1/dsh-frontier-math) | 0 | 2026-08-25 | 2026-08-25 | Evidence-gated frontier mathematics research workflow for DeepSeek Harness |
| 1836 | [intsig-textin/dsh-plugin-xparse](https://github.com/intsig-textin/dsh-plugin-xparse) | 0 | 2026-08-28 | 2026-08-31 | TextIn xParse document parsing tool and skill for DeepSeek Harness, with multi-document tasks, OAuth/AppKey authentication, and paid-operation approval. |
| 1837 | [isirin1131/dsh-easy-galgame](https://github.com/isirin1131/dsh-easy-galgame) | 0 | 2026-08-23 | 2026-08-23 | Easy Galgame 模式：一个文件 = 角色卡 + 世界书 + 剧本 + 规则 + 状态的 all-in-one 提示词。DSH 插件提供 galgame_read / galgame_write / galgame_ask 与 Galgame 模式系统提示词。 |
| 1838 | [iTrimut/GitHub-Road](https://github.com/iTrimut/GitHub-Road) | 0 | 2026-08-28 | 2026-08-28 | Github-Road: 大陆稳定访问 GitHub 官网的网络路径修复技能（hosts 直连 + 动态 IP 择优 + 30 分钟自动自愈，免代理、零费用）——非 agent 专属，任意智能体可用，也可纯手动运行。A network-path fix skill (not agent-specific) for reliable github.com access from mainland China. |
| 1839 | [ivvan3016/dsh-ui-pricing](https://github.com/ivvan3016/dsh-ui-pricing) | 0 | 2026-08-24 | 2026-08-25 | user-configurable cost pricing for dsh |
| 1840 | [ivvan3016/dsh-ui-task-notify](https://github.com/ivvan3016/dsh-ui-task-notify) | 0 | 2026-08-23 | 2026-08-24 | endows dsh with the ability to notify after the task is completed |
| 1841 | [jaaty/dsh-gsd-bundle](https://github.com/jaaty/dsh-gsd-bundle) | 0 | 2026-08-23 | 2026-08-30 | A DeepSeek Harness bundle reimplementing opengsd-core (Git Ship Done) as host-plane Cordis plugins, replacing the default agent-loop behaviour with the GSD phase loop. |
| 1842 | [JackyYangxx/dsh-plugins](https://github.com/JackyYangxx/dsh-plugins) | 0 | 2026-08-25 | 2026-08-27 | DeepSeek Harness (DSH) plugin workspace — home of lbx-agent-team, a multi-agent development team plugin (captain-led planner/checker/dever/tester with pipeline hard gates, git worktrees and a live web panel) |
| 1843 | [jasonguide/dsh-skills-hub](https://github.com/jasonguide/dsh-skills-hub) | 0 | 2026-08-28 | 2026-08-29 | 一个多 Agent 平台的 Skills 统一管理插件（DeepSeek Harness 插件），可以在DSH中统一管理codex、claude code、PI、OpenCode、Hermes、Openclaw等平台的Skills技能 |
| 1844 | [jdqingm/dsh-plan-build-toggle](https://github.com/jdqingm/dsh-plan-build-toggle) | 0 | 2026-08-31 | 2026-08-31 | OpenChamber-style persistent Plan\|Build composer toggle for DeepSeek Harness, with Tab-to-switch. Drives the native /plan channel over the host plan projection. |
| 1845 | [jedzqer/dsh-retry-plugin](https://github.com/jedzqer/dsh-retry-plugin) | 0 | 2026-08-21 | 2026-08-22 | 一款用于DeepSeek Harness（DSH）的插件，可以在AI API请求错误时自动发送继续的消息以重试。A plugin for DeepSeek Harness (DSH) that automatically sends continuation messages to retry when AI API requests fail. |
| 1846 | [Jensen-Yao/dsh-deepexcel](https://github.com/Jensen-Yao/dsh-deepexcel) | 0 | 2026-08-27 | 2026-08-28 | Deepcel 工作簿 · DeepSeek Harness (dsh) 皮肤中心 v2 皮肤：Excel 风格工作簿，单元格化消息、工作表网格、工作簿标签。Small-tailqwq/dsh-deepcel 的 v2 完整移植。 |
| 1847 | [jer67107-cyber/dsh-skin-chengzi](https://github.com/jer67107-cyber/dsh-skin-chengzi) | 0 | 2026-08-24 | 2026-08-25 | 橙子 · 深海蓝调 — DSH Web 皮肤中心深海蓝护眼皮肤（Deep sea blue skin for DSH web skin-center） |
| 1848 | [Jiachi5533/dsh-remote-gateway](https://github.com/Jiachi5533/dsh-remote-gateway) | 0 | 2026-08-28 | 2026-08-28 | Source-filtered remote gateway for DeepSeek Harness behind an authenticated reverse proxy |
| 1849 | [jiang12345-code/dsh-multi-role-debate](https://github.com/jiang12345-code/dsh-multi-role-debate) | 0 | 2026-08-26 | 2026-08-26 | 多角色并行论证 DSH 插件：codex/claude 实体 + DSH Judge 汇总 + 结果回对话 + 直接对话（聚合包 dsh-multi-role-debate） |
| 1850 | [jiang12345-code/dsh-openrouter-free](https://github.com/jiang12345-code/dsh-openrouter-free) | 0 | 2026-08-27 | 2026-08-27 | OpenRouter 免费模型面板 for DeepSeek Harness — 分级星标 · 一键切换 · 任务续跑友好 |
| 1851 | [jiang12345-code/dsh-self-restart](https://github.com/jiang12345-code/dsh-self-restart) | 0 | 2026-08-29 | 2026-08-29 | DSH self-restart plugin (Windows): reliable elevated restart via schtasks, transparent front-end recovery, auto-detect and resume in-progress sessions across reboots, business gate prevents wake self-excitation loops. |
| 1852 | [jiangchuangege/anime-pet-widget](https://github.com/jiangchuangege/anime-pet-widget) | 0 | 2024-01-19 | 2026-08-27 | jenkins测试 |
| 1853 | [jiaoTaiLang404/dsh-model-ocean-selector](https://github.com/jiaoTaiLang404/dsh-model-ocean-selector) | 0 | 2026-08-24 | 2026-08-24 | A DeepSeek Harness plugin with a vertical model list and an animated Three.js particle reasoning-effort control |
| 1854 | [JiayiXie-jpg/dsh-desktop-pet](https://github.com/JiayiXie-jpg/dsh-desktop-pet) | 0 | 2026-08-26 | 2026-08-26 | 一只住在 DSH 网页里的养成系桌宠：随编码活动升级进化、语音打气，还能用 AI 生成专属的透明动画形象。 |
| 1855 | [Jiazliang/dsh-worktree](https://github.com/Jiazliang/dsh-worktree) | 0 | 2026-08-22 | 2026-08-22 | Fork-like git worktree for DeepSeek Harness (DSH): create an isolated git worktree from a workspace/session and open a new session in it — optionally forking the conversation so the child inherits all history and works on its own branch. |
| 1856 | [jieguanya/tugu-dsh-balance-widget](https://github.com/jieguanya/tugu-dsh-balance-widget) | 0 | 2026-08-22 | 2026-08-22 | DeepSeek Harness (DSH) 余额插件：实时余额/今日消耗/7-30天趋势图 |
| 1857 | [jiesou/dsh-nous-portal-free-provider](https://github.com/jiesou/dsh-nous-portal-free-provider) | 0 | 2026-08-24 | 2026-08-24 | Nous Portal free-tier provider for dsh |
| 1858 | [jimmyzhang219/dsh-plan-and-execute](https://github.com/jimmyzhang219/dsh-plan-and-execute) | 0 | 2026-08-30 | 2026-08-30 | dsh插件plan-and-execute |
| 1859 | [jingyunstudio/jingyun-dsh](https://github.com/jingyunstudio/jingyun-dsh) | 0 | 2026-08-27 | 2026-08-29 | 基于 Jingyun Studio + DeepSeek Harness (DSH) 打造的一站式 AI 商业化桌面客户端 |
| 1860 | [jingzhonghui/dsh-mcp-manager](https://github.com/jingzhonghui/dsh-mcp-manager) | 0 | 2026-08-30 | 2026-08-30 | DSH dynamic Cordis plugin: visually manage MCP servers (stdio) from the settings sidebar, and expose their tools to the agent as mcp__<server>__<tool>. |
| 1861 | [JinRyu-online/dsh-svn-plugin](https://github.com/JinRyu-online/dsh-svn-plugin) | 0 | 2026-08-24 | 2026-08-24 | 面向 DeepSeek Harness Web GUI 的 SVN（Subversion）版本控制面板插件。以独立 tab 融入 dsh-better-sidebar 右侧边栏 |
| 1862 | [Jinsight-gif/dsh-plugin-gitbash](https://github.com/Jinsight-gif/dsh-plugin-gitbash) | 0 | 2026-08-23 | 2026-08-23 | DeepSeek Harness 插件：在 DSH 会话里运行 Windows 侧 Git for Windows Bash（WSL 自动探测路径）。Run commands on the Windows host's Git for Windows Bash from DeepSeek Harness — WSL-aware, auto-detects git-bash. |
| 1863 | [jinwendijv/dsh-applauncher](https://github.com/jinwendijv/dsh-applauncher) | 0 | 2026-08-27 | 2026-08-27 | DSH 的应用启动器插件：自动扫描本机已安装的电脑应用，在侧边栏“设置”图标上方提供一键启动，像 Windows 开始菜单一样，扫描添加后可以点击启动应用 |
| 1864 | [JJXjustin/dsh-session-rewind](https://github.com/JJXjustin/dsh-session-rewind) | 0 | 2026-08-31 | 2026-08-31 | DSH session and file rewind plugin (shadow git repo) |
| 1865 | [jo32/dsh-hackernews-reader](https://github.com/jo32/dsh-hackernews-reader) | 0 | 2026-08-23 | 2026-08-24 | A dsh-plugin Hacker News reader with app-scoped AI conversations for DeepDeck. |
| 1866 | [jo32/dsh-nga-reader](https://github.com/jo32/dsh-nga-reader) | 0 | 2026-08-23 | 2026-08-24 | A dsh-plugin NGA reader with app-scoped AI conversations for DeepDeck. |
| 1867 | [jo32/dsh-strudel-studio](https://github.com/jo32/dsh-strudel-studio) | 0 | 2026-08-29 | 2026-08-30 | A professional song-level Strudel visual sequencer with structured AI arrangement for DeepDeck. |
| 1868 | [jo32/dsh-video-sherlock](https://github.com/jo32/dsh-video-sherlock) | 0 | 2026-08-26 | 2026-08-26 | A local-first, evidence-backed video investigation app for DeepDeck. |
| 1869 | [joao-paulo-santos/dsh-approval-diff](https://github.com/joao-paulo-santos/dsh-approval-diff) | 0 | 2026-08-25 | 2026-08-26 | DSH plugin: replace file-change approval prompts with a real diff review (line diffs, word highlights, disk-sourced context, one file per card) |
| 1870 | [joao-paulo-santos/dsh-approval-first](https://github.com/joao-paulo-santos/dsh-approval-first) | 0 | 2026-08-25 | 2026-08-26 | Approval-first edit/write for DeepSeek Harness: shadow tools ask the user BEFORE a mutation the standing sandbox policy would deny, so the model never has to repeat a tool call with sandbox_permissions. In-policy writes stay silent, out-of-policy targets get an approval card on the first call. |
| 1871 | [joao-paulo-santos/dsh-bouncing-squares-example](https://github.com/joao-paulo-santos/dsh-bouncing-squares-example) | 0 | 2026-08-26 | 2026-08-27 | Example plugin for dsh-granular-settings: three bouncing squares, one per settings scope (session, workspace, global). Switch sessions and workspaces to watch each scope behave differently |
| 1872 | [joao-paulo-santos/dsh-diff-view](https://github.com/joao-paulo-santos/dsh-diff-view) | 0 | 2026-08-29 | 2026-08-29 | Diff view: a reusable two-text diff viewer for DSH client plugins — line LCS, word highlights, split/unified views, true line numbers across context collapse. |
| 1873 | [joao-paulo-santos/dsh-granular-prompt](https://github.com/joao-paulo-santos/dsh-granular-prompt) | 0 | 2026-08-27 | 2026-08-27 | Prompt composition manager for DSH: live census of every system-prompt section with suppress and replace, custom system prompts, and a persona library with a picker right in the chat composer |
| 1874 | [joao-paulo-santos/dsh-granular-settings](https://github.com/joao-paulo-santos/dsh-granular-settings) | 0 | 2026-08-26 | 2026-08-27 | Granular settings platform: one Granular Settings page (Workspace/Session/Plugin tabs) where other DSH plugins register scoped, namespaced controls (session, workspace, global). Nine control types, doorbell-only push via dsh-event-relay |
| 1875 | [joao-paulo-santos/dsh-md-view](https://github.com/joao-paulo-santos/dsh-md-view) | 0 | 2026-08-29 | 2026-08-29 | Markdown view: a safe markdown-to-React renderer for DSH client plugins — GitHub-subset markdown, shared stylesheet, no HTML injection. |
| 1876 | [joao-paulo-santos/dsh-scratchpad](https://github.com/joao-paulo-santos/dsh-scratchpad) | 0 | 2026-08-28 | 2026-08-28 | Scratch pad: one shared floating text surface in the middle of the screen, opened by other plugins through the client service scratchpad. |
| 1877 | [joao-paulo-santos/dsh-wo-github](https://github.com/joao-paulo-santos/dsh-wo-github) | 0 | 2026-08-29 | 2026-08-29 | Workspace Overview GitHub tab: About card, README rendered as markdown, and the default-branch commit history with per-file patches. |
| 1878 | [joao-paulo-santos/dsh-workspace-history](https://github.com/joao-paulo-santos/dsh-workspace-history) | 0 | 2026-08-28 | 2026-08-28 | Workspace history: journals every compaction summary to the workspace and adds a History subtab to the Workspace Overview tab for reading it back. |
| 1879 | [joao-paulo-santos/dsh-workspace-overview](https://github.com/joao-paulo-santos/dsh-workspace-overview) | 0 | 2026-08-28 | 2026-08-28 | Workspace overview: a Workspace Overview tab beside Chat with a subtab facade for other plugins, and a GitHub pill in the session header when the workspace has a github.com repository. |
| 1880 | [JoaquinDG/dsh-governor](https://github.com/JoaquinDG/dsh-governor) | 0 | 2026-08-23 | 2026-08-24 | Behavioural supervision for DeepSeek Harness agents: retry storms, reasoning-budget burn, and a backstop that survives host suspend. |
| 1881 | [JochenYang/dsh-remote](https://github.com/JochenYang/dsh-remote) | 0 | 2026-08-29 | 2026-08-29 | Operate DeepSeek Harness from your phone: self-hosted relay + desktop plugin tunnel with a mobile-adapted web UI. MIT |
| 1882 | [JoeeLiu/dsh-super-subscriptions](https://github.com/JoeeLiu/dsh-super-subscriptions) | 0 | 2026-08-28 | 2026-08-28 | Unified subscription providers, model routing, quota UI, and media tools for DeepSeek Harness |
| 1883 | [JoeyLearnsToCode/dsh-workspace-native-open](https://github.com/JoeyLearnsToCode/dsh-workspace-native-open) | 0 | 2026-08-28 | 2026-08-28 | dsh plugin for native open workspace / 用于本地打开工作区目录的 dsh 插件 |
| 1884 | [johnvictorio/dsh-custom-prompt](https://github.com/johnvictorio/dsh-custom-prompt) | 0 | 2026-08-27 | 2026-08-27 | DSH plugin that injects an editable section into the global system prompt, with a Settings page |
| 1885 | [JollY-Life/jolly-dsh-vision](https://github.com/JollY-Life/jolly-dsh-vision) | 0 | 2026-08-21 | 2026-08-22 | ModLens 风格的 DeepSeek Harness 视觉桥接插件：deepseek-v4-pro 当大脑、deepseek-v4-flash-vision-exp 当眼睛，提供 vision 工具与 (ds vision) 视觉孪生模型，让纯文本模型也能看图、直接贴图。 |
| 1886 | [joshryandavis/dsh-catalog-refresh](https://github.com/joshryandavis/dsh-catalog-refresh) | 0 | 2026-08-30 | 2026-08-30 | DSH plugin to automatically rebuild model catalogues for OpenRouter, OpenCode, Fireworks, etc |
| 1887 | [joshryandavis/dsh-goal-restart](https://github.com/joshryandavis/dsh-goal-restart) | 0 | 2026-08-30 | 2026-08-30 | DSH plugin to automatically restart goals on harness restart |
| 1888 | [jsoncode/dsh-get-balance](https://github.com/jsoncode/dsh-get-balance) | 0 | 2026-08-23 | 2026-08-24 | 余额与费用查询插件，支持多账号查询，实时token实时统计，中英双语，界面交互直观、开箱即用 |
| 1889 | [jsoncode/dsh-model-list](https://github.com/jsoncode/dsh-model-list) | 0 | 2026-08-27 | 2026-08-28 | OpenRouter free-models browser & one-click model config for DeepSeek Harness (DSH) — newest-first, local search, platform tabs. DSH 免费模型浏览器：按最新排序、本地搜索、一键添加到模型列表 |
| 1890 | [JularDepick/dsh-system-monitor-plugin](https://github.com/JularDepick/dsh-system-monitor-plugin) | 0 | 2026-08-23 | 2026-08-24 | A plugin for dsh: monitor the resource utilization of dsh system processes and report the results to the user in the form of charts. |
| 1891 | [junarch/voice_for_dsh](https://github.com/junarch/voice_for_dsh) | 0 | 2026-08-22 | 2026-08-23 | DSH Web 语音朗读插件：每轮输出口语化转写后朗读（代码/表格自动跳过）；免费浏览器 TTS + 可选豆包云 TTS。Read-aloud plugin for DeepSeek Harness web. |
| 1892 | [justhalfbit/dsh-plugin-memory](https://github.com/justhalfbit/dsh-plugin-memory) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness (DSH) 跨会话记忆插件：对话模型边干边记的 Markdown 项目记忆，支持专题文件渐进式披露、可选后台静默蒸馏、按项目隔离与热更新设置面板。机制对齐 Claude Code auto memory。 \| Agent-maintained cross-session Markdown memory: progressive-disclosure topic files, opt-in silent distillation, per-project isolation. Claude Code-aligned. |
| 1893 | [jwilson411/dsh-arxiv](https://github.com/jwilson411/dsh-arxiv) | 0 | 2026-08-29 | 2026-08-30 | DeepSeek Harness plugin: tiny read-only arXiv search + abstract fetch (Atom API, no PDF ingest) |
| 1894 | [jwilson411/dsh-canary](https://github.com/jwilson411/dsh-canary) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness plugin: plant a canary and deny tool args/URLs that echo it (CANARY_TRIP). |
| 1895 | [jwilson411/dsh-kokoro](https://github.com/jwilson411/dsh-kokoro) | 0 | 2026-08-30 | 2026-08-30 | DeepSeek Harness plugin: HTTP TTS client for jwilson411/kokoro-tts-api. No weights. |
| 1896 | [jwilson411/dsh-llamacpp](https://github.com/jwilson411/dsh-llamacpp) | 0 | 2026-08-29 | 2026-08-29 | DeepSeek Harness LLM adapter for a local llama.cpp OpenAI-compatible server. |
| 1897 | [jwilson411/dsh-loop-brake](https://github.com/jwilson411/dsh-loop-brake) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness plugin: identical tool+args circuit breaker (LOOP_BRAKE) |
| 1898 | [jwilson411/dsh-modelprint](https://github.com/jwilson411/dsh-modelprint) | 0 | 2026-08-30 | 2026-08-30 | DeepSeek Harness plugin: fingerprint provider, model id, sampling, tool schemas, and system-prompt prefix; pin the card and fail structured on drift. |
| 1899 | [jwilson411/dsh-otel](https://github.com/jwilson411/dsh-otel) | 0 | 2026-08-30 | 2026-08-30 | DeepSeek Harness plugin: emit OpenTelemetry spans from a session log (turn / step / tool execute). Export only. |
| 1900 | [jwilson411/dsh-plugin-kit](https://github.com/jwilson411/dsh-plugin-kit) | 0 | 2026-08-29 | 2026-08-29 | A minimal, tested template for DeepSeek Harness plugins. |
| 1901 | [jwilson411/dsh-secret-scrub](https://github.com/jwilson411/dsh-secret-scrub) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness plugin: redact known secret shapes before the model sees them; JSONL incidents never store the preimage |
| 1902 | [jwilson411/dsh-spend-receipt](https://github.com/jwilson411/dsh-spend-receipt) | 0 | 2026-08-29 | 2026-08-31 | A cache-aware JSONL cost receipt plugin for DeepSeek Harness. |
| 1903 | [jwilson411/dsh-ssrf-guard](https://github.com/jwilson411/dsh-ssrf-guard) | 0 | 2026-08-30 | 2026-08-31 | DeepSeek Harness plugin: fail-closed URL host/scheme allowlist that runs before a request is opened |
| 1904 | [jypjypjypjyp/dsh-agent-teams](https://github.com/jypjypjypjyp/dsh-agent-teams) | 0 | 2026-08-19 | 2026-08-25 | AgentTeams plugin for DeepSeek Harness |
| 1905 | [kaixinguo360/dsh-bsk-ws-bridge](https://github.com/kaixinguo360/dsh-bsk-ws-bridge) | 0 | 2026-08-26 | 2026-08-26 | DeepSeek Harness BrowserSkill 桥接插件：把本机 bsk daemon 的 WebSocket 经浏览器信道暴露给远程 BrowserSkill 扩展。配套的修改版 BrowserSkill 扩展：https://github.com/kaixinguo360/BrowserSkill-DSH-Remote |
| 1906 | [kaka-crypto/dsh-disk-guard](https://github.com/kaka-crypto/dsh-disk-guard) | 0 | 2026-08-28 | 2026-08-28 | Disk guard for DeepSeek Harness: redirect downloads/artifacts/caches/temp off the C: drive, inject a path-discipline prompt into every session, disk_guard tool for status/cleanup. |
| 1907 | [KamChiHei/dsh-deepseek-usage-monitor](https://github.com/KamChiHei/dsh-deepseek-usage-monitor) | 0 | 2026-08-21 | 2026-08-22 | DeepSeek Harness (dsh) plugin: token usage accounting and account balance with a live status card in DSH Web |
| 1908 | [kane-le/dsh-deepseek-usage](https://github.com/kane-le/dsh-deepseek-usage) | 0 | 2026-08-25 | 2026-08-25 | DeepSeek API 用量与余额查看插件（DSH Plugin）· /usage 命令实时查询余额并汇总本机 token 用量 |
| 1909 | [KarthusLorin/dsh-subagent-grok](https://github.com/KarthusLorin/dsh-subagent-grok) | 0 | 2026-08-29 | 2026-08-29 | One-shot Grok CLI subagent provider for DeepSeek Harness |
| 1910 | [Kehao/dsh-client-ui-weather](https://github.com/Kehao/dsh-client-ui-weather) | 0 | 2026-08-30 | 2026-08-30 | Deepseek harness 天气插件 |
| 1911 | [keke-shy/dsh-desktop](https://github.com/keke-shy/dsh-desktop) | 0 | 2026-08-16 | 2026-08-22 | Minimal Electron desktop shell embedding the official DeepSeek Harness web profile |
| 1912 | [kenny2077/dsh-web-kimi](https://github.com/kenny2077/dsh-web-kimi) | 0 | 2026-08-31 | 2026-08-31 | Kimi Coding web search + web fetch providers for the DeepSeek Harness with coding plan key |
| 1913 | [KeS1Ke/dsh-start-and-exit](https://github.com/KeS1Ke/dsh-start-and-exit) | 0 | 2026-08-24 | 2026-08-27 | dsh-start&exit: safe start, exit, and restart controls for the DeepSeek Harness Web profile, plus a loopback-only Windows foreground launcher. |
| 1914 | [Kevoyuan/dsh-trading212](https://github.com/Kevoyuan/dsh-trading212) | 0 | 2026-08-24 | 2026-08-25 | Read-only Trading 212 portfolio dashboard and dsh tools for holdings, history, risk, and trade markers. |
| 1915 | [KeyboardPrince/dsh-skill-manager](https://github.com/KeyboardPrince/dsh-skill-manager) | 0 | 2026-08-22 | 2026-08-22 | DSH 设置界面中的技能管理器插件：可视化管理全局/项目级 Skill（导入、编辑、删除、启用/禁用 SKILL.md 目录） |
| 1916 | [Kickstartparty3459/dsh-ios](https://github.com/Kickstartparty3459/dsh-ios) | 0 | 2026-08-22 | 2026-08-23 | Run live iOS simulators and your real iPhone over USB inside DeepSeek Harness conversations with 22 agent tools, MJPEG previews, and SwiftUI hot reload. |
| 1917 | [KimFischer99/DeepSeek-Harness-Desktop](https://github.com/KimFischer99/DeepSeek-Harness-Desktop) | 0 | 2026-08-15 | 2026-08-27 | 一个轻量的 macOS 桌面应用壳，Rust 编写，承载 DeepSeek Harness WebUI，一键启停 |
| 1918 | [kingcheng12/dsh-workspace-change-awareness](https://github.com/kingcheng12/dsh-workspace-change-awareness) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness plugin that surfaces concurrent workspace changes before an agent continues. |
| 1919 | [kittimzhe/dsh-plugin-authoring-guide](https://github.com/kittimzhe/dsh-plugin-authoring-guide) | 0 | 2026-08-29 | 2026-08-29 | Hands-on guide to building a DeepSeek Harness plugin (EN/ZH) — real code & pitfalls from dsh-session-export and dsh-session-recall |
| 1920 | [kittimzhe/dsh-session-recall](https://github.com/kittimzhe/dsh-session-recall) | 0 | 2026-08-25 | 2026-08-26 | Cross-session full-text recall for DeepSeek Harness: the model-facing recall tool searches past session transcripts via ctx.sessionQuery, with a persistent FTS index |
| 1921 | [kivensteven8-eng/dsh-file-download](https://github.com/kivensteven8-eng/dsh-file-download) | 0 | 2026-08-27 | 2026-08-27 | DSH 插件：把会话工作区文件变成浏览器直接下载的 HTTP 通道 —— 为 iPad 等局域网/域名设备设计。 |
| 1922 | [kkaktus463/dsh-plugin-desktop](https://github.com/kkaktus463/dsh-plugin-desktop) | 0 | 2026-08-23 | 2026-08-23 | Opens the DeepSeek Harness Web UI in a native window instead of a browser tab. |
| 1923 | [KL3jd/handwritten-ocr](https://github.com/KL3jd/handwritten-ocr) | 0 | 2026-08-27 | 2026-08-27 | DSH plugin for local OCR: handwritten Chinese + math → Markdown with LaTeX. GPU / CPU backends. |
| 1924 | [knownothing114/dsh-notify](https://github.com/knownothing114/dsh-notify) | 0 | 2026-08-28 | 2026-08-28 | A dsh plugin that raises a desktop notification whenever dsh needs your attention. |
| 1925 | [kobenfang/BigTimer](https://github.com/kobenfang/BigTimer) | 0 | 2026-08-29 | 2026-08-29 | 🕐 BigTimer · 定时任务+消息推送管家 — Scheduled tasks & message push manager for DeepSeek Harness (dsh) |
| 1926 | [Kogisune/dsh-skin-koi-pond](https://github.com/Kogisune/dsh-skin-koi-pond) | 0 | 2026-08-20 | 2026-08-28 | 🎏 锦鲤池塘 · Koi Pond theme for DeepSeek Harness (DSH) WebUI — 动画锦鲤 + 部件拆分 CSS |
| 1927 | [Kompetenzteam/dsh-locale-de](https://github.com/Kompetenzteam/dsh-locale-de) | 0 | 2026-08-23 | 2026-08-23 | German UI translation plugin for DeepSeek Harness (locale de): registers all locale namespaces in German. Deutsche UI-Uebersetzung fuer den DeepSeek Harness. |
| 1928 | [konanzheng/dsh-timeline](https://github.com/konanzheng/dsh-timeline) | 0 | 2026-08-26 | 2026-08-27 | show timeline for deepseek harness |
| 1929 | [kongdexu/dsh-win-notify](https://github.com/kongdexu/dsh-win-notify) | 0 | 2026-08-25 | 2026-08-25 | Real Windows OS toasts for DeepSeek Harness: task-finished / needs-input / needs-approval alerts in Notification Center. Windows-only, zero runtime dependencies. |
| 1930 | [ktao732084-arch/dsh-vibegap](https://github.com/ktao732084-arch/dsh-vibegap) | 0 | 2026-08-27 | 2026-08-27 | Vocabulary flashcards inside the dsh web UI - appear while your agent runs, retreat when it finishes. A VibeGap plugin. |
| 1931 | [ktao732084-arch/vibegap](https://github.com/ktao732084-arch/vibegap) | 0 | 2026-08-26 | 2026-08-27 | Mini-window for the gaps in vibe coding: vocabulary flashcards (and more panels) that auto-appear while your AI coding agent runs |
| 1932 | [KumarZX/kur-compact-trigger](https://github.com/KumarZX/kur-compact-trigger) | 0 | 2026-08-31 | 2026-08-31 | DSH 插件 · 会话级压缩（官方 auto 只能全局） / Per-session compaction; official auto is global-only |
| 1933 | [L3n3L/dsh-disk-cleaner](https://github.com/L3n3L/dsh-disk-cleaner) | 0 | 2026-08-22 | 2026-08-22 | Windows disk space analysis and safe cleanup plugin for DeepSeek Harness |
| 1934 | [LamplitIsles/dsh-companion](https://github.com/LamplitIsles/dsh-companion) | 0 | 2026-08-30 | 2026-08-30 | dsh as companion ai frontend in Svelte |
| 1935 | [LamplitIsles/kepos-tts](https://github.com/LamplitIsles/kepos-tts) | 0 | 2026-08-29 | 2026-08-30 | Qwen/Volcengine TTS for dsh |
| 1936 | [Lanzgale/dsh-listener](https://github.com/Lanzgale/dsh-listener) | 0 | 2026-08-30 | 2026-08-30 | 安全版本地语音输入插件 for DeepSeek Harness:同源宿主代理 + 127.0.0.1 + token,SenseVoice-Small INT8 ONNX 本地转写,音频不出网。 |
| 1937 | [Lanzgale/dsh-repo-browser](https://github.com/Lanzgale/dsh-repo-browser) | 0 | 2026-08-25 | 2026-08-26 | Repository Browser plugin for DeepSeek Harness — right-side GitHub repo list with local grouping and quick actions (move / private / archive) |
| 1938 | [LaoQianwocao/dsh-client-ui-board](https://github.com/LaoQianwocao/dsh-client-ui-board) | 0 | 2026-08-22 | 2026-08-23 | DSH Web 展板插件：会话视图第三标签，多层白板 + 锚点连线 |
| 1939 | [lasdrder0705/dsh-chat-zone-std](https://github.com/lasdrder0705/dsh-chat-zone-std) | 0 | 2026-08-26 | 2026-08-26 | dsh-std Community v0.15 chat zone: ~/dsh_CHAT/<date>/chatN as Tools and Commands. Install adapter-dsh first. |
| 1940 | [lasdrder0705/dsh-pro-vision-std](https://github.com/lasdrder0705/dsh-pro-vision-std) | 0 | 2026-08-26 | 2026-08-26 | dsh-std Community v0.15 ModelProvider: V4-Pro with Flash-Vision captions. Install adapter-dsh first. |
| 1941 | [lastplayer82/dsh-sticky-notes](https://github.com/lastplayer82/dsh-sticky-notes) | 0 | 2026-08-27 | 2026-08-27 | 灵感便签 (Sticky Notes) plugin for the dsh web GUI: jot ideas while the agent thinks — without interrupting it. Queue-channel sends/forwards, auto-persist (localStorage + host file), export TXT/JSON/MD, bilingual zh/en. DeepSeek Harness plugin · @lastplayer82/dsh-sticky-notes |
| 1942 | [law-star-cn/lawstar-dsh-mcp](https://github.com/law-star-cn/lawstar-dsh-mcp) | 0 | 2026-08-24 | 2026-08-24 | DeepSeek Harness plugin for LawStar MCP (legal-data): one-click API Key connect |
| 1943 | [lcsdg/dsh-quick-prompts](https://github.com/lcsdg/dsh-quick-prompts) | 0 | 2026-08-25 | 2026-08-25 | Quick-prompts bar for DeepSeek Harness (dsh): per-category snippet chips above the composer, orange placeholder highlighting, two-column prompt/category management, and per-session category memory. |
| 1944 | [leechengwei/dsh-session-intelligence](https://github.com/leechengwei/dsh-session-intelligence) | 0 | 2026-08-31 | 2026-08-31 | DSH 会话情报：固定右侧栏、初衷与最近用户需求摘要、会话活动和只读 Git 状态。 |
| 1945 | [lelens0/dsh-token-ledger](https://github.com/lelens0/dsh-token-ledger) | 0 | 2026-08-30 | 2026-08-31 | DeepSeek Harness plugin: monitor balance & usage across multiple LLM gateways (token ledger) |
| 1946 | [lemoncat7/dsh-partner](https://github.com/lemoncat7/dsh-partner) | 0 | 2026-08-27 | 2026-08-31 | Long-lived AI companions with WeChat channel routing for DeepSeek Harness |
| 1947 | [lemoncat7/dsh-remote-settings-compat](https://github.com/lemoncat7/dsh-remote-settings-compat) | 0 | 2026-08-22 | 2026-08-25 | Remote settings compatibility plugin for DeepSeek Harness |
| 1948 | [lemoncat7/dsh-ssh](https://github.com/lemoncat7/dsh-ssh) | 0 | 2026-08-23 | 2026-08-25 | SSH sessions, SFTP, terminals, proxies and port forwarding for DeepSeek Harness |
| 1949 | [lemoncat7/dsh-web-search](https://github.com/lemoncat7/dsh-web-search) | 0 | 2026-08-25 | 2026-08-25 | Configurable and secure multi-provider web search for DeepSeek Harness |
| 1950 | [Leo3-7/dsh-obsidian-inbox](https://github.com/Leo3-7/dsh-obsidian-inbox) | 0 | 2026-08-28 | 2026-08-28 | DSH skill: ingest the conclusions/mistakes/projects from conversations into an Obsidian vault via a 7-step workflow with two-level validation. 把对话结论/错题/项目按七步流程整理进 Obsidian 的 DeepSeek Harness 技能。 |
| 1951 | [LeoChen98/dsh-worktable-notebook-to-ppt](https://github.com/LeoChen98/dsh-worktable-notebook-to-ppt) | 0 | 2026-08-26 | 2026-08-26 | 基于 dsh-worktable 工作台搭建的「课本到 PPT」自动化工作流插件——在 DeepSeek Harness 中一键将 Jupyter Notebook 转化为专业可编辑的演示文稿（.pptx），让知识沉淀与分享更高效。 |
| 1952 | [leogottadothebest/DSH-Archived-Delete](https://github.com/leogottadothebest/DSH-Archived-Delete) | 0 | 2026-08-31 | 2026-08-31 | DSH 插件：在设置界面管理已归档对话——取消归档与永久删除 |
| 1953 | [leonardoxr/dsh-codex-usage](https://github.com/leonardoxr/dsh-codex-usage) | 0 | 2026-08-22 | 2026-08-24 | OpenAI Codex plan usage indicator for DeepSeek Harness |
| 1954 | [leonardoxr/dsh-coding-tools](https://github.com/leonardoxr/dsh-coding-tools) | 0 | 2026-08-23 | 2026-08-24 | Secure bounded coding tools for DeepSeek Harness |
| 1955 | [leonardoxr/dsh-image-preview](https://github.com/leonardoxr/dsh-image-preview) | 0 | 2026-08-23 | 2026-08-24 | Inline read_image previews for DeepSeek Harness |
| 1956 | [leonardoxr/dsh-status-bar-config](https://github.com/leonardoxr/dsh-status-bar-config) | 0 | 2026-08-23 | 2026-08-24 | Configurable conversation statistics row for DeepSeek Harness |
| 1957 | [leonardoxr/dsh-workspace-git](https://github.com/leonardoxr/dsh-workspace-git) | 0 | 2026-08-22 | 2026-08-24 | DeepSeek Harness plugin for cloning Git repositories as workspaces |
| 1958 | [LeonSone/dsh-question-rail](https://github.com/LeonSone/dsh-question-rail) | 0 | 2026-08-26 | 2026-08-27 | DSH web plugin: 模仿 deepseek 网页版界面右侧的问题条 — 右缘一条竖向问题栏，列出当前会话每一轮的用户提问，点击平滑滚动定位。DeepSeek Harness right-edge question rail. |
| 1959 | [LeonSone/dsh-trash](https://github.com/LeonSone/dsh-trash) | 0 | 2026-08-22 | 2026-08-22 | A DeepSeek Harness (DSH) plugin: every delete operation goes through a recoverable trash store — accidental deletes are one restore away. |
| 1960 | [lgquan/dsh-voco](https://github.com/lgquan/dsh-voco) | 0 | 2026-08-27 | 2026-08-27 | Persistent voice conversations for DSH with cloud speech recognition, Edge TTS, and background Agent delegation. |
| 1961 | [lgquan/dsh-workspace-memory](https://github.com/lgquan/dsh-workspace-memory) | 0 | 2026-08-28 | 2026-08-31 | Durable workspace-scoped memory for DeepSeek Harness and dsh-voco voice agents. |
| 1962 | [lhf6623/dsh-thrum](https://github.com/lhf6623/dsh-thrum) | 0 | 2026-08-16 | 2026-08-29 | DeepSeek Harness 输入氛围插件：为输入过程增添氛围。 |
| 1963 | [lhh666-6/dsh-copy-fix](https://github.com/lhh666-6/dsh-copy-fix) | 0 | 2026-08-23 | 2026-08-24 | Fix DSH Desktop copy buttons by bridging clipboard writes to the Electron main process. |
| 1964 | [lhh666-6/dsh-paste-file](https://github.com/lhh666-6/dsh-paste-file) | 0 | 2026-08-23 | 2026-08-24 | Paste/drop files into the DSH composer, save them under the current workspace, and insert relative paths. |
| 1965 | [lhh666-6/dsh-update-check](https://github.com/lhh666-6/dsh-update-check) | 0 | 2026-08-23 | 2026-08-24 | DSH update checker for the DSH Desktop installer channel and GitHub source releases, with one-click download/update. |
| 1966 | [lhh666-6/dsh-usage-cost](https://github.com/lhh666-6/dsh-usage-cost) | 0 | 2026-08-23 | 2026-08-24 | Real-time DeepSeek token usage and cost meter for DSH: status-bar capsule plus detail panel, local-only persistence. |
| 1967 | [lianginx/dsh-quote-selection](https://github.com/lianginx/dsh-quote-selection) | 0 | 2026-08-22 | 2026-08-22 | ❝ Quote selected chat text into the composer as a Markdown blockquote · DeepSeek Harness Web UI 插件：选中会话文字，一键引用 |
| 1968 | [lianginx/dsh-timeline-enhance](https://github.com/lianginx/dsh-timeline-enhance) | 0 | 2026-08-25 | 2026-08-25 | DSH Web UI plugin: auto-fold chat timeline processes + Deep diving fun tips |
| 1969 | [liangminhua/agent-notes-toolkit](https://github.com/liangminhua/agent-notes-toolkit) | 0 | 2026-08-30 | 2026-08-30 | Agent Notes mechanism as a portable toolkit: verification gates, scaffolding CLI, and the AN dsh preset/bundle |
| 1970 | [liangsheng999/dsh-client-ui-connection-status](https://github.com/liangsheng999/dsh-client-ui-connection-status) | 0 | 2026-08-26 | 2026-08-27 | DSH Web client plugin: a corner pill showing live connection state for the DeepSeek Harness Web UI. npm: dsh-client-ui-connection-status |
| 1971 | [liangsheng999/dsh-dream](https://github.com/liangsheng999/dsh-dream) | 0 | 2026-08-26 | 2026-08-27 | DSH host plugin: scheduled background 'dream' (memory consolidation) passes for DeepSeek Harness. npm: dsh-dream |
| 1972 | [liangxiaobing520/dsh-local-vector-memory](https://github.com/liangxiaobing520/dsh-local-vector-memory) | 0 | 2026-08-29 | 2026-08-29 | Fully local vector memory plugin for DeepSeek Harness: local embeddings, SQLite storage, automatic recall injection, dedup with conflict detection, soft-delete recycle bin, online backup. |
| 1973 | [liangzhipengdamon-maker/GovernLoop-DSH](https://github.com/liangzhipengdamon-maker/GovernLoop-DSH) | 0 | 2026-08-23 | 2026-08-25 | GovernLoop-DSH automatically connects DeepSeek Harness agents to independent ChatGPT review with checkpoints and evidence. |
| 1974 | [LianPing-cyber/dsh-browser-full-access](https://github.com/LianPing-cyber/dsh-browser-full-access) | 0 | 2026-08-29 | 2026-08-29 | Full-access background-tab fork of dsh-browser for DeepSeek Harness (DSH). Based on dsh-browser, MCP, and browser-use. |
| 1975 | [liceses/dsh-hmm-wait](https://github.com/liceses/dsh-hmm-wait) | 0 | 2026-08-22 | 2026-08-26 | 化口水为乐趣，把大肥鱼流的口水变成游戏连击！ |
| 1976 | [Lichtspur/deepseek-style-theme](https://github.com/Lichtspur/deepseek-style-theme) | 0 | 2026-08-26 | 2026-08-27 | DeepSeek official-home style theme for the dsh web GUI: fluid particle background, glass sidebar, glass composer, frosted header, running-subagent progress panel, DSTT time-based mode, and DeepSeek brand link |
| 1977 | [lihaoran0412/dsh-narrative-engine](https://github.com/lihaoran0412/dsh-narrative-engine) | 0 | 2026-08-25 | 2026-08-25 | DeepSeek Harness 沉浸叙事双向创作引擎：导入小说为可游玩世界，游玩后反向写成同人小说。仅处理虚构成年人(18+/adult)。 |
| 1978 | [lijian-ui/dsh-file-manager](https://github.com/lijian-ui/dsh-file-manager) | 0 | 2026-08-18 | 2026-08-27 | 为 DeepSeek Harness 桌面端（dsh web）开发的插件：聊天区右侧的 Explorer 文件面板 + Preview 预览面板（FileManager 风格，Apache-2.0 参考实现非抄录），以及输入框 @ 引用项目文件（树形多选弹窗 + 输入框内胶囊 + 行号） |
| 1979 | [lijian-ui/dsh-schedule-view](https://github.com/lijian-ui/dsh-schedule-view) | 0 | 2026-08-24 | 2026-08-27 | A cron-based scheduled task plugin for DeepSeek Harness (dsh) desktop: create / edit / delete / fire-now tasks from the settings panel, with cross-session agent follow-up and multi-level notifications. Zero LLM tools — purely human-driven scheduling. |
| 1980 | [lijian-ui/dsh-skill-manage](https://github.com/lijian-ui/dsh-skill-manage) | 0 | 2026-08-22 | 2026-08-27 | A skill management plugin for DeepSeek Harness (dsh) desktop: list / enable / disable / delete / add skills, filling the gap in dsh's official skill toggle control. |
| 1981 | [lijian-ui/dsh-term](https://github.com/lijian-ui/dsh-term) | 0 | 2026-08-19 | 2026-08-27 | Panel-style local terminal for the DSH web GUI. |
| 1982 | [lijian-ui/dsh-vision-toggle](https://github.com/lijian-ui/dsh-vision-toggle) | 0 | 2026-08-28 | 2026-08-28 | dsh-vision-toggle 是一个为 DeepSeek Harness (dsh) 提供「支持图片」开关的插件，让你在设置页按模型一键启用/禁用图片输入 |
| 1983 | [lim12137/dsh-llm-extra-retry](https://github.com/lim12137/dsh-llm-extra-retry) | 0 | 2026-08-26 | 2026-08-26 | Extra model-request recovery for DeepSeek Harness: retries PI_AI_ERROR failures once after a fixed 20s delay; other error codes keep the built-in dsh-llm-retry exponential backoff. |
| 1984 | [limlnx523/dsh-plus-plus](https://github.com/limlnx523/dsh-plus-plus) | 0 | 2026-08-27 | 2026-08-28 | DSH++ — a local-first control plane for DeepSeek Harness. Plugin security auditing and workflow regression testing. |
| 1985 | [Lion-Li-git/dsh-external-links](https://github.com/Lion-Li-git/dsh-external-links) | 0 | 2026-08-30 | 2026-08-30 | DSH desktop (Deepseek Harness EAC) plugin: open http/https/mailto/tel/file links in the default browser/app, bypassing the broken shell.open-external bridge |
| 1986 | [LionGateOS/dsh-local-voice-dictation](https://github.com/LionGateOS/dsh-local-voice-dictation) | 0 | 2026-08-21 | 2026-08-23 | Local voice plugin for DeepSeek Harness: microphone dictation with local STT plus assistant-response Kokoro TTS playback. |
| 1987 | [lionheartjie/DSH_Shell](https://github.com/lionheartjie/DSH_Shell) | 0 | 2026-08-23 | 2026-08-25 | DeepSeek Harness 的 Rust/Tauri 套壳 |
| 1988 | [lisongxuan/ds-hentai](https://github.com/lisongxuan/ds-hentai) | 0 | 2026-08-25 | 2026-08-28 | ExHentai-inspired UI for DeepSeek Harness. ExHentai风格DeepSeek Harness皮肤。 ds hentai / deepseek hentai |
| 1989 | [little3tar/dsh-backup](https://github.com/little3tar/dsh-backup) | 0 | 2026-08-23 | 2026-08-24 | 由于 dsh 的自定义范围太大，很难通过一个插件或者程序来完美备份自己的配置，所以我觉得可以通过 ai 来分析哪些配置需要备份、可以备份，以及在新的环境中如何恢复。有了这个 skills 导出的配置文件，任意 agent 都可以帮助恢复 dsh 的配置。 |
| 1990 | [LittleFishStars/dsh-opencode-tui](https://github.com/LittleFishStars/dsh-opencode-tui) | 0 | 2026-08-16 | 2026-08-22 | 为 DeepSeek Harness 制作的仿 OpenCode 的 TUI 界面插件 |
| 1991 | [liujia-io/dsh-image-picker](https://github.com/liujia-io/dsh-image-picker) | 0 | 2026-08-26 | 2026-08-26 | Paperclip image-picker button for the DeepSeek Harness web composer - pick reference images via the system file dialog and feed them into the official attachment pipeline. |
| 1992 | [Liujie-harsh/heart-health-dsh-suite](https://github.com/Liujie-harsh/heart-health-dsh-suite) | 0 | 2026-08-28 | 2026-08-28 | 适配心脏健康场景的 DeepSeek Harness 插件套件：在「心衰辅助诊断算法服务（heart-algo MCP）」之上， 为 DSH 会话提供一组受控的领域包装工具、驻留临床指导与原始工具隐藏策略。 |
| 1993 | [liuke-zhu/zhenxin-ai-video-manager](https://github.com/liuke-zhu/zhenxin-ai-video-manager) | 0 | 2026-08-25 | 2026-08-25 | 真的爱你：本地智能视频管家 Skill —— 说一句「真的爱你」，接管从素材分析到成片交付的完整剪辑流程 |
| 1994 | [liukj98/dsh-ui-tools](https://github.com/liukj98/dsh-ui-tools) | 0 | 2026-08-19 | 2026-08-22 | deepseek harness tools 插件 |
| 1995 | [liuwenji007/dsh-trust-check](https://github.com/liuwenji007/dsh-trust-check) | 0 | 2026-08-27 | 2026-08-27 | Static capability disclosure for DeepSeek Harness plugins — evidence-backed, zero-token, no safety claims. |
| 1996 | [liyongzheng666/dsh-browser-bridge](https://github.com/liyongzheng666/dsh-browser-bridge) | 0 | 2026-08-22 | 2026-08-22 | DSH browser bridge plugin + Firefox extension: browsers read/control via localhost WebSocket |
| 1997 | [lizhi00001/dsh-tools-plugins](https://github.com/lizhi00001/dsh-tools-plugins) | 0 | 2026-08-24 | 2026-08-24 | 将简短或模糊的指令改写为结构化 Prompt |
| 1998 | [ljc6413/pkg-dev](https://github.com/ljc6413/pkg-dev) | 0 | 2026-08-29 | 2026-08-30 | YiHe 编程认知内核 for DeepSeek Harness：27 领域包 + 55 RFB 经验库 + 工程工具链 + 商业/安全/进化体系（会进化的编程助手） |
| 1999 | [LJH-snow/dsh-tool-kubernetes](https://github.com/LJH-snow/dsh-tool-kubernetes) | 0 | 2026-08-27 | 2026-08-27 | Kubernetes tools for DeepSeek Harness: cluster, namespace, workload, pod, log, rollout, and manifest operations |
| 2000 | [LJH-snow/dsh-tool-monitoring](https://github.com/LJH-snow/dsh-tool-monitoring) | 0 | 2026-08-28 | 2026-08-28 | Prometheus and Alertmanager tool plugin for DeepSeek Harness |
| 2001 | [LJH-snow/dsh-tool-slack](https://github.com/LJH-snow/dsh-tool-slack) | 0 | 2026-08-30 | 2026-08-30 | Slack tools for DeepSeek Harness |
| 2002 | [ljlj7149-cloud/dsh-cognitio](https://github.com/ljlj7149-cloud/dsh-cognitio) | 0 | 2026-08-26 | 2026-08-27 | 纠错驱动的认知架构插件（DeepSeek Harness）：分层记忆 + 哨兵自动提醒 + 纠错进化 + 审批仲裁。让 AI 记得你的规矩，换模型换预设都有效；所有自动沉淀，你批准才生效。 |
| 2003 | [lkdxzhxi/dsh-glass-ui-theme](https://github.com/lkdxzhxi/dsh-glass-ui-theme) | 0 | 2026-08-29 | 2026-08-29 | 为 DeepSeek Harness 打造的液态玻璃主题插件：磨砂玻璃、可调色调、动态壁纸，让 DSH 界面焕然一新 |
| 2004 | [lnabc03/bright-drift](https://github.com/lnabc03/bright-drift) | 0 | 2026-08-31 | 2026-08-31 | Workspace drift awareness for AI coding agents — watches the workspace and injects a budgeted, attributed diff of external/user changes into the agent's context at each step boundary. |
| 2005 | [lnetrit-alt/dsh-system-control](https://github.com/lnetrit-alt/dsh-system-control) | 0 | 2026-08-26 | 2026-08-26 | DSH web plugin: sidebar-embedded DeepSeek balance readout with a black minimalist full-shutdown button. |
| 2006 | [loiasdi/dsh-prompthub-ecosystem](https://github.com/loiasdi/dsh-prompthub-ecosystem) | 0 | 2026-08-26 | 2026-08-26 | PromptHub Ecosystem for DeepSeek Harness (DSH): bilingual Plugin and Skill catalog with GitHub and local tarball installation. |
| 2007 | [lokih1028/dsh-prompt-optimizer](https://github.com/lokih1028/dsh-prompt-optimizer) | 0 | 2026-08-29 | 2026-08-29 | One-click prompt enhancement and structuring plugin for DeepSeek Harness (DSH) |
| 2008 | [Lorodn4x/dsh-firecrawl](https://github.com/Lorodn4x/dsh-firecrawl) | 0 | 2026-08-25 | 2026-08-26 | Firecrawl web search and markdown scrape providers for DeepSeek Harness ctx.web seam |
| 2009 | [Lorodn4x/dsh-voice](https://github.com/Lorodn4x/dsh-voice) | 0 | 2026-08-25 | 2026-08-26 | Voice messages for DeepSeek Harness web UI: Edge TTS playback button plus agent-sent voice notes |
| 2010 | [Lorvaste/DSH-Project-Initialization](https://github.com/Lorvaste/DSH-Project-Initialization) | 0 | 2026-08-29 | 2026-08-29 | DSH 插件：项目初始化插件，通过结构化的整理编排，需求与要素确认，无论是项目刚起步还是准备维护，都有一个好的开始. |
| 2011 | [lovezi0/dsh-model-extension](https://github.com/lovezi0/dsh-model-extension) | 0 | 2026-08-24 | 2026-08-25 | DSH自定义模型提供商时无法设置推理模式与多模态，可通过扩展插件解决 |
| 2012 | [lovezi0/dsh-web-noOpenBrowser](https://github.com/lovezi0/dsh-web-noOpenBrowser) | 0 | 2026-08-20 | 2026-08-23 | deepseek harness服务启动不要打开浏览器 |
| 2013 | [lovstudio/dsh-llm-config](https://github.com/lovstudio/dsh-llm-config) | 0 | 2026-08-29 | 2026-08-29 | Reusable LLM configuration profile library exposed to browser consumers as a Remote (DeepSeek Harness plugin) |
| 2014 | [lovstudio/dsh-plugin-marketplace](https://github.com/lovstudio/dsh-plugin-marketplace) | 0 | 2026-08-28 | 2026-08-29 | Local-first DeepSeek Harness plugin marketplace with GitHub and dshfind providers |
| 2015 | [loyalchiiina/dsh-font-enhancer](https://github.com/loyalchiiina/dsh-font-enhancer) | 0 | 2026-08-27 | 2026-08-27 | DIY 你的 DSH 界面：按区域自定义字体/字号/颜色 \| DIY your DSH UI fonts & colors |
| 2016 | [lrplrplrp/dsh-sidebar-gdhighlight](https://github.com/lrplrplrp/dsh-sidebar-gdhighlight) | 0 | 2026-08-30 | 2026-08-31 | godot语法高亮，依赖dsh-better-sidebar |
| 2017 | [Luawig/dsh-cloudflare-access](https://github.com/Luawig/dsh-cloudflare-access) | 0 | 2026-08-27 | 2026-08-27 | Cloudflare Access JWT verification and remote privileged authorization for DeepSeek Harness |
| 2018 | [Lubaoshuai/dsh-notify](https://github.com/Lubaoshuai/dsh-notify) | 0 | 2026-08-30 | 2026-08-30 | Push notifications for DeepSeek Harness: agent-callable notify_send tool + external delivery for schedule reminders (Telegram/Slack/Discord/飞书/钉钉/Bark/ntfy/webhook). DSH plugin. |
| 2019 | [LucienLL/dsh-peak-price-panel](https://github.com/LucienLL/dsh-peak-price-panel) | 0 | 2026-08-23 | 2026-08-24 | DeepSeek Harness plugin: peak/off-peak price watch, live account balance with tiered low-balance alerts, and a top-up button for the main web UI |
| 2020 | [LucienLL/dsh-service-watchdog](https://github.com/LucienLL/dsh-service-watchdog) | 0 | 2026-08-24 | 2026-08-24 | DeepSeek Harness plugin: restart/status of the DSH web service with a detached self-healing watchdog, second-confirmation, and login autostart |
| 2021 | [LucienLL/dsh-session-id](https://github.com/LucienLL/dsh-session-id) | 0 | 2026-08-24 | 2026-08-24 | Show and copy the current session ID in the DeepSeek Harness web UI header |
| 2022 | [LucienLL/dsh-session-memo](https://github.com/LucienLL/dsh-session-memo) | 0 | 2026-08-25 | 2026-08-26 | DSH 对话侧边备忘录插件：GitHub 同步状态 / npm 发布状态 / 项目版本 / 备忘标签，与 dsh-session-status 弱联动 |
| 2023 | [lucifergzsz414/dsh-windows-native](https://github.com/lucifergzsz414/dsh-windows-native) | 0 | 2026-08-31 | 2026-08-31 | Native-Windows (non-WSL) shell/encoding/filesystem gotchas for the DeepSeek Harness system prompt |
| 2024 | [LuckVd/dsh-pin-color](https://github.com/LuckVd/dsh-pin-color) | 0 | 2026-08-22 | 2026-08-23 | DeepSeek Harness (DSH) web 插件：会话置顶（本组/工作区全局）+ 会话 tab 颜色 + emoji，host 持久化，纯 DOM 增强不改 DSH 源码 |
| 2025 | [LUMOGRESS/dsh-skill-navigator](https://github.com/LUMOGRESS/dsh-skill-navigator) | 0 | 2026-08-29 | 2026-08-29 | DSH skill quick-picker and manager: one-click quick-pick (categories/search/context recommendations) + management (categories/updates/expert packs/market/panel settings). DSH 技能速查+管理插件。 |
| 2026 | [lunarmoon26/harness-alchemist](https://github.com/lunarmoon26/harness-alchemist) | 0 | 2026-08-23 | 2026-08-24 | One scaffold, five agent harnesses — portable coding-agent plugins for Claude Code, Codex, OpenCode, Antigravity, and DeepSeek Harness. |
| 2027 | [luoghong/dsh-session-recorder](https://github.com/luoghong/dsh-session-recorder) | 0 | 2026-08-29 | 2026-08-30 | 记录和deek Harness对话记录为md格式 |
| 2028 | [luomeii/dsh-review-squad](https://github.com/luomeii/dsh-review-squad) | 0 | 2026-08-30 | 2026-08-30 | DeepSeek Harness 并行多角色代码评审插件：/review 派出安全/正确性/测试/风格四名只读评审员子代理（可各自指定模型与思考强度），汇总为结构化报告。 |
| 2029 | [lurejewel/dsh-usage-plugin](https://github.com/lurejewel/dsh-usage-plugin) | 0 | 2026-08-25 | 2026-08-25 | Lightweight, native sidebar usage panel for DeepSeek Harness: official balance + token usage history from session logs. |
| 2030 | [lussey820/dsh-essentials-bundle](https://github.com/lussey820/dsh-essentials-bundle) | 0 | 2026-08-26 | 2026-08-27 | DSH (DeepSeek Harness) Web UI all-in-one essentials pack — a bundled collection, not a single-feature plugin: chat wallpaper / token usage stats / session manager / per-turn undo with artifact rollback / built-in file explorer & editor. Zero-dependency, inject-only, never overrides core. |
| 2031 | [luxueliu/luxueliu-agent-discipline-skills](https://github.com/luxueliu/luxueliu-agent-discipline-skills) | 0 | 2026-08-25 | 2026-08-27 | AI 不缺聪明，缺纪律！交付前自检（没从磁盘回读不算完成）/跑偏纠偏（一句「你偏了」就停）/系统化调试（同一个修复猜三次不收敛时用）/多 agent 接力（防旧状态盖掉新写入）——4 个单文件技能零依赖，每条都来自真实翻车事故，DeepSeek Harness / Claude Code / Codex 通用 |
| 2032 | [luxueliu/luxueliu-dsh-md-writing-tools](https://github.com/luxueliu/luxueliu-dsh-md-writing-tools) | 0 | 2026-08-25 | 2026-08-26 | DSH 侧栏写作还靠手点？Word 手感快捷键一次装齐：加粗/斜体/删除线/行内代码/标题升降/插链接/格式刷；重复按键即取消格式，多行整行感知，侧栏升级被覆盖一键装回 — DeepSeek Harness 写作插件 |
| 2033 | [luxueliu/luxueliu-dsh-story](https://github.com/luxueliu/luxueliu-dsh-story) | 0 | 2026-08-26 | 2026-08-26 | DSH 写小说缺的四件事一次配齐！世界书角色卡拖进输入框，正文整篇进上下文；剧情断了 /gemini-sum 一键交接新窗；/out 导出干净成稿；/sum 一句话成角色卡/世界书；[论坛体][第二人称] 打字即展开 — DeepSeek Harness 创作插件 |
| 2034 | [luxueliu/luxueliu-intel-scout](https://github.com/luxueliu/luxueliu-intel-scout) | 0 | 2026-08-25 | 2026-08-27 | 每天自动巡 RSS：AI 简报 + 脑神经/意识简报，关键词过滤后压成速览+详情。DSH 插件；脚本仍是 Python / 计划任务。 |
| 2035 | [lw-storm/dsh-plugin-version-management](https://github.com/lw-storm/dsh-plugin-version-management) | 0 | 2026-08-24 | 2026-08-25 | This plugin provides version management and rollback capabilities. When another plugin causes an error that prevents DSH from launching, forcing you to clear all plugins, this plugin can quickly restore every locally saved plugin configuration. |
| 2036 | [lyaoliu/dsh-reasoning-effort-slider](https://github.com/lyaoliu/dsh-reasoning-effort-slider) | 0 | 2026-08-29 | 2026-08-29 | DSH Desktop reasoning effort slider plugin - 7-level effort control with whale-mom skin |
| 2037 | [lylarcher/dsh-model-capabilities](https://github.com/lylarcher/dsh-model-capabilities) | 0 | 2026-08-29 | 2026-08-29 | 一个DSH插件，为自定义模型配置输入类型(input)、推理模式（reasoningEfforts） |
| 2038 | [lyuwen/dsh-as-service](https://github.com/lyuwen/dsh-as-service) | 0 | 2026-08-26 | 2026-08-26 | Running DSH as a service on the background |
| 2039 | [lyuwen/dsh-steer-button](https://github.com/lyuwen/dsh-steer-button) | 0 | 2026-08-26 | 2026-08-27 | Queue, Steer, and Backlog for DSH. More diverse way to interact with the agent while it's running. |
| 2040 | [lyuwen/dsh-thinking-summary](https://github.com/lyuwen/dsh-thinking-summary) | 0 | 2026-08-27 | 2026-08-27 | Readable thinking display for DeepSeek Harness |
| 2041 | [lyuwen/dsh-tui](https://github.com/lyuwen/dsh-tui) | 0 | 2026-08-28 | 2026-08-28 | [WIP] TUI for DeepSeeh-Harness |
| 2042 | [Lzh3070/dsh-search-hub](https://github.com/Lzh3070/dsh-search-hub) | 0 | 2026-08-29 | 2026-08-29 | DeepSeek Harness 联网搜索多入口管理插件：DeepSeek 官方 / GLM（智谱）/ Kimi 多搜索模型共存，置顶一个web_search生效，设置页一键切换免重启 |
| 2043 | [LZMW/dsh-memory](https://github.com/LZMW/dsh-memory) | 0 | 2026-08-24 | 2026-08-28 | Persistent long-term memory plugin for DeepSeek Harness (dsh): single memory tool, markdown storage, auto session summary, curator governance, user-profile injection. |
| 2044 | [lzxcs/archive-vault-pro](https://github.com/lzxcs/archive-vault-pro) | 0 | 2026-08-26 | 2026-08-26 | 归档会话库：查看所有工作区的已归档会话、只读回看内容、右键取消归档（不影响官方逻辑）。 |
| 2045 | [lzxcs/btw-pro](https://github.com/lzxcs/btw-pro) | 0 | 2026-08-26 | 2026-08-26 | /btw 旁路问答：不打断当前会话（含流式输出中），基于当前上下文回答一个问题；答案以「旁答」命令结果行显示在主会话里，不进入主模型上下文。 |
| 2046 | [lzxcs/chat-width-pro](https://github.com/lzxcs/chat-width-pro) | 0 | 2026-08-26 | 2026-08-26 | 对话页面宽度设置：把固定的内容宽度暴露到设置页，默认 748px（应用当前宽度）。 |
| 2047 | [lzxcs/dsh-enter-swap](https://github.com/lzxcs/dsh-enter-swap) | 0 | 2026-08-26 | 2026-08-26 | Swap the web UI composer shortcuts: Ctrl/Meta+Enter inserts a newline, Shift+Enter sends. |
| 2048 | [lzxcs/dsh-tray-notify](https://github.com/lzxcs/dsh-tray-notify) | 0 | 2026-08-26 | 2026-08-26 | DSH → 托盘通知：agent 停顿 / 提问 / 计划审批 / 授权时调用 notify-sender.py 弹窗（--source dsh，托盘按蓝色主题区分于 Claude Code）。纯 node 侧插件。 |
| 2049 | [lzxcs/edit-diff-pro](https://github.com/lzxcs/edit-diff-pro) | 0 | 2026-08-26 | 2026-08-26 | Claude Code 风格的 edit/write diff 卡片：±3 行上下文、绝对行号、可配置默认展开（默认折叠）。 |
| 2050 | [lzxcs/file-diff-pro](https://github.com/lzxcs/file-diff-pro) | 0 | 2026-08-26 | 2026-08-26 | 产物文件点击弹窗查看本轮 diff（代码类文件）；非代码文件维持桌面打开。 |
| 2051 | [lzxcs/lag-trace-pro](https://github.com/lzxcs/lag-trace-pro) | 0 | 2026-08-26 | 2026-08-26 | DSH web UI performance recorder: auto-captures page jank (long animation frames, long tasks, frame freezes) with context snapshots, stored under ~/.dsh/perf/ |
| 2052 | [lzxcs/paste-file-path-pro](https://github.com/lzxcs/paste-file-path-pro) | 0 | 2026-08-26 | 2026-08-26 | Pasting non-image files into the web composer inserts their paths as @file references (host-side clipboard reading). |
| 2053 | [lzyuan549/dsh-plugin-auth](https://github.com/lzyuan549/dsh-plugin-auth) | 0 | 2026-08-22 | 2026-08-22 | Username/password authentication gate for the DeepSeek Harness Web UI |
| 2054 | [maiziman/cedardsh-model-probe](https://github.com/maiziman/cedardsh-model-probe) | 0 | 2026-08-31 | 2026-08-31 | CedarDSH Model Probe — Detects reasoning and image support for custom DeepSeek Harness models. |
| 2055 | [mapan0424/deepseek-harness-channels](https://github.com/mapan0424/deepseek-harness-channels) | 0 | 2026-08-28 | 2026-08-28 | Community channel plugins for DeepSeek Harness: core, visual config, and Feishu channel. |
| 2056 | [MarceloSenai/dsh-plugin-kie-ai](https://github.com/MarceloSenai/dsh-plugin-kie-ai) | 0 | 2026-08-28 | 2026-08-28 | DeepSeek Harness plugin: image and video generation over the KIE AI API |
| 2057 | [MaRi23333/dsh-serverchan-watchdog](https://github.com/MaRi23333/dsh-serverchan-watchdog) | 0 | 2026-08-25 | 2026-08-28 | DeepSeek Harness 的 Server酱推送插件：审批、计划评审或问答超时未处理时，发送微信/Server酱³ App 提醒。第三方非官方项目。 |
| 2058 | [mario03690/dsh-devkit](https://github.com/mario03690/dsh-devkit) | 0 | 2026-08-22 | 2026-08-22 | The small deterministic operations an agent needs mid-task. JSON/YAML round-trip, JSON Schema v |
| 2059 | [mario03690/dsh-duizhang](https://github.com/mario03690/dsh-duizhang) | 0 | 2026-08-22 | 2026-08-22 | Reconciliation: statements, invoices and ledgers that have to balance. Bank/credit statement PD |
| 2060 | [mario03690/dsh-kuajing](https://github.com/mario03690/dsh-kuajing) | 0 | 2026-08-22 | 2026-08-22 | Cross-border commerce: HS codes, customs invoices, mainland reachability. HS/HTS code lookup an |
| 2061 | [mario03690/dsh-validate](https://github.com/mario03690/dsh-validate) | 0 | 2026-08-22 | 2026-08-22 | test |
| 2062 | [mario03690/dsh-writer](https://github.com/mario03690/dsh-writer) | 0 | 2026-08-22 | 2026-08-22 | Long-form drafts with the structure already decided. Blog posts, press releases, product and jo |
| 2063 | [Mars-Sea/dsh-deeppilot](https://github.com/Mars-Sea/dsh-deeppilot) | 0 | 2026-08-24 | 2026-08-24 | Native iPhone companion plugin for DeepSeek Harness — sessions, approvals, questions, notifications, and secure remote access. |
| 2064 | [Marsax110/dsh-model-fixer](https://github.com/Marsax110/dsh-model-fixer) | 0 | 2026-08-25 | 2026-08-25 | 模型无关的沙箱升级修正 + 按模型定制的协议提示段：任何模型（GPT 系最常见）在工具调用中错误携带 sandbox_permissions/justification 导致 'not strictly wider' 死循环时自动剥离；并按会话模型动态注入适配提示段。非 bundle 插件，HMR 实时生效。 |
| 2065 | [marshfolx/dsh-rescue-tui](https://github.com/marshfolx/dsh-rescue-tui) | 0 | 2026-08-24 | 2026-08-25 | a minimal emergency maintenance tui used when web ui is broken |
| 2066 | [masknull/dsh-fetch-models-search](https://github.com/masknull/dsh-fetch-models-search) | 0 | 2026-08-26 | 2026-08-26 | DSH plugin: adds a search box to the Fetch available models candidate dialog in DSH settings (browser-side DOM enhancement). DSH 插件：为「获取可用模型」候选弹窗增加搜索过滤。 |
| 2067 | [masknull/dsh-message-collapse](https://github.com/masknull/dsh-message-collapse) | 0 | 2026-08-31 | 2026-08-31 | DSH plugin: auto-collapse long user messages in the web chat. 用户消息超10行自动折叠。 |
| 2068 | [masknull/dsh-session-prompt](https://github.com/masknull/dsh-session-prompt) | 0 | 2026-08-23 | 2026-08-25 | DSH 插件:在每个会话的系统提示词最顶部注入自定义提示词,并可在 Web 设置页中即时编辑。 |
| 2069 | [masknull/dsh-workspace-default-path](https://github.com/masknull/dsh-workspace-default-path) | 0 | 2026-08-29 | 2026-08-29 | DSH 插件：添加工作区时记住上次使用的目录，下次打开浏览对话框直接定位（预填+自动记忆，官方流程不动）。DSH plugin: remember the last used workspace directory for Add workspace - prefill + auto-memory over the official flow. |
| 2070 | [Mason-1011/dsh-schematic](https://github.com/Mason-1011/dsh-schematic) | 0 | 2026-08-25 | 2026-08-30 | Live plugin-topology viewer for DeepSeek Harness — the wiring diagram of mounted plugins, their runtime activity, and a composer-side star map. Pure observer. |
| 2071 | [MasterBenC/shangshi-dsh](https://github.com/MasterBenC/shangshi-dsh) | 0 | 2026-08-31 | 2026-08-31 | Shangshi DeepSeek Harness plugin for local Qimen business timing. |
| 2072 | [MauricioPerera/kdd-gates](https://github.com/MauricioPerera/kdd-gates) | 0 | 2026-08-27 | 2026-08-27 | KDD methodology gates as DeepSeek Harness (dsh) plugin tools |
| 2073 | [mc856/dsh-project-portfolio](https://github.com/mc856/dsh-project-portfolio) | 0 | 2026-08-31 | 2026-08-31 | Unofficial DSH plugin: long-term, cross-project memory for coding agents — embedded project-portfolio skill + portfolio_status/portfolio_log tools over plain markdown. Not affiliated with DeepSeek. |
| 2074 | [me9rez/dsh-pwsh-style](https://github.com/me9rez/dsh-pwsh-style) | 0 | 2026-08-28 | 2026-08-28 | 修改 DSH 会话回复中 pwsh(PowerShell) 工具卡片的主题、字体与可读性增强。Restyle pwsh tool-call cards in DSH: themes, system fonts, copy & expand, workdir display. |
| 2075 | [MEMZ-Edge01/GrokBot_in_DeepseekHerness](https://github.com/MEMZ-Edge01/GrokBot_in_DeepseekHerness) | 0 | 2026-08-22 | 2026-08-31 | 将GrokBot宠物代入DSH网页端并加入拖拽效果和通知功能 |
| 2076 | [Mengshang-spec/dsh-third-party-api-balance-wallet](https://github.com/Mengshang-spec/dsh-third-party-api-balance-wallet) | 0 | 2026-08-27 | 2026-08-27 | 第三方 API 接入 DSH 查询余额插件 |
| 2077 | [mengxingGG/dsh-plugin-marketplace](https://github.com/mengxingGG/dsh-plugin-marketplace) | 0 | 2026-08-25 | 2026-08-25 | GitHub plugin discovery and one-click profile installation for DeepSeek Harness |
| 2078 | [mervin1944/dsh-version-badge](https://github.com/mervin1944/dsh-version-badge) | 0 | 2026-08-31 | 2026-08-31 | DSH 版本号徽标插件：侧边栏设置按钮上方显示 dsh 版本，带检查更新与一键部署。DSH version badge plugin with update check & one-click deploy. |
| 2079 | [metabolism-tools/workspace-metabolism](https://github.com/metabolism-tools/workspace-metabolism) | 0 | 2026-08-15 | 2026-08-31 | Govern what Claude Code, Codex, Aider and OpenClaw leave in your workspace: one JSON policy file, audit, recyclable clean, rollback, hash-chained audit trail. |
| 2080 | [Meteor-system/superpowers-for-dsh](https://github.com/Meteor-system/superpowers-for-dsh) | 0 | 2026-08-25 | 2026-08-26 | SuperPowers for DSH: portable Superpowers skills and a native DeepSeek Harness preset |
| 2081 | [meyaomiao/dsh-files-native](https://github.com/meyaomiao/dsh-files-native) | 0 | 2026-08-30 | 2026-08-30 | DSH 插件：接近原生质感的附件上传（拖入/粘贴/回形针，图片与文件混排） |
| 2082 | [mhdfy1988/dsh-codex-auth](https://github.com/mhdfy1988/dsh-codex-auth) | 0 | 2026-08-23 | 2026-08-26 | ChatGPT/Codex authorization plugin for DeepSeek Harness |
| 2083 | [mhdfy1988/dsh-skill-manager](https://github.com/mhdfy1988/dsh-skill-manager) | 0 | 2026-08-24 | 2026-08-26 | Non-invasive Skill lifecycle manager for DeepSeek Harness |
| 2084 | [mhdfy1988/dsh-skin-platform](https://github.com/mhdfy1988/dsh-skin-platform) | 0 | 2026-08-23 | 2026-08-26 | Independent multi-package skin platform for DeepSeek Harness |
| 2085 | [MichaelGong/dsh-session-hover-preview](https://github.com/MichaelGong/dsh-session-hover-preview) | 0 | 2026-08-27 | 2026-08-27 | Codex-style user-message navigation for DeepSeek Harness conversations |
| 2086 | [Mide69/dsh-boot-doctor](https://github.com/Mide69/dsh-boot-doctor) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness plugin: console log sink and stuck-plugin warnings |
| 2087 | [minatoAI/dsh-net-proxy-plugin](https://github.com/minatoAI/dsh-net-proxy-plugin) | 0 | 2026-08-30 | 2026-08-31 | DeepSeek Harness fallback network proxy plugin: detects system proxies, probes overseas connectivity (Google/GitHub), routes dsh outbound HTTP through a working local proxy |
| 2088 | [ming-14/dsh-forwarder](https://github.com/ming-14/dsh-forwarder) | 0 | 2026-08-23 | 2026-08-24 | Make DeepSeek Harness (DSH) accessible over the local area network for other devices such as phones and tablets to access without modifying any DSH configuration |
| 2089 | [Minglink/dsh-better-sidebar](https://github.com/Minglink/dsh-better-sidebar) | 0 | 2026-08-25 | 2026-08-25 | 开放的侧边栏底座，支持三方拓展注册新侧边栏页面 |
| 2090 | [Minglink/dsh-deep-whale](https://github.com/Minglink/dsh-deep-whale) | 0 | 2026-08-25 | 2026-08-25 | 适用于 DeepSeek Harness 的鲸鱼娘系列皮肤主题 |
| 2091 | [Minglink/dsh-plugin-agent-workflow](https://github.com/Minglink/dsh-plugin-agent-workflow) | 0 | 2026-08-25 | 2026-08-25 | DeepSeek Harness Agent Workflow 工作流引擎插件 |
| 2092 | [Minglink/modlens](https://github.com/Minglink/modlens) | 0 | 2026-08-25 | 2026-08-25 | DeepSeek Harness 外挂视觉多模态与 OCR 桥接插件 |
| 2093 | [mingzhong15/dsh-cursor-passthrough](https://github.com/mingzhong15/dsh-cursor-passthrough) | 0 | 2026-08-27 | 2026-08-27 | Add a Cursor passthrough group to the DSH chat model picker. |
| 2094 | [MisRightW/dsh-taskboard](https://github.com/MisRightW/dsh-taskboard) | 0 | 2026-08-20 | 2026-08-21 | dsh-taskboard |
| 2095 | [Missher12/dsh-missher-evolution](https://github.com/Missher12/dsh-missher-evolution) | 0 | 2026-08-24 | 2026-08-25 | Privacy-bounded self-improvement plugin for DeepSeek Harness |
| 2096 | [Missher12/dsh-project-ops](https://github.com/Missher12/dsh-project-ops) | 0 | 2026-08-27 | 2026-08-27 | Scoped project task discovery and execution receipts for DeepSeek Harness |
| 2097 | [MitsukiJoe/dsh-better-ux](https://github.com/MitsukiJoe/dsh-better-ux) | 0 | 2026-08-17 | 2026-08-23 | Web UX kit for DeepSeek Harness: session row actions and a large model picker |
| 2098 | [MitsukiJoe/dsh-vision-router-inline](https://github.com/MitsukiJoe/dsh-vision-router-inline) | 0 | 2026-08-17 | 2026-08-23 | Display companion for dsh-vision-router: square picture button on each original model row |
| 2099 | [ml020/dsh-workbuddy](https://github.com/ml020/dsh-workbuddy) | 0 | 2026-08-28 | 2026-08-28 | Wordless-styled WorkBuddy hero for DSH: replaces the blank-session brand mark and workspace picker while keeping the native composer. |
| 2100 | [mobaixingyao/dsh-inform](https://github.com/mobaixingyao/dsh-inform) | 0 | 2026-08-25 | 2026-08-25 | dsh-inform 是一款为 deepseek harness开发的任务提醒插件，能够在 DSH 完成任务、需要批准 或 需要回答 时自动调用系统通知发出提醒 |
| 2101 | [MochiNek0/dsh-vendor-login](https://github.com/MochiNek0/dsh-vendor-login) | 0 | 2026-08-25 | 2026-08-25 | Sign in to AI coding plans that have no API key — Claude Pro/Max/Team, ChatGPT Plus/Pro, Copilot, SuperGrok — from the dsh settings UI. |
| 2102 | [Momojie-S/dsh-archive-retention](https://github.com/Momojie-S/dsh-archive-retention) | 0 | 2026-08-29 | 2026-08-29 | DSH 插件: 归档会话定期清理 —— 物理归档堆与页面归档会话超保留期(页面可配天/小时,cron 调度)自动物理删除 |
| 2103 | [Momojie-S/dsh-subagent-cleanup](https://github.com/Momojie-S/dsh-subagent-cleanup) | 0 | 2026-08-25 | 2026-08-26 | DSH 插件: 子agent会话清理 —— 会话自清 + 运维侧跨workspace大扫除(归档可逆/可彻底删除) |
| 2104 | [Momojie-S/dsh-subagent-idle-delivery](https://github.com/Momojie-S/dsh-subagent-idle-delivery) | 0 | 2026-08-25 | 2026-08-25 | DSH plugin: hold busy-parent subagent notices, deliver as fresh turns when idle (hold-and-release) |
| 2105 | [Monicaxixi/dsh-loglens](https://github.com/Monicaxixi/dsh-loglens) | 0 | 2026-08-24 | 2026-08-24 | DeepSeek Harness dsh-plugin for bounded, cursor-aware log inspection |
| 2106 | [Moolmool114/dsh-client-ui-recipes](https://github.com/Moolmool114/dsh-client-ui-recipes) | 0 | 2026-08-23 | 2026-08-23 | Interface Recipes — a DeepSeek Harness dsh.client plugin: user-defined, switchable chat-surface display schemes (timeline, result panel, process groups, catalog, dimming). |
| 2107 | [Moonshile/moonshile-dsh-plugins](https://github.com/Moonshile/moonshile-dsh-plugins) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness (DSH) plugins — dsh-workspace-sort: re-sorts sidebar workspaces by last activity once per day. One-command npm bundle install. |
| 2108 | [moonwellxh/DSH-Launcher](https://github.com/moonwellxh/DSH-Launcher) | 0 | 2026-08-27 | 2026-08-30 | DSH 魔偶助手（DSH一键启动托盘）(DeepSeek Harness launcher / tray) |
| 2109 | [moreWax/dsh-prime-agent](https://github.com/moreWax/dsh-prime-agent) | 0 | 2026-08-24 | 2026-08-25 | Closed learning loop for DeepSeek Harness: Prime Agent memory/skills bridge + OKF/OpenWiki provenance-aware knowledge serving |
| 2110 | [moreWax/dsh-remote-exec](https://github.com/moreWax/dsh-remote-exec) | 0 | 2026-08-24 | 2026-08-25 | SSH / MOSH / SAM remote execution providers for DeepSeek Harness — run the agent locally, execute on your servers |
| 2111 | [morphlinglan/dsh-leopard-gecko](https://github.com/morphlinglan/dsh-leopard-gecko) | 0 | 2026-08-28 | 2026-08-28 | 豹纹守宫旅行桌宠小插件：一只会自己出门旅行、寄回明信片、带回特产的守宫。庭院三叶草随时间生长，收割后可在商店购买便当与护身符。 |
| 2112 | [mtaech/dsh-browser-tool](https://github.com/mtaech/dsh-browser-tool) | 0 | 2026-08-25 | 2026-08-25 | DSH 浏览器工具：驱动 Chromium 标签页（headless / CDP attach / 拉起桌面应用 / 经 Browser Relay 接管真实 Chrome），open-close-run 三段式 + tab 脚本 API，移植自 oh-my-pi |
| 2113 | [mtdx2001/dsh-think-translate](https://github.com/mtdx2001/dsh-think-translate) | 0 | 2026-08-29 | 2026-08-29 | Display-layer translation for the DeepSeek Harness Web UI: thinking chain, task cards and answers in 8 languages - pure display layer, originals untouched, local-first with failover. |
| 2114 | [Muredsa/dsh-benchup](https://github.com/Muredsa/dsh-benchup) | 0 | 2026-08-26 | 2026-08-26 | Install with npm i dsh-benchup. Reproducible, profile-aware benchmarks for DeepSeek Harness — compare models, plugins, prompts, and agent strategies. |
| 2115 | [Mutton-hub/adatile-mcp](https://github.com/Mutton-hub/adatile-mcp) | 0 | 2026-08-22 | 2026-08-23 | AdaTile-MCP: high-resolution image adaptive tiling MCP server for DeepSeek vision model (deepseek-v4-flash-vision-exp). L1-L6 pipeline (fastpath, saliency, adaptive tiling, Files API assembly, streaming VLM, rule-based merge) + eval harness. Setup: clone, run setup.bat, add your agent MCP config -> see README. |
| 2116 | [MuziiXzx/dsh-taskdone-notify](https://github.com/MuziiXzx/dsh-taskdone-notify) | 0 | 2026-08-23 | 2026-08-23 | 任务完成时通知用户 |
| 2117 | [my-dsh/dsh-session-attention](https://github.com/my-dsh/dsh-session-attention) | 0 | 2026-08-28 | 2026-08-28 | Session attention overlay plugin for DeepSeek Harness: character dance animation while any session awaits user action |
| 2118 | [my-dsh/dsh-token-usage-dashboard](https://github.com/my-dsh/dsh-token-usage-dashboard) | 0 | 2026-08-28 | 2026-08-28 | Cross-session token usage dashboard plugin for DeepSeek Harness: SQLite-backed capture + browser dashboard panel |
| 2119 | [mycodesite/dsh-rules](https://github.com/mycodesite/dsh-rules) | 0 | 2026-08-26 | 2026-08-27 | DeepSeek Harness (dsh) 插件：全局+项目两级 Markdown 规则注入（RuleBase） |
| 2120 | [mykeura/dsh-minimalist-themes](https://github.com/mykeura/dsh-minimalist-themes) | 0 | 2026-08-26 | 2026-08-27 | 18 minimalist color themes for DeepSeek Harness. Pick one with a single click — it's just another plugin. |
| 2121 | [N9-Developer-Empowerment/DSH-Vibeify](https://github.com/N9-Developer-Empowerment/DSH-Vibeify) | 0 | 2026-08-26 | 2026-08-29 | Turn AI work into a living local magazine for DeepSeek Harness. DeepSeek, ChatGPT, or both. |
| 2122 | [Nath-Vikky/dsh-codekin](https://github.com/Nath-Vikky/dsh-codekin) | 0 | 2026-08-24 | 2026-08-28 | Codekin: a creature-collection and match-three RPG for DeepSeek Harness Web. |
| 2123 | [NattoCB/dsh-plugin-sidebar-views](https://github.com/NattoCB/dsh-plugin-sidebar-views) | 0 | 2026-08-31 | 2026-08-31 | Sidebar views switcher for DeepSeek Harness: workspaces / recent sessions, pinned sessions group, per-row pin & copy-session-id menu |
| 2124 | [navid-kianfar/dsh-add-assets](https://github.com/navid-kianfar/dsh-add-assets) | 0 | 2026-08-26 | 2026-08-26 | Options plate on the DeepSeek Harness composer's + button — pick files and folders from the project or anywhere on the machine, upload from your device, or run a slash command — with inline path chips and a Claude Code-style attachment preview. |
| 2125 | [navid-kianfar/dsh-advanced-sidebar](https://github.com/navid-kianfar/dsh-advanced-sidebar) | 0 | 2026-08-26 | 2026-08-26 | Advanced sidebar operations for the DeepSeek Harness Web Client: git changes, a terminal, a file browser, a dev-server preview, background tasks, Open in, Archive and Delete. |
| 2126 | [navid-kianfar/dsh-memory](https://github.com/navid-kianfar/dsh-memory) | 0 | 2026-08-26 | 2026-08-26 | Persistent, searchable, per-project memory for the DeepSeek Harness: decisions, rules, and session context in a queryable DuckDB file, with the rule set injected into every model request — plus a full management UI in the Web Client. |
| 2127 | [navid-kianfar/dsh-tasks-manager](https://github.com/navid-kianfar/dsh-tasks-manager) | 0 | 2026-08-26 | 2026-08-26 | DeepSeek Harness plugin: a project task board kept with the project as a queryable SQLite file, with a kanban/list view in the Web Client, model-facing task tools, and cards you can dispatch to the agent as background jobs. |
| 2128 | [navid-kianfar/dsh-usage-info](https://github.com/navid-kianfar/dsh-usage-info) | 0 | 2026-08-26 | 2026-08-26 | Context occupancy and account balance for the DeepSeek Harness Web Client — a session-header readout with a swappable balance provider. |
| 2129 | [navid-kianfar/dsh-worktree](https://github.com/navid-kianfar/dsh-worktree) | 0 | 2026-08-26 | 2026-08-26 | Git worktrees and branches for the DeepSeek Harness Web Client: a session-header chip that switches branches, creates worktrees, and opens them as harness workspaces. |
| 2130 | [Nay-1/dsh-skill-manage](https://github.com/Nay-1/dsh-skill-manage) | 0 | 2026-08-22 | 2026-08-22 | DeepSeek Harness 技能管理设置页插件：图形化管理用户级/项目级技能的安装、卸载与调用启停 |
| 2131 | [NecromanAlbert/dsh-i-have-adhd](https://github.com/NecromanAlbert/dsh-i-have-adhd) | 0 | 2026-08-26 | 2026-08-26 | Always-on ADHD-friendly output for every DeepSeek Harness session. Host systemPrompt, not a skill catalog item. |
| 2132 | [NecromanAlbert/dsh-self-restart](https://github.com/NecromanAlbert/dsh-self-restart) | 0 | 2026-08-26 | 2026-08-26 | Any DSH session can request a Desktop restart, then the same persisted session is resumed and followup'd with its mission. |
| 2133 | [NecromanAlbert/dsh-skill-slash-fuzzy](https://github.com/NecromanAlbert/dsh-skill-slash-fuzzy) | 0 | 2026-08-25 | 2026-08-26 | Resolve unique kebab-case skill substrings in DeepSeek Harness slash tokens. |
| 2134 | [NeoRrrr/dsh-project-skill-paths](https://github.com/NeoRrrr/dsh-project-skill-paths) | 0 | 2026-08-25 | 2026-08-25 | Project-scoped custom Skill roots for DeepSeek Harness |
| 2135 | [NevermindZZT/dsh-manager-plugin](https://github.com/NevermindZZT/dsh-manager-plugin) | 0 | 2026-08-23 | 2026-08-24 | dsh manger 远程工具对应使用的 dsh 插件，直接完成 dsh 远程访问 |
| 2136 | [NexusAgentX/dsh-advisor](https://github.com/NexusAgentX/dsh-advisor) | 0 | 2026-08-23 | 2026-08-26 | dsh plugin bundle porting the rpiv advisor subsystem: an on-demand zero-parameter advisor() tool that forwards the full session to a separately-configured reviewer model. |
| 2137 | [nicecx/dsh-auto-approver](https://github.com/nicecx/dsh-auto-approver) | 0 | 2026-08-31 | 2026-08-31 | Configurable auto-approval for DeepSeek Harness: intercepts approval/request and answers allowed-once/rejected by policy (allow-all/allowlist/off + denyAlways), with a full audit log. |
| 2138 | [nicecx/dsh-reset-handoff](https://github.com/nicecx/dsh-reset-handoff) | 0 | 2026-08-30 | 2026-08-30 | DSH never restarts itself: host plugin that hands reset requests to an external ops agent (e.g. Hermes) via a versioned JSON protocol — preflight → gate → restart → health-check → recover → deliver back |
| 2139 | [nicecx/dsh-task-queue](https://github.com/nicecx/dsh-task-queue) | 0 | 2026-08-31 | 2026-08-31 | Tiered task queue for DSH↔Hermes: queue.json single source of truth, lease/claim model, concurrency-1; Hermes-side cron consumes, DSH-side enqueues. Includes busy-mutex for the approve fast path. |
| 2140 | [nickkkkkk123123/dsh-resume-on-restart](https://github.com/nickkkkkk123123/dsh-resume-on-restart) | 0 | 2026-08-28 | 2026-08-28 | DSH 插件：重启后自动唤醒 agent 并投递信息性消息，agent 自主决定是否恢复工作 |
| 2141 | [nickkkkkk123123/dsh-whale-girl](https://github.com/nickkkkkk123123/dsh-whale-girl) | 0 | 2026-08-27 | 2026-08-27 | 鲸鱼娘·灵动挂件 — 会卖萌、会记账、会弹跳的 DSH 桌面挂件插件（余额/用量/上下文/峰谷/右键菜单/拖动甩抛） |
| 2142 | [nienieai/dsh-canmv-k230-bridge](https://github.com/nienieai/dsh-canmv-k230-bridge) | 0 | 2026-08-21 | 2026-08-26 | DSH 动态插件：桥接 CanMV K230 开发板（悬浮面板 + 串口运行脚本与预览） |
| 2143 | [ningbonb/dsh-web-desktop](https://github.com/ningbonb/dsh-web-desktop) | 0 | 2026-08-31 | 2026-08-31 | Electron launcher for DeepSeek Harness Web profiles / DeepSeek Harness Web Profile 的 Electron 桌面启动器 |
| 2144 | [nishuoyang/dsh-wallpaper-bg](https://github.com/nishuoyang/dsh-wallpaper-bg) | 0 | 2026-08-15 | 2026-08-25 | DeepSeek Harness Web UI Standalone Wallpaper Background Plugin: Three sources including built-in wallpapers, custom uploads, and Wallpaper Engine library (read-only). Supports image, video, and scene preview rendering, along with adjustments for overlay, blur, brightness, and safe zoom. |
| 2145 | [niushuanan/dsh-adaptive-update](https://github.com/niushuanan/dsh-adaptive-update) | 0 | 2026-08-26 | 2026-08-26 | Check upstream manually or every six hours, use a narrowly scoped agent for compatibility work, and switch atomically with rollback. |
| 2146 | [niushuanan/dsh-chat-migration](https://github.com/niushuanan/dsh-chat-migration) | 0 | 2026-08-29 | 2026-08-29 | Native DeepSeek chat migration and workspace-free chat mode for DeepSeek Harness |
| 2147 | [niushuanan/dsh-image-vision](https://github.com/niushuanan/dsh-image-vision) | 0 | 2026-08-26 | 2026-08-26 | Let vision-capable models read native attachments while giving text-only models an image tool that supports follow-up questions. |
| 2148 | [niushuanan/dsh-model-usage](https://github.com/niushuanan/dsh-model-usage) | 0 | 2026-08-26 | 2026-08-26 | Inspect model quotas, periods, and refresh state by provider in Settings, with data loaded only when the user opens the page. |
| 2149 | [niushuanan/dsh-multi-window](https://github.com/niushuanan/dsh-multi-window) | 0 | 2026-08-26 | 2026-08-26 | Open multiple independent conversations side by side, each with isolated navigation, drafts, and runtime state. |
| 2150 | [niushuanan/dsh-parallel-worktree](https://github.com/niushuanan/dsh-parallel-worktree) | 0 | 2026-08-26 | 2026-08-26 | Move parallel tasks into isolated Git worktrees, inspect conflicts, and merge the results safely into the current branch. |
| 2151 | [niushuanan/dsh-pure-chat](https://github.com/niushuanan/dsh-pure-chat) | 0 | 2026-08-26 | 2026-08-26 | Start a chat immediately without a workspace, work mode, or execution permissions while keeping image and text-file uploads. |
| 2152 | [niushuanan/dsh-selection-memory](https://github.com/niushuanan/dsh-selection-memory) | 0 | 2026-08-26 | 2026-08-26 | Quote, discuss, or remember selected conversation text, then maintain durable context in separate editable user and AI memories. |
| 2153 | [niushuanan/dsh-skill-manager](https://github.com/niushuanan/dsh-skill-manager) | 0 | 2026-08-26 | 2026-08-26 | Browse installed Skills, their files, and content in Settings, then adaptively import from a file, folder, ZIP, or GitHub with AI. |
| 2154 | [niushuanan/dsh-teamwork](https://github.com/niushuanan/dsh-teamwork) | 0 | 2026-08-26 | 2026-08-26 | Run collaborating agents and external experts concurrently under one coordinating agent, then bring every result back into the current task. |
| 2155 | [niushuanan/dsh-token-overview](https://github.com/niushuanan/dsh-token-overview) | 0 | 2026-08-26 | 2026-08-26 | See tokens, cache usage, calls, active periods, and estimated cost across AI clients on the whole computer. |
| 2156 | [niushuanan/dsh-whale-girl](https://github.com/niushuanan/dsh-whale-girl) | 0 | 2026-08-26 | 2026-08-26 | Add a native cross-page companion whose presence, shortcuts, and feedback follow the current DSH session state. |
| 2157 | [NiuZhuang/dsh-git-ai](https://github.com/NiuZhuang/dsh-git-ai) | 0 | 2026-08-22 | 2026-08-23 | A DeepSeek Harness plugin that records which files the agent edited, with which model, and in which session into git-ai |
| 2158 | [njuptlzf/dsh-ponytail](https://github.com/njuptlzf/dsh-ponytail) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness (DSH) 插件：常驻注入 Ponytail 懒高级工程师规范，5 个同伴技能落盘为可调用的 skill。安装：dsh plugin add github:njuptlzf/dsh-ponytail |
| 2159 | [Nkjv2/dsh-ui-pet](https://github.com/Nkjv2/dsh-ui-pet) | 0 | 2026-08-23 | 2026-08-23 | A canvas sprite-sheet pet plugin for the DeepSeek Harness web GUI. A dsh bundle + client plugin that renders a pointer-following mascot in the shell.overlay layer. MIT licensed. |
| 2160 | [nmsl1234/dsh-privacy-gate](https://github.com/nmsl1234/dsh-privacy-gate) | 0 | 2026-08-31 | 2026-08-31 | dsh-plugin |
| 2161 | [NOirBRight/dsh-mobile-pairing](https://github.com/NOirBRight/dsh-mobile-pairing) | 0 | 2026-08-21 | 2026-08-29 | DSH Mobile Remote pairing plugin |
| 2162 | [NOirBRight/dsh-plugins](https://github.com/NOirBRight/dsh-plugins) | 0 | 2026-08-29 | 2026-08-30 | Independent catalog of DSH plugins and mobile companion published by NOirBRight |
| 2163 | [NonchalantLudens/dsh-side-dir](https://github.com/NonchalantLudens/dsh-side-dir) | 0 | 2026-08-23 | 2026-08-24 | Project directory preview for the DeepSeek Harness web GUI — details-panel file tree + read-only file preview via a fenced /dirpreview command |
| 2164 | [Nth-5620/dsh-crystal-viewer](https://github.com/Nth-5620/dsh-crystal-viewer) | 0 | 2026-08-29 | 2026-08-30 | A crystal-structure visualization window for DeepSeek Harness: 3D structure + Q-peak viewer and parameter panel, opened as a dsh-better-sidebar tab. |
| 2165 | [null-object-0000/dsh-output-style](https://github.com/null-object-0000/dsh-output-style) | 0 | 2026-08-31 | 2026-08-31 | 会话级输出风格插件：/style 命令 + Web 选择器，改变模型如何呈现答案（default/adhd-friendly/eli5/bluf）。Session-scoped output styles for DeepSeek Harness. |
| 2166 | [NyaaCaster/dsh-yuque-kb](https://github.com/NyaaCaster/dsh-yuque-kb) | 0 | 2026-08-24 | 2026-08-28 | dsh web插件，语雀文档知识库化在dsh中调用 |
| 2167 | [odelbos/dsh-models-filter](https://github.com/odelbos/dsh-models-filter) | 0 | 2026-08-29 | 2026-08-31 | DeepSeek Harness plugin used to add an input filed to filter the models menu. (with arrow up/down + enter) |
| 2168 | [of1102/dsh-web-search-ark](https://github.com/of1102/dsh-web-search-ark) | 0 | 2026-08-25 | 2026-08-25 | Volcengine Ark web-search provider plugin for DeepSeek Harness |
| 2169 | [oh-summy/dsh-remote-control](https://github.com/oh-summy/dsh-remote-control) | 0 | 2026-08-30 | 2026-08-30 | Secure remote access for DeepSeek Harness (DSH): Cloudflare Tunnel + password gate + Feishu notifications. macOS first, Linux first-class. |
| 2170 | [oksure/dsh-mobile-comfort](https://github.com/oksure/dsh-mobile-comfort) | 0 | 2026-08-25 | 2026-08-25 | Touch-device comfort fixes for the DeepSeek Harness web client: ghost tooltip suppression + touch-action policy |
| 2171 | [Olina1Ye/internal-skill-workshop-plugin](https://github.com/Olina1Ye/internal-skill-workshop-plugin) | 0 | 2026-08-27 | 2026-08-27 | A read-only DeepSeek Harness Web plugin for browsing a configured Skill Base catalog. |
| 2172 | [Oliver0804/dsh-openrouter-monitor](https://github.com/Oliver0804/dsh-openrouter-monitor) | 0 | 2026-08-27 | 2026-08-27 | DSH plugin: OpenRouter account balance, per-key spend, alert thresholds and trend charts under the composer. |
| 2173 | [Oliver0804/dsh-peak-pricing](https://github.com/Oliver0804/dsh-peak-pricing) | 0 | 2026-08-17 | 2026-08-27 | DSH plugin: DeepSeek peak/off-peak pricing, flat rates for other providers like z-ai/glm-5.3-flash, live per-session cost estimate and a hover cache-hit trend chart. |
| 2174 | [Olympianz/dsh-deploy-master](https://github.com/Olympianz/dsh-deploy-master) | 0 | 2026-08-30 | 2026-08-30 | A DSH deploy-assistant plugin: GitHub publish + Linear sync + npm publish + community announcement. |
| 2175 | [Olympianz/dsh-desktop-packager](https://github.com/Olympianz/dsh-desktop-packager) | 0 | 2026-08-31 | 2026-08-31 | Package a built DeepSeek Harness checkout into a distributable macOS desktop app (.app + .dmg) with a standalone Node runtime and an Electron shell, customized through a Web Settings section (logo/VI theme, bundled plugins, bundled models, users & permissions). |
| 2176 | [Olympianz/dsh-heatmap](https://github.com/Olympianz/dsh-heatmap) | 0 | 2026-08-30 | 2026-08-30 | DeepSeek Harness 页面埋点与热力图分析插件：科学埋点采集、本地热力图与统计、CLI/HTTP 接口、上传授权。 |
| 2177 | [onclaw-dev/dsh-ima-copilot](https://github.com/onclaw-dev/dsh-ima-copilot) | 0 | 2026-08-30 | 2026-08-30 | 腾讯 IMA 是一个非常好的知识库应用，但是他们提供的skill版本针对公开知识库的检索方式只提供了基于文件标题的关键字检索，好一阵无语。为了补足在harness的这种知识库检索能力，基于tencent-ima-copilot-mcp迭代了对应的dsh版本。 |
| 2178 | [onclaw-dev/dsh-workflow-designer](https://github.com/onclaw-dev/dsh-workflow-designer) | 0 | 2026-08-31 | 2026-08-31 | `dsh-workflow-designer` 是面向 DeepSeek Harness 的提示词优先工作流设计插件。它收集当前 Agent 可见的本地 Skill、原生 Tool 与 MCP Tool，提供必要的可视化编排和约束编辑能力，并导出稳定的 YAML 中间表示。后续可由大模型及对应框架把 YAML 生成 Python、`workflow.mjs` 或其他代码工作流。 |
| 2179 | [oneirictouch/dsh-explorer-editor](https://github.com/oneirictouch/dsh-explorer-editor) | 0 | 2026-08-22 | 2026-08-22 | 左侧边栏的“资料浏览器”和主工作区的“文本编辑器”，页签方式展示，适合讨厌工作区被过度分割的人。 |
| 2180 | [opdsh/unity-plugin](https://github.com/opdsh/unity-plugin) | 0 | 2026-08-28 | 2026-08-28 | DeepSeek Harness plugin: control the Unity Editor through the unity CLI |
| 2181 | [Oscar-Williams/dsh-deepcanary](https://github.com/Oscar-Williams/dsh-deepcanary) | 0 | 2026-08-29 | 2026-08-30 | Local attention supervision for DeepSeek Harness: evidence-first signals, quiet notifications, and an actionable inbox. |
| 2182 | [oThTJx/dsh-always-apply](https://github.com/oThTJx/dsh-always-apply) | 0 | 2026-08-17 | 2026-08-27 | DeepSeek Harness plugin: injects alwaysApply-marked skill bodies into sessions before the first model request — no skill tool load needed. |
| 2183 | [oThTJx/dsh-superpowers](https://github.com/oThTJx/dsh-superpowers) | 0 | 2026-08-17 | 2026-08-27 | DeepSeek Harness plugin: obra/superpowers skill library adapted to dsh tooling, plus a session-start bootstrap — brainstorming, systematic debugging, TDD, planning and more. |
| 2184 | [outprintHelloLi/dsh-piggy-bank](https://github.com/outprintHelloLi/dsh-piggy-bank) | 0 | 2026-08-25 | 2026-08-25 | dsh插件：DeepSeek 余额展示 |
| 2185 | [pacoyi/dsh-memory-lite](https://github.com/pacoyi/dsh-memory-lite) | 0 | 2026-08-28 | 2026-08-28 | Lightweight cross-session memory plugin for DeepSeek Harness: approval-gated `memory` tool (save/recall/list/forget) + Settings card UI to browse, add, delete (two-click, trash/restore) and idempotent import/export. \| DeepSeek Harness 跨会话记忆插件：审批门控 memory 工具 + 设置页UI「记忆库」卡片（查看/新增/删除、两击确认、回收站恢复、导入/导出记忆——幂等迁移、冲突拒绝）。 |
| 2186 | [PaidaxingTuT/dsh-code-runner](https://github.com/PaidaxingTuT/dsh-code-runner) | 0 | 2026-08-29 | 2026-08-29 | 在 DSH-better-sidebar 中一键运行侧边栏代码文件，让代码可以在dsh终端中运行 |
| 2187 | [Pappet/dsh-tool-imagegen](https://github.com/Pappet/dsh-tool-imagegen) | 0 | 2026-08-30 | 2026-08-31 | Text-to-image and image-to-image generation for DeepSeek Harness via OpenRouter's unified Image API, with capability-gated parameters |
| 2188 | [Parker-xia/dsh-research-refs](https://github.com/Parker-xia/dsh-research-refs) | 0 | 2026-08-26 | 2026-08-26 | DSH plugin: tidy messy pasted citations into uniformly formatted references (refs_parse / refs_verify / refs_dedup / refs_format + research-refs skill) |
| 2189 | [Pasumao/dsh-plugin-windows-guard](https://github.com/Pasumao/dsh-plugin-windows-guard) | 0 | 2026-08-25 | 2026-08-25 | DeepSeek Harness (dsh) Windows 环境防坑守则 skill 插件（纯数据）：编码/转义/路径/进程/乱码预防规则，无修复工具 |
| 2190 | [paulalesius/dsh-openai-api](https://github.com/paulalesius/dsh-openai-api) | 0 | 2026-08-24 | 2026-08-24 | OpenAI-compatible /v1/chat/completions (streaming and non-streaming) and /v1/models endpoint on the DSH web server. |
| 2191 | [pauloapoloni/dsh-pr-checks](https://github.com/pauloapoloni/dsh-pr-checks) | 0 | 2026-08-26 | 2026-08-27 | DSH plugin: status and progress of GitHub Actions checks for open PRs, in the sidebar footer. |
| 2192 | [peikuo/dayreel](https://github.com/peikuo/dayreel) | 0 | 2026-08-30 | 2026-08-30 | Dayreel — a DeepSeek Harness (dsh) community plugin: turn your day of work sessions into a designed daily report + a narrated summary video. |
| 2193 | [peiyucn/dsh-sparrow](https://github.com/peiyucn/dsh-sparrow) | 0 | 2026-08-30 | 2026-08-30 | A collection of small DeepSeek Harness (DSH) web plugins: chat input suggestions, an image-vision channel for text-only models, and archived-session management. |
| 2194 | [perinchiang/dsh-memory-dashboard](https://github.com/perinchiang/dsh-memory-dashboard) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness embedded read-only viewer for TencentDB Agent Memory's four-layer local memory |
| 2195 | [PerryLink/dsh-plugin-certification](https://github.com/PerryLink/dsh-plugin-certification) | 0 | 2026-08-29 | 2026-08-30 | Community certification spec and registry for DeepSeek Harness plugins: five machine-checkable dimensions, A-D grades, and a security veto. |
| 2196 | [PerryLink/dsh-plugin-kit](https://github.com/PerryLink/dsh-plugin-kit) | 0 | 2026-08-26 | 2026-08-27 | Shared zero-runtime-dependency toolkit for PerryLink DSH plugins: a pluggable Provider registry seam, fail-closed approval and adaptive session-event gates, mechanical verify scripts, shared sanitize/pricing/judge modules, and a new-plugin skeleton. |
| 2197 | [PerryLink/dsh-plugin-portal](https://github.com/PerryLink/dsh-plugin-portal) | 0 | 2026-08-26 | 2026-08-27 | Zero-dependency static portal rendering the @perrylink DeepSeek Harness plugin ecosystem as grouped cards: one page, no build step, no runtime framework. |
| 2198 | [PerryLink/perrylink](https://github.com/PerryLink/perrylink) | 0 | 2026-08-16 | 2026-08-30 | DeepSeek Harness ecosystem: 33 plugins - second-model approval, permission rules, memory, MCP panel, supply-chain security & certification |
| 2199 | [phillarmonic/dsh-llm-kimi](https://github.com/phillarmonic/dsh-llm-kimi) | 0 | 2026-08-25 | 2026-08-25 | A Kimi K3 connector plugin for the DeepSeek Harness LLM capability |
| 2200 | [piaohua/dsh-schedule-command](https://github.com/piaohua/dsh-schedule-command) | 0 | 2026-08-22 | 2026-08-22 | DeepSeek Harness 的 /schedule 定时任务命令 —— 一句话创建会话内单次/周期任务，⏰ 标识自动识别定时会话。/schedule command for DeepSeek Harness — create session-local one-shot/recurring tasks in plain language; ⏰ marks schedule sessions at a glance. |
| 2201 | [pick1e-morty/dsh-suggest-reply](https://github.com/pick1e-morty/dsh-suggest-reply) | 0 | 2026-08-22 | 2026-08-23 | 帮我想想 —— 一个基于 DSH-better-sidebar 的侧边栏 tab：用你自己写的 system prompt 对主对话最新一条 AI 回复生成候选回复，点击直填输入框。 |
| 2202 | [ping1999/dsh-minimap](https://github.com/ping1999/dsh-minimap) | 0 | 2026-08-29 | 2026-08-29 | VS Code-style minimap (text thumbnail + draggable viewport) overlay for the dsh web GUI's side file viewer |
| 2203 | [pipipigu/dsh-ssh-control](https://github.com/pipipigu/dsh-ssh-control) | 0 | 2026-08-28 | 2026-08-28 | Unified, non-intrusive SSH control center for DeepSeek Harness (DSH) |
| 2204 | [pipiwolve/dsh-baidu-ocr](https://github.com/pipiwolve/dsh-baidu-ocr) | 0 | 2026-08-25 | 2026-08-26 | Baidu cloud OCR bundle for DeepSeek Harness: drag images/PDFs in, OCR to Markdown with PaddleOCR-VL or Unlimited-OCR. 百度云 OCR 插件：拖入图片/PDF 识别为 Markdown 并写入本地文件。 |
| 2205 | [pixellover1433/dsh-plugin-dev-skills](https://github.com/pixellover1433/dsh-plugin-dev-skills) | 0 | 2026-08-30 | 2026-08-30 | This set of skills allows your agent to create plugins for Deepseek Harness. |
| 2206 | [PlusQi/dsh-plugins](https://github.com/PlusQi/dsh-plugins) | 0 | 2026-08-28 | 2026-08-27 | 个人 DeepSeek Harness (DSH) 插件集 |
| 2207 | [pn1024/dsh-ppt-master](https://github.com/pn1024/dsh-ppt-master) | 0 | 2026-08-31 | 2026-08-31 | PPT Master skill packaged as a DeepSeek Harness (dsh) plugin: AI-driven presentation workflow for editable PPTX decks, SVG snapshots, native template filling, and PPTX enhancement. |
| 2208 | [PolinniZhong/dsh-skill-trace](https://github.com/PolinniZhong/dsh-skill-trace) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness Skill 追踪：看清 Agent 实际加载的 Skill，把运行过程变成可复看、可学习的本地收据。 |
| 2209 | [popeye1113/dsh-question-jump-bar](https://github.com/popeye1113/dsh-question-jump-bar) | 0 | 2026-08-25 | 2026-08-25 | DSH Web 插件：会话右侧的问题索引标尺（Question Jump Bar），每个刻度一次提问，悬停预览、点击/键盘跳转。 |
| 2210 | [Practice019/dsh-doubao-plugin](https://github.com/Practice019/dsh-doubao-plugin) | 0 | 2026-08-22 | 2026-08-23 | DSH 插件：通过本地 Quicker 转发（doubao web2api） 提供 `doubao_ask` 动态搜索/图片生成/多模态识图工具， 并支持**粘贴图片 → 本地路径**（paste-to-path）。 |
| 2211 | [princeofdream/dsh-codebase-memory-mcp](https://github.com/princeofdream/dsh-codebase-memory-mcp) | 0 | 2026-08-25 | 2026-08-25 | dsh-codebase-memory-mcp |
| 2212 | [Proton1917/dsh-harness-plugin](https://github.com/Proton1917/dsh-harness-plugin) | 0 | 2026-08-17 | 2026-08-28 | Independent TypeScript plugins for DeepSeek Harness: live stats, Web UI customization, and a medical Fable mode |
| 2213 | [publieople/dsh-omniroute-models](https://github.com/publieople/dsh-omniroute-models) | 0 | 2026-08-28 | 2026-08-28 | DSH plugin: searchable/filterable model manager for OmniRoute (or any OpenAI-compatible gateway) — provider directory, modality discovery, multi-select enable. |
| 2214 | [QChengW/dsh-conversation-shortcuts](https://github.com/QChengW/dsh-conversation-shortcuts) | 0 | 2026-08-27 | 2026-08-27 | DSH web plugin for conversation keyboard shortcuts |
| 2215 | [qewregrfhnm/dsh-session-manager](https://github.com/qewregrfhnm/dsh-session-manager) | 0 | 2026-08-22 | 2026-08-22 | Full session management plugin for DeepSeek Harness (DSH) web UI: delete/trash/restore, workspace grouping, move sessions between workspaces, unread markers, context compaction threshold. Fully local, bilingual zh/en. |
| 2216 | [qgx1992/dsh-model-select-style](https://github.com/qgx1992/dsh-model-select-style) | 0 | 2026-08-27 | 2026-08-27 | DSH web 插件：把输入框模型选择控件替换为两个独立按钮（供应商 + 模型两级联动，支持推理等级调节） |
| 2217 | [qgx1992/dsh-notify](https://github.com/qgx1992/dsh-notify) | 0 | 2026-08-28 | 2026-08-28 | DSH 通知显示层插件：全局 toast 栈，订阅桌面壳 __dshExo 桥事件，点击经官方 sessions runtime 程序化激活会话；无壳时降级订阅 sessions store 自绘。可插拔通知显示层的 web 侧。 |
| 2218 | [qianxiao1213/zcode-usage-stats](https://github.com/qianxiao1213/zcode-usage-stats) | 0 | 2026-08-22 | 2026-08-22 | 仿zcode的使用统计 - DSH Token 用量统计插件(趋势图/仪表盘/活跃热力图) v0.1.0 |
| 2219 | [qiaoji1990-alt/aifred-dsh-task-ledger](https://github.com/qiaoji1990-alt/aifred-dsh-task-ledger) | 0 | 2026-08-25 | 2026-08-25 | Provider-neutral task lifecycle and idempotent event ledger plugin for DeepSeek Harness. Works standalone for any DSH project and optionally integrates with Aifred through a bridge. |
| 2220 | [qingmumingyang/dsh-doc-toolkit](https://github.com/qingmumingyang/dsh-doc-toolkit) | 0 | 2026-08-23 | 2026-08-24 | DSH 文档读写工具包 - PDF/DOCX/XLSX/CSV 读写与 PDF 导出（利用dsh制作的，希望能帮到你们） |
| 2221 | [qingshanyuluo/dsh-mobile-ux](https://github.com/qingshanyuluo/dsh-mobile-ux) | 0 | 2026-08-25 | 2026-08-26 | DeepSeek Harness mobile: CSS-only UI plugin, password-protected Cloudflare tunnel and a tiny Android WebView app - use DSH on your phone. |
| 2222 | [qinshige/dsh-performance-guard](https://github.com/qinshige/dsh-performance-guard) | 0 | 2026-08-25 | 2026-08-31 | Host and Web performance diagnostics, repeated plugin-isolation campaigns, and safe recovery for DeepSeek Harness. |
| 2223 | [qipenglin/dsh-plugin-manager](https://github.com/qipenglin/dsh-plugin-manager) | 0 | 2026-08-28 | 2026-08-29 | Profile plugin manager for DeepSeek Harness |
| 2224 | [qipenglin/dsh-theme-spectrum](https://github.com/qipenglin/dsh-theme-spectrum) | 0 | 2026-08-28 | 2026-08-29 | Light and dark theme presets for DeepSeek Harness Web |
| 2225 | [qipenglin/dsh-web-access](https://github.com/qipenglin/dsh-web-access) | 0 | 2026-08-27 | 2026-08-27 | Optional Web access authentication plugin for DeepSeek Harness |
| 2226 | [qiqiangvae/dsh-my-favorites](https://github.com/qiqiangvae/dsh-my-favorites) | 0 | 2026-08-24 | 2026-08-24 | dsh 收藏夹插件，可以收藏网址和会话，支持快捷键切换会话 |
| 2227 | [Qiwei-QW/dsh-r-ide](https://github.com/Qiwei-QW/dsh-r-ide) | 0 | 2026-08-22 | 2026-08-24 | A four-pane R IDE (Editor / Console / Environment / Plots) integrated into DeepSeek Harness as a tab of [dsh-better-sidebar](https://github.com/omdsh-dev/DSH-better-sidebar), with one dedicated R process per conversation. |
| 2228 | [qt-11564/dsh-git-seam](https://github.com/qt-11564/dsh-git-seam) | 0 | 2026-08-29 | 2026-08-29 | Structured git tools for DeepSeek Harness: diff-before-commit gate + deterministic porcelain parsing (Chinese/UTF-8 paths, Windows) |
| 2229 | [quan-v/dsh-safe-gate](https://github.com/quan-v/dsh-safe-gate) | 0 | 2026-08-25 | 2026-08-25 | dsh 装前守门:OSV 供应链扫描 + 插件契约检查。 Pre-flight safety gate for dsh plugins/MCP. |
| 2230 | [QuanQQQ/dsh-plugin-dev-manager](https://github.com/QuanQQQ/dsh-plugin-dev-manager) | 0 | 2026-08-24 | 2026-08-26 | Stable control plane for isolated DeepSeek Harness plugin development |
| 2231 | [Quophic/dsh-plugin-installer](https://github.com/Quophic/dsh-plugin-installer) | 0 | 2026-08-18 | 2026-08-23 | DeepSeek Harness（dsh）插件安全安装/卸载器：自动备份配置、失败自动回滚（卸载失败自动重新安装插件）、重启并做健康检查。\| Safe dsh plugin installer & uninstaller: config backup, rollback (reinstall on uninstall failure), restart & health check. |
| 2232 | [QWE13-ART/dsh-skill-folder](https://github.com/QWE13-ART/dsh-skill-folder) | 0 | 2026-08-30 | 2026-08-30 | Fold the DSH skill catalog prompt surface: static KV-cache-stable catalog + BM25/bge-m3 hybrid skill_search + autoRoute hints. v0.3.0. npm: dsh-skill-folder |
| 2233 | [QWE13-ART/dsh-tool-folder](https://github.com/QWE13-ART/dsh-tool-folder) | 0 | 2026-08-30 | 2026-08-30 | Fold the DSH tool surface per request + ChainGuard firewall (high-risk block + exfil-chain detection + anti-obfuscation) + BM25/bge-m3 hybrid tools_search. Shrinks schema tokens 80-90% while keeping selection accuracy. v0.2.0 adds a semantic retrieval leg (local Ollama bge-m3, RRF hybrid) and ChainGuard obfuscation detection. npm: dsh-tool-folder |
| 2234 | [RaberShef/dsh-pin-session](https://github.com/RaberShef/dsh-pin-session) | 0 | 2026-08-26 | 2026-08-27 | Pin DSH sessions to the top of the sidebar and mark them unread for later. |
| 2235 | [RagnarPitla/dsh-field-guide](https://github.com/RagnarPitla/dsh-field-guide) | 0 | 2026-08-24 | 2026-08-24 | An evidence-badged field guide to DeepSeek Harness (dsh), plus a working plugin. Every claim marked with how it was verified. Independent and unofficial. |
| 2236 | [raktim-mondol/dsh-researchcraft](https://github.com/raktim-mondol/dsh-researchcraft) | 0 | 2026-08-28 | 2026-08-28 | ResearchCraft as a DeepSeek Harness (DSH) profile plugin: research persona, scientific skills catalogue, living lab notebook, and specialist subagents. |
| 2237 | [raktim-mondol/dsh-tui-en](https://github.com/raktim-mondol/dsh-tui-en) | 0 | 2026-08-22 | 2026-08-22 | English-only fork of dsh-TUI — Claude Code-style terminal UI for DeepSeek Harness |
| 2238 | [rand0wn/dsh-malware-audit](https://github.com/rand0wn/dsh-malware-audit) | 0 | 2026-08-21 | 2026-08-22 | DeepSeek Harness (dsh) plugin: real AST-based scan of installed plugins for malicious-intent patterns, with an optional periodic schedule and auto-quarantine on critical findings. Advisory-by-default, not an antivirus signature database. |
| 2239 | [randomix777/dsh-plugin-subs](https://github.com/randomix777/dsh-plugin-subs) | 0 | 2026-08-28 | 2026-08-31 | DSH plugin: OAuth sign-in for Claude, Codex, Grok, Antigravity, OpenRouter, Agnes AI — expose subscription LLMs as DeepSeek Harness providers |
| 2240 | [randomix777/dsh-sprite-gen](https://github.com/randomix777/dsh-sprite-gen) | 0 | 2026-08-28 | 2026-08-31 | Sprite Sheet Generator with AI Image Generation for DeepSeek Harness |
| 2241 | [Ranz-Feng/dsh-web-import](https://github.com/Ranz-Feng/dsh-web-import) | 0 | 2026-08-26 | 2026-08-26 | Import DeepSeek Web (chat.deepseek.com) chat history into DeepSeek Harness as resumable, workspace-grouped sessions with original titles preserved. |
| 2242 | [RaulLazaro/dsh-pwa-plugin](https://github.com/RaulLazaro/dsh-pwa-plugin) | 0 | 2026-08-31 | 2026-08-31 | PWA plugin for DeepSeek Harness — adds offline support and install-as-app capability with service worker, manifest, and official DeepSeek icons. |
| 2243 | [raydez/dsh-pet-plugin](https://github.com/raydez/dsh-pet-plugin) | 0 | 2026-08-18 | 2026-08-22 | deepseek harness pet plugin（桌面宠物插件） |
| 2244 | [rayfalling/dsh-tool-visibility](https://github.com/rayfalling/dsh-tool-visibility) | 0 | 2026-08-25 | 2026-08-26 | DSH plugin: control which tool schemas are injected into the DeepSeek Harness model context — settings UI + tools.restrict filter + persisted state |
| 2245 | [Raywh/dsh-song-download](https://github.com/Raywh/dsh-song-download) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness 歌曲下载插件：搜索（B站/YouTube）+ 下载（MP3 320k 酷狗兼容）+ LRC 歌词（站点字幕 + 网易云兜底）。DSH plugin: song search & download with lyrics. |
| 2246 | [rchen1207/dsh-password-generator](https://github.com/rchen1207/dsh-password-generator) | 0 | 2026-08-24 | 2026-08-25 | 生成密码，只生不存 |
| 2247 | [renat3u/dsh-upgrade-skill](https://github.com/renat3u/dsh-upgrade-skill) | 0 | 2026-08-30 | 2026-08-30 | dsh 插件升级适配skill |
| 2248 | [renchengxiang/dsh-web-search-tavily](https://github.com/renchengxiang/dsh-web-search-tavily) | 0 | 2026-08-28 | 2026-08-28 | Tavily-backed web search provider for DeepSeek Harness, with Settings → Plugins configuration UI |
| 2249 | [Reseezhang/ue-log-reader](https://github.com/Reseezhang/ue-log-reader) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness 插件：UE 日志速读卡 — 模型调用 uelog 工具扫描 Saved/Logs，流式解析+聚合去重后渲染速读卡片，一键复制缺陷单摘要 |
| 2250 | [Reseezhang/vizcb-codeblock-visualizer](https://github.com/Reseezhang/vizcb-codeblock-visualizer) | 0 | 2026-08-28 | 2026-08-29 | DeepSeek Harness 可视化插件：svg/html/mermaid 代码块渲染为图表卡片（宿主端 mermaid、深色主题配色、节点文字自适应、灯箱、保存导出） |
| 2251 | [RichDavidMu/create-dsh-plugin](https://github.com/RichDavidMu/create-dsh-plugin) | 0 | 2026-08-20 | 2026-08-24 | Scaffold a DeepSeek Harness plugin project — a working plugin with one model-facing tool, a profile bundle that mounts it, dsh's own toolchain, and documentation an agent can follow without reading dsh's source. |
| 2252 | [rjn32s/dsh-whois-plugin](https://github.com/rjn32s/dsh-whois-plugin) | 0 | 2026-08-22 | 2026-08-23 | RDAP-backed whois tool plugin for DeepSeek Harness (dsh) — look up domain registration data as a model tool |
| 2253 | [rm-Vstar/web-search-tinyfish](https://github.com/rm-Vstar/web-search-tinyfish) | 0 | 2026-08-28 | 2026-08-28 | A TinyFish web searching plugin for Deepseek Harness |
| 2254 | [robauto-ai/dsh-growth](https://github.com/robauto-ai/dsh-growth) | 0 | 2026-08-21 | 2026-08-22 | Digital growth and commerce harness. Grow your brand and transact agent to agent. Monetize your repo or skill via Robauto or let the agent grow your site traffic.  Deepseek harness plugin, works with MetaAI, Copilot, Grok, Claude, Google, Bing, Hubspot and Perplexity agents.  |
| 2255 | [robbin810130/dsh-rtk](https://github.com/robbin810130/dsh-rtk) | 0 | 2026-08-24 | 2026-08-24 | Community DSH plugin that applies explicit RTK command-output filtering to bash tools at boot. |
| 2256 | [robbin810130/dsh-vault-plugin](https://github.com/robbin810130/dsh-vault-plugin) | 0 | 2026-08-24 | 2026-08-27 | DSH 保险箱插件：项目与对话的前台隐私锁 |
| 2257 | [robbywang25/dsh-llm-mlx](https://github.com/robbywang25/dsh-llm-mlx) | 0 | 2026-08-25 | 2026-08-26 | DeepSeek Harness plugin for local MLX-LM models with loopback-only defaults and optional managed server startup |
| 2258 | [Rock-ql/dsh-git-branch](https://github.com/Rock-ql/dsh-git-branch) | 0 | 2026-08-25 | 2026-08-25 | DSH Desktop plugin: git branch pill in the composer, with local/remote listing and confirmed checkout \| DSH 对话栏 Git 分支胶囊 |
| 2259 | [rocklau/dsh-ui-tool-graph](https://github.com/rocklau/dsh-ui-tool-graph) | 0 | 2026-08-22 | 2026-08-22 | Tool-call value graph tab for the DeepSeek Harness (dsh) Web UI: cost/duration/error weights over conversation trajectories with one-click next-turn optimization prompts. |
| 2260 | [rogerdigital/dsh-vet](https://github.com/rogerdigital/dsh-vet) | 0 | 2026-08-29 | 2026-08-29 | Security vetting for DeepSeek Harness (DSH) plugins: permission & supply-chain audits before install, graded via the open dsh-vet/v1 report standard. |
| 2261 | [rootkiller6788/dsh-launcher](https://github.com/rootkiller6788/dsh-launcher) | 0 | 2026-08-31 | 2026-08-31 | DSHL — A desktop launcher for managing AI runtimes, instances, plugins, MCP servers, skills, profiles, and distributions. |
| 2262 | [royenheart/dsh-migrate-bot](https://github.com/royenheart/dsh-migrate-bot) | 0 | 2026-08-25 | 2026-08-26 | Automatically migrate dsh plugins to the new version. |
| 2263 | [rrrrrredy/context-continuity](https://github.com/rrrrrredy/context-continuity) | 0 | 2026-08-28 | 2026-08-31 | Local-first continuity plugin for Codex and DeepSeek Harness across compaction, resume, and handoff. |
| 2264 | [rrrrrredy/dsh-execution-fidelity-guard](https://github.com/rrrrrredy/dsh-execution-fidelity-guard) | 0 | 2026-08-31 | 2026-08-31 | Unofficial alpha execution-fidelity guard bundle for DeepSeek Harness. |
| 2265 | [rrrrrredy/intent-loop](https://github.com/rrrrrredy/intent-loop) | 0 | 2026-08-31 | 2026-08-31 | Local-first, traceable current-intent state for Codex and DeepSeek Harness. |
| 2266 | [Rudyy898/dsh-drag-path](https://github.com/Rudyy898/dsh-drag-path) | 0 | 2026-08-27 | 2026-08-27 | dsh-plugin |
| 2267 | [rudyz666/dsh-bili-asr](https://github.com/rudyz666/dsh-bili-asr) | 0 | 2026-08-23 | 2026-08-23 | 解析 B站视频链接，提取完整脚本/字幕：优先字幕轨，无字幕用本地 whisper 转写，导出 SRT/TXT/JSON。DeepSeek Harness 插件，跨平台 Windows/macOS/Linux（纯 Node）。 |
| 2268 | [Ruixinhua/dsh-universe-api](https://github.com/Ruixinhua/dsh-universe-api) | 0 | 2026-08-27 | 2026-08-27 | Offline, deterministic public API discovery for DeepSeek Harness and DSH Desktop. |
| 2269 | [ruiyukirin/dsh-douyin-oem-touliu-report](https://github.com/ruiyukirin/dsh-douyin-oem-touliu-report) | 0 | 2026-08-28 | 2026-08-28 | 抖音本地推 OEM 投流日报/周报自动化插件 - Douyin OEM ad daily/weekly report automation plugin for DeepSeek Harness (Author: Kirin) |
| 2270 | [runcat-tommy/dsh-plugin-runcat-inventory](https://github.com/runcat-tommy/dsh-plugin-runcat-inventory) | 0 | 2026-08-26 | 2026-08-28 | 逃咪-插件总览（Runcat Plugin Overview）—— 更好用的 DSH 插件列表：表格视图、状态过滤、启用/停用开关（热生效）、配置查看与复制、中英双语界面。 |
| 2271 | [runcat-tommy/dsh-theme-manager](https://github.com/runcat-tommy/dsh-theme-manager) | 0 | 2026-08-28 | 2026-08-28 | Two-level theme manager for DeepSeek Harness Web: pick a culture/scene or a national flag first, then a concrete style. 40 built-in styles (ink wash, ukiyo-e, Suzhou garden, cyberpunk, 20 flags & more). |
| 2272 | [runcat-tommy/dsh-view-manager](https://github.com/runcat-tommy/dsh-view-manager) | 0 | 2026-08-27 | 2026-08-28 | Manage DeepSeek Harness Web GUI view tabs (Chat/Trajectory): enable, hide, reorder & rename with zh/en locale. |
| 2273 | [runfali/dsh-paperclip](https://github.com/runfali/dsh-paperclip) | 0 | 2026-08-24 | 2026-08-24 | dsh 零侵入式 bundle 插件：📎 输入框上传按钮 + 待发送文件浮层（仅文件名，可移除）· read_document 多格式读取工具（txt / pdf / docx / xlsx / json / md / ini / conf，支持 offset/limit 分页）· 设置 → 通用设置一个开关。标准 Cordis bundle 插件，不改 DSH 源码，内容寻址落盘去重，深浅色主题自适应。 |
| 2274 | [runfali/dsh-skill-curator](https://github.com/runfali/dsh-skill-curator) | 0 | 2026-08-25 | 2026-08-25 | 为 dsh 打造的自动技能策展插件：每 N 轮真实对话，后台起一个评审子代理阅读会话摘要，主动把值得沉淀的经验提炼为 ~/.dsh/skills/<name>/SKILL.md - 把 Hermes 的「后台评审自我改进」闭环移植到 DSH，零侵入 bundle 插件，不改 dsh 源码。 |
| 2275 | [RyanShen3/dsh-toutiao-reader](https://github.com/RyanShen3/dsh-toutiao-reader) | 0 | 2026-08-29 | 2026-08-29 | 读网页/头条文章全文的 DSH 插件：webfetch 工具 + toutiao-reader 经验技能 |
| 2276 | [Rycbartbad/dsh-key-manager](https://github.com/Rycbartbad/dsh-key-manager) | 0 | 2026-08-29 | 2026-08-29 | Multiple API keys per provider for DeepSeek Harness: pools with notes, one-click switching that really takes effect |
| 2277 | [RyensX/dsh-remote-gateway](https://github.com/RyensX/dsh-remote-gateway) | 0 | 2026-08-23 | 2026-08-24 | 提供安全的反向代理，使DeepSeek Harness可以远程访问，随时随地和AI对话。/ Provides a secure reverse proxy, enabling DeepSeek Harness to be accessed remotely and to converse with AI anytime, anywhere. |
| 2278 | [Ryu6Zero/dsh-hindsight](https://github.com/Ryu6Zero/dsh-hindsight) | 0 | 2026-08-25 | 2026-08-26 | 🧠 Cross-session memory for DeepSeek Harness backed by Hindsight. Self-contained dsh-plugin: /hindsight commands + hindsight_recall/remember/status/list/forget agent tools. Lightweight, no dsh-mnemon, no orchestrator. |
| 2279 | [S-AN-Shu/dsh-skill-manager](https://github.com/S-AN-Shu/dsh-skill-manager) | 0 | 2026-08-25 | 2026-08-26 | Security-bounded Agent Skill management and GitHub marketplace plugin for DeepSeek Harness and DSH Desktop |
| 2280 | [s1lencewill/dsh-markdown-reader](https://github.com/s1lencewill/dsh-markdown-reader) | 0 | 2026-08-23 | 2026-08-23 | DSH Web GUI full-screen Markdown reader with GFM, outline, KaTeX, Mermaid, and relative resource navigation. |
| 2281 | [SaitoAsuka1121/dsh-client-ui-elasticsearch](https://github.com/SaitoAsuka1121/dsh-client-ui-elasticsearch) | 0 | 2026-08-24 | 2026-08-24 | dsh elasticsearch plugin |
| 2282 | [sam-midlight/dsh-loop-rescue](https://github.com/sam-midlight/dsh-loop-rescue) | 0 | 2026-08-22 | 2026-08-22 | DRAFT — DeepSeek Harness guard that breaks an agent out of a tool-call loop and escalates to a stronger model for one concrete next action. Window-based detection with a progress epoch, so it catches cycles the stock single-slot repeat guard resets away. |
| 2283 | [sandersyao/dsh-plugin-ui-session-fork](https://github.com/sandersyao/dsh-plugin-ui-session-fork) | 0 | 2026-08-25 | 2026-08-25 | deepseek harness 插件 增加会话分组方式“树形” |
| 2284 | [sANDzER0/dsh-hippocampus](https://github.com/sANDzER0/dsh-hippocampus) | 0 | 2026-08-26 | 2026-08-26 | Cross-session project memory for DeepSeek Harness — capture / consolidate / recall, keyword + optional local-Ollama semantic search. Inspired by magic-context. |
| 2285 | [saqie803/ponytail](https://github.com/saqie803/ponytail) | 0 | 2026-08-29 | 2026-08-29 | Ship production-ready code with one line of AI-generated output, built for 20 agents and zero ceremony. |
| 2286 | [sazzadurrahmaan/dsh-telegram](https://github.com/sazzadurrahmaan/dsh-telegram) | 0 | 2026-08-22 | 2026-08-22 | Telegram channel for DeepSeek Harness — chat with your agent from Telegram, with a deny-by-default allowlist and in-chat approval for destructive tools. |
| 2287 | [sdoygb/geometry-knowledge](https://github.com/sdoygb/geometry-knowledge) | 0 | 2026-08-26 | 2026-08-26 | 几何论（共扼谱几何 CSG）知识库插件 for DeepSeek Harness: 纯离线 BM25 检索，零运行时依赖 |
| 2288 | [secyborg/dsh-command-rail](https://github.com/secyborg/dsh-command-rail) | 0 | 2026-08-25 | 2026-08-25 | DSH web plugin: a Codex-style command-history rail covering the WHOLE session |
| 2289 | [secyborg/dsh-compact-chat-ui](https://github.com/secyborg/dsh-compact-chat-ui) | 0 | 2026-08-25 | 2026-08-25 | DSH web plugin: a settings card to tune chat reading density — font size, line height, and block spacing of the conversation area (assistant markdown + user bubbles), applied live |
| 2290 | [secyborg/dsh-find-bar](https://github.com/secyborg/dsh-find-bar) | 0 | 2026-08-25 | 2026-08-25 | DSH web plugin: a Cmd/Ctrl+F find bar (like the browser's built-in find) for the desktop Electron shell, which has none |
| 2291 | [secyborg/dsh-glm-web-search](https://github.com/secyborg/dsh-glm-web-search) | 0 | 2026-08-26 | 2026-08-26 | DSH host plugin: GLM (Zhipu) web-search provider for the ctx.web seam — structured results, no model turn, reuses your ZAI coding key |
| 2292 | [seewhydee/dsh-emacs-bridge](https://github.com/seewhydee/dsh-emacs-bridge) | 0 | 2026-08-23 | 2026-08-27 | Deepseek Harness to Emacs bridge |
| 2293 | [seiriosPlus/miaoda_for_deepseek_harness](https://github.com/seiriosPlus/miaoda_for_deepseek_harness) | 0 | 2026-08-26 | 2026-08-29 | miaoda_for_deepseek harness |
| 2294 | [seoeaa/dsh-locale-ru](https://github.com/seoeaa/dsh-locale-ru) | 0 | 2026-08-31 | 2026-08-31 | Русский интерфейс (локаль ru) для DeepSeek Harness — custom locale plugin. 26 namespaces, ~690 строк. / Russian locale plugin for DeepSeek Harness. |
| 2295 | [SeverusZh/dsh-ollama-usage](https://github.com/SeverusZh/dsh-ollama-usage) | 0 | 2026-08-27 | 2026-08-27 | Ollama Cloud 用量余量可视化 DeepSeek Harness 插件:5h 会话/周用量双横条 + 设置页面板,Key 与快照持久化,自动刷新,登录引导。Ollama Cloud usage & quota visualization plugin for DeepSeek Harness. |
| 2296 | [ShadowQuill/DialogueContextBridge](https://github.com/ShadowQuill/DialogueContextBridge) | 0 | 2026-08-26 | 2026-08-26 | 对话上下文桥接 — 为大语言模型(LLM)/AI 智能体的对话做跨会话上下文桥接的 DSH 插件：把一次对话的共识打包成可移植快照，一键引入新对话（三层快照 / SQLite+FTS5 / AES-256-GCM） |
| 2297 | [shaneconner/canon](https://github.com/shaneconner/canon) | 0 | 2026-08-10 | 2026-08-30 | Canonical project memory for the Pi coding agent: one governing article per asset, an append-only journal, capsule surfacing. A project wiki with a spine. |
| 2298 | [shaneconner/dsh-claude-bridge](https://github.com/shaneconner/dsh-claude-bridge) | 0 | 2026-08-30 | 2026-08-31 | Use a Claude Pro or Max subscription as a DeepSeek Harness model provider, via the Claude Code CLI. |
| 2299 | [shaneconner/dsh-provider-login](https://github.com/shaneconner/dsh-provider-login) | 0 | 2026-08-30 | 2026-08-31 | Sign in to DeepSeek Harness model providers with a Claude Pro/Max or ChatGPT Plus/Pro subscription. |
| 2300 | [ShanHaiFish/dsh-theme-brick](https://github.com/ShanHaiFish/dsh-theme-brick) | 0 | 2026-08-30 | 2026-08-30 | DSH 主题插件（Brick/砌砖）：纯 token 覆盖层，暖石膏与火烧黏土、灰缝线条、一砖一色，零全局 CSS；Settings → General 开关可随时关闭还原。A restrained token-only theme for DeepSeek Harness web — plaster & fired-clay, one accent, no global CSS, with an on/off switch. |
| 2301 | [shao-01-test/dsh-chat-rail](https://github.com/shao-01-test/dsh-chat-rail) | 0 | 2026-08-26 | 2026-08-26 | dsh-chat-rail — DeepSeek Harness 聊天右侧导航拉条插件：按「提问→回答」轮次显示彩色节点（绿/黄/红/蓝表状态），点击即跳转对应提问与回答段落，悬停展开状态面板，刚回答完有闪光动画，关键词自动提炼成短句。一个拉条，快速定位整场对话。 |
| 2302 | [shaomingbo/dsh-anyrouter](https://github.com/shaomingbo/dsh-anyrouter) | 0 | 2026-08-31 | 2026-08-31 | Dedicated provider bundle for the relay: Claude via Claude Code transport, GPT/Codex via Responses, for DeepSeek Harness |
| 2303 | [shaomingbo/dsh-open-in-editor](https://github.com/shaomingbo/dsh-open-in-editor) | 0 | 2026-08-26 | 2026-08-26 | Open DSH Web produced files in a configurable local macOS IDE |
| 2304 | [shaomingbo/dsh-session-reference-copy](https://github.com/shaomingbo/dsh-session-reference-copy) | 0 | 2026-08-23 | 2026-08-24 | Copy canonical cross-session references from the DeepSeek Harness Web session header. |
| 2305 | [shaomingbo/dsh-subscription-antigravity](https://github.com/shaomingbo/dsh-subscription-antigravity) | 0 | 2026-08-29 | 2026-08-29 | Google Antigravity subscription reuse for DeepSeek Harness: browser PKCE sign-in, loopback OpenAI-compatible proxy to Cloud Code Assist, Gemini/Claude/GPT-OSS model routes. |
| 2306 | [shaomingbo/dsh-token-usage](https://github.com/shaomingbo/dsh-token-usage) | 0 | 2026-08-30 | 2026-08-30 | Accounts, subscription allowance observations, and local usage ledger for DeepSeek Harness |
| 2307 | [shayexiangpaimeng/dsh-memory](https://github.com/shayexiangpaimeng/dsh-memory) | 0 | 2026-08-31 | 2026-08-31 | Append-only layered memory plugin for DeepSeek Harness: five-layer partitioning, write gate, keyword recall, claim-anchors verification |
| 2308 | [shengyvself/narrative-prompt-polish](https://github.com/shengyvself/narrative-prompt-polish) | 0 | 2026-08-28 | 2026-08-30 | DSH 插件：主输入框 ✨ 一键把草稿润色成清晰、可执行的提示词，经 better-sidebar 侧栏对话多轮打磨后回填。A DSH plugin: ✨ one-click draft polish into agent-ready prompts, multi-turn side-chat via better-sidebar (>=0.16.1). |
| 2309 | [shenhuanageshei/dsh-git-status](https://github.com/shenhuanageshei/dsh-git-status) | 0 | 2026-08-31 | 2026-08-31 | DSH 插件：会话视图实时 git 状态展示 + 分支切换（会话头徽标 + 输入区环境行）。官方 bundle 插件，dsh plugin --profile web add：github:shenhuanageshei/dsh-git-status#v0.1.0 |
| 2310 | [shenhuanageshei/dsh-session-link-pro](https://github.com/shenhuanageshei/dsh-session-link-pro) | 0 | 2026-08-31 | 2026-08-31 | Session deep links + full session export (markdown/JSON) + approved cross-session messaging with pairing for DeepSeek Harness (dsh). |
| 2311 | [shenhuanageshei/dsh-thincoder-suite](https://github.com/shenhuanageshei/dsh-thincoder-suite) | 0 | 2026-08-31 | 2026-08-31 | DSH plugin porting thincoder self-discipline suite: advisor convergent review / engineering mode / escalate / consult |
| 2312 | [ShenXuAkaEkstasis/dsh-ai-shopping-assistant](https://github.com/ShenXuAkaEkstasis/dsh-ai-shopping-assistant) | 0 | 2026-08-28 | 2026-08-28 | AI Shopping Assistant plugin for DeepSeek Harness (DSH), with product comparison, price analysis, merchant/review evidence and source-quality checks. |
| 2313 | [shimingming520/dsh-audiogen](https://github.com/shimingming520/dsh-audiogen) | 0 | 2026-08-28 | 2026-08-29 | AI audio generation plugin for the DeepSeek Harness web GUI: multi-vendor TTS, music, sound effects and voice design with a sidebar panel, model comparison, resource library and Agent tools. |
| 2314 | [shine-233/dsh-waimao](https://github.com/shine-233/dsh-waimao) | 0 | 2026-08-25 | 2026-08-25 | 外贸获客插件 for DeepSeek Harness (dsh): Google 三层搜客 + WhatsApp 客服审核台 + 邮件触达闭环 (ICP 评分/跟进序列/CRM/报价PDF), 零依赖 |
| 2315 | [ShineFree7/dsh-daily-log](https://github.com/ShineFree7/dsh-daily-log) | 0 | 2026-08-23 | 2026-08-23 | Daily work log plugin for DeepSeek Harness: /daily scaffold + daily_log_write/read/list tools, YYYY-MM-DD.md + theme-aware HTML dashboard |
| 2316 | [shizhanyu13/dsh-ironbound-policy](https://github.com/shizhanyu13/dsh-ironbound-policy) | 0 | 2026-08-26 | 2026-08-26 | @shizhanyu13/dsh-ironbound-policy — DSH plugin: Ironbound hard-gate guard. Blocks dangerous shell commands before they reach a tool, with a double-layer degrade counter over tools/execute. dsh-plugin. |
| 2317 | [shizhanyu13/dsh-waom](https://github.com/shizhanyu13/dsh-waom) | 0 | 2026-08-26 | 2026-08-26 | @shizhanyu13/dsh-waom — DSH plugin: autonomous-ops (WAOM). Monitor / decide / drive a subagent fix / evaluate independently (GAN). dsh-plugin. |
| 2318 | [Short-Arm-Ape/dsh-intranet-browser](https://github.com/Short-Arm-Ape/dsh-intranet-browser) | 0 | 2026-08-31 | 2026-08-31 | Bypasses the SSRF protection of @yeesy369dsh-browser-playwright |
| 2319 | [shuaihaoV/dsh-mcp-skill-control](https://github.com/shuaihaoV/dsh-mcp-skill-control) | 0 | 2026-08-25 | 2026-08-25 | DSH（DeepSeek Harness）Web GUI 的 MCP 服务器管理面板：状态查看、启停/重启、新增/删除、JSON 导入，以及本地技能启停控制。 |
| 2320 | [SHUJILAI/dsh-model-auto-hot-switch](https://github.com/SHUJILAI/dsh-model-auto-hot-switch) | 0 | 2026-08-28 | 2026-08-28 | Automatic per-task model hot-switching for DeepSeek Harness (dsh): image-aware tasks route to the vision model automatically, every other task keeps your default model. Zero extra tokens, no context disturbance. |
| 2321 | [shxtmaker/dsh-usage-monitor](https://github.com/shxtmaker/dsh-usage-monitor) | 0 | 2026-08-26 | 2026-08-28 | DSH 用量监控插件：供应商周期限额显示（DeepSeek/OpenCode/Command Code）+ 自动探测 DSH 已添加供应商并自动填入 API Key |
| 2322 | [sidleo/dsh-desktop](https://github.com/sidleo/dsh-desktop) | 0 | 2026-08-22 | 2026-08-22 | DeepSeek Harness 桌面壳：打开应用=启动 dsh web 服务并加载界面，关闭应用=自动停止服务。Electron desktop shell for DeepSeek Harness (DSH) |
| 2323 | [sidleo/skill-filesystem-plus](https://github.com/sidleo/skill-filesystem-plus) | 0 | 2026-08-17 | 2026-08-23 | Configurable skill discovery provider for DeepSeek Harness (DSH): cwd/project/ancestors/global layers with editable parent dirs, plugin card UI, disk persistence |
| 2324 | [sijie-ni-0214/dsh-subagent-error-details](https://github.com/sijie-ni-0214/dsh-subagent-error-details) | 0 | 2026-08-26 | 2026-08-26 | DSH plugin: deliver the real failure reason (e.g. RATE_LIMIT 429) to the parent agent when a background subagent fails |
| 2325 | [SiriusWJ/dsh-mihome](https://github.com/SiriusWJ/dsh-mihome) | 0 | 2026-08-30 | 2026-08-30 | Mi Home (米家) control for DeepSeek Harness agents — list homes/devices, read props, control devices behind a human approval gate. |
| 2326 | [siweimofang/dsh-plugin-zhishe-baojia-shenhe](https://github.com/siweimofang/dsh-plugin-zhishe-baojia-shenhe) | 0 | 2026-08-21 | 2026-08-22 | 知设装修报价审核DSH插件 - 支持视觉OCR截图输入 |
| 2327 | [siweimofang/dsh-plugin-zhishe-bikeng-qa](https://github.com/siweimofang/dsh-plugin-zhishe-bikeng-qa) | 0 | 2026-08-21 | 2026-08-22 | 知设装修避坑问答DSH插件 |
| 2328 | [siweimofang/dsh-plugin-zhishe-common](https://github.com/siweimofang/dsh-plugin-zhishe-common) | 0 | 2026-08-22 | 2026-08-22 | 知设 DSH 插件共享基础设施 - 知识库加载/检索/基准价格/风险评估 |
| 2329 | [siweimofang/dsh-plugin-zhishe-zaojia-gusuan](https://github.com/siweimofang/dsh-plugin-zhishe-zaojia-gusuan) | 0 | 2026-08-22 | 2026-08-22 | 知设装修造价估算DSH插件 |
| 2330 | [siweimofang/zhishe-a2a](https://github.com/siweimofang/zhishe-a2a) | 0 | 2026-08-22 | 2026-08-22 | 知设AI装修顾问 - 主仓库(知识库+DSH插件+GEO) |
| 2331 | [SJCLZ/MixlabLz-dsh-skills](https://github.com/SJCLZ/MixlabLz-dsh-skills) | 0 | 2026-08-27 | 2026-08-27 | MixlabLz's collection of DSH (DeepSeek Harness) skills and plugins |
| 2332 | [slohmaier/dsh-a11y-announcer](https://github.com/slohmaier/dsh-a11y-announcer) | 0 | 2026-08-21 | 2026-08-25 | Accessibility plugin for DeepSeek Harness web UI: announces tool calls and finished assistant messages via aria-live for screen readers |
| 2333 | [SMOKTEA/dsh-chartlab](https://github.com/SMOKTEA/dsh-chartlab) | 0 | 2026-08-26 | 2026-08-28 | Let the agent turn your data into an interactive chart.  \|  一句话：让 Agent 帮你把数据变成一张可交互的图表。 |
| 2334 | [snail-vs/dsh-llm-oauth](https://github.com/snail-vs/dsh-llm-oauth) | 0 | 2026-08-22 | 2026-08-22 | OAuth login plugin for DeepSeek Harness (DSH), enabling subscription LLM accounts such as ChatGPT Plus/Pro to work without API keys. |
| 2335 | [snow-The/dsh-research-lab](https://github.com/snow-The/dsh-research-lab) | 0 | 2026-08-31 | 2026-08-31 | Research lab toolkit for DeepSeek Harness: AutoSci wiki, ASI-Bench eval ledger, self-building FTS5 retrieval, arXiv digest/review, writing rewrite |
| 2336 | [soarGuo/dsh-skin-lab](https://github.com/soarGuo/dsh-skin-lab) | 0 | 2026-08-25 | 2026-08-25 | Skin Lab for the DSH Web GUI: token browser, live try-on, theme freeze, spectrum presets with SVG backdrops, custom backdrop upload. Everything is a plugin. |
| 2337 | [soberbiak/amazon-sucareer](https://github.com/soberbiak/amazon-sucareer) | 0 | 2026-08-28 | 2026-08-30 | 基于真实证据，把亚马逊运营经历酥成招聘方看得懂、面试讲得透的职业定位、简历与求职表达。拒绝硬编 KPI，争取人生大结果。 |
| 2338 | [softspark/dsh-orchestrator](https://github.com/softspark/dsh-orchestrator) | 0 | 2026-08-26 | 2026-08-27 | DeepSeek Harness bundle for one-shot Claude Code and GitHub Copilot Gemini delegation through native subscription logins. |
| 2339 | [songying2024/dsh-bookmarks-dock](https://github.com/songying2024/dsh-bookmarks-dock) | 0 | 2026-08-22 | 2026-08-22 | DeepSeek Harness (DSH) left-side bookmark dock plugin |
| 2340 | [soulYANG/dsh-baogongtou](https://github.com/soulYANG/dsh-baogongtou) | 0 | 2026-08-26 | 2026-08-26 | 包工头：DeepSeek Harness 工作 agent 皮肤。能力还是 dsh，嘴和按钮是包工头。 |
| 2341 | [Sparrived/dsh-plugin-workspace-skill](https://github.com/Sparrived/dsh-plugin-workspace-skill) | 0 | 2026-08-22 | 2026-08-22 | DSH Cordis plugin: skill-create authoring guide + workspace-level skill isolation for .dsh/skills |
| 2342 | [SpringNyan/dsh-public-proxy](https://github.com/SpringNyan/dsh-public-proxy) | 0 | 2026-08-22 | 2026-08-24 | A DeepSeek Harness plugin that exposes the DSH Web UI for LAN access |
| 2343 | [sqs404/dsh-client-ui-beautify](https://github.com/sqs404/dsh-client-ui-beautify) | 0 | 2026-08-23 | 2026-08-23 | DeepSeek Harness UI beautify plugin / one-click skin: settings-backed switch, aurora background, glass panels |
| 2344 | [squirrelbullet/dsh-client-ui-vibecontroller](https://github.com/squirrelbullet/dsh-client-ui-vibecontroller) | 0 | 2026-08-21 | 2026-08-22 | Floating controller overlay for DeepSeek Harness with voice input and game-like button layout. |
| 2345 | [sskkde/dsh-oh-my-agent](https://github.com/sskkde/dsh-oh-my-agent) | 0 | 2026-08-25 | 2026-08-25 | oh-my-openagent (OmO) core capabilities ported as a DeepSeek Harness plugin: ultrawork, role delegation, rules engine, boulder memory, hooks, Sisyphus main-prompt discipline |
| 2346 | [StabCut/dsh-plugin-restart-desktop](https://github.com/StabCut/dsh-plugin-restart-desktop) | 0 | 2026-08-21 | 2026-08-24 | DSH Desktop sidebar restart button: orderly relaunch of DSH Desktop from the sidebar settings row (based on desktopActions.requestRestart). |
| 2347 | [STARDUSTLC666/dsh-dream](https://github.com/STARDUSTLC666/dsh-dream) | 0 | 2026-08-26 | 2026-08-26 | DSH 做梦插件：会话回放（梦原料）→ 反思 → 梦境日记（记忆巩固）→ 高频教训幂等桥接 AGENTS.md。多帧 zstd 会话读取、默认隐私脱敏、零运行时依赖。Dream plugin for DeepSeek Harness: session replay, reflection, dream journal, memory bridge. |
| 2348 | [STARDUSTLC666/dsh-suite](https://github.com/STARDUSTLC666/dsh-suite) | 0 | 2026-08-27 | 2026-08-27 | STARDUSTLC 插件全家桶：一条命令装入 18 个 DSH 插件（办公流/媒体工坊/DevOps/做梦）。The STARDUSTLC plugin suite: 18 DSH plugins, one command. |
| 2349 | [Starlight-bananice/dsh-zhushou](https://github.com/Starlight-bananice/dsh-zhushou) | 0 | 2026-08-24 | 2026-08-25 | DSH 侧边栏助手插件（dsh-zhushou）：在侧边栏管理/选择助手，选中后在 DSH 会话内直接以助手人设对话；不选则保持原生会话。 |
| 2350 | [starsinc1708/dsh-tool-council](https://github.com/starsinc1708/dsh-tool-council) | 0 | 2026-08-26 | 2026-08-27 | Map-reduce council of subagents for the DeepSeek Harness: one task fans out to independent members, their findings are deduplicated, verified by a separate panel, and reduced to a quorum report |
| 2351 | [stayhpjinng/dsh-provider-proxy](https://github.com/stayhpjinng/dsh-provider-proxy) | 0 | 2026-08-29 | 2026-08-29 | Provider-scoped HTTP/HTTPS forward proxy plugin for DeepSeek Harness |
| 2352 | [steven-ngle/dsh-elden](https://github.com/steven-ngle/dsh-elden) | 0 | 2026-08-30 | 2026-08-30 | Elden Ring style event overlays for the DeepSeek Harness web UI |
| 2353 | [striveh/dsh-capability-resolver](https://github.com/striveh/dsh-capability-resolver) | 0 | 2026-08-25 | 2026-08-25 | Read-only local capability and community plugin discovery for DeepSeek Harness |
| 2354 | [StudyforDS/Deepseek_dsh-plugin](https://github.com/StudyforDS/Deepseek_dsh-plugin) | 0 | 2026-08-30 | 2026-08-31 | dsh-plugin |
| 2355 | [suanniniu/dsh-standard-toolkit](https://github.com/suanniniu/dsh-standard-toolkit) | 0 | 2026-08-17 | 2026-08-23 | DeepSeek Harness 标准工具插件(Standard ToolKit):工具管家——平时工具不占位,会话按需自动装载/用完自动收纳,省token;支持 load_tool / register_new_tool 现场造工具。Tool manager plugin for DeepSeek Harness / dsh. |
| 2356 | [substitute525/dsh-tool-monitor](https://github.com/substitute525/dsh-tool-monitor) | 0 | 2026-08-28 | 2026-08-28 | 一个 dsh-plugin：后台监听文件或命令输出，输出到达时唤醒所属会话，并在 Web 会话头部提供实时监听的列表与输出查看面板。MIT License。 |
| 2357 | [SuCriss/dsh-voice-control](https://github.com/SuCriss/dsh-voice-control) | 0 | 2026-08-31 | 2026-08-31 | Voice control for DeepSeek Harness web: speech-to-text into the composer and spoken playback of assistant replies, zero dependencies |
| 2358 | [SUFE-Chaoyi/dsh-plugin-csv-report](https://github.com/SUFE-Chaoyi/dsh-plugin-csv-report) | 0 | 2026-08-31 | 2026-08-31 | 基于 DeepSeek Harness 的可复用 CSV 描述统计与可复现报告插件 |
| 2359 | [Suguyun/dsh-bili-miniplay](https://github.com/Suguyun/dsh-bili-miniplay) | 0 | 2026-08-28 | 2026-08-28 | 跨平台 fork of dsh-bili-widget：DSH B站悬浮看片小窗（Node 原生 fetch，macOS/Linux/Windows 通用） |
| 2360 | [SuiBbinggan/dsh-cn-plugin-center](https://github.com/SuiBbinggan/dsh-cn-plugin-center) | 0 | 2026-08-25 | 2026-08-25 | China-friendly plugin center for DeepSeek Harness with curated and verified community plugins. |
| 2361 | [Suixin04/dsh-session-migrator](https://github.com/Suixin04/dsh-session-migrator) | 0 | 2026-08-24 | 2026-08-25 | DeepSeek Harness 可视化跨设备会话迁移插件｜Visual cross-device session migration with drag-and-drop ZIP, JSONL, and folder imports. |
| 2362 | [sujiu0616-art/DSH-CustomWallpapers-Glassmorphism-Theme](https://github.com/sujiu0616-art/DSH-CustomWallpapers-Glassmorphism-Theme) | 0 | 2026-08-21 | 2026-08-22 | dsh可自定义壁纸玻璃风主题 |
| 2363 | [sujiu222/dsh-one-click-archive](https://github.com/sujiu222/dsh-one-click-archive) | 0 | 2026-08-22 | 2026-08-23 | One-click time-based conversation archiving for the DeepSeek Harness Web GUI |
| 2364 | [sunnystarye-ui/dsh-plugin-text-quote](https://github.com/sunnystarye-ui/dsh-plugin-text-quote) | 0 | 2026-08-24 | 2026-08-24 | Codex-style text annotation for DeepSeek Harness conversations / 对话文字批注插件 |
| 2365 | [sunnywangzi/dsh-server-admin](https://github.com/sunnywangzi/dsh-server-admin) | 0 | 2026-08-22 | 2026-08-22 | DSH 服务器管理面板：在线重启/停止、systemd 一键保活、在线安装插件、状态监控、活跃会话、命令终端 \| DSH Server Admin: online restart/stop, systemd keep-alive, plugin install, status monitor, active sessions, command terminal |
| 2366 | [sunyuhuirong/fsviewer](https://github.com/sunyuhuirong/fsviewer) | 0 | 2026-08-29 | 2026-08-30 | Codex-style right-edge workspace for DeepSeek dsh web: file tree + preview, embedded browser, and side chat |
| 2367 | [superkonka/dsh-poor-mode](https://github.com/superkonka/dsh-poor-mode) | 0 | 2026-08-27 | 2026-08-27 | 穷鬼模式 Poor Mode — 供应商感知的分时省钱 DSH agent preset：复杂任务可选「立即执行」或「闲时执行」（DeepSeek 峰谷半价；其他平台可自定义规则） |
| 2368 | [SuperstructureJH/dsh-workbuddy-ppt](https://github.com/SuperstructureJH/dsh-workbuddy-ppt) | 0 | 2026-08-26 | 2026-08-26 | Editable PPTX generation for DSH with bundled authoring skills and deterministic PPTD validation |
| 2369 | [susirial/dsh-traebao](https://github.com/susirial/dsh-traebao) | 0 | 2026-08-23 | 2026-08-23 | Conversation-aware TRAE Bao digital pet for DeepSeek Harness Desktop |
| 2370 | [suyukun/dsh-plugin-publish](https://github.com/suyukun/dsh-plugin-publish) | 0 | 2026-08-26 | 2026-08-26 | Ship your skills, grow your influence — a model-agnostic publishing protocol for AI agent skills: preflight checks, GitHub repo, index PRs, marketplace submissions, promo copy. 把 agent 技能标准化发布到 GitHub 的流程协议。 |
| 2371 | [suyukun/dsh-tech-selection](https://github.com/suyukun/dsh-tech-selection) | 0 | 2026-08-26 | 2026-08-26 | Stop letting your AI guess — a research protocol for tech decisions that any AI agent (DSH/Claude/Cursor/Codex) can follow: quantified requirements, T1-T6 source tiers, quality gates, traceable verdicts. 模型无关的技术选型调研协议。 |
| 2372 | [svcomplex-dev/dsh-svw-waveform](https://github.com/svcomplex-dev/dsh-svw-waveform) | 0 | 2026-08-24 | 2026-08-24 | DeepSeek Harness plugin for viewing and analyzing VCD/FST waveforms with SVW. |
| 2373 | [svgop/dsh-generative-ideas](https://github.com/svgop/dsh-generative-ideas) | 0 | 2026-08-26 | 2026-08-29 | Roadmap ideation for DeepSeek Harness — generate and compare distinct roadmap options via headless agent runs, pick one, export as goal.md |
| 2374 | [svgop/dsh-rich-context](https://github.com/svgop/dsh-rich-context) | 0 | 2026-08-26 | 2026-08-29 | Agent instruction manager for DSH — edit and template the AGENTS.md files the harness actually reads (global + per-workspace) |
| 2375 | [svgop/dsh-rich-tracking](https://github.com/svgop/dsh-rich-tracking) | 0 | 2026-08-26 | 2026-08-29 | Percent-progress scoreboard for DeepSeek Harness — evidence-bound rows, git-captured checkpoints, pursue/align/dismiss operator whip |
| 2376 | [syfun/dsh-dogpet](https://github.com/syfun/dsh-dogpet) | 0 | 2026-08-27 | 2026-08-27 | 🐕 中华田园犬桌面宠物 - DSH Desktop Pet |
| 2377 | [syncended/deepseek-harness-messenger](https://github.com/syncended/deepseek-harness-messenger) | 0 | 2026-08-25 | 2026-08-29 | Messenger bridge plugin for DeepSeek Harness, starting with Telegram |
| 2378 | [syncended/deepseek-harness-usage](https://github.com/syncended/deepseek-harness-usage) | 0 | 2026-08-26 | 2026-08-26 | Token usage, model cost analytics, trends, and activity heatmaps for DeepSeek Harness |
| 2379 | [szymonsheng2045/dsh-carbonclub](https://github.com/szymonsheng2045/dsh-carbonclub) | 0 | 2026-08-28 | 2026-08-28 | A zero-model-cost human waiting room for DeepSeek Harness |
| 2380 | [tang-zhilei/dsh-group-chat-view](https://github.com/tang-zhilei/dsh-group-chat-view) | 0 | 2026-08-21 | 2026-08-22 | DSH group chat style conversation view plugin |
| 2381 | [Tangweiwei227/dsh-asc](https://github.com/Tangweiwei227/dsh-asc) | 0 | 2026-08-29 | 2026-08-29 | App Store Connect CLI (asc) as a native tool for DeepSeek Harness — structured argv, JSON output, no-shell execution. |
| 2382 | [taod8205-spec/model-switcher-dsh](https://github.com/taod8205-spec/model-switcher-dsh) | 0 | 2026-08-28 | 2026-08-28 | DeepSeek Harness 模型与推理强度一键切换插件，支持胶囊滑杆、档位吸附和极高态视觉。 |
| 2383 | [TARS-snail/dsh-notify](https://github.com/TARS-snail/dsh-notify) | 0 | 2026-08-25 | 2026-08-26 | Desktop notifications for DeepSeek Harness sessions, only while you are away |
| 2384 | [tatselkrik/dsh-web-search-ddg](https://github.com/tatselkrik/dsh-web-search-ddg) | 0 | 2026-08-24 | 2026-08-24 | Keyless DuckDuckGo web search provider for DeepSeek Harness (ctx.web seam) — no API keys, no accounts, zero tokens per search. Strict-mode scraping, redirect unwrapping, dedupe, entity-safe parsing, committed builds, one-command profile install. |
| 2385 | [TelosmaYLX/dsh-session-notify](https://github.com/TelosmaYLX/dsh-session-notify) | 0 | 2026-08-28 | 2026-08-28 | 当dsh任务完成/阻塞/提问等情况时，自动推送windows消息进行提醒，支持自定义文案和图片，以及显示会话用时、消耗token、速度tps等指标。Automatically push Windows notifications upon completion of a dsh task, supporting custom text and images, as well as displaying metrics including session duration, token consumption, and TPS speed. |
| 2386 | [termanli/dsh-fulltext-search](https://github.com/termanli/dsh-fulltext-search) | 0 | 2026-08-24 | 2026-08-24 | A DSH (DeepSeek Harness) Web GUI plugin that searches file contents in the current session working directory from the sidebar file manager (dsh-better-sidebar), returning file + line number + matching line preview. |
| 2387 | [TheChengXi/dsh-session-sync](https://github.com/TheChengXi/dsh-session-sync) | 0 | 2026-08-25 | 2026-08-25 | 广播会话修改实现多窗口同步  |
| 2388 | [TheHeartFickle/dsh-conversation-folding](https://github.com/TheHeartFickle/dsh-conversation-folding) | 0 | 2026-08-21 | 2026-08-22 | DSH 对话流渲染增强插件 —— 折叠过程，保留正文，长对话更清爽。 |
| 2389 | [TheHeartFickle/dsh-solo-agent](https://github.com/TheHeartFickle/dsh-solo-agent) | 0 | 2026-08-21 | 2026-08-26 | DSH 插件：向用户 agent-presets 注入 `solo` preset,优化上下文占用和模型调度。 |
| 2390 | [thinkingpeach-sketch/wan3-agent-skills](https://github.com/thinkingpeach-sketch/wan3-agent-skills) | 0 | 2026-08-19 | 2026-08-22 | Portable WAN3 image and video generation skills for AI coding agents |
| 2391 | [tianhanly/dsh-genshin-redirect](https://github.com/tianhanly/dsh-genshin-redirect) | 0 | 2026-08-30 | 2026-08-31 | 完成任务自动跳转到原神 Automatically jump to Genshin Impact after completing the task |
| 2392 | [tianhanly/dsh-official-port-nav](https://github.com/tianhanly/dsh-official-port-nav) | 0 | 2026-08-29 | 2026-08-30 | Perfectly replicate DeepSeek's official right-side chat navigation in Harness |
| 2393 | [tianhanly/dsh-verification-meme](https://github.com/tianhanly/dsh-verification-meme) | 0 | 2026-08-30 | 2026-08-31 | Every time you press a key, a security verification pops up. 每按一个harness的按键都会跳出一个安全验证 |
| 2394 | [tianhanly/dsh-warm-reminder](https://github.com/tianhanly/dsh-warm-reminder) | 0 | 2026-08-29 | 2026-08-29 | 智能温馨提醒插件，检测使用时长自动提示喝水、护眼、休息，支持深夜关怀与节假日祝福。基于DSH/Cordis框架开发。 |
| 2395 | [tianyuegithub/dsh-pactflow](https://github.com/tianyuegithub/dsh-pactflow) | 0 | 2026-08-30 | 2026-08-30 | DSH PactFlow（零脉模式）外部 Profile Bundle |
| 2396 | [Tieboyh/dsh-chat-enhancer](https://github.com/Tieboyh/dsh-chat-enhancer) | 0 | 2026-08-24 | 2026-08-24 | Focused conversation enhancements for DeepSeek Harness Web, starting with zoomable fullscreen Mermaid diagrams. |
| 2397 | [Tieboyh/dsh-notes-markdown](https://github.com/Tieboyh/dsh-notes-markdown) | 0 | 2026-08-24 | 2026-08-24 | Editable Markdown notes in the DeepSeek Harness sidebar |
| 2398 | [Tieboyh/dsh-usage-center](https://github.com/Tieboyh/dsh-usage-center) | 0 | 2026-08-24 | 2026-08-24 | Native DSH settings page for daily provider usage, subscription quotas, balances, and API price estimates. |
| 2399 | [Tiko9527/dsh-image-tiler](https://github.com/Tiko9527/dsh-image-tiler) | 0 | 2026-08-23 | 2026-08-23 | DSH high-resolution image tiler: slices large images into <=800x800 tiles before sending to DeepSeek. Highly AI-native, only DeepSeek participation. |
| 2400 | [Tiko9527/task-router](https://github.com/Tiko9527/task-router) | 0 | 2026-08-23 | 2026-08-23 | DSH task delegation router plugin: main model plans/verifies, sub-models search/browse/code/verify. Highly AI-native, built with GLM/DeepSeek/Qwen assistance. |
| 2401 | [Tinnikx/dsh-desktop](https://github.com/Tinnikx/dsh-desktop) | 0 | 2026-08-20 | 2026-08-29 | DeepSeek Harness 的 Linux Electron 桌面客户端，由claude opus生成, 打包后开箱即用, 已更新至0.1.1-rc.2, 插件安装方式与web端一致, 支持"插件市场"插件, 可以安装插件市场后在插件市场中搜索并安装插件, 也可以通过正常命令 ./bin/dsh plugin --profile web add xxxx, download in the Release Page. |
| 2402 | [Tinnikx/dsh-operation-improve](https://github.com/Tinnikx/dsh-operation-improve) | 0 | 2026-08-30 | 2026-08-31 | DeepSeek Harness 客户端增强插件：侧边栏多选与右键菜单、对话起点导航列、逐行开始时间戳、活跃标记配色、选区右键菜单、思考区限高、设置页 Harness 高级配置面板。仅占一个 slot，不发布。 |
| 2403 | [tkwkeven/dsh-lark](https://github.com/tkwkeven/dsh-lark) | 0 | 2026-08-20 | 2026-08-22 | Feishu/Lark channel for DeepSeek Harness: prefix-created task sessions, thread routing, streaming thinking cards, interactive questions, media delivery, lifecycle notices, runtime policies, web mirror |
| 2404 | [tkwkeven/dsh-sim-restart](https://github.com/tkwkeven/dsh-sim-restart) | 0 | 2026-08-20 | 2026-08-22 | Simulated-restart testing for DeepSeek Harness plugins: verifies plugins survive restart (module eval → apply → smoke → dispose) in isolated subprocesses, with a resident auto-watcher and agent feedback loop |
| 2405 | [tkwkeven/dsh-tool-github](https://github.com/tkwkeven/dsh-tool-github) | 0 | 2026-08-20 | 2026-08-22 | GitHub REST API tools and web GUI panel for DeepSeek Harness: bind account, search code/issues, manage PRs, clone workspaces |
| 2406 | [tkwkeven/dsh-ytdlp](https://github.com/tkwkeven/dsh-ytdlp) | 0 | 2026-08-20 | 2026-08-22 | Video/audio download tools for DeepSeek Harness, powered by yt-dlp (video_info / video_download) |
| 2407 | [TnzGit/dsh-live-perf-gauges](https://github.com/TnzGit/dsh-live-perf-gauges) | 0 | 2026-08-27 | 2026-08-27 | Real-time Decode tok/s, TTFT and Prefill throughput dashboard for DeepSeek Harness. |
| 2408 | [todayer/todayer-dsh-telegram-bridge](https://github.com/todayer/todayer-dsh-telegram-bridge) | 0 | 2026-08-24 | 2026-08-26 | DeepSeek Harness Telegram bridge (bot) plugin, Hermes-style: per-topic sessions, DM topics, group gating, media, commands. Fork/extension of hi-wenw/dsh-telegram-channel. |
| 2409 | [Traveritas/petween](https://github.com/Traveritas/petween) | 0 | 2026-08-21 | 2026-08-29 | Agent pet plugin for DeepSeek Harness (dsh): a few pose images in, expressive comic-style motion out — WAAPI timeline engine, custom animation editor, pose presets, and extension services for companion plugins |
| 2410 | [Traveritas/petween-physics](https://github.com/Traveritas/petween-physics) | 0 | 2026-08-25 | 2026-08-29 | Throw-physics companion plugin for Petween (drag-fling, wall bounce, ground slide), consuming the petween extension services |
| 2411 | [Triple3h/dsh-image-read](https://github.com/Triple3h/dsh-image-read) | 0 | 2026-08-19 | 2026-08-23 | DSH native plugin: structured image analysis via multimodal APIs (read_image_mimo tool) with provider failover, caching, SSRF protection and a Web UI config card. DSH 原生插件：多模态识图，返回结构化 JSON 证据，支持故障转移/缓存/SSRF 防护/Web 配置卡片。 |
| 2412 | [Triple3h/dsh-input-enhancement](https://github.com/Triple3h/dsh-input-enhancement) | 0 | 2026-08-20 | 2026-08-23 | DSH Web plugin: input enhancement — paste text collapse, file/folder attachment paste & drag-drop, bubble attachment folding, message fold, attachment management & cleanup. DSH Web 插件：输入增强——粘贴文本折叠、附件上传、消息折叠。 |
| 2413 | [Triple3h/dsh-reasoning-effort](https://github.com/Triple3h/dsh-reasoning-effort) | 0 | 2026-08-19 | 2026-08-23 | DSH Web plugin: per-model reasoning-effort configuration and selection — settings page + slider embedded in the model picker. DSH Web 插件：逐模型推理力度配置与选择（设置页 + 模型选择器内嵌滑块）。 |
| 2414 | [Triple3h/dsh-rxresume](https://github.com/Triple3h/dsh-rxresume) | 0 | 2026-08-23 | 2026-08-23 | DSH plugin that talks to the Reactive Resume REST API directly: create, read, patch, and manage resumes over /api/openapi with an API key. 直接对接 Reactive Resume REST API 管理简历的 DSH 插件。 |
| 2415 | [Triple3h/dsh-session-enhance](https://github.com/Triple3h/dsh-session-enhance) | 0 | 2026-08-19 | 2026-08-23 | DSH Web plugin: session sidebar enhancements — copy session ID from the context menu, etc. DSH Web 插件：会话栏增强（上下文菜单一键复制会话 ID 等）。 |
| 2416 | [Triple3h/dsh-stats-expand](https://github.com/Triple3h/dsh-stats-expand) | 0 | 2026-08-20 | 2026-08-23 | DSH Web client plugin: unwrap the session stats bar to full-width, click to toggle truncation (preference persisted). DSH Web 客户端插件：会话底部统计条解除限宽、单行完整铺满，点击可切回官方截断。 |
| 2417 | [TropicWiden/dsh-history-question-nav](https://github.com/TropicWiden/dsh-history-question-nav) | 0 | 2026-08-25 | 2026-08-25 | A DeepSeek Harness web plugin that lists every question you ask in the current session in a right-side panel, and scrolls to the matching answer when you click one.  DeepSeek Harness Web 插件：在窗口右侧列出当前会话的每个提问，点击即定位到对应回答。 |
| 2418 | [trueRISCOacnt/maa-dsh-skill](https://github.com/trueRISCOacnt/maa-dsh-skill) | 0 | 2026-08-28 | 2026-08-30 | 基于 MaaAssistantArknights (MAA) 官方命令行工具 maa-cli 构建的 DeepSeek Harness Skill：让 DeepSeek Harness 直接驱动 MaaCore，自动化完成《明日方舟》日常任务。 |
| 2419 | [TTsdzb/dsh-global-proxy](https://github.com/TTsdzb/dsh-global-proxy) | 0 | 2026-08-21 | 2026-08-22 | 更好的代理支持。 |
| 2420 | [tumi-huakai/dsh-plugin-meow-speech](https://github.com/tumi-huakai/dsh-plugin-meow-speech) | 0 | 2026-08-28 | 2026-08-28 | 喵语定制：DSH 消息正文显示层文本替换插件（仅界面显示，不改动真实对话内容） |
| 2421 | [tuofangzhe/dsh-plugins](https://github.com/tuofangzhe/dsh-plugins) | 0 | 2026-08-24 | 2026-08-24 | Community plugin registry for DeepSeek Harness (DSH) plugins, Skills & MCP — DSH 插件目录与中文安装配置教程 · 52dsh.com |
| 2422 | [TussalZeus18028/dsh-conflict-checker](https://github.com/TussalZeus18028/dsh-conflict-checker) | 0 | 2026-08-26 | 2026-08-26 | Detect DeepSeek Harness plugin conflicts and internal issues; manage plugins (enable/disable/uninstall) from a settings page. |
| 2423 | [tuzkier/valley-liang](https://github.com/tuzkier/valley-liang) | 0 | 2026-08-28 | 2026-08-28 | 梁文谷：替换 DeepSeek Harness Web 品牌标识，并按北京时间高峰时段切换图片。 |
| 2424 | [uckkk/dsh-fat-loss-cal](https://github.com/uckkk/dsh-fat-loss-cal) | 0 | 2026-08-20 | 2026-08-21 | 减脂热量计算 |
| 2425 | [uckkk/dsh-future-cbdc](https://github.com/uckkk/dsh-future-cbdc) | 0 | 2026-08-21 | 2026-08-21 | 央行数字货币 |
| 2426 | [uckkk/dsh-future-fusion](https://github.com/uckkk/dsh-future-fusion) | 0 | 2026-08-21 | 2026-08-21 | 核聚变能源 |
| 2427 | [uckkk/dsh-future-longevity](https://github.com/uckkk/dsh-future-longevity) | 0 | 2026-08-21 | 2026-08-21 | 长寿医学 |
| 2428 | [uckkk/dsh-gift-etiquette](https://github.com/uckkk/dsh-gift-etiquette) | 0 | 2026-08-21 | 2026-08-21 | 送礼避讳 |
| 2429 | [uckkk/dsh-k2c](https://github.com/uckkk/dsh-k2c) | 0 | 2026-08-21 | 2026-08-21 | 开尔文转摄氏 |
| 2430 | [uckkk/dsh-kenya](https://github.com/uckkk/dsh-kenya) | 0 | 2026-08-21 | 2026-08-21 | 肯尼亚国家 |
| 2431 | [uckkk/dsh-palau](https://github.com/uckkk/dsh-palau) | 0 | 2026-08-21 | 2026-08-21 | 帕劳国 |
| 2432 | [UnforgetMemory/um-dsh-websearch](https://github.com/UnforgetMemory/um-dsh-websearch) | 0 | 2026-08-27 | 2026-08-27 | Exa (exa.ai) web search provider plugin for DeepSeek Harness (DSH): dynamic enabled switch, credentials-service key resolution, bilingual settings card. |
| 2433 | [Unintendedz/dsh-session-workspace](https://github.com/Unintendedz/dsh-session-workspace) | 0 | 2026-08-23 | 2026-08-24 | Move cold DeepSeek Harness sessions between registered workspaces |
| 2434 | [Unintendedz/dsh-ui-enhancements](https://github.com/Unintendedz/dsh-ui-enhancements) | 0 | 2026-08-23 | 2026-08-23 | Small, focused UI enhancements for DeepSeek Harness |
| 2435 | [unknowbug/dsh-thinking-loop-guard](https://github.com/unknowbug/dsh-thinking-loop-guard) | 0 | 2026-08-27 | 2026-08-27 | Detect & break thinking-chain loops in DSH agents at the turn boundary (no proxy). Ported from ollama-loop-guard. |
| 2436 | [UnKnownFish125/dsh-livetaskboard](https://github.com/UnKnownFish125/dsh-livetaskboard) | 0 | 2026-08-26 | 2026-08-27 | 派生动态任务看板插件：独立任务状态机、存储、看板 UI、外援（sol + 保底子代理）；从 dsh-deepmemory 派生。 |
| 2437 | [upJiang/dsh-cron-job](https://github.com/upJiang/dsh-cron-job) | 0 | 2026-08-27 | 2026-08-31 | dsh 插件，定时任务+多渠道推送 |
| 2438 | [uppercrusteve/dsh-plugin-split-and-solve](https://github.com/uppercrusteve/dsh-plugin-split-and-solve) | 0 | 2026-08-29 | 2026-08-29 | DSH plugin: split batch / multi-subproblem research tasks into small questions and solve them with sub-agents |
| 2439 | [Ury479/dsh-wukong-zenfire](https://github.com/Ury479/dsh-wukong-zenfire) | 0 | 2026-08-25 | 2026-08-25 | Wukong Zenfire skin plugin for DeepSeek Harness (DSH) WebUI and Desktop |
| 2440 | [useful-money/Deepseek-Harness-branch-map-plugin](https://github.com/useful-money/Deepseek-Harness-branch-map-plugin) | 0 | 2026-08-31 | 2026-08-31 | dsh-plugin; branch map show; branch map mange |
| 2441 | [valkia/dsh-plugin-computer-use](https://github.com/valkia/dsh-plugin-computer-use) | 0 | 2026-08-24 | 2026-08-24 | Computer Use plugin for DeepSeek Harness using Open Computer Use MCP |
| 2442 | [valkia/dsh-plugin-git-log](https://github.com/valkia/dsh-plugin-git-log) | 0 | 2026-08-24 | 2026-08-24 | Git Log commit graph and history workbench for DeepSeek Harness |
| 2443 | [vb2250158/dsh-plugins](https://github.com/vb2250158/dsh-plugins) | 0 | 2026-08-27 | 2026-08-27 | Open-source DeepSeek Harness plugin bundle with portable multi-computer synchronization |
| 2444 | [veermetri05/dsh-plugins](https://github.com/veermetri05/dsh-plugins) | 0 | 2026-08-25 | 2026-08-25 | Collection of DeepSeek Harness (DSH) plugins — web-search-omp ported from oh-my-pi (23 providers, fallback chain, credential-free) |
| 2445 | [Victor-770/dsh-plugin-directory](https://github.com/Victor-770/dsh-plugin-directory) | 0 | 2026-08-14 | 2026-08-25 | DeepSeek Harness 插件目录：中英双语、按功能分类、README 全文搜索、按热度排序。 |
| 2446 | [Viktirr/dsh-llm-lmstudio](https://github.com/Viktirr/dsh-llm-lmstudio) | 0 | 2026-08-28 | 2026-08-29 | LM Studio (OpenAI-compatible local server) adapter plugin for DeepSeek Harness |
| 2447 | [vimalinx/Dsh-dev](https://github.com/vimalinx/Dsh-dev) | 0 | 2026-08-22 | 2026-08-22 | Version-aware workspace core for building DeepSeek Harness plugins |
| 2448 | [VinciBeans/dsh-smooth-plugin](https://github.com/VinciBeans/dsh-smooth-plugin) | 0 | 2026-08-24 | 2026-08-31 | 让 DSH 的会话滚底从"官方瞬时跳变"变成流畅顺滑的跟随滚动：会话装载与"回到最新"保持瞬时，而流式内容增长期间，消息列以恒定速度平滑跟随，起步轻柔、收尾绵软。 |
| 2449 | [vinokok/dsh-external-access-guide](https://github.com/vinokok/dsh-external-access-guide) | 0 | 2026-08-24 | 2026-08-24 | 远程 VPS 上部署 DSH 并通过 HTTPS 安全开放外网访问 \| Deploy DSH on a remote VPS and expose it securely over HTTPS |
| 2450 | [vINyLogY/dsh-bluebubbles](https://github.com/vINyLogY/dsh-bluebubbles) | 0 | 2026-08-22 | 2026-08-23 | Who needs openclaw? |
| 2451 | [Viviana-Luna/dsh-window](https://github.com/Viviana-Luna/dsh-window) | 0 | 2026-08-24 | 2026-08-28 | macOS 薄桌面客户端，为本机 DSH 提供 Liquid Glass UI。 |
| 2452 | [vladlearns/dsh-fs-deny-policy](https://github.com/vladlearns/dsh-fs-deny-policy) | 0 | 2026-08-24 | 2026-08-25 | DeepSeek Harness plugin: a deployment deny list of filesystem roots the model may never touch |
| 2453 | [wang-junjian/dsh-github-trending](https://github.com/wang-junjian/dsh-github-trending) | 0 | 2026-08-23 | 2026-08-24 | DeepSeek Harness 插件 GitHub Trending |
| 2454 | [wangyong1972/dsh-computer-use-macos](https://github.com/wangyong1972/dsh-computer-use-macos) | 0 | 2026-08-22 | 2026-08-23 | Native macOS computer-use plugin for DeepSeek Harness with trusted mouse/keyboard control, screenshots, and multi-display selection. |
| 2455 | [wangyuanchuan2022/dsh-mobile-ux](https://github.com/wangyuanchuan2022/dsh-mobile-ux) | 0 | 2026-08-25 | 2026-08-25 | 一个包、零配置：把 DeepSeek Harness 网页版在手机宽度下的体验从头打磨一遍——响应式抽屉布局、字号/间距适配、≥44px 触控目标、按钮/菜单/表格移动端交互、安全区适配。桌面宽度显示与使用完全不受影响。 |
| 2456 | [wangzhanchao883/dsh-screenshot-capture](https://github.com/wangzhanchao883/dsh-screenshot-capture) | 0 | 2026-08-24 | 2026-08-24 | Point-and-shoot screenshot capture plugin for DeepSeek Harness: clipboard watcher + system floating window (comment & key-point, copy/save-doc/save-image) + instant OCR (Tongyi Qianwen) + Obsidian per-day merging + evening AI organization. 指哪拍哪 · DSH 截图即存插件:剪贴板监听 + 系统级悬浮窗 + 即时 OCR + Obsidian 按天合并 + 晚间 AI 整理 |
| 2457 | [wantosure/dsh-plugin-browser-memory](https://github.com/wantosure/dsh-plugin-browser-memory) | 0 | 2026-08-26 | 2026-08-26 | Local-first DeepSeek Harness plugin for searching Chrome, Edge, and Brave bookmarks, history, and downloads. |
| 2458 | [wbycloud/dsh-composer-tokens](https://github.com/wbycloud/dsh-composer-tokens) | 0 | 2026-08-31 | 2026-08-31 | DSH web GUI composer real-time token counter plugin (client-side, v1) |
| 2459 | [weekitmo/dsh-trace](https://github.com/weekitmo/dsh-trace) | 0 | 2026-08-31 | 2026-08-31 | A DeepSeek Harness Web plugin for inspecting redacted LLM HTTP request and response traces. |
| 2460 | [weibaohui/dsh-continue](https://github.com/weibaohui/dsh-continue) | 0 | 2026-08-31 | 2026-08-31 | 自动续跑插件 for DeepSeek Harness — 有序规则表：按失败类型路由 继续续跑 / 换模型 / 压缩后继续 / 停止 |
| 2461 | [weibaohui/dsh-sync](https://github.com/weibaohui/dsh-sync) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness 插件：会话同步与冲突解决（apiproxy、token 内联） |
| 2462 | [weibaohui/dsh-tasks](https://github.com/weibaohui/dsh-tasks) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness 插件：cron 定时事项——定时/立即执行新建 agent 会话提交提示词，全屏管理界面 |
| 2463 | [weibaohui/hermes-loop](https://github.com/weibaohui/hermes-loop) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness 插件：Hermes 循环——review/curator 自动化与会话循环管理 |
| 2464 | [weibaohui/skills-management](https://github.com/weibaohui/skills-management) | 0 | 2026-08-31 | 2026-08-31 | DeepSeek Harness 插件：技能市场——安装/删除/详情 API + 管理界面 |
| 2465 | [Weiyang742/dsh-cross-session-messaging](https://github.com/Weiyang742/dsh-cross-session-messaging) | 0 | 2026-08-31 | 2026-08-31 | Cross-session relay for DeepSeek Harness: peer discovery and text delivery between independent dsh processes. |
| 2466 | [wenhao4126/dsh-herdr](https://github.com/wenhao4126/dsh-herdr) | 0 | 2026-08-26 | 2026-08-26 | Expose Herdr workspaces, panes, and coding agents as DeepSeek Harness tools. |
| 2467 | [wenyixiaoqingnian/ds-mobile-skin](https://github.com/wenyixiaoqingnian/ds-mobile-skin) | 0 | 2026-08-30 | 2026-08-30 | Mobile DeepSeek-app look for DSH Web GUI + dsh-token-viewer billing patch |
| 2468 | [wf-ping/dsh-message-injector](https://github.com/wf-ping/dsh-message-injector) | 0 | 2026-08-30 | 2026-08-30 | dsh（DeepSeek Harness）插件：预设消息注入内容组合，每条消息自动注入 —— auto-inject preset content into every message |
| 2469 | [wheam/dsh-session-groups](https://github.com/wheam/dsh-session-groups) | 0 | 2026-08-22 | 2026-08-23 | Provider-owned virtual session groups for the DeepSeek Harness Web sidebar. |
| 2470 | [whutzefengxie-ops/dsh-shadow-mind](https://github.com/whutzefengxie-ops/dsh-shadow-mind) | 0 | 2026-08-24 | 2026-08-28 | Independent Shadow agent orchestration plugin for DeepSeek Harness |
| 2471 | [Wickaninnish/dsh-skill-manager](https://github.com/Wickaninnish/dsh-skill-manager) | 0 | 2026-08-22 | 2026-08-27 | DeepSeek Harness 技能运维插件：自动发现、审计、去重和优化技能，构建安全可控的维护闭环。 |
| 2472 | [Wilfred-wei/dsh-fingerprint-relay](https://github.com/Wilfred-wei/dsh-fingerprint-relay) | 0 | 2026-08-23 | 2026-08-24 | DSH plugin: managed local fingerprint relays so DSH can reach providers that gate on the client's TLS fingerprint |
| 2473 | [Wilson-Lai-Ab/dsh-idea-style](https://github.com/Wilson-Lai-Ab/dsh-idea-style) | 0 | 2026-08-21 | 2026-08-26 | DSH plugin |
| 2474 | [windrover/dsh-long-term-memory](https://github.com/windrover/dsh-long-term-memory) | 0 | 2026-08-25 | 2026-08-26 | Layered deterministic long-term memory for DeepSeek Harness: CJK-aware BM25 recall, JSONL storage, per-assembly context injection, write guards and threat scanning. |
| 2475 | [winghv/dsh-acp-activity](https://github.com/winghv/dsh-acp-activity) | 0 | 2026-08-30 | 2026-08-30 | Community ACP automation server for DeepSeek Harness with committed tool-activity frames (tool_call/tool_call_update) — dsh-plugin |
| 2476 | [WinnieJQ/dsh-conversation-cost](https://github.com/WinnieJQ/dsh-conversation-cost) | 0 | 2026-08-28 | 2026-08-28 | Per-conversation DeepSeek API cost badge for DeepSeek Harness (dsh): zero-dependency sessionCost projection with peak/off-peak pricing and a live hover-card badge in the web conversation header. |
| 2477 | [Wisdoverse/dsh-inline-media-viewer-plugin](https://github.com/Wisdoverse/dsh-inline-media-viewer-plugin) | 0 | 2026-08-26 | 2026-08-28 | Inline image, video, and audio previews for DeepSeek Harness Web, with workspace-safe local files, direct web media, and an optional ComfyUI proxy. |
| 2478 | [Wisdoverse/dsh-skills-manager-plugin](https://github.com/Wisdoverse/dsh-skills-manager-plugin) | 0 | 2026-08-28 | 2026-08-28 | Skill manager for DeepSeek Harness: proactive skill activation with trigger hooks, GitHub source sync, and a Settings management UI. |
| 2479 | [Witchwarren2344/dsh-mnemosyne-memory](https://github.com/Witchwarren2344/dsh-mnemosyne-memory) | 0 | 2026-08-29 | 2026-08-29 | Provide long-term memory, vector semantic search, and LLM reflection for DeepSeek Harness (DSH) with this free, MIT-licensed plugin. |
| 2480 | [wjf1/dsh-commandcode](https://github.com/wjf1/dsh-commandcode) | 0 | 2026-08-30 | 2026-08-30 | DSH-Desktop LLM provider plugin for Command Code with model catalog sync, request retry, multi-credential support, and a settings UI. |
| 2481 | [WJNCT55555/dsh-crt-theme](https://github.com/WJNCT55555/dsh-crt-theme) | 0 | 2026-08-26 | 2026-08-27 | Dual-palette CRT terminal theme for DeepSeek Harness Web |
| 2482 | [wkfedor/deepseek-harness-voice-input](https://github.com/wkfedor/deepseek-harness-voice-input) | 0 | 2026-08-22 | 2026-08-23 | Local voice typing and speech-to-text plugin for DeepSeek Harness (dsh), powered by multilingual Whisper. |
| 2483 | [Wlain/deepseek-plugin](https://github.com/Wlain/deepseek-plugin) | 0 | 2026-08-26 | 2026-08-31 | Kling AI remote MCP plugin for DeepSeek Harness |
| 2484 | [wly8691-jpg/dsh-office-com](https://github.com/wly8691-jpg/dsh-office-com) | 0 | 2026-08-26 | 2026-08-26 | DSH plugin: COM-driven real Office automation (VBA/pivot/recalc/layout) |
| 2485 | [wodongx123/dsh-language-control](https://github.com/wodongx123/dsh-language-control) | 0 | 2026-08-28 | 2026-08-28 | DSH plugin: force agent chain-of-thought to stay in Chinese — 让 Agent 的思考过程也自动使用中文 |
| 2486 | [WolffyCode/deepseek-harness-plugin](https://github.com/WolffyCode/deepseek-harness-plugin) | 0 | 2026-08-25 | 2026-08-29 | Multi-engine Claude CLI and Codex CLI integration for DeepSeek Harness |
| 2487 | [wolfsonliu/zotero-skill](https://github.com/wolfsonliu/zotero-skill) | 0 | 2026-08-25 | 2026-08-25 | An agent-usable Zotero skill for AI agent — search, read, and write your local Zotero library through a single Python CLI. \| 面向 AI  Agent 的 Zotero 技能：通过单一 Python CLI 搜索、读取、写入本地 Zotero 文献库。 |
| 2488 | [WooLeo1995/dsh-llm-ai](https://github.com/WooLeo1995/dsh-llm-ai) | 0 | 2026-08-27 | 2026-08-27 | 替换 llm-pi-ai 模型配置，主要处理 dsh-llm-pi-ai 厂商和模型更新不及时的问题 |
| 2489 | [woshishadowhunter/dsh-seed-society](https://github.com/woshishadowhunter/dsh-seed-society) | 0 | 2026-08-25 | 2026-08-25 | Yogacara eight-consciousness agent society plugin for DeepSeek Harness: mneme memory consolidation tuning, llm-deepseek reasoning fix, MCP society bridge, and six seed skills |
| 2490 | [wpc725562-dotcom/deepfusion](https://github.com/wpc725562-dotcom/deepfusion) | 0 | 2026-08-25 | 2026-08-25 | DeepFusion: DSH x Reasonix 融合 Agent 引擎 (DeepSeek-native 编排 + 前缀缓存优化) |
| 2491 | [wr-web/dsh-context-tree](https://github.com/wr-web/dsh-context-tree) | 0 | 2026-08-26 | 2026-08-27 | Reusable trajectory-tree context, exact-turn forks, and bounded cross-session recall for DeepSeek Harness |
| 2492 | [writeCasually/dsh-opencode-go-models](https://github.com/writeCasually/dsh-opencode-go-models) | 0 | 2026-08-23 | 2026-08-23 | DSH 插件：自动同步 opencode-go 模型清单到 pi-ai catalog，按官方文档精确标记协议（anthropic-messages / openai-completions / openai-responses）与多模态支持 |
| 2493 | [WSL043/dsh-dictation](https://github.com/WSL043/dsh-dictation) | 0 | 2026-08-28 | 2026-08-28 | DeepSeek Harness 语音输入：本地多语言识别与 Codex Desktop 听写，只写入可编辑草稿。 |
| 2494 | [WSL043/dsh-image-viewer](https://github.com/WSL043/dsh-image-viewer) | 0 | 2026-08-26 | 2026-08-27 | 维护模式：DSH 可选共享图片查看器，提供缩放、原图下载、图库与区域标注。 |
| 2495 | [WSYXIUBA/dsh-plugin-starmap](https://github.com/WSYXIUBA/dsh-plugin-starmap) | 0 | 2026-08-21 | 2026-08-22 | 🪐 DSH 插件星座图 — DeepSeek Harness 插件依赖关系可视化（自动扫描/分类/依赖图） |
| 2496 | [wuruihi/dsh-memory-loader](https://github.com/wuruihi/dsh-memory-loader) | 0 | 2026-08-24 | 2026-08-24 | DSH plugin: deterministic two-level memory injection (global + project MEMORY.md + today's notes) at session start |
| 2497 | [Wuxie233/dsh-plugin-blank-session-gc](https://github.com/Wuxie233/dsh-plugin-blank-session-gc) | 0 | 2026-08-18 | 2026-08-23 | Keep at most one unused blank DSH conversation |
| 2498 | [wuyiwuaa1-ship-it/dsh-read-image-jpeg-fallback](https://github.com/wuyiwuaa1-ship-it/dsh-read-image-jpeg-fallback) | 0 | 2026-08-25 | 2026-08-26 | DSH plugin that converts read_image PNG/WebP attachments to JPEG for LM Studio compatibility. |
| 2499 | [wwskills/dsh-long-memory](https://github.com/wwskills/dsh-long-memory) | 0 | 2026-08-25 | 2026-08-25 | Long-term cross-session memory plugin for DeepSeek Harness |
| 2500 | [wwwwwald/dsh-story](https://github.com/wwwwwald/dsh-story) | 0 | 2026-08-21 | 2026-08-23 | One prompt to cinematic story. AI-powered script-to-video pipeline for DeepSeek Harness. |
| 2501 | [wxjgit/permission-popup](https://github.com/wxjgit/permission-popup) | 0 | 2026-08-27 | 2026-08-27 | 当前会话或后台会话正在等待权限审批时，插件会在页面角落显示审批卡片，让你无需切回原会话就能选择“允许一次”或“拒绝”。 |
| 2502 | [wyb587285-dot/git-ai-tracker](https://github.com/wyb587285-dot/git-ai-tracker) | 0 | 2026-08-31 | 2026-08-31 | GitHub AI repo tracker: star ratings, growth leaderboard, Markdown reports and web dashboard. |
| 2503 | [xain/ui-beep](https://github.com/xain/ui-beep) | 0 | 2026-08-26 | 2026-08-26 | **dsh-beep** — an agent-heartbeat sonification plugin for the DeepSeek Harness Web surface. |
| 2504 | [xarleyn/dsh-doc-impact](https://github.com/xarleyn/dsh-doc-impact) | 0 | 2026-08-28 | 2026-08-28 | Documentation impact enforcement for DeepSeek Harness — keep docs in sync by linking code changes to affected documentation. |
| 2505 | [xarleyn/dsh-session-scope](https://github.com/xarleyn/dsh-session-scope) | 0 | 2026-08-28 | 2026-08-28 | Per-session workspace scoping for DeepSeek Harness — expose only selected directories to agents with focused and isolated enforcement. |
| 2506 | [xarleyn/dsh-sleev](https://github.com/xarleyn/dsh-sleev) | 0 | 2026-08-26 | 2026-08-27 | Sleev integration for DeepSeek Harness with route-aware LLM telemetry and context-optimization observability |
| 2507 | [xchannel1987/dsh-mobile-xc](https://github.com/xchannel1987/dsh-mobile-xc) | 0 | 2026-08-28 | 2026-08-29 | DSH Web mobile UI adaptation plugin with overlay drawer, safe-area support, and canary version detection |
| 2508 | [xchannel1987/dsh-power-xc](https://github.com/xchannel1987/dsh-power-xc) | 0 | 2026-08-28 | 2026-08-29 | DSH power control plugin with restart/shutdown menu and Windows-style overlay animation |
| 2509 | [xchannel1987/dsh-reverse-proxy-xc](https://github.com/xchannel1987/dsh-reverse-proxy-xc) | 0 | 2026-08-28 | 2026-08-29 | DSH LAN reverse proxy plugin for accessing Web GUI from mobile devices |
| 2510 | [xchannel1987/dsh-session-xc](https://github.com/xchannel1987/dsh-session-xc) | 0 | 2026-08-28 | 2026-08-29 | DSH session enhancement plugin with session count display, archive management, and cross-workspace move |
| 2511 | [xchannel1987/dsh-token-usage-xc](https://github.com/xchannel1987/dsh-token-usage-xc) | 0 | 2026-08-28 | 2026-08-29 | DSH token usage statistics plugin with daily/7-day trends and cache hit rate |
| 2512 | [xdongHo/dsh-wechat-mobile-skin](https://github.com/xdongHo/dsh-wechat-mobile-skin) | 0 | 2026-08-31 | 2026-08-31 | WeChat-style mobile skin for the DeepSeek Harness Web GUI: mobile browsers get a WeChat chat list and chat page, desktop stays untouched. |
| 2513 | [xfqz86/dsh-usage-stats](https://github.com/xfqz86/dsh-usage-stats) | 0 | 2026-08-23 | 2026-08-27 | DSH Web 插件：侧边栏中的 Token 使用统计 |
| 2514 | [xhqm-xyz/mira_live2d](https://github.com/xhqm-xyz/mira_live2d) | 0 | 2026-08-22 | 2026-08-23 | DSH Live2D 看板娘插件：会话界面浮层（拖拽/滚轮缩放/右键表情菜单）+ 模型可说话（OpenAI/阿里 TTS）+ MCP 工具（状态/切模型/表情动画开关/思考等待表情） |
| 2515 | [XianmingLF/xmlf-plugin-manager](https://github.com/XianmingLF/xmlf-plugin-manager) | 0 | 2026-08-21 | 2026-08-28 | 管理当前第三方已安装插件的信息 比较简单的版本 可按照自己的需求修改 |
| 2516 | [xiaobaiyg09/dsh-pickdom](https://github.com/xiaobaiyg09/dsh-pickdom) | 0 | 2026-08-23 | 2026-08-23 | PickDOM - 在 DSH 中框选本地 HTML 与 Web 页面元素，并将结构化引用交给 Agent |
| 2517 | [xiaokaizhou/dsh-media-preview](https://github.com/xiaokaizhou/dsh-media-preview) | 0 | 2026-08-30 | 2026-08-31 | DSH 插件：在聊天记录中自动将本地音视频路径渲染为可播放的预览组件 |
| 2518 | [XIAOke8698/dsh-lego-plugin](https://github.com/XIAOke8698/dsh-lego-plugin) | 0 | 2026-08-23 | 2026-08-24 | DeepSeek Harness（DSH）Web 界面插件的乐高式可视化视图 |
| 2519 | [xiaoso456/dsh-tool-plus](https://github.com/xiaoso456/dsh-tool-plus) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness 基础工具增强：持久 bash、结构化 read、多模式 edit、原子 write、双引擎 grep/glob、图像直读，一个插件全覆盖 |
| 2520 | [XiaoWind/dsh-btw](https://github.com/XiaoWind/dsh-btw) | 0 | 2026-08-26 | 2026-08-26 | DeepSeek Harness plugin: a /btw slash command to add notes without interrupting the agent |
| 2521 | [XiaoWind/dsh-vault](https://github.com/XiaoWind/dsh-vault) | 0 | 2026-08-26 | 2026-08-26 | DeepSeek Harness plugin: portable workspace vault for DSH conversations and logs |
| 2522 | [XiaoWind/dsh-weneedfirst](https://github.com/XiaoWind/dsh-weneedfirst) | 0 | 2026-08-21 | 2026-08-22 | DeepSeek Harness plugin: make the chain of thought open with We need instead of Let me |
| 2523 | [xiaoxiao44443/dfy-dsh-plugins](https://github.com/xiaoxiao44443/dfy-dsh-plugins) | 0 | 2026-08-17 | 2026-08-28 | Personal plugins for DeepSeek Harness |
| 2524 | [xiaoxingyuemiao/dsh-bg-plugin](https://github.com/xiaoxingyuemiao/dsh-bg-plugin) | 0 | 2026-08-27 | 2026-08-27 | DSH 自定义背景插件：为 DSH Web GUI 应用远程/本地图片背景，支持清晰度、压暗、模糊调节，设置面板保持默认外观。 |
| 2525 | [xiaoyaoPanPan/dsh-media](https://github.com/xiaoyaoPanPan/dsh-media) | 0 | 2026-08-24 | 2026-08-24 | DeepSeek Harness (dsh) 插件：把挂载目录变成可检索的媒体库 - 视频/图片自动打标、语义检索、系统打开与资源管理器定位 |
| 2526 | [xiaozhiaixue/dsh-model-toggle](https://github.com/xiaozhiaixue/dsh-model-toggle) | 0 | 2026-08-15 | 2026-08-22 | 在DSH中一键切换Flash/Pro，都是MAX |
| 2527 | [xiaozhiaixue/dsh-session-id](https://github.com/xiaozhiaixue/dsh-session-id) | 0 | 2026-08-17 | 2026-08-22 | 在DSH会话区底部显示会话ID，点击一下就能复制 |
| 2528 | [XingPeng-Pixel/dsh-commandcode-usage](https://github.com/XingPeng-Pixel/dsh-commandcode-usage) | 0 | 2026-08-24 | 2026-08-25 | DSH插件：实时监测Command Code用量，侧边栏挂件+仪表盘迷你挂件显示 |
| 2529 | [xinvxueyuan/cordis-plugin-github](https://github.com/xinvxueyuan/cordis-plugin-github) | 0 | 2026-08-17 | 2026-08-23 | Cordis / DeepSeek Harness plugin — normalized GitHub API tools for AI agents (gh CLI by default, native HTTP fallback) |
| 2530 | [xiong18166089606-design/dsh-trade-assistant](https://github.com/xiong18166089606-design/dsh-trade-assistant) | 0 | 2026-08-24 | 2026-08-24 | 外贸询盘回复与多语言产品文案工具（DeepSeek Harness 插件）- 询盘解析、回复结构、本地化文案，零模型依赖 |
| 2531 | [xiuyuan18/dsh-auto-approve](https://github.com/xiuyuan18/dsh-auto-approve) | 0 | 2026-08-25 | 2026-08-25 | Unofficial community plugin: automatic review of sandbox escalation requests for DeepSeek Harness (Codex Guardian-style) plus an /approve slash command |
| 2532 | [xiyi123465/dsh-usage-calendar](https://github.com/xiyi123465/dsh-usage-calendar) | 0 | 2026-08-25 | 2026-08-26 | DeepSeekAPI余额查询插件 |
| 2533 | [xlin20021/dsh-mcp-hub](https://github.com/xlin20021/dsh-mcp-hub) | 0 | 2026-08-29 | 2026-08-29 | dsh-mcp-hub |
| 2534 | [xlin20021/dsh-stock-chart](https://github.com/xlin20021/dsh-stock-chart) | 0 | 2026-08-29 | 2026-08-29 | dsh-stock-chart |
| 2535 | [xobexo/dsh-smart-scenario-router](https://github.com/xobexo/dsh-smart-scenario-router) | 0 | 2026-08-27 | 2026-08-27 | 国产模型优先，按任务类型自动切换模型，支持可视化配置面板 |
| 2536 | [xswt442-cmd/dsh-treekeeper](https://github.com/xswt442-cmd/dsh-treekeeper) | 0 | 2026-08-27 | 2026-08-27 | 对账 DSH 任务账本与 OS 进程树，定位归属、检测泄漏并安全治理｜Reconcile DSH task ledgers with OS process trees for attribution, leak detection, and safe governance. |
| 2537 | [xuqingsakura/dsh-subagent-team](https://github.com/xuqingsakura/dsh-subagent-team) | 0 | 2026-08-22 | 2026-08-22 | 一个官方 bundle 形态的独立插件，可经 GitHub / npm 安装到 DSH（桌面端与 web 端皆可）。 提供模型可见的角色工具（team_read / team_write / team_code_write / team_code_review …）， 以及一套真正的事件驱动团队运行时（建队 / 成员 / 任务依赖 / 邮箱 / 自动调度 / 右下角活动浮层）。 |
| 2538 | [xusuyang030218/dsh-preview-ui](https://github.com/xusuyang030218/dsh-preview-ui) | 0 | 2026-08-24 | 2026-08-24 | DSH (DeepSeek Harness) file preview & editor plugin: in-browser workspace file tree, multi-format preview, online editing, version history, search. DSH 文件预览插件。 |
| 2539 | [xuviga/dsh-plugin-mnemosyne](https://github.com/xuviga/dsh-plugin-mnemosyne) | 0 | 2026-08-25 | 2026-08-26 | Mnemosyne - an error-memory plugin for DeepSeek Harness that learns from the agent's own mistakes and blocks recurring ones |
| 2540 | [xyingsoft/dsh-chat](https://github.com/xyingsoft/dsh-chat) | 0 | 2026-08-29 | 2026-08-29 | dsh-chat 设计文档：面向自建团队、受管团队与企业组织的 DSH Web 协作平台 |
| 2541 | [Xylocarpro/dsh-plugin-recycle-bin](https://github.com/Xylocarpro/dsh-plugin-recycle-bin) | 0 | 2026-08-29 | 2026-08-30 | 强制 DSH 删除走回收站、禁用 del/rm/Remove-Item，回收站或硬盘满时停手询问用户。 |
| 2542 | [xyzs996/dsh-switch-cost](https://github.com/xyzs996/dsh-switch-cost) | 0 | 2026-08-24 | 2026-08-25 | DeepSeek Harness (dsh) plugin to compare LLM API cost across models and providers: prices the current session on the model that ran it, then reprices the same token counts against 15 routes on file. DeepSeek peak/off-peak resolved per UTC hour, cache read and write priced separately, every rate with its source and check date. |
| 2543 | [y2zyyr/dsh-restart-control](https://github.com/y2zyyr/dsh-restart-control) | 0 | 2026-08-18 | 2026-08-23 | @y2zyyr/dsh-restart-button — one-click Restart DSH button in Settings → General (DSH Desktop), using the official desktopRuntime.requestRestart() facade. |
| 2544 | [Ya-MiC/hermes](https://github.com/Ya-MiC/hermes) | 0 | 2026-08-23 | 2026-08-23 | Ya-MiC GitHub 全景索引 / Curated index of Ya-MiC's repos & stars — DeepSeek Harness (DSH) compliant, multilingual, multi-branch |
| 2545 | [Ya-MiC/zhanzhen](https://github.com/Ya-MiC/zhanzhen) | 0 | 2026-08-24 | 2026-08-26 | 湛箴 — 中小企业审计风险平台 v1 框架（FastAPI + Vue3，规则引擎本地运行，证据哈希链） |
| 2546 | [yajiangandchenchen/dsh-sandbox-permissions-not-strictly-wider-justification-empty-fix](https://github.com/yajiangandchenchen/dsh-sandbox-permissions-not-strictly-wider-justification-empty-fix) | 0 | 2026-08-27 | 2026-08-27 | 修复 sandbox_permissions 和 justification 字段在 pwsh/bash/fs/dsh-sandbox 中的 no-op 升级报错。当会话已是 danger-full-access 模式时，模型携带空 justification 或重申同一模式被拒的问题。 |
| 2547 | [yangbobo2021/relay-dsh-plugin-files](https://github.com/yangbobo2021/relay-dsh-plugin-files) | 0 | 2026-08-24 | 2026-08-26 | Workspace file explorer side-view plugin for DeepSeek Harness Workbench. |
| 2548 | [yangbobo2021/relay-dsh-plugin-terminal](https://github.com/yangbobo2021/relay-dsh-plugin-terminal) | 0 | 2026-08-24 | 2026-08-26 | Provider-neutral interactive terminal bottom-view plugin for DeepSeek Harness Workbench. |
| 2549 | [yangbobo2021/relay-dsh-plugin-workbench](https://github.com/yangbobo2021/relay-dsh-plugin-workbench) | 0 | 2026-08-24 | 2026-08-26 | Extensible Workbench shell plugin for DeepSeek Harness with public side and bottom view contracts. |
| 2550 | [yangdongzhen590/dsh-knj-extension-center](https://github.com/yangdongzhen590/dsh-knj-extension-center) | 0 | 2026-08-31 | 2026-08-31 | DSH ????:????????? zip ?????/??/?????????DSH skill center: browse by region, install from zip, manage enable/disable, uninstall, trash restore, search. |
| 2551 | [yangdongzhen590/dsh-knj-obsidian](https://github.com/yangdongzhen590/dsh-knj-obsidian) | 0 | 2026-08-28 | 2026-08-28 | DSH ??? Obsidian:AI agent ?????????????UI ?????(v1-v7) |
| 2552 | [yangdongzhen590/dsh-knj-prompts](https://github.com/yangdongzhen590/dsh-knj-prompts) | 0 | 2026-08-31 | 2026-08-31 | DSH ???????:????? ? ????????????(?? {??}),???????Prompt-scenario picker for DeepSeek Harness. |
| 2553 | [yangdongzhen590/dsh-knj-session-management](https://github.com/yangdongzhen590/dsh-knj-session-management) | 0 | 2026-08-31 | 2026-08-31 | Session management for DeepSeek Harness: archive/restore/delete persisted sessions, per-workspace retention policy and a size governance panel. DSH ??????:??/??/???????,????????????,????????? |
| 2554 | [yangkunlun/dsh-fairy](https://github.com/yangkunlun/dsh-fairy) | 0 | 2026-08-22 | 2026-08-22 | DeepSeek Harness 的多窗插件 |
| 2555 | [yangzhe1991/dsh-futu-mcp](https://github.com/yangzhe1991/dsh-futu-mcp) | 0 | 2026-08-31 | 2026-08-31 | DSH plugin: connect to Futu (富途) MCP via OAuth 2.1 with deferred authorization; tokens stored securely outside the workspace (~/.dsh, 0600) |
| 2556 | [yangzhe1991/dsh-project-session-store](https://github.com/yangzhe1991/dsh-project-session-store) | 0 | 2026-08-29 | 2026-08-29 | DSH plugin: store each project's session logs inside the project directory (.dsh/sessions/) \| DSH 插件:把每个项目的会话日志保存在项目目录(.dsh/sessions/)下,不再集中到 ~/.dsh/sessions |
| 2557 | [yankihue/deepseek-harness-voice-mode](https://github.com/yankihue/deepseek-harness-voice-mode) | 0 | 2026-08-23 | 2026-08-25 | Voice mode for DeepSeek Harness: live captions, push-to-talk, spoken agent replies, barge-in, and real thread control via ElevenLabs. |
| 2558 | [yanqd0/dsh-covtrim](https://github.com/yanqd0/dsh-covtrim) | 0 | 2026-08-29 | 2026-08-29 | DSH plugin: one-shot test coverage flow — run tests with coverage, compress with covtrim, return compact TSV to the agent |
| 2559 | [yanqd0/dsh-mint](https://github.com/yanqd0/dsh-mint) | 0 | 2026-08-29 | 2026-08-29 | DSH plugin: mint issue tracking integration — session context injection, event reminders, plan binding, mint_query tool, and a session tab |
| 2560 | [yaodongH/dsh-doc-review](https://github.com/yaodongH/dsh-doc-review) | 0 | 2026-08-23 | 2026-08-23 | dsh-doc-review — DeepSeek Harness Web 文档审阅弹窗插件：设计文档与方案审阅以全幅渲染 Markdown 弹窗呈现 (Design documents & plan reviews in a full rendered-Markdown modal) |
| 2561 | [yaodongH/dsh-vscode-bridge](https://github.com/yaodongH/dsh-vscode-bridge) | 0 | 2026-08-30 | 2026-08-30 | DSH web 插件：在 DeepSeek Harness 中心区嵌入固定版本 code-server（VS Code Web），跟随当前工作空间，支持自定义端口/路径与热切换。 |
| 2562 | [yaotongsb/dsh-phosphor](https://github.com/yaotongsb/dsh-phosphor) | 0 | 2026-08-29 | 2026-08-29 | A full-screen, Matrix-styled TUI frontend for DeepSeek Harness — built with React + Ink as a Cordis bundle plugin |
| 2563 | [Yaya716/dsh-add-image-button](https://github.com/Yaya716/dsh-add-image-button) | 0 | 2026-08-23 | 2026-08-23 | Persistent "Add image" button in the composer tool row for DeepSeek Harness Web: opens the system file picker (image/*, multi-select) and routes selected images through the official draft attachment pipeline. |
| 2564 | [Yaya716/dsh-msg-nav-track](https://github.com/Yaya716/dsh-msg-nav-track) | 0 | 2026-08-25 | 2026-08-25 | Conversation message navigation rail for DeepSeek Harness Web: a track on the right side of the session scroll area with ▲/▼ endpoints and evenly spaced dots for user messages; click a dot to jump exactly to that message. |
| 2565 | [ydlstartx/dsh-pdf-reader](https://github.com/ydlstartx/dsh-pdf-reader) | 0 | 2026-08-22 | 2026-08-23 | AI-powered PDF reader for DeepSeek Harness with annotations, multi-PDF workflows, mixed image-text evidence, and on-demand OCR. |
| 2566 | [yhPrime/dsh-github-installer](https://github.com/yhPrime/dsh-github-installer) | 0 | 2026-08-29 | 2026-08-29 | GitHub 仓库一键安装插件：粘贴任意 GitHub 插件仓库网址即可安装（标准 dsh plugin add github:… 协议，同 dsh-market）。Install any DeepSeek Harness plugin from a GitHub repo URL. |
| 2567 | [Yicijiuhaobala/dsh-session-delete](https://github.com/Yicijiuhaobala/dsh-session-delete) | 0 | 2026-08-24 | 2026-08-24 | Adds a "Delete session" item to the DSH session-row context menu (next to rename/fork/archive) — permanently removes session logs from disk, with live-session protection. |
| 2568 | [Yidien/dsh-host-router](https://github.com/Yidien/dsh-host-router) | 0 | 2026-08-29 | 2026-08-29 | dsh 外挂式网络路由插件:按域名勾选走本地代理(Clash 等),其余直连;内置嗅探,设置页勾选即生效。 |
| 2569 | [Yiklek/dsh-settings-manager](https://github.com/Yiklek/dsh-settings-manager) | 0 | 2026-08-23 | 2026-08-24 | DSH web plugin: manage how plugin sections appear in the global Settings dialog — show/hide, reorder, rename, and make the settings navigation scrollable — without touching upstream. |
| 2570 | [ylxmf2005/dsh-scheduled](https://github.com/ylxmf2005/dsh-scheduled) | 0 | 2026-08-23 | 2026-08-23 | Durable heartbeat and cron automations for DeepSeek Harness |
| 2571 | [yogeek/dsh-plugin-toggle](https://github.com/yogeek/dsh-plugin-toggle) | 0 | 2026-08-25 | 2026-08-26 | Enable/disable DeepSeek Harness (dsh) plugins from Settings > Plugins, grouped into collapsible categories |
| 2572 | [yonglun/deepseek-harness-themes](https://github.com/yonglun/deepseek-harness-themes) | 0 | 2026-08-27 | 2026-08-28 | 74 non-invasive DeepSeek Harness themes generated from awesome-design-md |
| 2573 | [yongshuai0314/dsh-turnsnap](https://github.com/yongshuai0314/dsh-turnsnap) | 0 | 2026-08-27 | 2026-08-27 | Zero-config per-turn git checkpoints for DeepSeek Harness: every completed agent turn in a git workspace becomes one tagged [turnsnap] commit |
| 2574 | [yoshino-xiao7/dsh-codex](https://github.com/yoshino-xiao7/dsh-codex) | 0 | 2026-08-28 | 2026-08-29 | 社区维护的 DeepSeek Harness Codex 插件：OAuth、模型、图片与流式恢复；非官方 / Community Codex plugin for DSH: OAuth, models, images, stream recovery; unofficial. |
| 2575 | [youridol/dsh-plugin](https://github.com/youridol/dsh-plugin) | 0 | 2026-08-27 | 2026-08-27 | DeepSeek Harness 插件收录总库：收录遵循 Cordis 框架、经官方 profile 机制挂载的 DSH 插件。收录插件自动同步上游，自研插件可手动维护。 |
| 2576 | [YpipaQ/dsh-whale-usage](https://github.com/YpipaQ/dsh-whale-usage) | 0 | 2026-08-23 | 2026-08-23 | dsh-whale-usage: a self-contained DeepSeek Harness (DSH) plugin that bridges the whale-widget and usage-stats plugins (balance widget + accounting/real-time-token/app-usage settings). Personal localization bridge, MIT. |
| 2577 | [yth1120/dsh-web-workbench](https://github.com/yth1120/dsh-web-workbench) | 0 | 2026-08-23 | 2026-08-23 | Public mirror for the dsh-external/dsh-web-workbench plugin suite; canonical organization repository is private by org policy. |
| 2578 | [Yu-Zhuang1/dsh-workspace-snapshot-fork](https://github.com/Yu-Zhuang1/dsh-workspace-snapshot-fork) | 0 | 2026-08-31 | 2026-08-31 | Fork DeepSeek Harness sessions together with their historical workspace state. |
| 2579 | [YUANMINGXUE/dsh-search](https://github.com/YUANMINGXUE/dsh-search) | 0 | 2026-08-26 | 2026-08-26 | Local-browser web search & page fetch plugin for DeepSeek Harness (dsh): browser_search / browser_fetch over Chrome DevTools Protocol, no API key. |
| 2580 | [YuemingHub/Ming-Capability-Pack](https://github.com/YuemingHub/Ming-Capability-Pack) | 0 | 2026-08-21 | 2026-08-22 | 依托于deepseek harness  做真有用的插件 |
| 2581 | [YUEYUEXYS/dsh-think-ultra](https://github.com/YUEYUEXYS/dsh-think-ultra) | 0 | 2026-08-30 | 2026-08-30 | Reasoning layer for the official DeepSeek Harness: every request stays on native max effort, with isolated Flash/Vision/Pro depth controls, stability axes and reasoning toolboxes built above it. Delivered build only; commercial use open, reverse/modify/extract closed. |
| 2582 | [yul761/dsh-blackjack](https://github.com/yul761/dsh-blackjack) | 0 | 2026-08-20 | 2026-08-25 | Third-party community perk game: play blackjack inside dsh and win model credit spendable only through this plugin. Not affiliated with any model vendor. \| 社区第三方福利小游戏：在 dsh 里玩 21 点，赢取仅限本插件内消费的模型额度。与任何模型厂商无关。 |
| 2583 | [yummy4727/dsh-context-branch](https://github.com/yummy4727/dsh-context-branch) | 0 | 2026-08-21 | 2026-08-22 | Context-branching conversation tree plugin for DeepSeek Harness. Avoid cold-start waste and show full tool/reasoning steps. |
| 2584 | [yunxiiQwQ/drool-whale-pet-for-dsh](https://github.com/yunxiiQwQ/drool-whale-pet-for-dsh) | 0 | 2026-08-27 | 2026-08-27 | 适用于dsh的pet插件 |
| 2585 | [yunxiyang/dsh-web-search-litellm](https://github.com/yunxiyang/dsh-web-search-litellm) | 0 | 2026-08-31 | 2026-08-31 | Web search provider for the DeepSeek Harness ctx.web seam via the LiteLLM proxy OpenAI Responses API (DeepSeek native server-side web_search) |
| 2586 | [Yurzi/dsh-web-fetch-enhanced](https://github.com/Yurzi/dsh-web-fetch-enhanced) | 0 | 2026-08-28 | 2026-08-28 | Configurable non-public address allowlists for DeepSeek Harness web_fetch |
| 2587 | [Yurzi/dsh-web-search-enhanced](https://github.com/Yurzi/dsh-web-search-enhanced) | 0 | 2026-08-29 | 2026-08-29 | Multi-protocol web_search provider for DeepSeek Harness |
| 2588 | [yustillrain/dsh-plugin-tool-repository](https://github.com/yustillrain/dsh-plugin-tool-repository) | 0 | 2026-08-26 | 2026-08-26 | DSH 插件仓库 第三方插件 让你可视化管理已安装的 skill/插件 对skill/插件功能进行介绍和分类  |
| 2589 | [Yuuz12/dsh-tavily](https://github.com/Yuuz12/dsh-tavily) | 0 | 2026-08-30 | 2026-08-31 | Tavily-backed web search provider plugin for DeepSeek Harness (DSH) — multi-key balance-aware rotation with failover, manageable from the DSH web settings. |
| 2590 | [YuYangOUC/dsh-power-button](https://github.com/YuYangOUC/dsh-power-button) | 0 | 2026-08-24 | 2026-08-24 | Self-contained power control for DeepSeek Harness: sidebar power button, restart/shutdown engine. |
| 2591 | [yx-yinhe/dsh-message-navigator](https://github.com/yx-yinhe/dsh-message-navigator) | 0 | 2026-08-27 | 2026-08-27 | ChatGPT-style message navigator for DeepSeek Harness conversations with hover previews and smooth jump navigation. |
| 2592 | [yybukn/dsh-table-attach](https://github.com/yybukn/dsh-table-attach) | 0 | 2026-08-31 | 2026-08-31 | 在dph中可以直接拖动.xlsx和.csv的表格文件到输入框中 |
| 2593 | [YYfather/dsh-balance](https://github.com/YYfather/dsh-balance) | 0 | 2026-08-23 | 2026-08-24 | DeepSeek Harness 余额与开销插件：状态栏显示 DeepSeek/MiMo 余额与逐请求计费开销（本会话/本次活跃/最近一次/上次对话），支持多模型+峰谷定价与花费超线提醒 |
| 2594 | [YYfather/dsh-mimo-plugin](https://github.com/YYfather/dsh-mimo-plugin) | 0 | 2026-08-23 | 2026-08-24 | MiMo (Xiaomi) tools as a standard DeepSeek Harness Cordis dynamic plugin: web search, image/audio/video understanding, ASR transcription, TTS, voice design and voice cloning, with a first-use API key setup card and Settings page. |
| 2595 | [YYfather/dsh-token-vault](https://github.com/YYfather/dsh-token-vault) | 0 | 2026-08-23 | 2026-08-24 | Secure credential vault for DeepSeek Harness: tokens never leave the host — the agent runs gh/npm/npx/node/git with the token injected in the environment. Manage from 设置 → 凭证库 / 市场 → 已安装. |
| 2596 | [Yyyyyylor/dsh-asuka-school-theme](https://github.com/Yyyyyylor/dsh-asuka-school-theme) | 0 | 2026-08-25 | 2026-08-27 | Theme-Asuka — An unofficial Asuka-inspired theme plugin for DeepSeek Harness Web UI, featuring time-of-day wallpapers, adaptive palette transitions, and restrained EVA-02 visual details. |
| 2597 | [YZDame/dsh-suhuang-scroll](https://github.com/YZDame/dsh-suhuang-scroll) | 0 | 2026-08-25 | 2026-08-25 | DSH Web plugin for Suhuang Scroll grading controls in Better Sidebar |
| 2598 | [yzhangjy/dsh-path-anonymizer](https://github.com/yzhangjy/dsh-path-anonymizer) | 0 | 2026-08-23 | 2026-08-24 | DSH plugin: anonymize workspace-external file paths before model requests, with user confirmation |
| 2599 | [yzhangjy/dsh-pattern-search](https://github.com/yzhangjy/dsh-pattern-search) | 0 | 2026-08-23 | 2026-08-24 | DSH plugin: regex pattern search over the current conversation — /pattern-search window + pattern_search tool to observe model output behavior |
| 2600 | [z7ping/narratica](https://github.com/z7ping/narratica) | 0 | 2026-08-28 | 2026-08-28 | AI 原生故事创作与媒体生产工作区｜AI-native storytelling workspace for novels, screenplays, and media production. |
| 2601 | [zaalipro/dsh-workflows](https://github.com/zaalipro/dsh-workflows) | 0 | 2026-08-20 | 2026-08-23 | DeepSeek workflows exactly like grok build CLI. Adds /create-workflow and /workflows slash commands to DeepSeek harness |
| 2602 | [zbc0315/dsh-synomega](https://github.com/zbc0315/dsh-synomega) | 0 | 2026-08-25 | 2026-08-25 | Organic reaction prediction for DeepSeek Harness: retrosynthesis, forward prediction, route planning, SynScore, and multi-component evolution — with in-chat molecule, reaction, and route-tree visualisation. Runs entirely locally. |
| 2603 | [zdjmrq/dsh-chat-mode](https://github.com/zdjmrq/dsh-chat-mode) | 0 | 2026-08-26 | 2026-08-26 | DSH 插件：为 DeepSeek Harness 增加「对话」纯聊天模式（ChatGPT 式）——侧边栏新会话模式切换（DSH/对话）、对话会话仅提问+搜索工具、专属 \/chat 聊天工作区 |
| 2604 | [zengfr/AutoCoding](https://github.com/zengfr/AutoCoding) | 0 | 2026-08-21 | 2026-08-22 | AutoCoding UltraVibe — 无人值守自动化编程工程化 |
| 2605 | [zengweicheng666/dsh-svn-tools](https://github.com/zengweicheng666/dsh-svn-tools) | 0 | 2026-08-29 | 2026-08-29 | SVN (Subversion) tools + sidebar UI for DeepSeek Harness: 33 agent tools with UTF-8 Chinese commit logs, plus an SVN panel in dsh-better-sidebar. |
| 2606 | [zenvertao/dsh-inline-comments](https://github.com/zenvertao/dsh-inline-comments) | 0 | 2026-08-26 | 2026-08-26 | 选中即批注，刷新亦留存 —— DSH 行内批注插件 |
| 2607 | [zeros335882878/dsh-paper-survey](https://github.com/zeros335882878/dsh-paper-survey) | 0 | 2026-08-25 | 2026-08-25 | Literature survey agent for DeepSeek Harness (dsh): interpret-first workflow, 3 skills (paper-survey / paper-interpret / paper-deck), zero-dependency. 文献综述 Agent：解读先行 → 用户确认 → A/B 两页结构生成综述 PPT。 |
| 2608 | [zeroUsr0721/dsh-web-polysearch](https://github.com/zeroUsr0721/dsh-web-polysearch) | 0 | 2026-08-25 | 2026-08-26 | Multi-source web search tool for DeepSeek Harness — queries DeepSeek / DuckDuckGo / Exa / Google / Bing in parallel, merges results, fetches page content. Part of the [dsh-plugin](https://github.com/topics/dsh-plugin) ecosystem. |
| 2609 | [Zessi-C/biofigure-self-evolve](https://github.com/Zessi-C/biofigure-self-evolve) | 0 | 2026-08-29 | 2026-08-30 | Self-evolving bioinformatics figure library skill: learn plots from papers/PDFs/WeChat articles/screenshots into reusable recipes (R/Python), imitate them when plotting. 自进化的生信 figure 学习库与复用引擎 |
| 2610 | [zhang-jiazhi/dsh-prompt-optimizer](https://github.com/zhang-jiazhi/dsh-prompt-optimizer) | 0 | 2026-08-30 | 2026-08-30 | 将原作者 linshenkx 的 prompt-optimizer 移植到 DeepSeek Harness 的第三方插件（非官方） |
| 2611 | [zhangguiping-xydt/dsh-possibility-space](https://github.com/zhangguiping-xydt/dsh-possibility-space) | 0 | 2026-08-31 | 2026-08-31 | Explore AI outputs as a steerable semantic possibility space for DeepSeek Harness. |
| 2612 | [zhangguiping-xydt/dsh-session-lab](https://github.com/zhangguiping-xydt/dsh-session-lab) | 0 | 2026-08-28 | 2026-08-28 | DeepSeek Harness session teaching, evidence capsules, and controlled trajectory comparison |
| 2613 | [zhangkkkai/dsh-getman-panel](https://github.com/zhangkkkai/dsh-getman-panel) | 0 | 2026-08-28 | 2026-08-31 | API 测试侧边栏面板（Getman），作为 dsh-better-sidebar 的配套插件：  请求编辑：方法（GET/POST/PUT/PATCH/DELETE/HEAD/OPTIONS）+ URL + Params / Headers / Body 响应查看：状态码徽章、耗时、大小、响应体（JSON 自动美化，右上角可一键复制）/ 响应头 历史记录：全局共享最近 100 条请求（所有工作空间共用），点击回填、单项删除、一键清空 绕过 CORS：通过 host 半代理转发，任意 HTTP(S) 接口都能测试 |
| 2614 | [zhangkkkai/dsh-spec-panel](https://github.com/zhangkkkai/dsh-spec-panel) | 0 | 2026-08-28 | 2026-08-28 | 一个基于 dsh-better-sidebar 的 SDD（规范驱动开发，Spec-Driven Development）配套插件：在侧边栏提供一个 Spec 工作台，围绕 OpenSpec 的标准目录结构，让「先写规范 → 再实现 → 再验证」的流程一目了然、可操作。 |
| 2615 | [zhangkkkai/dsh-todo-panel](https://github.com/zhangkkkai/dsh-todo-panel) | 0 | 2026-08-27 | 2026-08-28 | 一个基于 dsh-better-sidebar 的 TODO 任务清单侧边栏插件：卡片式布局、优先级颜色标记、中文界面、按会话持久化。 |
| 2616 | [zhangliang0115/ai-plugin](https://github.com/zhangliang0115/ai-plugin) | 0 | 2026-08-29 | 2026-08-29 | One command to install any AI agent skill/plugin into every agent — Claude Code, DeepSeek Harness (dsh), Codex, Gemini CLI, Copilot, Cursor. Zero-dependency CLI + cross-agent marketplace. |
| 2617 | [zhangzhenwen1/dsh-task-effort](https://github.com/zhangzhenwen1/dsh-task-effort) | 0 | 2026-08-30 | 2026-08-30 | Auto-adjust model reasoning effort per task with DeepSeek peak-pricing-period capping: off/low/high/max classification, [effort=...] markers, error escalation, countdown notices |
| 2618 | [zhaozixi/dsh-attention](https://github.com/zhaozixi/dsh-attention) | 0 | 2026-08-28 | 2026-08-30 | DSH 跑任务时你通常只能盯着进度条。dsh-attention 把这段等待变成有产出的碎片时间 |
| 2619 | [zhchxiao123/dsh-devflow-plugins](https://github.com/zhchxiao123/dsh-devflow-plugins) | 0 | 2026-08-26 | 2026-08-30 | File-backed development workflow for DeepSeek Harness: durable cards, artifact and agent checks, human approvals, and a read-only web board. |
| 2620 | [zhengjy01/dsh-cloudflare-mcp](https://github.com/zhengjy01/dsh-cloudflare-mcp) | 0 | 2026-08-31 | 2026-08-31 | Cloudflare MCP connection for DeepSeek Harness |
| 2621 | [zhengjy01/dsh-qqbot-panel](https://github.com/zhengjy01/dsh-qqbot-panel) | 0 | 2026-08-31 | 2026-08-31 | Visual web settings panel for the official @tencent-connect/dsh-qqbot plugin: manage AppID/AppSecret, c2c & group access/allowlists, workspace picker, and scan-to-bind from the DSH web settings page |
| 2622 | [zhengjy01/dsh-task-dispatcher](https://github.com/zhengjy01/dsh-task-dispatcher) | 0 | 2026-08-25 | 2026-08-26 | Task dispatcher for DeepSeek Harness: use TickTick (滴答清单) 5️⃣AI as daily task dispatcher (timer + auto-execute + flomo/macOS notify) |
| 2623 | [zhengjy01/dsh-vercel-mcp](https://github.com/zhengjy01/dsh-vercel-mcp) | 0 | 2026-08-30 | 2026-08-30 | Vercel MCP connection for DeepSeek Harness (DSH): official OAuth 2.0 flow (dynamic client registration + PKCE) against mcp.vercel.com, Vercel API tools under mcp__vercel__*, and a web settings panel |
| 2624 | [zhibailu/dsh-vsc](https://github.com/zhibailu/dsh-vsc) | 0 | 2026-08-23 | 2026-08-31 | Run DeepSeek Harness (DSH), a local AI agent, inside VS Code — native sidebar panel + editor bridge. A pure protocol client: no rewriting DSH, no second server |
| 2625 | [zhm20001/dsh-plugin-palette-board](https://github.com/zhm20001/dsh-plugin-palette-board) | 0 | 2026-08-31 | 2026-08-31 | 本项目为 DeepSeek Harness web 控制台带来一块 2D 调色盘应用板。唤出悬浮面板，即时搜索、分类过滤、全键盘导航，把散落在侧栏与浏览器里的插件页面收进一张可自定义的卡片网格。   |
| 2626 | [zhm20001/dsh-usage-board](https://github.com/zhm20001/dsh-usage-board) | 0 | 2026-08-27 | 2026-08-28 | dsh-usage-board 是专为 DSH (DeepSeek Harness) 设计的用量与成本可视化看板插件。  插件能实时捕获会话内的 Token 消耗、Step 耗时和异常指标，支持冷启动增量回溯历史全量会话，并按 Sub-agent DAG 调用关系进行树状归集与反向明细穿透。 |
| 2627 | [zhou1736948757-cpu/dsh-auto-continue](https://github.com/zhou1736948757-cpu/dsh-auto-continue) | 0 | 2026-08-25 | 2026-08-25 | Automatically resumes replies cut off at the output token limit — built for self-hosted Ollama users with small output caps. · 回答被输出上限截断时自动续写，面向自部署 Ollama 用户。 |
| 2628 | [zhoujianbin/dsh-codex-continue](https://github.com/zhoujianbin/dsh-codex-continue) | 0 | 2026-08-29 | 2026-08-30 | DSH 插件：读取本机 Codex 项目与会话，一键在 DSH 里继续。Read local OpenAI Codex sessions and continue them in DeepSeek Harness. |
| 2629 | [zhouStar7/dsh-kanban](https://github.com/zhouStar7/dsh-kanban) | 0 | 2026-08-25 | 2026-08-25 | AI-assisted local project task board for DeepSeek Harness (DSH) |
| 2630 | [zhubaodian1027/dsh-token-panel](https://github.com/zhubaodian1027/dsh-token-panel) | 0 | 2026-08-22 | 2026-08-22 | DSH Web GUI panel: AI quota (Kimi Coding, Codex Plus, DeepSeek…) + merged local token usage (DSH, Codex, Claude Code, Kimi Code, Hermes, Pi…). |
| 2631 | [zhubaohi/dsh-gpu-pulse](https://github.com/zhubaohi/dsh-gpu-pulse) | 0 | 2026-08-30 | 2026-08-30 | Floating GPU monitor (nvidia-smi) for the DSH Web UI — live per-GPU utilization, VRAM, temperature, power and fan, in the corner of the page. |
| 2632 | [zhulianxing/dsh-clawpay](https://github.com/zhulianxing/dsh-clawpay) | 0 | 2026-08-24 | 2026-08-24 | DeepSeek Harness (DSH) plugin |
| 2633 | [zhulianxing/dsh-kankan-mail](https://github.com/zhulianxing/dsh-kankan-mail) | 0 | 2026-08-24 | 2026-08-24 | DeepSeek Harness (DSH) plugin |
| 2634 | [zhulianxing/dsh-lookhere](https://github.com/zhulianxing/dsh-lookhere) | 0 | 2026-08-24 | 2026-08-24 | DeepSeek Harness (DSH) plugin |
| 2635 | [zhulianxing/dsh-starstack](https://github.com/zhulianxing/dsh-starstack) | 0 | 2026-08-24 | 2026-08-24 | DeepSeek Harness (DSH) plugin |
| 2636 | [ZhuoSir/dsh-chatops](https://github.com/ZhuoSir/dsh-chatops) | 0 | 2026-08-25 | 2026-08-25 | dsh-chatops 是 DeepSeek Harness 的 IM 桥接插件：微信扫码绑定官方 ClawBot 机器人（腾讯 iLink 协议），或接入飞书自建应用，即可在手机 IM 里列出/切换/驱动所有 DSH 会话——发文字就是发 prompt，任务完成自动推送结果，危险操作推送审批（飞书支持卡片按钮一键批准）。多通道并行、纯官方接口、零公网部署 |
| 2637 | [ZhuYanTech/dsh-biomni](https://github.com/ZhuYanTech/dsh-biomni) | 0 | 2026-08-15 | 2026-08-31 | DeepSeek Harness biomni plugin |
| 2638 | [ZiFan1117/bazidiy](https://github.com/ZiFan1117/bazidiy) | 0 | 2026-08-26 | 2026-08-26 | 基于 DeepSeek Harness 的八字五行手串定制插件 |
| 2639 | [zisen123/dsh-reasoning-ruler](https://github.com/zisen123/dsh-reasoning-ruler) | 0 | 2026-08-30 | 2026-08-30 | Minimal reasoning-effort ruler for the DSH web composer: hairline + sliding marker, per-model memory, optimistic switching, streamlined model picker |
| 2640 | [Zn-Dk/dsh-mnemon-gc](https://github.com/Zn-Dk/dsh-mnemon-gc) | 0 | 2026-08-22 | 2026-08-23 | 接入 dsh-mnemon GC 治理插件：冲突驱动的正确性纠错，自动巡检报告。 |
| 2641 | [Zn-Dk/dsh-plugin-creator](https://github.com/Zn-Dk/dsh-plugin-creator) | 0 | 2026-08-21 | 2026-08-25 | Agent skill: scaffold and iterate DSH (DeepSeek Harness) Web plugins. |
| 2642 | [ZomiCC/ghost-refresh](https://github.com/ZomiCC/ghost-refresh) | 0 | 2026-08-25 | 2026-08-25 | Ghost Refresh (鬼影提神) |
| 2643 | [zootguru/dsh-vpn-ops](https://github.com/zootguru/dsh-vpn-ops) | 0 | 2026-08-22 | 2026-08-22 | Safety-gated WireGuard and VLESS Reality operations for DeepSeek Harness |
| 2644 | [zouxiaoyang/dsh-commandcode-usage](https://github.com/zouxiaoyang/dsh-commandcode-usage) | 0 | 2026-08-31 | 2026-08-31 | CommandCode usage & balance panel for DeepSeek Harness / DSH 的 CommandCode 用量与余额面板 |
| 2645 | [zouyuanqing/dsh-verify-reflux](https://github.com/zouyuanqing/dsh-verify-reflux) | 0 | 2026-08-25 | 2026-08-25 | Three-plane probabilistic verifier for DeepSeek Harness: tiered logprob/sample/template judges, seeded tournament best-of-N, layered context reflux. |
| 2646 | [zpliao123/dsh-ark-quota](https://github.com/zpliao123/dsh-ark-quota) | 0 | 2026-08-27 | 2026-08-27 | Volcengine Ark Coding Plan / Agent Plan quota plugin for DeepSeek Harness (DSH) Web GUI: side float widget + settings page, persistent credentials, periodic auto-refresh, ark_coding_plan_usage model tool. |
| 2647 | [zptalk0221-cpu/dsh-remote-desktop](https://github.com/zptalk0221-cpu/dsh-remote-desktop) | 0 | 2026-08-26 | 2026-08-26 | 远程桌面移动化插件：为 DeepSeek Harness 提供手机横屏外壳与中文输入法 |
| 2648 | [zsagi1368/dsh-webstack](https://github.com/zsagi1368/dsh-webstack) | 0 | 2026-08-23 | 2026-08-24 | WebStack (网栈) — integrated web search & fetch kernel plugin for DeepSeek Harness (DSH). 免费池开箱即搜 · SSRF 四道闸 · 双语诊断 |
| 2649 | [zuojinxin/dsh-provider-switch](https://github.com/zuojinxin/dsh-provider-switch) | 0 | 2026-08-28 | 2026-08-28 | Provider on/off switches, model search, and inline provider renaming for DeepSeek Harness. |
| 2650 | [zxheyi/dsh-work](https://github.com/zxheyi/dsh-work) | 0 | 2026-08-27 | 2026-08-27 | A plugin-native AI desktop for real work, built on DeepSeek Harness. |
| 2651 | [Zzc269/dsh-soft-glass-ui](https://github.com/Zzc269/dsh-soft-glass-ui) | 0 | 2026-08-16 | 2026-08-22 | Unofficial soft-glass visual theme plugin for DeepSeek Harness. |
| 2652 | [zzhi191/dsh-plugin-night-dog](https://github.com/zzhi191/dsh-plugin-night-dog) | 0 | 2026-08-29 | 2026-08-29 | A tan DeepSeek mascot dog named 夜官 that lives in the corner of the DSH web GUI: floats, reacts to the harness, adapts to the theme, and acts out a full repertoire (pant, stand, walk, tilt, yawn, bark, spin, whimper, lie down to sleep). Pure client plugin, installable from the DSH Community Market. |

## 从快照消失的已核准仓库 / Approved repositories missing from the snapshot

已核准但已不在当前快照中（删除或改名），核实后从 [data/approved.json](../approved.json) 移除或更新名称。

Approved but no longer present in the current snapshot (deleted or renamed) — after checking, remove them from [data/approved.json](../approved.json) or update the name.

- 0Ra1n416/DSH-GUI
- 222wcnm/dsh-manager
- 3yi2u34yu32/dsh-balance-peak
- 911218sky/dsh-llm-bounded-retry
- 918154429/dsh-codex-import
- ABccgh/imakb
- ABccgh/ws-cleaner
- AI-Scarlett/dsh-safe-plugin-manager
- alfonsoferrertorres-cyber/saare-suite
- Arslan-jh/deepseek-harness-usage
- AwesomeHou/dsh-trajectory-collapse
- Badegg404/dsh-code-review
- Baisbt/dsh-api-balance
- bitterSmilezzz/dsh-model-fix
- BlackDawnNova/dsh-web-open
- blueWhalei/dsh-verify-gate
- CarlMarkswx/dsh-imagen
- cdxDNRF/wishadel-theme
- CharlesAQ/dsh-fgo-chaldea
- Cheerwhy/dsh-chat-anchors
- chendefine/dsh-cdp-live-view
- Chillizu/MiopIIk
- chinaRXQ/dsh-wallpaper
- cking000bigdemon/dsh-toolbelt
- coder-wu/dsh-finance-data
- coeasy/oh-my-dsh
- collapsey/xiaokui-pet
- crack-time/dsh-web-ui-skin
- dabaicai001/star-deepseek-harness-desktop
- daha1216/dsh-skill-adult-tension-narrative
- Daseanle/dsh-mcp-orchestrator
- Daseanle/dsh-obsidian-bridge
- Daseanle/dsh-teacher-preset
- ddtcorex/agent-dev-skills
- Deklan-Deng/Dcode
- dHR-P/dsh-anchored-wsl
- dolcejust-spec/dsh-event-watch
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
- fff122/dsh-agent-arcade
- fff122/dsh-prompt-presets
- fff122/dsh-research-notes
- fff122/dsh-task-checklist
- Foo1Moon/dsh-web-visualuiconfig
- Francis-Xavier-code/dsh-balance-plugin
- fryghost/deepseek-eyes
- g-yixuan/dsh-sidechat
- Gaq152/dsh-attention
- Gaq152/dsh-credits
- ggggggggggz/dsh-config
- GooDAnDReaDY/dsh-fal-image-gen
- gushiaoke/dsh-qq-bot
- harryopo/dsh-remote-ide
- hawkongz/doubao-vision-dsh
- he110Warudo/dsh-window
- Hed1an/dsh-bring-local-llm
- Howe829/dsh-runtime
- htq20080119/dsh-token-stats
- huaxiren6/dsh-email-reader
- huaxiren6/dsh-remote-qr-button
- huaxiren6/dsh-sms-webhook
- hyls9527/dsh-local-vision
- ihuajiu/dsh-code-security
- ihuajiu/dsh-plugins-finder
- iTrimut/dsh-remote-access
- jianxx/dsh-cc-plugins
- JIAQI23333/dsh-visual-plan
- JimchengChina/dsh-action-outbox
- JimchengChina/dsh-frontier-repro
- jiuge2467/DSH-WhaleDeck
- joshryandavis/dsh-llm-kiro
- JUSTMONIKA2022/dsh-sandbox-escalation-fix
- JxaMe/dsh-condense
- kaijia323/dsh-ymc-sidebar
- KannaKuron/dsh-deepseek-vision-bridge
- kedoupi/dsh-plugins
- kiligzzz/dsh-capability-manager
- KitDoesIt/dsh-compaction-instant
- krystal-cao/deepseek-harness-desktop
- lamost423/dsh-trace-compare
- LBurny/deepseek-harness-desktop
- lesliechowsh/dsh-memo
- lhf6623/dsh-vibe
- liguobao/deepseek-harness-remote
- liustack/aimanager
- liustack/pptfast
- lo2589/deepseek-harness-meida
- looput/dsn-finance-lab
- lovstudio/dsh-plugin-creator-skill
- lovstudio/dsh-plugin-publisher-skill
- LVSUGARS/dsh-web-manager
- lvyunqi/dsh-memory-enhanced
- LXW419/dsh-claude-importer
- mattismegevand/dsh-dock
- mattismegevand/dsh-git
- mattismegevand/dsh-open
- mattismegevand/dsh-terminal
- meliodascz89/deepseek-harness-plugins
- mianyoubiaoqing/MistyMoon-DSH
- morlay/session-persistence-rdb
- mrgaoang/dsh-remote
- mrlfarano/dsh-tailscale-surface
- mrpulor-gh/nuphus-mcp
- Mrzhailiming/deepseek-pet
- muvuula/DeepSeek-Harness-Core
- Nexus-Aethra/DSH-plugin-switch
- nnbw-liu/deepseek-ai-dsh-llm-local
- NSOiO/talon-ui
- omdsh-dev/fabric
- omdsh-dev/Qwen-MM-Plugins
- onlyforchris/dsh-plugin-manager
- openma-ai/deepseek-harness-typescript-sdk
- oThTJx/dsh-skill-always-apply
- oThTJx/dsh-skill-impeccable
- oThTJx/dsh-skill-karpathy-guidelines
- oThTJx/dsh-skill-ponytail
- oThTJx/dsh-skill-superpowers
- oThTJx/dsh-skill-taste
- pgmi-builds/dashr
- Physicolor/harness-ui-enhancer
- Physicolor/harness-widgets
- PolinniZhong/dsh-session-kb
- pppolf/dsh-webgate
- qingzhuo-cn/agent-fix
- QLM1234/dsh-dynamic-assembler
- qq1376868542-lang/dsh-tools
- rayafriandion/deepseek-harness-tui
- raydez/deepseek-harness-pet-plugin
- riesbri/dsh-tui
- ruisenbai/dsh-inline-comments
- sandbaseai/sandbase-skills
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
- sd1g1/dsh-minimal-rules
- sd1g1/dsh-subagent-model-override
- sd3247930/SkyDome
- seaskyblue/dsh-channel-feishu
- Semidia/dsh-friendly-errors
- sidleo/skill-scan
- sjh9714/clippy-harness
- sjh9714/dsh-lean
- sjh9714/dsh-what-changed
- songoao25/dsh-song-memory
- sparkmio/dsh-sfversion
- sqs404/dsh-gdi-art-plugins
- statem-li/dsh-better-markdown
- statem-li/dsh-browser
- statem-li/dsh-image-gallery
- statem-li/dsh-reasoning-effort
- statem-li/dsh-tool-summary
- statem-li/dsh-usage-skill
- statem-li/dsh-vision-helper
- statem-li/dsh-zh-thinking
- tianji-qingtian/dsh-spec-loop
- TiantianFlow/dsh-tailscale-gateway
- TimeCraker/dsh-claude-import
- trewvip-arch/dsh-open-in-app
- TuringCorp-net/mosaic_compress
- urzeye/dsh-outline
- vcxmug/dsh-enhance
- wezoo-wb/dsh-desktop-min
- wings1848/dsh-economizer
- worldwonderer/oh-story-dsh
- WSL043/dsh-native-session-delete
- WSYXIUBA/dsh-plugin-constellation
- xiaoliang2/dsh-compact-after-task
- xie-tj/deepseek-harness-latest-user-message-revision
- XSakura666/ChronoAgent
- y2zyyr/dsh-restart-button
- yamingmou/dsh-message-editor
- yhyfhgs/dsh-providers-extension
- yishengdaxiaonengjihui/dsh-plugin-manager
- youridol/dsh-sess
- Yvesgao/dsh-desktop-launcher
- zhaimingyou/aisync
- zhangyoufu-123/stylotrace
- zhongjie10086/dsh-adaptive-native-standard
- zhoupengjie/dsh-motion-manager
- zhouzhencheng07/dsh-free-search
- zhouzhencheng07/dsh-memory
- zhu1090093659/dsh-web-ui
