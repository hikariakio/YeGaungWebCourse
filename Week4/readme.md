# Week 4: Node.js Environment Setup

Welcome to **Week 4** of the **Ye Gaung Web Development Course**! This week, we'll be setting up the **Node.js environment**, a crucial component for executing JavaScript outside of the browser. Establishing Node.js is an important step towards utilizing modern JavaScript frameworks like React, which we will cover next week.

---

## Table of Contents

1. [Goal](#goal)
2. [Key Concepts](#key-concepts)
   - [1. What is Node.js?](#1-what-is-nodejs)
   - [2. Why Do We Need Node.js for React?](#2-why-do-we-need-nodejs-for-react)
   - [3. Installing Node.js](#3-installing-nodejs)
   - [4. Verifying Node.js and npm](#4-verifying-nodejs-and-npm)
3. [Activities](#activities)
   - [Activity 1: Running a Simple Node.js Script](#activity-1-running-a-simple-nodejs-script)
   - [Activity 2: Using npm to Install a Package](#activity-2-using-npm-to-install-a-package)
4. [Homework](#homework)
5. [Useful Resources](#useful-resources)

---

## Before the Class

1. **Task**: Install Node.js and npm on your system. (Refer to [Key Concepts](#key-concepts) for help)

---

## Goal

By the end of this week, you will:

- Understand what **Node.js** is and why it is significant for modern web development.
- Learn how to install and set up **Node.js** and **npm** (Node Package Manager) on your machine.
- Prepare your development environment for installing and running React.

---

## Key Concepts

### 1. What is Node.js?

Node.js is a **JavaScript runtime** that allows you to execute JavaScript code outside of a web browser. It is commonly used for building server-side applications, command-line tools, and various other applications. Node.js also includes npm, a package manager that helps you install and manage libraries and dependencies efficiently.

### 2. Why Do We Need Node.js for React?

React, like many modern JavaScript frameworks, relies on a **build toolchain** to compile and execute efficiently. Node.js provides the runtime environment required for running the development server, while npm is responsible for managing the installation of dependencies such as React, Webpack, and Babel.

### 3. Installing Node.js

Follow these steps to install Node.js on your system:

1. **Go to the Node.js website**: [https://nodejs.org](https://nodejs.org)
2. **Download the LTS version** (Long-Term Support), which is the most stable.
3. **Run the installer** and follow the instructions for your operating system:
   - **Windows**: Download the `.msi` file and run the installer.
   - **macOS**: Download the `.pkg` file and run the installer.
   - **Linux**: Use a package manager like `apt`, `yum`, or `dnf` to install Node.js.

### 4. Verifying Node.js and npm

After installing Node.js, verify your setup by following these steps:

1. **Open a terminal** (Command Prompt, PowerShell, or Terminal).
2. Run the following commands:
   ```bash
   node -v
   npm -v
   ```
   These commands will output the version numbers of Node.js and npm. If you see version numbers, it means the installation was successful.

---

## Activities

### Activity 1: Running a Simple Node.js Script

1. Create a new file named `app.js` and add the following code:
   ```javascript
   console.log("Node.js is successfully installed!");
   ```
2. Run the script using Node.js by typing the following command in your terminal:
   ```bash
   node app.js
   ```
3. You should see `Node.js is successfully installed!` printed in your terminal.

### Activity 2: Using npm to Install a Package

1. In your terminal, navigate to a project folder.

2. Initialize a new Node.js project by running:

   ```bash
   npm init -y
   ```

   This command will create a `package.json` file in your project, which tracks project dependencies.

3. Install a package using npm, for example:

   ```bash
   npm install lodash
   ```

4. Create a new file named `test.js` and use the installed package:

   ```javascript
   const _ = require('lodash');
   console.log(_.random(1, 100));
   ```

   Run the file using Node.js:

   ```bash
   node test.js
   ```

---

## Homework

1. **Task 1**: Create a Node.js script that prints the current date and time.
2. **Task 2**: Explore npm and install a package of your choice. Use it in a simple Node.js project.

---

## Useful Resources

1. **Node.js Official Website**: [https://nodejs.org/](https://nodejs.org/)
2. **npm Documentation**: [https://docs.npmjs.com/](https://docs.npmjs.com/)
3. **MDN Web Docs: Introduction to Node.js**: [https://developer.mozilla.org/en-US/docs/Learn/Server-side/Node\_server\_without\_framework](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Node_server_without_framework)

---

Happy coding! Node.js is an indispensable tool in modern web development, and mastering it will provide you with a strong foundation for building robust and scalable web applications.

