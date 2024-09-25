
# Week 2: CSS + Bootstrap (Responsive Design Basics)

Welcome to **Week 2** of the **Ye Gaung Web Development Course**! This week, we will build on our knowledge of CSS by introducing more advanced selectors like IDs and class names. We will also introduce **Bootstrap**, a popular CSS framework, and how to link it via a CDN.

---

## Table of Contents

1. [Goal](#goal)
2. [Key Concepts](#key-concepts)
    - [1. CSS Selectors: IDs and Class Names](#1-css-selectors-ids-and-class-names)
    - [2. Introducing Bootstrap](#2-introducing-bootstrap)
    - [3. Adding Bootstrap via CDN](#3-adding-bootstrap-via-cdn)
3. [Activities](#activities)
4. [Homework](#homework)
5. [Useful Resources](#useful-resources)

---

## Goal

By the end of this week, you will:
- Understand how to use CSS **IDs** and **class names** to target specific HTML elements.
- Learn the basics of **Bootstrap** and how to add it to your project using a CDN.

---

## Key Concepts

### 1. CSS Selectors: IDs and Class Names

In CSS, we can style specific elements using **IDs** and **class names**. This gives us more flexibility to target individual elements or groups of elements.

#### ID Selectors
- IDs are unique and should only be used for a single element on a page.
- To target an element by ID, use the `#` symbol followed by the ID name.

**Example:**

```html
<p id="intro">This is an introduction paragraph.</p>
```

```css
#intro {
    color: green;
    font-weight: bold;
}
```

- The above CSS rule will make the text inside the element with `id="intro"` green and bold.

#### Class Selectors
- Classes can be reused for multiple elements on a page.
- To target an element by class name, use the `.` (dot) symbol followed by the class name.

**Example:**

```html
<p class="highlight">This is highlighted text.</p>
<p class="highlight">This is another highlighted paragraph.</p>
```

```css
.highlight {
    background-color: yellow;
    font-style: italic;
}
```

- Both paragraphs with the class `highlight` will have a yellow background and italic text.

### 2. Introducing Bootstrap

**Bootstrap** is a popular CSS framework that helps you build responsive, mobile-first websites quickly. It comes with pre-built CSS classes for layout, typography, buttons, and more.

Some key features of Bootstrap include:
- **Grid System**: Helps create flexible and responsive layouts using rows and columns.
- **Typography and Utilities**: Provides ready-to-use classes for styling text, aligning elements, and spacing.
- **Pre-styled Components**: Bootstrap includes components like buttons, forms, navigation bars, and more, which are already styled and easy to customize.

### 3. Adding Bootstrap via CDN

To start using Bootstrap, you don’t need to download any files. You can link to it directly using a **Content Delivery Network (CDN)**.

#### How to Add Bootstrap via CDN

1. Go to the `<head>` section of your HTML file.
2. Add the following `<link>` tag to include Bootstrap:

```html
<head>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-ENjdO4Dr2bkBIFxQpeoYT1FIs9hoxfa6b0z4F6I1VUoy3PVlEVmb5d5F5yN6v0H" crossorigin="anonymous">
</head>
```

3. Now, you can start using Bootstrap classes in your HTML elements.

---

## Activities

### Activity 1: Using CSS IDs and Classes

1. Create an HTML file with different elements (paragraphs, headings, and lists).
2. Add unique IDs to some elements and class names to others.
3. Style those elements using the `#` for IDs and `.` for class names in your CSS file.

**Example HTML:**

```html
<h1 id="main-heading">Welcome to My Website</h1>
<p class="highlight">This is a highlighted paragraph.</p>
<p class="highlight">This is another highlighted paragraph.</p>
```

**Example CSS:**

```css
#main-heading {
    color: blue;
    text-align: center;
}

.highlight {
    background-color: yellow;
    font-style: italic;
}
```

### Activity 2: Adding Bootstrap to Your Page

1. Add Bootstrap to your HTML page via CDN.
2. Create a simple layout using Bootstrap’s grid system. Use `col` classes to create responsive columns.

**Example Bootstrap Layout:**

```html
<div class="container">
    <div class="row">
        <div class="col">
            Column 1
        </div>
        <div class="col">
            Column 2
        </div>
        <div class="col">
            Column 3
        </div>
    </div>
</div>
```

- The columns will stack on smaller screens and sit side by side on larger screens.

---

## Homework

1. **Task 1**: Use IDs and class names to style various elements in your webpage.
2. **Task 2**: Add Bootstrap to your project using the CDN link and create a responsive layout with at least 3 columns.
3. **Task 3**: Explore Bootstrap’s typography and components by using pre-built classes for headings, buttons, and forms.

---

## Useful Resources

1. **Bootstrap Official Documentation**: [https://getbootstrap.com/](https://getbootstrap.com/)
2. **MDN Web Docs on CSS**: [https://developer.mozilla.org/en-US/docs/Web/CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)
3. **W3Schools Bootstrap Tutorial**: [https://www.w3schools.com/bootstrap5/](https://www.w3schools.com/bootstrap5/)

---

Happy coding! Feel free to experiment with Bootstrap’s grid system and components to build your first responsive webpage.
