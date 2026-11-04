# Practice 2.1 — Hero 的配色、对齐和间距

## 使用已学知识

CSS Selector、`background-color`、`color`、`text-align`、`padding`、`margin` 和 Border。

## 需求

只调整现有练习网站的样式，不新增 JavaScript，不直接复制完整答案。

| 区域 | 验收条件 |
| --- | --- |
| Body | 背景 `#F3F6FB`；默认外边距清零 |
| Header | 背景 `#233C63`、白色文字、Padding 20px，不额外设置外边距 |
| Hero | 背景 `#EAF2FF`、文字 `#243247`，不显示边框 |
| Hero | 上下 Padding 60px、左右 20px |
| Hero | 文字水平居中；距离下一段内容约 30px |

## 功能验收

1. 在桌面浏览器中查看布局；观察页面边缘是否有非预期留白。
2. CSS 不能含无用的空规则；若有重复 `body` 或 `header`，解释层叠结果并考虑整理。
3. 能说清每个地方为什么选 Padding 而不是 Margin。

## 渐进提示（需要时再看）

- **内部留白**：尝试用双值 `padding` 简写。
- **区域间距**：考虑 `margin-bottom`。
- **四周默认空白**：浏览器一般会给 `body` 一个默认 Margin。
- **同一属性出现多次**：后写的规则可能覆盖前面的声明，注意 specificity / cascade。

## 交付

继续在 [projects/campusconnect](../../../projects/campusconnect/) 自己修改；独立变式或复盘放到 [My-Work](../../My-Work/)；检查后创建有意义的 Commit。
