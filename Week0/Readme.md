
# Week 0: Setting Up Your Development Environment

Welcome to Week 0 of the web development course! Before we dive into coding, we need to set up the right tools for web development. In this guide, you'll learn how to install and configure Visual Studio Code (VS Code), a popular code editor, along with some helpful extensions and resources to make your coding experience smooth and efficient.

---

## Table of Contents
1. [Installing Visual Studio Code (VS Code)](#installing-visual-studio-code)
2. [Setting Up Extensions in VS Code](#setting-up-extensions-in-vs-code)
    - Live Server
    - Prettier
    - HTML Boilerplate
    - Auto Rename Tag
    - CSS Peek
    - Bracket Pair Colorizer 2
    - IntelliSense for CSS Class Names in HTML
3. [Basic VS Code Usage](#basic-vs-code-usage)
4. [Useful Resources](#useful-resources)

---

## Installing Visual Studio Code

### Step 1: Download VS Code
- Go to the official Visual Studio Code website: [https://code.visualstudio.com/](https://code.visualstudio.com/)
- Download the version for your operating system:
  - **Windows**: Click on the "Windows" download button.
  - **macOS**: Click on the "macOS" download button.

## Setting Up Extensions in VS Code

Extensions in VS Code enhance your productivity and make development easier. Below are some essential extensions for HTML, CSS, and JavaScript development.

### 1. **Live Server**
- **Purpose**: Automatically refreshes your browser when you save your code. It provides a local development server with live reload capabilities.
- **Installation**:
   1. Open VS Code.
   2. Go to the Extensions tab on the left sidebar (or press `Ctrl + Shift + X`).
   3. Search for **Live Server** by _Ritwick Dey_ and click "Install".
- **Usage**: 
   1. Open any HTML file.
   2. Right-click on the file and select "Open with Live Server".
   3. Your browser will open, and you will see the webpage automatically update as you make changes in your code.
- **Link**: [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)

### 2. **Prettier - Code Formatter**
- **Purpose**: Automatically formats your code for better readability. It ensures consistent spacing, indentation, and line breaks.
- **Installation**:
   1. Go to the Extensions tab.
   2. Search for **Prettier** and click "Install".
- **Usage**:
   1. Format your code using `Shift + Alt + F`.
   2. Right-click on the file and modify your default formatter from `Format Document With`. 
   
- **Link**: [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)

### 3. **HTML Boilerplate**
- **Purpose**: Quickly generate a basic HTML template structure.
- **Installation**:
   1. Go to the Extensions tab.
   2. Search for **HTML Boilerplate** and click "Install".
- **Usage**:
   1. Inside an HTML file, type `html:5` and press `Tab`.
   2. This will generate a basic HTML structure.
- **Link**: [HTML Boilerplate](https://marketplace.visualstudio.com/items?itemName=sidthesloth.html5-boilerplate)

### 4. **Auto Rename Tag**
- **Purpose**: Automatically renames the closing HTML tag when you modify the opening tag.
- **Installation**:
   1. Go to the Extensions tab.
   2. Search for **Auto Rename Tag** and click "Install".
- **Usage**: 
   1. Edit the opening tag in an HTML element, and the closing tag will automatically update.
- **Link**: [Auto Rename Tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-rename-tag)

### 5. **CSS Peek**
- **Purpose**: Allows you to quickly navigate between HTML and CSS by showing where CSS classes are defined.
- **Installation**:
   1. Go to the Extensions tab.
   2. Search for **CSS Peek** and click "Install".
- **Usage**:
   1. Hold `Ctrl` and click on a CSS class name in an HTML file to jump to its definition in the CSS file.
- **Link**: [CSS Peek](https://marketplace.visualstudio.com/items?itemName=pranaygp.vscode-css-peek)

### 6. **Bracket Pair Color DLW**
- **Purpose**: Colorizes matching brackets to make nested structures easier to read.
- **Installation**:
   1. Go to the Extensions tab.
   2. Search for **Bracket Pair Color DLW** and click "Install".
- **Usage**: This extension automatically colorizes brackets and tags for better readability.
- **Link**: [Bracket Pair Color DLW](https://marketplace.visualstudio.com/items?itemName=BracketPairColorDLW.bracket-pair-color-dlw)

### 7. **IntelliSense for CSS Class Names in HTML**
- **Purpose**: Provides auto-completion for CSS class names in HTML files.
- **Installation**:
   1. Go to the Extensions tab.
   2. Search for **CSS Class IntelliSense** and click "Install".
- **Usage**:
   1. While typing class names in HTML files, this extension will suggest matching class names from your CSS files.
- **Link**: [CSS Class IntelliSense](https://marketplace.visualstudio.com/items?itemName=Zignd.html-css-class-completion)

---

## Basic VS Code Usage

Now that you’ve installed VS Code and the necessary extensions, here are some common tasks you'll perform:

### 1. **Creating a New File**
   - Press `Ctrl + N` to create a new file.
   - To save it, press `Ctrl + S` and give the file a name (e.g., `index.html`).

### 2. **Opening the Command Palette**
   - Press `Ctrl + Shift + P` to open the Command Palette, which allows you to access all of VS Code’s commands.
   
### 3. **Integrated Terminal**
   - Press `` Ctrl + Shift + ` `` to open VS Code's built-in terminal. This is useful for running commands like `npm start` when we get to React.
   
### 4. **Basic Shortcuts**
   - **Save**: `Ctrl + S`
   - **Open a file**: `Ctrl + O`
   - **Auto-format code**: `Alt + Shift + F`
   - **Search in files**: `Ctrl + Shift + F`

---

## Playing Around with the Code

Once you've installed the necessary extensions, you can test your setup by opening and editing the files in your project.

### Step 1: Open `index.html` and `styles.css`
- In your project folder, find and open the `index.html` and `styles.css` files.
- These files contain a basic webpage structure and some CSS for styling.

### Step 2: Use **Live Server**
- Right-click on the `index.html` file and choose **"Open with Live Server"**.
- This will open the webpage in your browser and automatically refresh whenever you save changes to your files.

### Step 3: Test Extensions
- **Live Server**: As you edit the HTML and CSS, watch your changes appear in real-time in the browser.
- **Prettier**: Save the file to see how Prettier automatically formats the HTML.
- **CSS Peek**: In `index.html`, hold `Ctrl` and click on a class name like `course-image` to jump to the relevant styles in `styles.css`.

Now, go ahead and play around with the code. Modify the content, style it, and watch how the extensions assist you in real-time!


---

## Useful Resources

Here are some websites and resources that will help you learn and practice HTML, CSS, and JavaScript:

1. **Mozilla Developer Network (MDN)** - The best documentation for HTML, CSS, and JavaScript.
   - [MDN Web Docs](https://developer.mozilla.org/en-US/)

2. **W3Schools** - A beginner-friendly platform for tutorials and references.
   - [W3Schools](https://www.w3schools.com/)

3. **CSS-Tricks** - Helpful CSS techniques and best practices.
   - [CSS-Tricks](https://css-tricks.com/)

4. **FreeCodeCamp** - Free interactive coding tutorials and exercises.
   - [FreeCodeCamp](https://www.freecodecamp.org/)

---

By the end of Week 0, you should have a fully set-up development environment and be familiar with how to use VS Code for writing and previewing your web projects. In the next session, we'll jump right into building webpages with HTML and CSS.

Happy coding!
