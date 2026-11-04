# Lesson 1.1 — HTML Document Structure（文档结构）

## 目标

理解 HTML 为什么不是一段随意排列的文字；区分 HTML、CSS、JavaScript 的基本职责。

## 核心概念

**HTML (HyperText Markup Language)** 是描述内容及其结构的标记语言。浏览器将 HTML 解析成 **DOM (Document Object Model)** 树，再配合 CSS 进行布局和绘制。

- **Tag（标签）**：如 `<p>`、`</p>`。
- **Element（元素）**：起始标签、内容、结束标签组成的整体；部分元素是 void element，例如 `<img>`。
- **Attribute（属性）**：起始标签上的额外信息，例如 `href`、`id`、`class`。

## 最小页面示例

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Page</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <h1>Hello!</h1>
    <p>This is a paragraph.</p>
</body>
</html>
```

逐项理解：

- `<!DOCTYPE html>`：声明现代 HTML 文档类型。
- `html`：文档根元素；`lang` 提示页面主要语言。
- `head`：元数据、标题、CSS 引用等，通常不是可见正文。
- `body`：页面内容。
- `meta charset`：声明字符编码，通常为 UTF-8。
- `meta name="viewport"`：帮助移动端按设备宽度设置布局视口。
- `title`：浏览器标签页标题，不是页面正文标题。
- `link rel="stylesheet"`：关联外部 CSS 文件。

## 元素嵌套与树

```text
html
├── head
│   └── title
└── body
    ├── h1
    └── p
```

父元素包含子元素；结束标签的位置决定层级。不是所有标签都能随意嵌套，例如 `p` 不能包含 `section`。

## 易错点

1. 把 `title` 当作页面可见的大标题；页面可见标题应使用 `h1` 等。
2. 忘记闭合需要结束标签的元素，导致后续内容结构混乱。
3. 文件路径不对，导致 `style.css` 没有加载。
4. 认为 HTML 标签只是为了让文字变大；标题和段落有真正的语义。

## 自查

能否说明：HTML 负责什么？`head` 和 `body` 的职责如何区分？`class` 与元素标签有什么区别？

**实践题**：[Hero HTML 结构](Practice/01-hero-html.md)。不要从参考中直接复制完整答案。
