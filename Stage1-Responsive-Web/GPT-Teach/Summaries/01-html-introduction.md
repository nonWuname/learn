# Lesson 1.1 — HTML Introduction & Document Structure: Summary

**Stage:** 1 — Responsive Web Development  
**Topic:** HTML Fundamentals  
**Status:** Learner-reviewed reference

## 1. HTML and Related Technologies

**HTML** = **HyperText Markup Language**.

HTML describes the **structure and semantics** of web content.

- **HyperText:** Text linking to other documents and resources.
- **Markup:** Tags that organize and identify content.
- **Language:** Standardized syntax and parsing rules.

| Technology | Responsibility |
| --- | --- |
| HTML (HyperText Markup Language) | Content, structure, and semantics |
| CSS (Cascading Style Sheets) | Presentation and layout |
| JavaScript | Programming logic and interaction |

HTML itself supports built-in hyperlinks and basic form submission.

## 2. Tag, Element, Attribute

```html
<p class="intro">Hello World!</p>
```

- **Opening tag:** `<p class="intro">`
- **Tag name:** `p` (paragraph)
- **Closing tag:** `</p>`
- **Attribute:** `class="intro"` (name: `class`; value: `intro`)
- **Element:** The whole paragraph represented by the markup

Some elements such as `<meta>` and `<img>` are **void elements** and have no closing tag.

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
| `<!DOCTYPE html>` | Document type declaration; enables modern standards mode |
| `<html>` | Root element |
| `lang="en"` | Primary document language |
| `<head>` | Document metadata |
| `<meta charset="UTF-8">` | Character encoding declaration |
| `<title>` | Document title (commonly shown in the browser tab) |
| `<body>` | Renderable page content |
| `<h1>` | Heading Level 1 |
| `<p>` | Paragraph |

The `head` holds metadata; the `body` holds page content. **`title` is not `h1`**, and **`h1` is not `header`**.

## 4. Language Examples

`lang` is an attribute, **not** an independent tag.

| Example | Meaning |
| --- | --- |
| `lang="en"` | English |
| `lang="en-CA"` | Canadian English |
| `lang="en-US"` | American English |
| `lang="zh-CN"` | Chinese as used in mainland China |
| `lang="zh-TW"` | Chinese as used in Taiwan |
| `lang="fr"` | French |
| `lang="fr-CA"` | Canadian French |
| `lang="ja"` | Japanese |

The correct language declaration helps assistive technologies and other tools interpret the document.

## 5. Unicode and UTF-8

- **Unicode** assigns characters unique code points.
- **UTF-8** (Unicode Transformation Format — 8-bit) encodes Unicode code points as one to four bytes.

| Character | Code point | UTF-8 hex bytes |
| --- | --- | --- |
| `A` | `U+0041` | `41` |
| `你` | `U+4F60` | `E4 BD A0` |

`<meta charset="UTF-8">` declares the encoding but does **not** automatically convert the file. Actual and declared encodings should match; otherwise, text may display as **mojibake**.

## 6. Nesting and Relationships

```text
html
├── head
│   ├── meta
│   └── title
└── body
    ├── h1
    └── p
```

- **Parent:** Contains a direct child element.
- **Child:** Directly contained by a parent element.
- **Sibling:** Shares the same parent as another element.

HTML content rules restrict valid nesting. Browsers parse the document into a **DOM (Document Object Model)**.

## 7. Common Mistakes

1. Confusing `h1` with `header`.
2. Treating `title` as a body heading.
3. Writing `lang` as a separate element instead of an attribute.
4. Confusing tags, elements, and attributes.
5. Writing a backslash instead of the forward slash in a closing tag.
6. Treating Unicode and UTF-8 as unrelated alternatives.
7. Ignoring element-nesting restrictions.

## 8. Learning Outcomes

The learner should be able to create an HTML document independently, explain the major elements, identify attributes and nesting relationships, distinguish `title` from `h1`, use `lang` and `charset` correctly, and describe the basic Unicode/UTF-8 relationship.

**Completion is determined by demonstrated understanding and independent implementation, not by copying a long personal summary.**
