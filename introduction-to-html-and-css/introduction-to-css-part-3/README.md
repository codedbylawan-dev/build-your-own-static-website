# 🎨 CSS — Day 4

**Date:** October 23, 2025

**Focus:** Font Properties & Text Decorations

**Goal:** Learn how to customize text appearance using font-family, size, style, weight, and decoration.

---

## 🖋️ 1. Font Family

The CSS `font-family` property specifies the **font** used for an element.

```css
@import url("https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap");

.main-heading {
  font-family: "Roboto";
}

.paragraph {
  font-family: "Roboto";
}
```

### 🧠 Notes

- To use external fonts, **import** them from Google Fonts or other sources.
- Always use **quotes** around font names.
- Check for **spelling mistakes** — they can break your font styles.

### ✅ Valid Value Example

`"Roboto"`

---

## 🔠 2. Font Size

The CSS `font-size` property specifies the **size of the font**.

```css
.main-heading {
  font-size: 36px;
}

.paragraph {
  font-size: 28px;
}
```

### 🧠 Notes

- Always use **px** (pixels) for font size unless using responsive units like `em` or `rem`.
- No spaces between the number and `px`.
- No quotes around the value.

---

## ✍️ 3. Font Style

The CSS `font-style` property specifies the **style** of the text.

Possible values:

| Value   | Description           |
| ------- | --------------------- |
| normal  | Default text          |
| italic  | Slanted text          |
| oblique | Slightly slanted text |

```css
.main-heading {
  font-style: italic;
}

.paragraph {
  font-style: normal;
}
```

---

## 🧱 4. Font Weight

The CSS `font-weight` property controls **how thick or thin** the text looks.

```css
.main-heading {
  font-weight: bold;
}

.paragraph {
  font-weight: 200;
}
```

### 🧠 Notes

- Can use **keywords** like `normal`, `bold`, or numeric values from **100–900**.
- Values must be **multiples of 100**.

---

## 🌈 5. Text Decoration

The CSS `text-decoration` property adds **decorative styles** to text.

```css
.main-heading {
  text-decoration: underline;
}

.paragraph {
  text-decoration: overline;
}
```

| Value        | Description                |
| ------------ | -------------------------- |
| underline    | Underlines the text        |
| line-through | Strikes through the text   |
| overline     | Adds a line above the text |

### 🧠 Notes

- Use hyphenated values (e.g., `line-through`).
- No quotes required.
- Check spelling carefully.

---

## 🧪 6. Mini Project — Tourism Page (Font Styling)

### `index.html`

```html
<!DOCTYPE html>
<html>
  <head>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <h1 class="main-heading">Tourism</h1>
    <p class="paragraph">Plan your trip wherever you want to go</p>
  </body>
</html>
```

### `styles.css`

```css
@import url("https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap");

.main-heading {
  font-family: "Roboto";
  font-size: 36px;
  font-style: italic;
  font-weight: bold;
  text-decoration: underline;
}

.paragraph {
  font-family: "Roboto";
  font-size: 28px;
  font-style: normal;
  font-weight: 200;
  text-decoration: overline;
}
```

---

## ✅ Concepts Learned

- `font-family` → sets font type.
- `font-size` → sets text size.
- `font-style` → controls italic or normal style.
- `font-weight` → controls boldness.
- `text-decoration` → adds underline, overline, or strike-through.

---

## 🧭 Next Step (Day 5 Preview)

**Topic:** CSS Box Model

You’ll learn:

- Margin, Padding, and Border
- Height & Width
- Background and Box Layout Practice
- Mini Project: _Tourism Info Card Layout_

---
