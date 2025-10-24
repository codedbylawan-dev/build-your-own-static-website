# 🧱 **Day 6 — CSS Box Model | Part 2**

📅 **Date:** October 26, 2025

---

## 🎯 **Focus**

Learn how to style borders, corners, padding, and colors in CSS to enhance the look and spacing of elements.

---

## 🥅 **Goal**

Understand and apply:

- **Borders** (width, style, color, radius)
- **Padding** (space inside elements)
- **Hex codes** for colors in CSS

---

## 📘 **Concepts Learned**

### 1. **Border Width**

Specifies the thickness of borders around an HTML element.

```css
.button {
  border-width: 2px;
}
```

🧠 **Tip:**
`border-width: 0px;` removes the border completely.

⚠️ **Warning:**
To make `border-width` visible, you must define `border-style`.
(_HTML `<button>` has default border styling._)

---

### 2. **Border Radius**

Defines how rounded the corners of an element should be.

```css
.button {
  border-radius: 20px;
}
```

| **Property**                 | **Usage**                  |
| ---------------------------- | -------------------------- |
| `border-top-left-radius`     | Rounds top-left corner     |
| `border-top-right-radius`    | Rounds top-right corner    |
| `border-bottom-left-radius`  | Rounds bottom-left corner  |
| `border-bottom-right-radius` | Rounds bottom-right corner |

🧠 **Quick Tip:**
Add a background color to see the border radius effect clearly.

---

### 3. **Border Color**

Sets the color of the borders.

```css
.button {
  border-color: orange;
}
```

⚠️ **Warning:**
Just like `border-width`, this requires `border-style` to be visible.

---

### 4. **Border Style**

Specifies the appearance of borders (solid, dashed, dotted, etc.).

```css
.button {
  border-style: dashed;
}
```

| **Value** | **Description**     |
| --------- | ------------------- |
| `dotted`  | Dotted border       |
| `dashed`  | Dashed border       |
| `solid`   | Solid border        |
| `none`    | No border (default) |

---

### 5. **Padding**

Defines the space between an element’s content and its border.

```css
.card {
  padding: 10px;
}
```

---

### 6. **CSS Colors — Hex Codes**

CSS supports multiple color formats — **color names, RGB, HSL, Hex**, etc.
Hex codes are a popular way to pick specific shades.

| **Color Name** | **Hex Code** |
| -------------- | ------------ |
| orange         | `#ffa500`    |
| red            | `#ff0000`    |
| blue           | `#0000ff`    |
| green          | `#008000`    |
| —              | `#012d36`    |
| —              | `#432711`    |
| —              | `#25b1cc`    |

```css
.button {
  background-color: #25b1cc;
}
```

🧭 **Tip:**
Use Google’s **Color Picker** by typing “color picker” in the search bar to explore 16 million+ colors.

---

## 🧩 **Mini Project**

```html
<!DOCTYPE html>
<html>
  <head></head>
  <body>
    <div class="card">
      <h1>Tourism</h1>
      <p>Plan your trip wherever you want to go</p>
      <button class="button">Get Started</button>
    </div>
  </body>
</html>
```

```css
.button {
  border-width: 2px;
  border-style: solid;
  border-color: #25b1cc;
  border-radius: 20px;
  background-color: #25b1cc;
  padding: 10px 20px;
}
```

---

## 🧠 **Learned Concepts Summary**

- `border-width`, `border-color`, `border-style`, and `border-radius` shape and color an element’s border.
- `padding` adds space inside the element.
- Hex codes like `#25b1cc` allow precise color selection.
- Always specify `border-style` for borders to appear.

---

Would you like me to prepare **Day 7 — CSS Box Model | Part 3 (Margin, Outline, Box Shadow, Display, Positioning)** in the same format next?
