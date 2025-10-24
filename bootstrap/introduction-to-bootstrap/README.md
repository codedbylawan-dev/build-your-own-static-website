# 📘 Day 7 — Introduction to Bootstrap

**📅 Date:** October 24, 2025

---

## 🎯 Focus

To understand **Bootstrap basics**, **reusability of CSS**, and **predefined Bootstrap class names** for buttons, colors, and backgrounds.

---

## 🧠 Goal

Learn how to use **Bootstrap CDN**, apply **Bootstrap classes**, and explore **predefined reusable components** like buttons, text styles, and background utilities.

---

## 📝 Topics Covered

### 1. Reusability of CSS Rulesets

You can define a CSS ruleset once and reuse it across multiple HTML elements by assigning the same class.

```css
.button {
  width: 138px;
  height: 36px;
  border-width: 0px;
  border-radius: 10px;
}
```

```html
<button class="button">Get Started</button>
<button class="button">Visit Now</button>
```

---

### 2. Multiple Class Names in HTML

You can assign multiple class names separated by spaces to a single element.

```html
<button class="button button-green">Get Started</button>
```

```css
.button {
  width: 138px;
  height: 36px;
  border-width: 0px;
  border-radius: 10px;
}

.button-green {
  background-color: #8cc63f;
}
```

**Syntax:**

```html
<tag class="name1 name2 name3">Content</tag>
```

---

### 3. Bootstrap

**Definition:**
Bootstrap is a **large collection of predefined reusable code snippets** written in **HTML, CSS, and JavaScript** for building responsive web designs.

---

### 3.1 Using Bootstrap (CDN)

To use Bootstrap, include this **CDN link** inside the `<head>` element:

```html
<link
  rel="stylesheet"
  href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css"
/>
<script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/popper.js@1.16.1/dist/umd/popper.min.js"></script>
<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>
```

---

### 3.2 Predefined Styles in Bootstrap

#### 🟦 3.2.1 Buttons

To style buttons, use the **Bootstrap class** `btn`.

```html
<button class="btn btn-primary">Get Started</button>
<button class="btn btn-success">Visit Now</button>
```

**Outline Buttons:**
Replace `btn` with `btn-outline` to create buttons with outlines instead of solid colors.
Example:

```html
<button class="btn btn-outline-primary">Get Started</button>
```

---

#### 🟩 3.2.2 Text Colors

Bootstrap text color classes:

- `text-primary`
- `text-secondary`
- `text-success`
- `text-danger`
- `text-warning`
- `text-info`
- `text-light`
- `text-dark`

Example:

```html
<p class="text-primary">Tourism</p>
<p class="text-danger">Alert Message</p>
```

---

#### 🔠 3.2.3 Text Transform

Bootstrap provides text transform classes like:

- `text-uppercase`
- `text-lowercase`
- `text-capitalize`

Example:

```html
<p class="text-uppercase">plan your trip</p>
```

---

#### 🎨 3.2.4 Background Colors

Bootstrap background color classes:

- `bg-primary`
- `bg-secondary`
- `bg-success`
- `bg-danger`
- `bg-warning`
- `bg-info`

Example:

```html
<div class="bg-warning text-center">
  <h1 class="text-primary">Tourism</h1>
  <p class="text-lowercase">PLAN your TRIP.</p>
  <button class="btn btn-primary">Get Started</button>
</div>
```

---

### ⚠️ Note

Avoid using Bootstrap predefined class names (like `.btn`, `.card`, `.alert`) in your own CSS. It can cause **unexpected results**.

✅ **Do's**

```css
.button {
  border-radius: 5px;
  height: 50px;
  width: 138px;
  background-color: blue;
  color: white;
}
```

❌ **Don'ts**

```css
.btn {
  border-radius: 5px;
  height: 50px;
  width: 138px;
  background-color: blue;
  color: white;
}
```

---

## 📚 Learned Concepts

- Reusability of CSS rulesets
- Using multiple class names in HTML
- Bootstrap setup using CDN
- Predefined Bootstrap classes for buttons, text, and backgrounds
- Safe practices while using Bootstrap

---
