# Lesson 1.2 — Semantic HTML（语义化结构）

## 为什么需要语义？

不写 CSS 时，`div` 和 `section` 可能显示得很像，但它们表达的含义不同。HTML 用来描述「这是什么内容」，CSS 主要描述「这看起来怎样」。

| 元素 | 语义 | 使用场景 |
| --- | --- | --- |
| `header` | 页眉或某区域头部 | 网站名称、导航入口 |
| `nav` | 导航链接区域 | 页面或站点导航 |
| `main` | 当前页面的主要内容 | 首页正文主体 |
| `section` | 具有主题的章节 | Hero、Events 等 |
| `footer` | 页面或章节页脚 | 版权、相关链接 |
| `div` | 不赋予额外语义的通用容器 | 布局、样式分组 |
| `p` | 段落 | 文字段落 |

## 示例（只演示结构）

```html
<body>
    <header>
        <h1>Example Club</h1>
        <nav><a href="#events">Events</a></nav>
    </header>
    <main>
        <section>
            <h2>Welcome</h2>
            <p>Discover our community.</p>
        </section>
        <section id="events">
            <h2>Upcoming Events</h2>
        </section>
    </main>
    <footer>
        <p>Copyright information</p>
    </footer>
</body>
```

`main` 是主要内容的范围，而 `section` 可以是其中的多个主题章节。Hero 是一个设计术语，**不是** HTML 内置的 `<hero>` 标签。用 `section` 及合理的标题、文案即可表达。

## 实际意义

- 屏幕阅读器等辅助技术可以利用 `main`、`nav` 等地标区域（landmarks）导航。
- 阅读源码的人更容易理解结构。
- 自动化工具更容易定位有明确含义的区域。

**注意**：`section` 不一定自动成为可命名的 landmark；通常需要一个可访问名称（例如 `aria-labelledby`）。语义标签也不会凭空形成漂亮的布局。

## 易错点

- 把 `main` 当成万能容器，或每个 `section` 都创建一个 `main`。
- 把 `p` 当成可以包住任意内容的 `div`。
- 把视觉样式与语义等同：看起来正常，不代表嵌套合理。

## 自查

为什么 Hero 应当位于当前页面的 `main` 内？为什么 `section` 不等同于 `p`？

**实践题**：[Hero HTML 结构](Practice/01-hero-html.md)。
