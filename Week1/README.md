
# Week 1: HTML + CSS (Basics)

Welcome to **Week 1** of the **Ye Gaung Web Development Course**! This week, we will dive into the basics of HTML and CSS—the core technologies for building web pages.

By the end of this week, you will be able to create a simple web page with proper structure and styling using HTML and CSS.

---

## Table of Contents

1. [Goal](#goal)
2. [Key Concepts](#key-concepts)
   - [1. HTML Structure](#1-html-structure)
   - [2. Essential HTML Tags](#2-essential-html-tags)
   - [3. Block vs Inline Elements](#3-block-vs-inline-elements)
   - [4. CSS Basics](#4-css-basics)
   - [5. Linking External CSS](#5-linking-external-css)
3. [Activities](#activities)
   - [Activity 1: Building a Simple Profile Page](#activity-1-building-a-simple-profile-page)
4. [Homework](#homework)
5. [Useful Resources](#useful-resources)
6. [Next Steps](#next-steps)

---

## Goal

The goal of this week is to:
- Introduce the foundational knowledge of HTML and CSS.
- Get comfortable building basic web pages.
- Understand the structure of HTML documents.
- Learn how to style HTML elements using CSS.

---

## Key Concepts

### 1. HTML Structure

- **HTML (HyperText Markup Language)** defines the structure of web content.
- Every HTML document starts with a **doctype declaration** and contains `<html>`, `<head>`, and `<body>` elements.

**Basic HTML Structure (Boilerplate):**

```html
<!doctype html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document Title</title>
  </head>
  <body>
    <!-- Content goes here -->
  </body>
</html>
```

### 2. Essential HTML Tags

- **Headings (`<h1>` - `<h6>`):** Define headings and subheadings.
- **Paragraphs (`<p>`):** Contain blocks of text.
- **Links (`<a>`):** Create hyperlinks to other pages.
- **Images (`<img>`):** Embed images.
- **Lists:**
  - **Unordered List (`<ul>`):** Bullet points.
  - **Ordered List (`<ol>`):** Numbered items.
  - **List Item (`<li>`):** Individual items in a list.
- **Forms (`<form>`, `<input>`):** Collect user input.

**Example:**

```html
<h1>This is a Heading</h1>
<p>This is a paragraph with some text.</p>
<a href="https://example.com">Visit Example.com</a>
<img src="image.jpg" alt="Sample Image">
<ul>
    <li>First Item</li>
    <li>Second Item</li>
</ul>
```

### 3. Block vs Inline Elements

- **Block-level Elements:** Start on a new line and take up the full width available.
  - Examples: `<div>`, `<h1>`, `<p>`, `<ul>`, `<li>`, `<form>`

- **Inline Elements:** Do not start on a new line and only take up as much width as necessary.
  - Examples: `<span>`, `<a>`, `<img>`, `<strong>`, `<em>`

### 4. CSS Basics

**CSS (Cascading Style Sheets)** is used to style and layout web pages. CSS can be added in three ways:

1. **Inline CSS:** Using the `style` attribute inside HTML tags.
   ```html
   <p style="color: blue;">This text is blue.</p>
   ```

2. **Internal CSS:** Within a `<style>` tag inside the `<head>` section.
   ```html
   <head>
       <style>
           p {
               color: blue;
           }
       </style>
   </head>
   ```

3. **External CSS:** Linking an external `.css` file using the `<link>` tag.
   ```html
   <head>
       <link rel="stylesheet" href="styles.css">
   </head>
   ```

### 5. Linking External CSS

If your codebase is large or shared across multiple pages, always link an external CSS file for better organization.

### Basic CSS Properties for Week 1

Below are some basic CSS properties that will help you style your HTML elements:

#### 1. **Color**

- The `color` property changes the text color of an element.

  **Example:**

  ```css
  p {
    color: blue;
  }
  ```

#### 2. **Font Size**

- The `font-size` property sets the size of the text.

  **Example:**

  ```css
  h1 {
    font-size: 24px;
  }
  ```

#### 3. **Background Color**

- The `background-color` property sets the background color of an element.

  **Example:**

  ```css
  body {
    background-color: #f0f0f0;
  }
  ```

#### 4. **Text Alignment**

- The `text-align` property aligns the text horizontally within an element.

  **Example:**

  ```css
  h1 {
    text-align: center;
  }
  ```

#### 5. **Margins and Padding**

- **Margin:** The `margin` property adds space outside of an element’s border.
- **Padding:** The `padding` property adds space inside of an element’s border.

  **Example:**

  ```css
  p {
    margin: 20px;
    padding: 10px;
  }
  ```

## Activities

### Activity 1: Building a Simple Profile Page

Create a simple profile page using the concepts learned. It should include headings, paragraphs, images, links, and basic CSS styling.

## Homework

1. Create a new HTML page that uses at least:
   - 3 headings (`<h1>`, `<h2>`, `<h3>`)
   - A paragraph (`<p>`)
   - An image (`<img>`)
   - A link (`<a>`)
   - Basic CSS for styling (color, background color, and font size)

## Useful Resources

- [HTML Documentation](https://developer.mozilla.org/en-US/docs/Web/HTML)
- [CSS Documentation](https://developer.mozilla.org/en-US/docs/Web/CSS)

## Next Steps

In **Week 2**, we'll explore more advanced CSS techniques and start building responsive layouts. Get ready to expand your web development toolkit!
