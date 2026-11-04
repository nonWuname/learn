# Lesson 1.3 — Links and IDs（链接与页面内导航）

## 核心概念

`<a>`（anchor element）创建超链接。常见属性：

- `href`：链接目标。例如 `https://example.com` 是外部地址。
- `id`：当前 HTML 文档内元素的唯一标识符（同一文档应避免重复 ID）。
- `href="#events"`：把当前页面导航到 `id="events"` 的元素附近。

## 原理示例

```html
<nav>
    <a href="#contact">Contact</a>
</nav>
<section id="contact">
    <h2>Contact Us</h2>
</section>
```

浏览器匹配链接中的 fragment identifier（`#contact`）与页面的目标 ID。与 CSS 或 JavaScript 无关，普通 HTML 就能完成这种导航。

## 易错点

1. 链接写 `href="events"`：这通常是相对 URL，不等于 `#events`。
2. 目标元素没有匹配的 `id`，所以点击后不跳转到预期区域。
3. 一个页面中多个元素使用同一个 ID。
4. 把 `a` 误认为必须有按钮外观；默认链接外观可以由 CSS 修改，但语义仍然是链接。

## 自查

为什么 `href="#events"` 需要与 `id="events"` 配套？`class` 能否直接替代这里的 `id`？

**实践题**：[给 Hero 添加 Events 链接](Practice/02-event-link.md)。
