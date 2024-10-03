
# Week 3: Bootstrap (Deep Dive)

Welcome to **Week 3** of the **Ye Gaung Web Development Course**! This week, we will dive deeper into **Bootstrap**, focusing on using the grid system to create responsive layouts. You will learn how to structure web pages using rows and columns, which are core concepts of Bootstrap.

---

## Table of Contents

1. [Goal](#goal)
2. [Key Concepts](#key-concepts)
   - [1. Bootstrap Grid System](#1-bootstrap-grid-system)
   - [2. Responsive Layouts with Rows and Columns](#2-responsive-layouts-with-rows-and-columns)
   - [3. Using Bootstrap Classes](#3-using-bootstrap-classes)
3. [Activities](#activities)
4. [Homework](#homework)
5. [Useful Resources](#useful-resources)

---

## Goal

By the end of this week, you will:
- Understand how to use Bootstrap’s grid system to create responsive layouts.
- Use rows and columns to build structured web pages.
- Apply basic Bootstrap classes for styling.

---

## Key Concepts

### 1. Bootstrap Grid System

Bootstrap’s grid system is based on a 12-column layout, which means each row can hold up to 12 columns. You can divide the row into multiple columns, each taking up a portion of the available width.

- The **container** class wraps your content and provides padding for it.
- The **row** class creates a horizontal group of columns.
- The **col** classes create columns inside a row.

### 2. Responsive Layouts with Rows and Columns

Bootstrap makes it easy to create layouts that adjust automatically to different screen sizes. The columns you create using the **col-** classes will resize based on the screen size.

**Example of a 3-column layout:**
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

You can also specify how many columns each div should take up on different screen sizes. For example:

```html
<div class="container">
  <div class="row">
    <div class="col-md-6 col-lg-4">
      Column 1 (Takes up 6 columns on medium screens, 4 columns on large screens)
    </div>
    <div class="col-md-6 col-lg-4">
      Column 2 (Takes up 6 columns on medium screens, 4 columns on large screens)
    </div>
    <div class="col-md-6 col-lg-4">
      Column 3 (Takes up 6 columns on medium screens, 4 columns on large screens)
    </div>
  </div>
</div>
```

### 3. Using Bootstrap Classes

Here are some useful Bootstrap classes you can use in your layouts:

- **Container**: Wraps your content and adds padding.
  ```html
  <div class="container">Your content here</div>
  ```
  
- **Row**: Groups columns together horizontally.
  ```html
  <div class="row">Your columns go here</div>
  ```
  
- **Columns**: Create responsive columns inside a row using **col**, **col-sm**, **col-md**, **col-lg**, and **col-xl** classes, depending on the screen size.
  ```html
  <div class="col-md-4">This column takes up 4 out of 12 columns on medium screens</div>
  ```

---

## Activities

### Activity 1: Building a Basic Responsive Page

1. Create a new HTML file and link the Bootstrap CDN.
2. Use the Bootstrap grid system to create a layout with 3 sections:
   - A **header** section with a title.
   - A **content** section with 3 columns (each column should have some text or images).
   - A **footer** section with contact information.

**Example HTML**:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Week 3: Bootstrap Grid</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>

    <div class="container">
        <header class="row">
            <div class="col">
                <h1 class="text-center">My Bootstrap Page</h1>
            </div>
        </header>

        <main class="row">
            <div class="col-md-4">
                <h2>Column 1</h2>
                <p>This is the first column of the page content.</p>
            </div>
            <div class="col-md-4">
                <h2>Column 2</h2>
                <p>This is the second column of the page content.</p>
            </div>
            <div class="col-md-4">
                <h2>Column 3</h2>
                <p>This is the third column of the page content.</p>
            </div>
        </main>

        <footer class="row">
            <div class="col text-center">
                <p>&copy; 2024 My Bootstrap Page</p>
            </div>
        </footer>
    </div>

</body>
</html>
```

- The layout should be responsive. On smaller screens, the columns will stack on top of each other.

### Activity 2: Experiment with Different Grid Layouts

1. Try creating layouts with 2 columns, 4 columns, or a mix of column sizes.
2. Use **col-md-6**, **col-lg-3**, etc., to control how many columns each div should take up at different screen sizes.

---

## Homework

1. **Task 1**: Create a responsive webpage with a header, main content area (with multiple columns), and a footer.
2. **Task 2**: Explore Bootstrap’s **container-fluid** class and use it to create a full-width layout.
3. **Task 3**: Use Bootstrap’s typography classes (like **text-center**, **text-left**) to style your text.

---

## Useful Resources

1. **Bootstrap Official Documentation**: [https://getbootstrap.com/](https://getbootstrap.com/)
2. **MDN Web Docs on CSS**: [https://developer.mozilla.org/en-US/docs/Web/CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)
3. **W3Schools Bootstrap Tutorial**: [https://www.w3schools.com/bootstrap5/](https://www.w3schools.com/bootstrap5/)

---

Happy coding! This week is all about creating responsive, well-structured web pages using Bootstrap’s powerful grid system.
