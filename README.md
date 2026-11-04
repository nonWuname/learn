# Web Development Learning Lab

一个按阶段推进、以**独立编程与复盘**为核心的 Web Development 学习仓库。

> 当前练习项目是 **CampusConnect**；它不是最终要交付的汉服社团网站。真正的汉服 Club 产品将在明确朋友的需求后单独规划（必要时建立新仓库）。

## 学习方法（固定工作流）

1. **Learn**：GPT 讲解**一个自然小节**，包括概念、原理、语法、示例、易错点。
2. **Challenge**：GPT 发布具体需求、限制与验收标准，**不直接给完整实现**。
3. **Implement**：由我独立写代码、测试；卡住时向 GPT 要分级提示。
4. **Review**：GPT 对照实际代码和验收标准检查；未掌握的内容针对性补练。
5. **Summarize**：**我亲自**在 My-Work 中整理理解与错误经验，GPT 只做批改与补充。
6. **Commit**：完成功能或总结后提交一个有意义的版本记录，必要时 Push 到 GitHub。

每一个小章节都能回看：**GPT 的教材 → GPT 的需求 → 我的实现 → 我的总结 → Git 历史**。

## 目录

```text
learn/
├── README.md
├── Stage1/
│   ├── README.md
│   ├── GPT-Teach/
│   │   ├── 01-html-document.md
│   │   ├── 02-semantic-html.md
│   │   ├── 03-links-and-ids.md
│   │   └── Practice/
│   │       ├── 01-hero-html.md
│   │       └── 02-event-link.md
│   └── My-Work/
│       └── README.md
├── Stage2/
│   ├── README.md
│   ├── GPT-Teach/
│   │   ├── 01-css-selectors.md
│   │   ├── 02-css-box-model.md
│   │   └── Practice/
│   │       └── 01-style-hero.md
│   └── My-Work/
│       └── README.md
└── projects/
    └── campusconnect/
        ├── index.html
        └── style.css
```

**为什么教学和项目分开？** `StageN/GPT-Teach/` 是课程参考与题目；`StageN/My-Work/` 保存自己写的独立练习与总结。`projects/campusconnect/` 则是一份持续迭代的网站源码；不必每个阶段复制一个新网站。阶段成果由 Git Commit、必要时由 Tag 标记。

## 学习路线

- **Stage 1 — HTML Foundations**：文档结构、语义标签、链接、图片、列表、表单。
- **Stage 2 — CSS + Responsive**：选择器、Cascade、Box Model、Display、Flexbox、Grid、Media Queries。
- **Stage 3 — JavaScript Fundamentals**：变量、条件、循环、函数、数组、对象。
- **Stage 4 — Interactive Web**：DOM、Event、表单、Fetch、异步。
- **Stage 5 — Independent Projects**：独立完成新需求与小项目，迁移检验。
- **Stage 6 — Hanfu Club MVP**：先调研需求，再选择后端、存储、部署方案；按需另开正式产品仓库。

当前只建立已接触过的 Stage 1 / Stage 2 材料；未来章节**学到时再新增**，不要提前把答案堆满仓库。

## 工作约定

- GPT 的讲义与任务：保存至对应 `StageN/GPT-Teach/`；每次一个主题。
- 我自己的代码、题目答卷与总结：保存在 `StageN/My-Work/`；GPT 不替我写个人总结。
- 持续演化的网站代码：`projects/campusconnect/`。
- 独立练习的答案不放入 GPT-Teach，以避免练习时直接看到答案。
- 对应 Git Commit 例子：`docs: add CSS box-model lesson`、`feat: style hero section`、`docs: add my box-model summary`。

## 当前项目

[CampusConnect](projects/campusconnect/) — HTML/CSS 学习用的持续迭代练习网站。正式 Hanfu Club 项目另行确定需求与名称。
