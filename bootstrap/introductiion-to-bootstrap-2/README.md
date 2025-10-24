# 📘 Day 8 — Flexbox Properties

**Date:** October 25, 2025

---

## 🎯 Focus

To understand **Bootstrap Flexbox properties**, including how to define a Flexbox container, set directions, and align items using `justify-content` classes.

---

## 🧠 Goal

Learn to control the **layout and alignment of elements** in Bootstrap using **Flexbox utilities** like `d-flex`, `flex-row`, `flex-column`, and `justify-content-*` classes.

---

## 📝 Topics Covered

### 1. Flexbox Container

The Bootstrap class `d-flex` defines a **Flexbox container**.
The direct child elements of this container are called **flex items**.

```html
<div class="d-flex">
  <div>
    <h1>Tourism</h1>
    <p>Plan your trip.</p>
    <button>Get Started</button>
  </div>
</div>
```

- The element with `class="d-flex"` is the **Flexbox container**.
- The direct child `<div>` is the **flex item**.
- Nested elements like `<h1>`, `<p>`, and `<button>` are **not flex items** because they’re not direct children.

> **Note:** Wrapping elements inside a Flexbox container is **mandatory** to apply Flexbox properties.

---

### 2. Flex Direction

Specifies the **direction of flex items** within the Flexbox container.

| Class Name    | Direction of Flex Items |
| ------------- | ----------------------- |
| `flex-row`    | Horizontal (Default)    |
| `flex-column` | Vertical                |

#### 🟦 2.1 `flex-row`

Moves the flex items **horizontally**.

```html
<div class="d-flex flex-row">
  <div>
    <h1>Tourism</h1>
    <p>Plan your trip.</p>
    <button>Get Started</button>
  </div>
</div>
```

#### 🟩 2.2 `flex-column`

Moves the flex items **vertically**.

```html
<div class="d-flex flex-column">
  <div>
    <h1>Tourism</h1>
    <p>Plan your trip.</p>
    <button>Get Started</button>
  </div>
</div>
```

> **Note:** `flex-row` is the default direction for Flexbox in Bootstrap.

---

### 3. Justify Content

Used to **align flex items** along the **main axis** (based on Flex Direction).

| Class Name                | Description                                    |
| ------------------------- | ---------------------------------------------- |
| `justify-content-start`   | Aligns items at the **start**                  |
| `justify-content-center`  | Aligns items at the **center**                 |
| `justify-content-end`     | Aligns items at the **end**                    |
| `justify-content-between` | Distributes items with **equal space between** |

---

#### 3.1 `justify-content-start`

Aligns items at the **start** of the container.

```html
<div class="d-flex flex-column justify-content-start">
  <div>
    <h1>Tourism</h1>
    <p>Plan your trip.</p>
    <button>Get Started</button>
  </div>
</div>
```

| Flex Direction | Alignment |
| -------------- | --------- |
| `flex-row`     | Left      |
| `flex-column`  | Top       |

---

#### 3.2 `justify-content-center`

Centers the flex items within the container.

```html
<div class="d-flex flex-column justify-content-center">
  <div>
    <h1>Tourism</h1>
    <p>Plan your trip.</p>
    <button>Get Started</button>
  </div>
</div>
```

| Flex Direction | Alignment           |
| -------------- | ------------------- |
| `flex-row`     | Center (Horizontal) |
| `flex-column`  | Center (Vertical)   |

---

#### 3.3 `justify-content-end`

Aligns flex items at the **end** of the container.

```html
<div class="d-flex flex-column justify-content-end">
  <div>
    <h1>Tourism</h1>
    <p>Plan your trip.</p>
    <button>Get Started</button>
  </div>
</div>
```

| Flex Direction | Alignment |
| -------------- | --------- |
| `flex-row`     | Right     |
| `flex-column`  | Bottom    |

---

## Mini Project

```html
<!DOCTYPE html>
<html>
  <head>
    <link
      rel="stylesheet"
      href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css"
      integrity="sha384-JcKb8q3iqJ61gNV9KGb8thSsNjpSL0n8PARn9HuZOnIxN0hoP+VmmDGMN5t9UJ0Z"
      crossorigin="anonymous"
    />
    <script
      src="https://code.jquery.com/jquery-3.5.1.slim.min.js"
      integrity="sha384-DfXdz2htPH0lsSSs5nCTpuj/zy4C+OGpamoFVy38MVBnE+IbbVYUew+OrCXaRkfj"
      crossorigin="anonymous"
    ></script>
    <script
      src="https://cdn.jsdelivr.net/npm/popper.js@1.16.1/dist/umd/popper.min.js"
      integrity="sha384-9/reFTGAW83EW2RDu2S0VKaIzap3H66lZH81PoYlFhbGU+6BZp6G7niu735Sk7lN"
      crossorigin="anonymous"
    ></script>
    <script
      src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"
      integrity="sha384-B4gt1jrGC7Jh4AgTPSdUtOBvfO8shuf57BaghqFfPlYxofvL8/KUEfYiJOMMV+rV"
      crossorigin="anonymous"
    ></script>
  </head>
  <body>
    <div class="bg-container d-flex flex-column justify-content-end">
      <div class="tourism-card">
        <h1 class="main-heading">Tourism</h1>
        <p class="paragraph">Plan your trip.</p>
        <button class="button">Get Started</button>
      </div>
    </div>
  </body>
</html>
```

```css
@import url("https://fonts.googleapis.com/css2?family=Bree+Serif&family=Caveat:wght@400;700&family=Lobster&family=Monoton&family=Open+Sans:ital,wght@0,400;0,700;1,400;1,700&family=Playfair+Display+SC:ital,wght@0,400;0,700;1,700&family=Playfair+Display:ital,wght@0,400;0,700;1,700&family=Roboto:ital,wght@0,400;0,700;1,400;1,700&family=Source+Sans+Pro:ital,wght@0,400;0,700;1,700&family=Work+Sans:ital,wght@0,400;0,700;1,700&display=swap");

.bg-container {
  background-image: url("https://d2clawv67efefq.cloudfront.net/ccbp-static-website/ocean.jpg");
  height: 100vh;
  background-size: cover;
}
.tourism-card {
  text-align: center;
  background-color: white;
  padding: 5px;
  border-top-left-radius: 25px;
  border-top-right-radius: 25px;
}
.main-heading {
  font-family: "Roboto";
}
.paragraph {
  font-family: "Roboto";
}
.button {
  color: white;
  background-color: #25b1cc;
  width: 138px;
  height: 36px;
  border-width: 0px;
  border-radius: 20px;
}
```

#### 3.4 `justify-content-between`

Places equal space **between** flex items.

```html
<div class="d-flex flex-column justify-content-between">
  <div>
    <h1>Tourism</h1>
    <p>Plan your trip.</p>
    <button>Get Started</button>
  </div>
</div>
```

| Flex Direction | Alignment                |
| -------------- | ------------------------ |
| `flex-row`     | Equal horizontal spacing |
| `flex-column`  | Equal vertical spacing   |

---

**Example:**

```html
<!DOCTYPE html>
<html>
  <head>
    <link
      rel="stylesheet"
      href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css"
      integrity="sha384-JcKb8q3iqJ61gNV9KGb8thSsNjpSL0n8PARn9HuZOnIxN0hoP+VmmDGMN5t9UJ0Z"
      crossorigin="anonymous"
    />
    <script
      src="https://code.jquery.com/jquery-3.5.1.slim.min.js"
      integrity="sha384-DfXdz2htPH0lsSSs5nCTpuj/zy4C+OGpamoFVy38MVBnE+IbbVYUew+OrCXaRkfj"
      crossorigin="anonymous"
    ></script>
    <script
      src="https://cdn.jsdelivr.net/npm/popper.js@1.16.1/dist/umd/popper.min.js"
      integrity="sha384-9/reFTGAW83EW2RDu2S0VKaIzap3H66lZH81PoYlFhbGU+6BZp6G7niu735Sk7lN"
      crossorigin="anonymous"
    ></script>
    <script
      src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"
      integrity="sha384-B4gt1jrGC7Jh4AgTPSdUtOBvfO8shuf57BaghqFfPlYxofvL8/KUEfYiJOMMV+rV"
      crossorigin="anonymous"
    ></script>
  </head>
  <body>
    <div class="d-flex flex-column justify-content-between box-container">
      <div class="box box-orange"><p>Box 1</p></div>
      <div class="box box-green"><p>Box 2</p></div>
    </div>
  </body>
</html>
```

```css
@import url("https://fonts.googleapis.com/css2?family=Bree+Serif&family=Caveat:wght@400;700&family=Lobster&family=Monoton&family=Open+Sans:ital,wght@0,400;0,700;1,400;1,700&family=Playfair+Display+SC:ital,wght@0,400;0,700;1,700&family=Playfair+Display:ital,wght@0,400;0,700;1,700&family=Roboto:ital,wght@0,400;0,700;1,400;1,700&family=Source+Sans+Pro:ital,wght@0,400;0,700;1,700&family=Work+Sans:ital,wght@0,400;0,700;1,700&display=swap");

.box {
  width: 100px;
  height: 100px;
  color: white;
}
.box-orange {
  background-color: orange;
}
.box-green {
  background-color: green;
}
.box-container {
  width: 100vw;
  height: 100vh;
}
```

---

## 📚 Learned Concepts

- `d-flex` creates a Flexbox container.
- `flex-row` and `flex-column` define item direction.
- `justify-content-*` classes control alignment (start, center, end, between).
- Default direction for Flexbox in Bootstrap is **`flex-row`**.
- Wrapping elements inside a Flex container is essential to apply these properties.

---
