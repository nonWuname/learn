# Lesson 2.2 — CSS Box Model：Padding 与 Margin

## 四层结构

从内到外：

```text
Content → Padding → Border → Margin
```

- **Content**：文字、图片等内容。
- **Padding**：内容与 Border 之间的内部留白，属于元素的盒子；背景默认会延伸到 Padding。
- **Border**：边框。
- **Margin**：边框外面的空间，不由该元素自身背景填充。

## 控制方式

```css
.card {
    padding: 20px;
    margin-bottom: 30px;
}
```

`padding` 可以改变文字到卡片边框的距离；`margin-bottom` 通常用来拉开当前元素与下面内容的距离。

## 简写顺序

- 一个值：四边相同。例 `padding: 20px;`
- 两个值：上下、左右。例 `padding: 60px 20px;`
- 三个值：上、左右、下。
- 四个值：上、右、下、左（顺时针）。

`margin` 使用同样的简写规律。

例如：

```css
.hero {
    padding: 60px 20px;
    margin-bottom: 30px;
}
```

表示 Hero 上下内部间距 60px，左右内部间距 20px；下方外部间距 30px。

## 容易混淆的三个属性

- `padding`：元素内部间距。
- `margin`：元素外部间距。
- `text-align: center`：主要用于容器内**行内内容**的水平对齐，**不等同于**将整个盒子居中。

`margin: 0 auto;` 在某些布局条件下可使具有受限宽度的普通块盒水平居中，与 `text-align` 用途不同。

## 额外提醒

- Padding 不接受负值；Margin 可以有负值，但初学阶段不建议滥用。
- 默认 `box-sizing: content-box` 下，声明的 `width` 不包含 Padding / Border；`box-sizing: border-box` 会改变宽度计算方式。
- 普通布局中的相邻块级元素的竖直 Margin 有时会发生 margin collapsing（外边距折叠），不是总能相加。

## 自查

如何让文字离卡片边框更远？如何只让 Hero 距下一块内容 30px？如何理解 `margin: 10px; margin-bottom: 30px;` 的最终结果？

**练习**：[Style Hero](Practice/01-style-hero.md)。
