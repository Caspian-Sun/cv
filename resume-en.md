# Daotao Sun (Tom)

**Forward Deployed Engineer** · 10 yrs experience · Based in Hangzhou, China · Open to remote

📞 +86 132 8200 1310 · ✉️ 459269440@qq.com
🔗 GitHub: https://github.com/Caspian-Sun · LinkedIn: https://www.linkedin.com/in/caspian-sun-404b6140b

---

## Summary

10-year full-stack engineer and team lead who spent the last year building an **AI-driven R&D methodology** ([`claude-code-workflow`](https://github.com/Caspian-Sun/claude-code-workflow)) and applying it across three completely different stacks — React/UmiJS (web), Tauri + Rust (desktop), and Flutter (Android + iOS + HarmonyOS).

I specialize in turning generic AI capabilities (Claude, GPT, Gemini) into production-grade engineering workflows for specific verticals — exactly what a Forward Deployed Engineer does.

**Currently looking for** FDE / Applied AI Engineer / Solutions Engineer roles, ideally at AI infrastructure companies, AI-native startups, or consultancies deploying AI to real customers.

---

## Highlights

- **AI methodology**: Designed and shipped an 8-step SDLC framework with hard gates, traceability chain, and five-part collaboration architecture (commands / skills / subagents / hooks / rules). Open-sourced, bilingual (EN/ZH).
- **Cross-stack proven**: The same methodology survives unchanged across TypeScript-only (UmiJS), Rust + TS (Tauri), and Dart (Flutter) — three different stacks, three different platforms (Web / Desktop / Mobile), three different domains (admin / dev tools / Web3 wallet).
- **Production track record**: Cpcash Web3 wallet shipped **138 commits, 167 tasks closed at 100%, in 13 days**, on three mobile OSes (Android / iOS / HarmonyOS).
- **Frontend depth**: 8 years of low-code platform + design system experience, including a self-built low-code platform (ServerUI) and a refactor of Formily for visual form design at scale.
- **People leadership**: Led frontend teams of 20+ engineers (Pinming, Lanzhong), owned hiring, code review, perf reviews, technical roadmap.
- **Cross-discipline background**: BA in Fine Arts + minor in CS — strong design intuition, useful for AI-assisted design tooling work.

---

## Featured Projects

### claude-code-workflow — AI R&D Methodology Framework

> Breaks "Requirements → Design → Code → Test → Deploy" into traceable commands, skills, subagents, and rules. AI executes; humans gate every critical checkpoint.

**Why this is FDE work**: The whole project is a Forward Deployed engagement with my own team — taking a generic AI capability (Claude Code CLI) and turning it into a production workflow for a specific vertical (software R&D).

- **8-step SDLC pipeline** (`/prd → /plan → /code → /test → /review → /build → /deploy → /release`) with hard gates (`prd-check`, `plan-check`) that AI cannot silently skip
- **Traceability chain**: PRD anchor → task ID → source `@prd/@rules` → test `it()`. Change any link, scan downstream automatically.
- **Five-part architecture**: Commands (decisions) + Skills (scripts) + Subagents (parallel/isolated context) + Hooks (silent guards) + Rules (long-term constraints)
- **Cross-domain portable**: Same framework powers three different projects (frontend / desktop / mobile) without a single line of core code rewrite
- Open-source · MIT license · bilingual docs · full GitHub packaging

🔗 https://github.com/Caspian-Sun/claude-code-workflow

### Cpcash Wallet — Web3 Mobile Wallet (Flutter, 3 OSes)

> Crypto wallet shipping from a single Dart codebase to Android, iOS, and HarmonyOS. *(Private repo, walkthrough available on request.)*

- **138 commits in 13 days**, every commit tagged with a task ID (`T001-T043 — 43/43 = 100%`)
- **167 tasks closed at 100%** across 5 modules (account / assets / home / transfer / receive)
- **4 structured bug reports**, all closed-loop. Bug density ≈ 2.4% — low for Web3.
- **HarmonyOS-specific `MissingPluginException` resolved in-line** without forking a platform branch
- Business depth: BIP39 mnemonics, BIP44 derivation, EVM multi-chain transfer/receive, local key custody, multi-wallet
- Full methodology adherence report records all execution details + honest gaps

### Spider — Tauri Desktop Meta-Tool

> A desktop tool that visualizes any `claude-code-workflow` repo as a kanban — *a tool built with the methodology to render the methodology.*

A dogfooding + self-referential engineering case. Proves the framework is self-consumable.

- **Stack**: Tauri 2 + **Rust backend** (PTY/scan/watcher/IPC) + React frontend (15 feature modules)
- Visualizes `.claude/commands/` workflows as a DAG kanban — one lane per `/command`, one card per real PTY session
- Demonstrates the methodology's `@prd / @task / @rules` chain works identically across TS and Rust

🔗 https://github.com/Caspian-Sun/spider

---

## Experience

### Youzan / Zhiqing Information Tech | Frontend Engineer | Nov 2024 - Apr 2025

Worked on Youzan's foundational design system (UiDraft) and the UXtwo AI product, extending AI-driven design tooling on top of Figma's uiobject model.

- Led UiDraft design system development and maintenance; standardized cross-platform UI consistency
- Contributed to UXtwo AI features: smart recommendations and auto-generated UI flows
- Shipped **UIdraft Chrome extension** (React + TS) — DFS/DSF-based component hierarchy detection for complex cross-merge scenarios

### Zheshang Bank Treasury Project | Frontend Architect | Oct 2023 - Nov 2024
*(on-site, via Shenzhou Digital)*

- Authored frontend engineering standards; **PR review cycle: 3 days → 6 hours**
- Solved `qiankun` micro-frontend's `Proxy` polyfill issue for legacy browser support
- **Cut initial render from 5,000ms to 200ms (25x)** by analyzing the call/resource tree and pruning unused assets per business path
- Led the Tuotu low-code platform delivery; integrated S2 large-grid component
- Embedded React modules inside the legacy Vue codebase without rewrites
- Built an online component service center (inspired by ServerUI), letting users hot-load components

### Yichengyicun (Startup) | Engineering Manager | Feb 2023 - Aug 2023

End-to-end ownership: tech selection, team execution, process design, customer-facing delivery.

**Flagship product — Fenchao**: Loyalty-points app with active/passive QR-code payment, three platforms (WeChat MiniApp + Android + iOS).
- Frontend: uniapp / React Native / React / Canvas (later refactored to Flutter — custom widgets + container layout)
- Backend: Go (gin) + MySQL + MongoDB + Redis + Nginx
- Owned full-stack development, project planning, and on-the-ground customer rollout

### Pinming Technology | Full-Stack Engineer | Oct 2021 - Jan 2023

Led the frontend team; owned architecture, low-code platform, BI dashboards, micro-services frontend.

- **Yuanbi**: Forked and extended Formily into a visual drag-and-drop form designer; non-engineers can author forms independently
- **Xunjian (Inspection)**: Construction-industry daily inspection across web + mini-program + H5 (React/Antd/Umi + uniapp + Vue2/Vue3)
- **BI dashboards**: Core components for large-scale data visualization
- Optimized CDN distribution; resolved asset-loading issues in mainland China + Hong Kong
- Owned digital construction line: mini-program + H5 + App

### Hangzhou Lanzhong Data | Full-Stack Engineer → Frontend Lead | Aug 2018 - Oct 2021

Led the frontend team; focused on low-code, with parallel ownership of products, project delivery, and multi-platform apps.

- **ServerUI (low-code platform)** — *self-built, maintained since Nov 2020*
  - Data center with MVVM two-way binding; custom module loader `relation`
  - **Vue / React / Angular running on the same page** with compile-time + runtime sandbox isolation
  - Online "Fx" runtime, decompiling component lifecycle for hot extensibility (inspired by serverless)
  - `webServerModule` registry + `serverui_online_html` online composition + `serverUIcomment` seamless embedding
  - Design write-up: https://blog.csdn.net/u014080304/article/details/114393458
- **Shangpintong SaaS** (apparel & retail supply chain): qiankun + Vue2/Vue3/TS legacy/new coexistence; node-based micro-service frontend gateway
- **dataflow**: d3.js + dag.js visualization of warehouse script dependencies; fast render across hundreds of nodes
- **Internal tooling**: ci/cd scaffolds + internal-source install/uninstall tools (tricky: rollback module state on uninstall by diffing old vs new config snapshots)
- **Retail line**: Liufuya / Li-Ning / Peacebird / Yiming / Bee recruitment systems, including large-data Canvas-based tables and Echart re-wrappers

### iSoftStone | Frontend Engineer | Jul 2015 - Jul 2018

On-site at Alipay; frontend development, interaction implementation, performance optimization.

---

## Education

**Shangrao Normal University** · BA · Major: Fine Arts · Minor: Computer Science · 2011 - 2015

> Fine Arts → design sensibility → design-system engineering → AI + design tooling (UIdraft / Figma uiobject DSL). This trajectory is the differentiator for design-aware AI applied engineering.

---

## Writing / Output

- ServerUI low-code design notes — https://blog.csdn.net/u014080304/article/details/114393458
- `claude-code-workflow` methodology — bilingual docs at the GitHub repo
- *(In progress: a series on "Three counterintuitive design choices in shipping AI workflows")*
