# GitHub 个人主页改造方案 — Caspian-Sun

> GitHub 有个"特殊仓库"功能: 如果你创建一个仓库, 名字和你的用户名一样
> (`Caspian-Sun/Caspian-Sun`), 它的 README.md 会显示在你的个人主页顶部。
>
> 招聘方点进你 GitHub 主页第一眼看到的就是这个 README。**这是 FDE 候选人
> 的"门面"**, 比任何简历都先被看到。

---

## 一、操作步骤

### Step 1: 创建特殊仓库

```bash
# 在 GitHub 网页上:
# 1. 点 "+" → New repository
# 2. Repository name: Caspian-Sun  (必须和你的 GitHub 用户名完全一致)
# 3. Public
# 4. 勾选 "Add a README file"
# 5. Create repository
```

### Step 2: 把下面 README 内容贴进去, commit

### Step 3: 设置 Pinned Repositories (置顶仓库)

去 https://github.com/Caspian-Sun 个人主页:
- 点 "Customize your pins"
- 选择 6 个最重要的仓库, 推荐顺序:

```
1. claude-code-workflow   ← 方法论 (最核心)
2. spider                  ← 元工具 (跨栈证据)
3. [Cpcash 公开镜像 / 或保留私有不 pin]
4. [ServerUI 如果有公开仓库]
5. [其他能体现 AI 工程化的小项目]
6. [一个体现你写作 / 思考能力的仓库]
```

如果不到 6 个就 pin 3 个最强的, 别凑数。

---

## 二、推荐的 README.md 内容

把下面整段复制到 `Caspian-Sun/Caspian-Sun` 仓库的 `README.md`:

````markdown
### Hi 👋 I'm Tom (Daotao Sun)

I'm a **Forward Deployed Engineer** with 10 years of full-stack experience,
currently focused on turning generic AI capabilities into production-grade
engineering workflows for specific verticals.

---

### 🔭 What I'm building

**[claude-code-workflow](https://github.com/Caspian-Sun/claude-code-workflow)**
— An AI-driven R&D methodology framework. Breaks "Requirements → Design →
Code → Test → Deploy" into traceable commands, skills, subagents, and rules.
8-step SDLC with hard gates, `@rules` traceability chain, and a five-part
collaboration architecture. Open source, bilingual (EN/ZH).

**[spider](https://github.com/Caspian-Sun/spider)**
— A Tauri 2 desktop tool that visualizes any `claude-code-workflow` repo as
a kanban. A meta-tool: built with the methodology to render the methodology.
Rust + React.

**Cpcash Wallet** *(private repo, walkthrough on request)*
— A Web3 mobile wallet shipping from a single Flutter codebase to Android,
iOS, and HarmonyOS. 138 commits, 167 tasks closed at 100%, 13 days from
init to dev/staging release.

---

### 🧰 Stack range

`TypeScript` · `Rust` · `Dart` · `Go` · `Python` · `Java` · `Node`
React · UmiJS · Tauri · Flutter · Vue · Solidity · Ant Design

---

### 🎯 Currently looking for

**Forward Deployed Engineer** / **Applied AI Engineer** / **Solutions
Engineer** roles, ideally at AI infrastructure companies, AI-native
startups, or consultancies deploying AI to real customers.

Open to remote · based in Hangzhou, China · willing to relocate.

📫 Reach me: **459269440@qq.com** · WeChat **13282001310**

---

### 📌 Background

Before AI, I:
- Led frontend teams of 20+ at Pinming and Lanzhong
- Built a self-hosted low-code platform (ServerUI) running Vue + React +
  Angular on the same page with sandbox isolation
- Shipped products across finance (Zheshang Bank), construction (Pinming),
  retail SaaS (Shangpintong / Li-Ning / Peacebird), and Web3 (Cpcash)
- Studied Fine Arts (undergrad) before CS — strong design intuition

---

### ✍️ Writing

- [ServerUI low-code design notes](https://blog.csdn.net/u014080304/article/details/114393458) (CSDN, Chinese)
- [`claude-code-workflow` methodology docs](https://github.com/Caspian-Sun/claude-code-workflow) (bilingual)
- *More long-form writing coming soon — follow this profile to get notified.*

---

<sub>"Generic AI is impressive. AI deployed into someone's actual workflow is
useful. That's the only gap that matters."</sub>
````

---

## 三、设计取舍说明

### 为什么这样写

| 元素 | 作用 |
|------|------|
| 开头 1 句话定位 | 5 秒判定: "这人是 FDE 苗子, 继续看" |
| 三个 What I'm building | 把最强弹药前置, 链接直达 |
| Stack range 一行展示 | 不堆 badge, 用代码块呈现, 朴素但全面 |
| Currently looking for | 把求职意向写明, HR 不用猜 |
| Background 放在中段 | 信息层次: 当前 > 资历 |
| Writing 板块 | 体现"会思考会输出" |
| 结尾 quote | 留个记忆点, 一句话讲清 FDE 哲学 |

### 不要做的事

- ❌ **不要堆 badge** (shields.io 那一排 5 行的 badge 是新手感)
- ❌ **不要放 GitHub stats 卡片** (大家都有, 没差异化)
- ❌ **不要写 "学习中..." / "正在成长..."** (FDE 要的是 senior 气质)
- ❌ **不要放表情符号过量** (1-2 个章节图标可以, 全文洒满就 low)
- ❌ **不要列爱好** (除非和工作高度相关, 否则浪费可贵的首屏空间)

### 可选增强 (做完上面再考虑)

1. **加一个 Featured Talks / Podcasts** 板块, 如果你有公开分享
2. **加一个 Mentoring** 板块, 如果你愿意指导 junior, 这是 senior 标签
3. **每月更新一次 "Currently focused on"**, 让访问者感觉这个人在动

---

## 四、Pinned Repos 文案优化

每个 Pinned Repo 都有一个 **30 字描述**, 招聘方在你的 GitHub 主页能看到。
默认的描述往往很烂, 要重写:

| 仓库 | 推荐描述 (30 字内) |
|------|------------------|
| `claude-code-workflow` | `AI-driven R&D workflow: 8 steps, hard gates, @rules traceability. Bilingual.` |
| `spider` | `Tauri+Rust desktop tool that visualizes any claude-code-workflow repo as a kanban.` |

去每个 repo 的 Settings → 顶部的 Description 字段改。

---

## 五、CTA: 让访客有"下一步"

特殊 README 的最大问题是 **看完没有下一步**。建议在结尾放一个明确的 CTA:

```markdown
---

### Want to chat?

If you're hiring for FDE roles or just want to talk about AI in production,
the fastest way to reach me:

- 📧 459269440@qq.com (English / Chinese both fine)
- 💬 WeChat: 13282001310
- 🔗 [LinkedIn](https://www.linkedin.com/in/caspian-sun-404b6140b)

I respond within 24h.
```

把这段加在底部, 招聘方就不会"看完 README 不知道下一步"。
