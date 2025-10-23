# Introduction To CSS — Part - 1

# 🎨 CSS — Day 2

**Date:** October 23, 2025

**Focus:** Introduction to CSS — Part 1

**Goal:** Learn CSS syntax and how to align text within HTML elements.

---

## 🧱 1. HTML Refresher — Container Element

The HTML `<div>` element defines a **container** that groups other elements.

```html
<div>
  <h1>Tourism</h1>
  <p>Plan your trip wherever you want to go</p>
  <button>Get Started</button>
</div>
```

---

## 🎨 2. CSS Syntax

The structure of a CSS rule looks like this:

```css
selector {
  property1: value1;
  property2: value2;
}
```

---

## 🧭 3. Text Alignment

The CSS `text-align` property controls how text is positioned horizontally inside an element.

```css
.h-center {
  text-align: center;
}
```

| Value    | Description                   |
| -------- | ----------------------------- |
| `center` | Aligns the text to the center |
| `left`   | Aligns the text to the left   |
| `right`  | Aligns the text to the right  |

---

## 🧪 4. Mini Project — Tourism Page

### `index.html`

```html
<!DOCTYPE html>
<html>
  <head>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <div class="h-center">
      <h1>Tourism</h1>
      <p>Plan your trip wherever you want to go</p>
      <button>Get Started</button>
    </div>
  </body>
</html>
```

### `styles.css`

```css
.h-center {
  text-align: center;
}
```

---

## ✅ Concepts Learned

- CSS connects HTML and style.
- Syntax: selector → property → value.
- Text alignment using `text-align`.
- External CSS with `<link>` tag.

---
