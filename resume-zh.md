# 孙道涛 · 34 岁 · 杭州

**求职意向**:
- 主推 — **Forward Deployed Engineer / AI 应用工程师 / 解决方案工程师**
- 兼考虑 — 高级前端 / 前端架构师 / 全栈架构师

**期望薪资**: 35-60K · 杭州 (远程岗位可拓宽到一线)
**到岗时间**: 1 周内

📞 13282001310 · ✉️ 459269440@qq.com · 💬 微信 13282001310
🔗 GitHub: https://github.com/Caspian-Sun · LinkedIn: https://www.linkedin.com/in/caspian-sun-404b6140b

---

## 一句话定位

10 年技术 + 团队管理经验, 近 1 年深入 AI 工程化, **独立设计并落地了一套 AI 研发工作流方法论** ([claude-code-workflow](https://github.com/Caspian-Sun/claude-code-workflow)), 已在 **3 个完全不同的形态**上跑通生产级项目 —— 前端 (React/UmiJS) · 桌面 (Tauri + Rust) · 移动 (Flutter)。

擅长把通用 AI 能力封装成具体行业可用的工程方案 —— 这正是 FDE 岗位的核心能力。

---

## 核心能力 (Why me)

| 维度 | 具体内容 |
|------|---------|
| **AI 工程化** | 自研 8 步法 SDLC 框架, 含硬性闸门 + `@rules` 追溯链 + 5 件套协作机制 (commands / skills / subagents / hooks / rules); 熟悉 Claude / GPT / Gemini 的 prompt caching · tool use · agent workflow · MCP |
| **跨栈全栈** | TypeScript · Rust · Go · Python · Java · Node; 同一套方法论在 React / Tauri 双栈通用 |
| **架构与低代码** | 8 年低代码 / 设计系统经验 (ServerUI / Formily 二开 / 有赞 UiDraft); 解决过 Vue+React+Angular 同页沙箱、动态组件加载、qiankun 兼容性等深水区问题 |
| **团队管理** | 带过 20+ 人前端团队 (品茗 / 览众), 主导前端规范、CI/CD、code review、绩效评估 |
| **复合背景** | 美术学本科 + 副修计算机; 设计直觉强, 做过 Figma uiobject 反解 + DSL 编写 + Chrome 插件 (UIdraft) |
| **行业落地** | 金融 (浙商银行财资) · 建筑 (品茗 / 巡检) · 零售 SaaS (商品通 / 留夫鸭 / 李宁 / 太平鸟) · 设计工具 (有赞 UiDraft / UIdraft) |

---

## 代表项目 (近 1 年, FDE 视角)

### 1. claude-code-workflow — AI 研发工作流方法论

> 把 "需求 → 设计 → 代码 → 测试 → 上线" 全链路拆成可追溯的命令、技能、子代理和规则, 由 AI 执行, 人监督每个关键节点。

**为什么这是 FDE 案例**: 把通用 AI 能力 (Claude) 落地到具体行业 (软件研发) 的标准 FDE 工件。

- **8 步法 + 硬闸门** — `/prd → /plan → /code → /test → /review → /build → /deploy → /release`, 配合 `prd-check` / `plan-check` 硬阻断, AI 不能默默跳过
- **`@rules` 追溯链** — PRD 锚点 → 任务 ID → 源码 `@prd/@rules` → 测试 `it()`, 任何一环改动可向下游全扫
- **质量左移 · 发版硬门禁** — 发版前自动拦截「不合规产物」「新业务规则零测试」, 不达标硬阻断, 防带病上线 (固化成脚本, 不靠 AI 自觉)
- **自动化测试边界分诊** — 每条业务规则先判「可自动化 (单元/组件/状态)」vs「必须人工 (真实外部副作用/视觉/原生/性能)」, AI 不在不可测场景空转, 自动产出人工测试清单 — 知道「不测什么」和「测什么」同样重要
- **需求输入契约 + 依赖图并行** — 外部需求按完备性在 PRD 入口一次性暴露缺口 (🔴阻塞/🟡默认/🟢后补), 把返工从 dev/test 左移; 任务按依赖图拓扑分层, 独立任务并行 spawn 子代理、共享文件串行收口, 多模块交付吞吐显著提升
- **五件套架构** — Commands (决策) + Skills (脚本) + Subagents (并行/独立视角) + Hooks (静默守护) + Rules (长期约束), 边界清晰
- **跨域可移植** — 框架本体一行没改, 已在 3 个完全不同的栈上跑通 (前端/桌面/移动, 见 `docs/ADAPTING.md` 跨工种适配清单)
- 开源 + 中英双语 + 完整 GitHub 包装 (badges / LICENSE / contribution guide)

🔗 https://github.com/Caspian-Sun/claude-code-workflow

### 2. Spider — Tauri 桌面元工具

> 用方法论 (项目 1) 造出来的、用来可视化方法论 (项目 1) 的桌面工具。一个 dogfooding + 自指的工程案例, 证明方法论自身可消费。

- **技术栈**: Tauri 2 + **Rust 后端** (PTY/scan/watcher/IPC) + React 前端 (15 个 feature 模块)
- **价值**: 把任意 `claude-code-workflow` 仓库的 `.claude/` + `docs/` 可视化成 DAG 看板, 每条泳道一个 `/command`, 每张卡片承载真实 PTY 会话
- **跨栈证据**: 同一套 `@prd / @task / @rules` 追溯链在 TS + Rust 双栈通用, 仅需补 ADAPTING.md 中 Rust 注释语法适配

🔗 https://github.com/Caspian-Sun/spider

### 3. 跨平台移动端生产项目 — 方法论的第 3 个落地栈 (商业 · NDA)

> 把方法论 (项目 1) 应用到第 3 个、也是最复杂的栈:Flutter 移动端。一个真实上线、持续迭代的生产 App。

- **技术栈**: Flutter 3 + Dart 3 · Riverpod · go_router · 多模块 feature 架构 · 完整 CI/CD (构建 → 多渠道发布)
- **方法论无缝复用**: 同一套 8 步法 + `@prd/@rules` 追溯链在 Flutter/Dart 上原样跑通 (仅补 Dart 注释语法适配), 证明框架与语言/平台解耦
- **反哺框架**: 这个项目的真实交付压力, 直接催生了框架最新一轮加固 —— 发版硬门禁 (防带病发版)、自动化测试边界分诊、依赖图并行执行。**「做真实项目 → 提炼成工程能力」正是 FDE 的核心动作。**
- 商业项目, 暂无公开仓库 (实现细节可面谈)

---

## 工作经历

### 有赞 (杭州知擎信息科技) | 前端开发工程师 | 2024.11 - 2025.04

负责底层设计系统 UiDraft 和 UXtwo AI 系统的前端开发, 基于 Figma uiobject 原理扩展 AI 设计产品。

- 主导 UiDraft 设计系统编写与维护, 标准化 UI 组件提升跨平台体验一致性
- 参与 UXtwo AI 智能推荐 + 自动化界面生成功能, 落地 AI 优化设计师工作流
- 独立产出 **UIdraft Chrome 插件** (React + TS), 基于 DFS/DSF 实现多组件层级关系识别, 支持复杂场景组件交叉合并

### 浙商银行 财资项目 | 前端架构师 | 2023.10 - 2024.11
*(乙方驻场, 神州信息派驻)*

- 制定前端开发规范, 团队 PR review 周期从 3 天 → 6 小时
- 攻克 qiankun 框架向下兼容 (proxy) 难题, 让微前端项目支持低版本浏览器场景
- 优化首屏加载: 按 main 运行模式排查调用树 + 资源树, **5000ms → 200ms (25x 提升)**
- 主导脱兔低代码平台开发, 集成 S2 大数据表格至平台
- 用 React 编写功能模块嵌入 Vue 老项目, 实现新旧栈共存
- 搭建组件服务中心 (借鉴 ServerUI 思路), 用户可在线实时加载组件

### 杭州亦城亦村 (创业) | 技术经理 | 2023.02 - 2023.08

技术 + 项目管理 + 落地一体, 创业期间负责技术选型、团队执行力、流程优化。

**核心产品 — 分巢**: 积分 App, 主/被动扫码积分付款, 微信小程序 + 安卓 + iOS 三端。
- 前端: uniapp / React Native / React / Canvas (后期 Flutter 重构, 自定义 Widget + 重排 Container 布局)
- 后端: Go (gin) + MySQL + MongoDB + Redis + Nginx
- 独立完成全栈开发 + 项目规划 + 地推

### 品茗科技 | 全栈工程师 | 2021.10 - 2023.01

带前端团队, 主导前端架构 + 低代码平台 + BI 大屏 + 微服务前端。

- **元笔**: Formily 二开实现表单可视化拖拽, 非技术成员可独立创建表单
- **巡检**: 建筑行业日检 Web + 小程序 + H5 全端 (React/Antd/Umi + uniapp + Vue2/Vue3)
- **BI 大屏**: 大数据可视化核心组件, 服务 BI 事业线
- 优化 CDN 分发, 解决国内 + 香港地区资源加载问题
- 数字建造业务线小程序 / H5 / App 全端开发

### 杭州览众数据 | 全栈工程师 → 前端 Leader | 2018.08 - 2021.10

带前端团队, 主攻低代码方向, 同时负责产品 / 项目 / 多端开发。

- **ServerUI (lowcode)** *(独立长期项目, 2020.11 至今)*: 自研声明式低代码平台
  - 数据中心 (MVVM 双向绑定) + 模块加载器 `relation`
  - Vue / React / Angular 三栈在同一页面运行的**沙箱隔离机制** (编译时 + 运行实例)
  - 在线 Fx (借鉴 serverless), 通过反编译实例组件生命周期实现在线扩展
  - webServerModule 中心 + serverui_online_html 在线组合 + serverUIcomment 无缝穿插
  - 设计思考: https://blog.csdn.net/u014080304/article/details/114393458
- **商品通 SaaS** (服装零售供应链): qiankun + Vue2/Vue3/TS 新旧系统兼容; node 微服务前端中心
- **dataflow**: d3.js + dag.js 数仓脚本依赖可视化, 数百节点快速渲染
- **小览工具集**: ci/cd 脚手架 + 内部源 install/uninstall 工具 (难点: 模块卸载需还原配置环境)
- **零售业务线**: 留夫鸭 / 李宁 / 太平鸟 / 一鸣 / 生鲜 / Bee 招聘等多个项目, 含大数据可视化场景下的 canvas table + echart 二次封装

### 软通动力 | 前端开发工程师 | 2015.07 - 2018.07

驻场支付宝相关系统前端开发, 页面设计 + 交互实现 + 性能优化。

---

## 教育经历

**上饶师范学院** · 本科 · 美术学 (主修) + 计算机 (副修) · 2011 - 2015

> 美术 → 设计敏感 → 设计系统工程化 → AI + 设计工具 (UIdraft / Figma uiobject DSL) — 这是我的成长主线, 也是我做 AI 应用工程时的差异化优势。

---

## 技术博客 / 个人输出

- ServerUI 低代码设计思考 — https://blog.csdn.net/u014080304/article/details/114393458
- claude-code-workflow 方法论文档体系 (英文 + 中文双语) — 见 GitHub 仓库
- *(规划中: 把 "AI 工作流落地的 3 个反直觉设计" 系列写成博客)*
