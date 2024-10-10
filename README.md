# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

- I install the tailwind package via `npm create vite@latest` after selecting the modules for my template

<!-- how to install node js, vite & tailwind -->

# **node js:**

- download the installer package online
- run the installer
- check the version using command prompt line “node -v”

# **vite:**

- installed vite using the command line “npm install vite@latest”
- using the vite template module create a react package named Fundme*

/* packaged can be named whatever, edit to your taste/project need */

# **tailwind:**

- installed tailwind css using the following [command lines](https://tailwindcss.com/docs/guides/vite)
1. **Install Tailwind CSS**
    
    Install **`tailwindcss`** and its peer dependencies, then generate your **`tailwind.config.js`** and **`postcss.config.js`** files.
    
    Terminal
    
    `npm install -D tailwindcss postcss autoprefixernpx` 
    
    `tailwindcss init -p`
    
2. **Configure your template paths**
    
    Add the paths to all of your template files in your **`tailwind.config.js`** file.
    
    tailwind.config.js
    
    `~~/** @type {import('tailwindcss').Config} */
    export default {~~
      content: [
        "./index.html",
        "./src/**/*.{js,ts,jsx,tsx}",
      ],
      ~~theme: {
        extend: {},
      },
      plugins: [],
    }~~`
    
3. **Add the Tailwind directives to your CSS**
    
    Add the **`@tailwind`** directives for each of Tailwind’s layers to your **`./src/index.css`** file.
    
    index.css
    
    `@tailwind base;`
    
    `@tailwind components;`
    
    `@tailwind utilities;`
    
4. **Start your build process**
    
    Run your build process with **`npm run dev`**.
    
    Terminal
    
    `npm run dev`
    
5. **Start using Tailwind in your project**
    
    Start using Tailwind’s utility classes to style your content.
    
    App.jsx
    
    `export default function App() {
      return (
        <h1 className="text-3xl font-bold underline">
          Hello world!
        </h1>
      )
    }`