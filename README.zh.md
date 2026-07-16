# Jane's First Intern Copilot 🎯 — 中文说明

[English README →](README.md)

**这是我找到第一份实习的完整方法论，打包成了一个 Claude skill。** 没有人脉、没有经验、没有名校光环，靠三件事拿到 offer：极度精简的简历、系统化海投、直接给创业公司创始人发 cold email。老板后来告诉我，从那么多人里选中我面试，就是因为我的信息足够 concise、表达足够清晰。

> 注意：这个 skill 是 English native 的——所有模版、示例和产出的简历/邮件都是地道英文（面向英语市场求职）。你可以用中文和 Claude 对话，但交付物默认是英文的。

## 它能帮你做什么

1. **改简历** — 一页纸，每条 bullet 都是 C-A-R 结构（Context–Action–Result），删掉所有空话套话。内置招聘者真实使用的"6 秒测试"。改简历的方法论**完全提炼自 [Stanford Career Education](https://careered.stanford.edu/resources)（斯坦福就业指导中心）公开发布的简历资源**——C-A-R 方法、动词表、"什么算经历"、ATS 筛选、简历检查清单都来自那里（Resources → Resume 一节），这个 skill 做的是把它们蒸馏成 Claude 能直接执行的规则。（个人项目，与斯坦福大学无关联、未获其背书。）
2. **搭建海投系统** — 申请追踪表、根据 deadline 倒推的每日配额、目标分级（A/B/C）、每 ~25 份申请做一次漏斗复盘。让"没有回复"变成数据而不是打击。
3. **写创始人 cold email** — 两套模版：~60 词的极简 fit 版（作者本人拿到实习用的就是它）和 ≤120 词的 hook 版，外加预先写好日期的两封 follow-up。这是转化率最高、但没人教学生的渠道。

内置诚实底线：只会把你真实的经历写得更锋利，绝不编造不存在的东西。

## 安装

skill 本质上就是一个 Markdown 文件夹，装好后 Claude 遇到相关话题会自动读取。

**Claude Code（推荐）：**

```bash
# 个人 skill，所有项目都能用（目标文件夹必须叫 first-intern，这是 skill 的名字）
git clone https://github.com/jo1-yo/janes-first-intern-copilot.git ~/.claude/skills/first-intern
```

没有构建步骤、没有依赖、不用配置。以后更新就在文件夹里 `git pull`，不想要了直接删文件夹。

**Claude.ai / 桌面版：**

1. 下载本仓库的 zip（绿色 **Code** 按钮 → **Download ZIP**）。
2. 打开 **Settings → Capabilities → Skills**，上传 zip 即可。

**验证装好了没：** 新开一个对话，说 *"I need help finding my first internship."* 如果 Claude 第一步是**先要你的简历再给建议**（而不是直接甩通用 tips），说明 skill 已生效。

## 怎么用

不需要任何命令——只要话题涉及实习、找工作、简历、cover letter、cold email、"投了没人回"，skill 就会自动触发。直接正常聊天：

- **改简历：** *"我投了 40 份实习申请零回复，这是我的简历：……"* → Claude 会先把你的简历解析成结构化清单给你确认（不会瞎扫一眼就给建议），然后诊断三个最大问题，逐条 before → after 重写，最后跑 6 秒测试。
- **海投系统：** *"简历改好了，我 6 月前要拿到 offer，接下来怎么办？"* → 给你一张预填好的追踪表、按 deadline 算出的每日配额（比如 8 周 ≈ 每天 3 份申请 + 半封 cold email），以及大平台之外的渠道。
- **Cold email：** *"我想去 XX 公司实习，从没写过 cold email。"* → 按你手上的素材选模版，第一次会逐句标注每句话为什么存在（让你学会公式），并连 follow-up 一起写好日期。
- **全流程：** *"我两个月内需要一份暑期实习，没有简历也不知道从哪开始。"* → 三个 workflow 串成一个计划，最后永远收敛成**恰好三条**带 deadline 的下一步行动。

## 仓库结构

```
SKILL.md                  # 入口：方法论、规则、流程
references/resume.md      # 简历：Step-0 提取、C-A-R、6 秒测试
references/mass-apply.md  # 海投系统：追踪表、分级、配额、漏斗
references/cold-email.md  # Cold email：A/B 模版、follow-up、完整范例
references/action-verbs.md# 动词表 + 一票否决的废词
assets/tracker-template.csv
```

## License

MIT — 见 [LICENSE](LICENSE)。
