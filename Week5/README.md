## Week 5: React Setup Guide

### Overview

This week, we will focus on setting up the environment needed to start working with React. We'll go through the installation process step-by-step to ensure everything is properly configured so that you can start building applications using React. By the end of this guide, you will have a working environment for React and understand the basics of creating components.

### Objectives

- Install Node.js and npm (Node Package Manager)
- Understand the purpose of Node.js for React development
- Create a React project using Create React App
- Run the React development server
- Understand the role of `App.js` in a React application
- Create a basic functional React component
- Create a functional component that accepts `name` and `src` props to display an image

### Step 1: Install Node.js and npm

1. **Download Node.js**:

   - Go to [Node.js official website](https://nodejs.org/).
   - Download the LTS (Long Term Support) version of Node.js for your operating system. The LTS version is recommended because it is stable and well-supported.

2. **Install Node.js**:

   - Run the downloaded installer and follow the instructions.
   - Make sure to include npm (Node Package Manager) during the installation. npm is essential for managing the packages needed for React and other JavaScript development.

3. **Verify Installation**:

   - Open a terminal or command prompt.
   - Type the following commands to check if Node.js and npm are installed correctly:
     ```sh
     node -v
     npm -v
     ```
   - You should see version numbers for both Node.js and npm. If you do, the installation was successful.

### Step 2: Create a React Project

1. **Install Create React App** (optional step for global installation):

   - Create React App is a tool that sets up a new React project with all the required configuration.
   - You can install Create React App globally by running:
     ```sh
     npm install -g create-react-app
     ```
   - Installing globally allows you to use the `create-react-app` command anywhere, but this step is optional.

2. **Create Your React Project**:

   - Navigate to the directory where you want to create your project. You can do this using the `cd` command in your terminal.

   - Run the following command to create a new React application:

     ```sh
     npx create-react-app my-app
     ```

   - Replace `my-app` with your desired project name. The `npx` command allows you to run Create React App without needing to install it globally.

3. **Navigate to Your Project Folder**:

   - After the project is created, navigate to your project directory by running:
     ```sh
     cd my-app
     ```
   - This will move you into the folder where your new React project is located.

### Step 3: Run the React Development Server

1. **Start the Development Server**:

   - In your project directory, run:
     ```sh
     npm start
     ```
   - This will start the development server and automatically open your new React app in your default web browser.
   - The development server is set up to automatically reload whenever you make changes to your code, making it easier to see updates in real-time.

2. **Verify the Setup**:

   - You should see the default React welcome page, which typically says "Edit `src/App.js` and save to reload." This means everything is set up correctly, and you are ready to start building.

### Step 4: Project Structure Overview

When you create a new React project, you will notice several files and folders in your project directory. Here is a brief overview:

- ``: Contains static files like `index.html`. This folder is used for assets that need to be served as they are, without modification.
  - ``: The main HTML file that contains a `<div>` with an ID of `root`. This is where your entire React application will be injected.
- ``: Contains React components and JavaScript files. This is where most of your development will happen.
  - ``: The entry point for the React application. It renders the `App` component into the `root` element in `index.html`.
  - ``: A functional component that serves as the main component of the application.
- ``: Lists dependencies, scripts, and other metadata for your project. It helps npm manage your project’s packages.

### Understanding `App.js`

The `App.js` file is the main component of your React application. It is the root component where all other components are eventually included. By default, `App.js` contains basic code to render a simple user interface.

- **Importing Dependencies**: At the top of `App.js`, React is imported along with other necessary dependencies. For example:

  ```js
  import React from 'react';
  import './App.css';
  ```

  The `React` import is necessary for any JSX code you write, while `./App.css` is used for styling the component.

- **App Component**: The `App` component is a functional component, meaning it is written as a JavaScript function that returns JSX (JavaScript XML). JSX is a syntax extension that allows you to write HTML-like code in JavaScript, which will be compiled to regular JavaScript by tools like Babel.

  ```js
  function App() {
    return (
      <div className="App">
        <h1>Welcome to React</h1>
      </div>
    );
  }
  ```

  This `App` component renders a `<div>` with a class name of `App`, and inside it, an `<h1>` element. You can modify this to change what is displayed on the screen.

- **Exporting the Component**: At the bottom of `App.js`, the `App` component is exported:

  ```js
  export default App;
  ```

  This allows other files to import and use the `App` component. For example, `index.js` imports `App` to render it to the DOM.

As you build your application, you will add more components to `App.js` or link them to keep the application organized and modular.

### Step 5: Create a Basic Functional Component

1. **Create a New Component**:

   - In the `src/` folder, create a new file called `Hello.js`.
   - This new file will contain a functional component. Add the following code to `Hello.js`:
     ```js
     import React from 'react';

     function Hello() {
       return (
         <div>
           <h1>Hello, React!</h1>
         </div>
       );
     }

     export default Hello;
     ```
   - Here, `Hello` is a functional component that returns a `<div>` containing an `<h1>` element with the text "Hello, React!".

2. **Use the Component in Your App**:

   - Open `src/App.js`.
   - To use the `Hello` component, you first need to import it by adding the following line at the top of `App.js`:
     ```js
     import Hello from './Hello';
     ```
   - Then, include the `Hello` component inside the `App` component’s return statement:
     ```js
     function App() {
       return (
         <div className="App">
           <Hello />
         </div>
       );
     }

     export default App;
     ```
   - This will render the `Hello` component inside the `App` component, and you should see "Hello, React!" displayed on the screen.

3. **Save and Check the Browser**:

   - After saving the changes, the development server should automatically reload. Open your browser, and you should see the updated page displaying "Hello, React!".

### Step 6: Create a Functional Component That Accepts `name` and `src` Props to Display an Image

1. **Create a New Component**:

   - In the `src/` folder, create a new file called `MyImage.js`.
   - This new file will contain a functional component that accepts `name` and `src` props to display an image. Add the following code to `MyImage.js`:
     ```js
     import React from 'react';

     function MyImage(props) {
       return (
         <div>
           <img src={props.src} alt={props.name} />
           <p>{props.name}</p>
         </div>
       );
     }

     export default MyImage;
     ```
   - The `MyImage` component accepts `name` and `src` props. It displays an image with the provided `src` and uses the `name` as both the `alt` text for accessibility and as a caption below the image.

2. **Use the Component in Your App**:

   - Open `src/App.js`.

   - Import the `MyImage` component by adding the following line at the top of `App.js`:

     ```js
     import MyImage from './MyImage';
     ```

   - Then, include the `MyImage` component inside the `App` component’s return statement and pass `name` and `src` props to it:

     ```js
     function App() {
       return (
         <div className="App">
           <Hello />
           <MyImage name="Image1" src="https://picsum.photos/id/237/200/200" />
         </div>
       );
     }

     export default App;
     ```

   - This will render the `MyImage` component inside the `App` component, and you should see an image along with the caption "Image1" displayed on the screen.

3. **Save and Check the Browser**:

   - After saving the changes, the development server should automatically reload. Open your browser, and you should see the updated page displaying the image along with the caption "Image1".

### Tips

- If you encounter any errors, make sure all dependencies are properly installed and try running `npm install` again. This command will install any missing packages listed in
