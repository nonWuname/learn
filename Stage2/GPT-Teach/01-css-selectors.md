# Lesson 2.1 — CSS Selectors 与 Cascade

## CSS 的基本形式

CSS (Cascading Style Sheets) 用来描述页面呈现方式。

```css
selector {
    property: value;
}
```

例如：

```css
p {
    color: #243247;
}
```

`p` 是 selector（选择器），`color` 是 property（属性），`#243247` 是 value（值）。

## 常见选择器

| 写法 | 匹配什么 |
| --- | --- |
| `h2` | 所有 h2 元素 |
| `.hero` | `class="hero"` 的元素 |
| `#events` | `id="events"` 的元素 |
| `nav a` | 在 nav 后代中的 a 元素 |
| `header > h1` | 直接以 header 为父元素的 h1 |

`nav a` 不是 HTML 的新标签，而是**后代选择器（descendant combinator）**；中间的空格有意义。

## Cascade（层叠）

当多条规则对同一个属性竞争时，浏览器要根据来源/重要性、层叠层、选择器优先级和声明顺序等决定最终值。初学阶段先记住：

- 相同来源与重要性等条件下，较高 specificity（优先级）的选择器一般胜出。
- 如果优先级等其他比较条件相同，较后出现的声明通常生效。
- 有些 CSS 属性可继承，例如 `color`；有些通常不继承，例如 `margin`。

例如：

```css
header { color: white; }
header { color: navy; }
```

在没有更高优先规则干预时，同样优先级的后者决定 `color`。

## 常见易错点

- 把 `.hero` 写成 `hero`：前者选择 class，后者选择名为 hero 的元素。
- 把 `nav a` 错误地理解为在 HTML 中创建特殊标签。
- 只凭视觉推断某条 CSS 必然生效，忽略其他规则覆盖。
- 重复写多个 `header` / `body` 规则，导致维护困难；重复本身不一定是错误，但需要看层叠结果。

## 自查

`header h1` 与 `header > h1` 有什么差别？为什么页面可能显示与文件顶部设置不同的颜色？
