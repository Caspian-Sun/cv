# 转型 FDE 投递包 — 道涛 · 2026-05

> 这个目录包含转型 Forward Deployed Engineer 求职的全套材料。
> 全部是 Markdown 格式, 用任何编辑器打开都能改。

---

## 📦 包内清单

### 简历 (HTML 直接打印 PDF, 推荐用法)

| 文件 | 风格 | 投什么质用什么 |
|------|------|---------------|
| `resume-senior-zh.html` | **Senior 简洁中文版** | 国内 AI 公司 · 字节豆包 · 智谱 · MiniMax · Moonshot · 大厂 AI 应用层 |
| `resume-senior-en.html` | **Senior 简洁英文版** | 海外 FDE: Anthropic · OpenAI · Scale AI · 海外 AI 创业 · LinkedIn 投递 |
| `resume-branded-zh.html` | **绿色品牌中文版** (含照片占位 + HELLO 头条) | 国内传统 HR · Boss 直聘 · 拉勾 · 中小企业 |

**生成 PDF 的方法 (3 步)**:
1. 在 Finder 双击 HTML 文件, 默认浏览器会打开
2. 右下角点 "打印 / 另存为 PDF" 按钮 (或 `Cmd+P`)
3. 弹窗里:
   - 目的地选 **"另存为 PDF"**
   - 纸张大小: **A4**
   - 边距: **无** 或 **最小**
   - 选项里 **取消勾选** "页眉和页脚"
   - 点 "保存"

> 替换照片 (仅 `resume-branded-zh.html`): 在 HTML 中找到 `.photo` 那个 div, 把里面的 `.hint` 整个删掉, 替换成 `<img src="你的照片.jpg" style="width:100%;height:100%;object-fit:cover;" />`。或在 CSS 的 `.photo` 里加 `background-image: url(your-photo.jpg);`。

### Markdown 源文件 (备份用, 改内容时改这里)

| 文件 | 用途 |
|------|------|
| `resume-zh.md` | 中文简历源 (Markdown) — HTML 内容从这里同步, 改这里再改 HTML 保持一致 |
| `resume-en.md` | 英文简历源 (Markdown) |

### 辅助材料

| 文件 | 用途 | 投递时怎么用 |
|------|------|------------|
| `pitch.md` | **5 个不同长度的自我介绍** | LinkedIn About / 微信介绍 / 面试开场 / 邮件投递 |
| `cover-letter-template.md` | **求职信模板** (中英双版) | 每投一家公司复制一份, 改占位符再发 |
| `github-profile-README.md` | **GitHub 主页改造方案** | `Caspian-Sun/Caspian-Sun` 仓库 README (已部署) |

---

## 🚀 30 天投递路线图 (强烈建议按这个节奏执行)

### Week 1 — 武装到牙齿

- [ ] **Day 1**: 仔细 review `resume-zh.md` 和 `resume-en.md`, 把项目数据
      / 公司名 / 起止月份等细节核对一遍 (我用的是简历上原文 + 我们的对话,
      可能有少量误差需要校准). 同步修改 3 个 `.html` 文件里的对应内容。
- [ ] **Day 2**: 浏览器打开 3 个 HTML 文件, 各自打印另存为 PDF, 命名:
      - `孙道涛-FDE-简历-Senior-202605.pdf`
      - `孙道涛-FDE-简历-品牌-202605.pdf`
      - `Daotao_Sun_FDE_Resume_202605.pdf`
- [ ] **Day 3**: 按 `github-profile-README.md` 改造 GitHub 主页:
  - [ ] 创建 `Caspian-Sun/Caspian-Sun` 特殊仓库
  - [ ] 贴 README, push
  - [ ] 设置 Pinned Repos: claude-code-workflow + spider + 1-2 个其他
  - [ ] 把每个 pinned repo 的 Description 字段重写成 30 字以内的精炼描述
- [ ] **Day 4-5**: LinkedIn 资料更新:
  - [ ] About 区贴 `pitch.md` 第 1 段 (英文 LinkedIn About 那段)
  - [ ] Headline 改成: `Forward Deployed Engineer | Built an AI R&D
        methodology applied across 3 stacks`
  - [ ] Experience 部分按英文简历重写, 一份一份对照过来
  - [ ] Featured 区把 claude-code-workflow 仓库 pin 上去
- [ ] **Day 6-7**: 写一篇技术博客 (中文 + 英文双语) 讲 claude-code-workflow
      的 3 个设计决策, 发到掘金 + Medium。**这是面试官 60% 概率会问的, 提前
      准备好链接备用**

### Week 2 — 海投阶段 (广度优先)

- [ ] **目标公司清单** (建议 20-30 家, 分三档):
  - **A 档 (重点公司, 5-8 家)**: Anthropic / OpenAI / Scale AI / 字节
        豆包应用团队 / 智谱 / Moonshot / MiniMax / 阿里通义应用层
  - **B 档 (高潜公司, 10-15 家)**: AI 创业公司中 50-200 人规模、有真实
        客户的, 招 "应用工程师 / 解决方案工程师 / 高级前端 + AI"
  - **C 档 (兜底, 5-10 家)**: 大厂前端架构师 / AI 中台工程师岗位, 作为
        Plan B
- [ ] 每天投 3-5 家, 每家**必须**用 cover letter 模板改一份个性化版本,
      不要群发模板感
- [ ] 投递渠道优先级: **内推 > LinkedIn DM > 招聘平台 > 官网投递**

### Week 3 — 面试响应

- [ ] 准备 **30 分钟项目深度讲解** 的 slides (PDF, 6-8 页):
  - 1 页背景: 我为什么做这个方法论
  - 2 页架构: 八步法 + @rules 追溯链
  - 2 页证据: Cpcash 跨栈数据 + Spider 元工具
  - 1 页坑: 还没解决的问题 (诚实 = 信任)
  - 1 页 ask: 我对这家公司能贡献什么
- [ ] 准备 **5-10 个反问问题**, 投每家公司前更新一次

### Week 4 — 谈判与决策

- [ ] 拿到至少 2-3 个 offer (才有谈判筹码)
- [ ] 比较时不要只看薪资, 看:
  - 这家公司是真做 FDE 还是挂羊头? (问他们最近 deploy 过哪些 AI 给客户)
  - 团队 senior 程度? (技术 leader 是不是真懂 AI)
  - 业务在不在风口? (有真实付费客户 vs 烧投资人钱)

---

## 🎯 投递时的几条铁律

1. **永远先讲 claude-code-workflow** — 不管面试 / 邮件 / 自我介绍, 这是
   你最强弹药, 先把它讲清楚再讲其他

2. **数字优先** — "138 commits / 13 天 / 167 任务 100%" > "效率显著提升"

3. **诚实记录失败** — 你写的方法论复盘里有"还没解决的问题"那一节,
   面试时**主动**讲, 比所有亮点都加分

4. **拒绝低薪** — 简历上原来写的 18-30K 是初级工程师价格, 现在你的履历
   应该是 **35-60K** (国内 AI 公司) 或 **$120K-$200K** (海外 FDE)。
   面试问 expected salary 时坚定地讲这个区间

5. **拒绝 "面试官说讲下你最熟悉的项目" 时讲低代码** — 那是历史包袱, 不是
   FDE 卖点。**永远先讲 AI 方法论**, 再用低代码作为 "我做过类似复杂工程
   架构" 的支撑材料

---

## 📊 投递记录模板 (建议自己维护一份)

可以另开一个 Notion / 飞书表格, 字段:

| 公司 | 岗位 | 投递日期 | 渠道 | 进展 | 一面日期 | 二面日期 | offer? | 备注 |
|------|------|---------|------|------|---------|---------|--------|------|

---

## 🔥 最后一句

**你不缺方法论, 缺的是把已经做的事讲清楚。**

这套材料已经把"讲清楚"这件事做完了。剩下的执行 = 投递 + 面试响应。
按照 30 天路线图走, 不要拖, 不要完美主义改材料 (90 分版本立刻投 >
100 分版本拖一个月)。

加油 🚀

---

*生成时间: 2026-05-19 · 由 Claude (Opus 4.7) 与道涛协作完成*
