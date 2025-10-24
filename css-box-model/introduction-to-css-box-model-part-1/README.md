# 🧱 **Day 5 — CSS Box Model | Part 1**

📅 **Date:** October 25, 2025

---

## 🎯 **Focus**

Understanding and practicing the **CSS Box Model basics**, including element height, width, background image, and viewport units.

---

## 🥅 **Goal**

Learn how to:

- Control the **height and width** of elements.
- Apply **background images and sizes**.
- Understand **viewport units** (`vh` and `vw`) and how they affect layouts.

---

## 📘 **Concepts Learned**

### 1. **Height**

Defines how tall an element should be.

```css
.card {
  height: 200px;
}
```

---

### 2. **Width**

Defines how wide an element should be.

```css
.card {
  width: 250px;
}
```

---

### 3. **Background Image**

Specifies a background image for an element.

```css
.card {
  background-image: url("https://d2clawv67efefq.cloudfront.net/ccbp-static-website/ocean.jpg");
}
```

| **Value**  | **Description**       |
| ---------- | --------------------- |
| `url(URL)` | The URL to the image. |

⚠️ **Note:**

- A valid image URL is required.
- The image depends on the element’s height—if not specified, it might not appear properly.

---

### 4. **Background Size**

Controls how the background image fits inside the element.

```css
.card {
  background-size: cover;
}
```

| **Value** | **Description**                                                                 |
| --------- | ------------------------------------------------------------------------------- |
| `cover`   | Scales the image while maintaining aspect ratio and covers full width & height. |

---

### 5. **Viewport Units**

The visible browser area where content is displayed.

#### **Viewport Height (`vh`)**

```css
.card {
  height: 50vh;
}
```

1vh = 1% of the viewport height.
`height: 100vh` = fills the entire screen height.

#### **Viewport Width (`vw`)**

```css
.card {
  width: 100vw;
}
```

1vw = 1% of the viewport width.
`width: 100vw` = fills the entire screen width.

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
      <button>Get Started</button>
    </div>
  </body>
</html>
```

```css
.card {
  height: 50vh;
  width: 100vw;
  background-image: url("https://d2clawv67efefq.cloudfront.net/ccbp-static-website/ocean.jpg");
  background-size: cover;
}
```

---

## 🧠 **Learned Concepts Summary**

- `height` and `width` define element dimensions.
- `background-image` adds an image to an element.
- `background-size: cover` fits images nicely within the box.
- `vh` and `vw` units depend on the browser window size.

---
