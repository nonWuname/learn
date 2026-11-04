# Lesson 1.1 — HTML Introduction & Document Structure

**Stage:** 1 — Responsive Web Development  
**Topic:** HTML Fundamentals

## Learning Objectives

By the end of this lesson, you should understand what HTML is, how it relates to CSS and JavaScript, the difference between tags, elements, and attributes, and the purpose of each part of a basic HTML document.

## 1. What Is HTML?

**HTML** stands for **HyperText Markup Language**.

HTML describes the *structure and semantics* of web content, rather than primarily specifying its appearance.

- **HyperText:** Text that can link to other documents and resources.
- **Markup:** Tags that identify and organize different kinds of content.
- **Language:** A standardized syntax that browsers can parse.

The three core web technologies serve distinct roles:

| Technology | Primary role |
| --- | --- |
| HTML — HyperText Markup Language | Content, structure, and semantics |
| CSS — Cascading Style Sheets | Presentation, styling, and layout |
| JavaScript | Programming logic, behavior, and interaction |

HTML can provide built-in functionality (such as hyperlinks and basic form submissions) without JavaScript.

## 2. Tags, Elements, and Attributes

Consider:

```html
<p class="intro">Hello World!</p>
```

- **Tag name:** `p` means *paragraph*.
- **Opening tag:** `<p class="intro">`.
- **Closing tag:** `</p>` (note the forward slash `/`).
- **Attribute:** `class="intro"`, where `class` is the name and `intro` is the value.
- **Element:** The complete paragraph structure represented by the markup.

Attributes supply additional information about an element. A `class` can be used for styling and scripting.

Some HTML elements are **void elements**, such as `<meta>` and `<img>`; they do not have closing tags.

## 3. Basic HTML Document

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <title>Example Page</title>
</head>

<body>
    <h1>Welcome!</h1>
    <p>This is my first webpage.</p>
</body>

</html>
```

| Syntax | Purpose |
| --- | --- |
| `<!DOCTYPE html>` | HTML document type declaration; enables standards mode in modern browsers (not an HTML element) |
| `<html>` | Root element |
| `lang="en"` | Declares the document's primary language |
| `<head>` | Contains document metadata |
| `<meta charset="UTF-8">` | Declares the HTML document character encoding |
| `<title>` | Document title, commonly displayed in the browser tab |
| `<body>` | Contains the document's renderable content |
| `<h1>` | First-level heading (*Heading Level 1*) |
| `<p>` | Paragraph |

### Head versus Body

The `head` is for metadata and references (for example, the title, encoding, and linked stylesheets). The `body` contains content such as headings, paragraphs, images, links, and forms.

**`title` is not `h1`:** `title` describes the document and belongs in the `head`; `h1` is a visible heading in the `body`. Also, `h1` means *Heading Level 1*, **not** `header` (which is a different semantic element).

### Language Attribute

`lang` is an **attribute**, not a standalone tag. Examples:

| Declaration | Meaning |
| --- | --- |
| `lang="en"` | English |
| `lang="en-CA"` | Canadian English |
| `lang="en-US"` | American English |
| `lang="zh-CN"` | Chinese as used in mainland China |
| `lang="zh-TW"` | Chinese as used in Taiwan |
| `lang="fr"` | French |
| `lang="fr-CA"` | Canadian French |
| `lang="ja"` | Japanese |

Correct language information helps assistive technologies and other tools interpret content. An individual element can also declare a different language.

## 4. Character Encoding

Computers store bytes, while documents represent characters.

**Unicode** is a character standard that assigns **code points** to characters. **UTF-8** (Unicode Transformation Format — 8-bit) is a variable-length encoding that represents Unicode code points as sequences of one to four bytes.

| Character | Unicode code point | UTF-8 bytes (hex) |
| --- | --- | --- |
| `A` | `U+0041` | `41` |
| `你` | `U+4F60` | `E4 BD A0` |

```html
<meta charset="UTF-8">
```

This declares the document's character encoding. If the file is actually stored using one encoding but decoded using a different, incompatible encoding, text may become corrupted or unreadable (**mojibake**).

**Important:** A character encoding declaration does not automatically convert the file. Keep the actual encoding and declared encoding consistent. Browsers may also obtain encoding information from HTTP headers.

## 5. Nesting and Hierarchy

HTML has a hierarchical structure:

```text
html
├── head
│   ├── meta
│   └── title
└── body
    ├── h1
    └── p
```

- **Parent:** An element directly containing another element.
- **Child:** An element directly contained by its parent.
- **Siblings:** Elements that share the same parent.

HTML nesting is restricted by content rules. Browsers parse HTML to construct the **DOM (Document Object Model)**, which JavaScript can later inspect or modify.

## 6. Common Mistakes

- Confusing `h1` with the different `header` element.
- Expecting `title` to render as an in-page heading.
- Writing `<lang="en">` instead of putting `lang="en"` on `<html>`.
- Treating a tag, element, and attribute as the same concept.
- Writing `<\p>` instead of `</p>`.
- Treating Unicode and UTF-8 as unrelated alternatives.
- Using invalid nesting.
- Assuming HTML is solely responsible for visual design or dynamic behavior.

## 7. Lesson Wrap-Up

HTML structures and describes content. CSS provides styling and layout. JavaScript enables programmatic behavior. A valid document requires deliberate structure, meaningful elements, and consistent encoding.

See the [reviewed summary](../Summaries/01-html-introduction.md) for a concise reference and the [challenge](../Challenges/01-first-html-page.md) for an independent implementation task.
