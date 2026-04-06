# Vibe Coding 101

> [!NOTE]
> I've marked some sections of this guide as "Edited by AI" because I used AI tools to help me with the writing and editing process. I wanted to make it clear which parts were generated or edited by AI and which parts were written by me. This is just to be transparent about the use of AI in the creation of this guide.

---

# HOW TO VIBE CODE AND CREATE BEAUTIFUL WEBSITES

This is a guide to help you vibe code and create beautiful websites. It covers how to make website using React, Vite, Tailwind CSS, as well as some tips and tricks to make your coding experience more enjoyable.

---

## Prerequisites

- Find your niche and research the topic a little to know your competitors.
- Explore others' websites to get to know what they have to offer
- Find a gap that they are missing, and try to improve or work on that
- Find your vibe and stick to it, don't try to copy others, be original and creative

---

## Designing your website

Before even starting a single line of code, explore designs.

**Where to find designs?**

- You can choose your own designs.
- Here are all the Designs you can use:
  - [Neubrutalism](./Designs/neubrutalism/)
  - [Minimalism](./Designs/minimalism/)
  - [Material Design](./Designs/material-design/)
  - [Flat Design](./Designs/flat-design/)
  - [Skeuomorphism](./Designs/skeuomorphism/)
  - [Brutalism](./Designs/brutalism/)
  - [Neumorphism](./Designs/neumorphism/)
  - [Glassmorphism](./Designs/glassmorphism/)
  - [Liquid Glass](./Designs/liquid-glass/)
  - etc.

You can also find designs on websites like:
- [Dribbble](https://dribbble.com)
- [Behance](https://www.behance.net)
- [Pinterest](https://www.pinterest.com)

**Analyzing Designs**

Once you find a design that you like, try to analyze it and understand how it works.

- What are the colors used?
- What are the fonts used?
- What are the shapes used?
- What are the animations used?
- What are the interactions used?
- What are the components used?
- What are the layouts used?
- What are the patterns used?
- What are the principles used?
- What are the best practices used?
- What are the accessibility features used?

**Creating Wireframes**

Once you understand the design, try to create a wireframe or a mockup of your website.

- You can use tools like [Figma](https://www.figma.com/), [Sketch](https://www.sketch.com/), [Adobe XD](https://adobexdplatform.com/), [Google Stitch](https://stitch.withgoogle.com/) etc. to create your wireframe or mockup.
- You can also use pen and paper to create your wireframe or mockup.

---

## Setting up your development environment

Once you have your design ready, it's time to set up your development environment.

- You can use any code editor you like, but I recommend using [Visual Studio Code](https://code.visualstudio.com/).
- You can also use other code editors like [Sublime Text](https://www.sublimetext.com/), [Atom](https://atom-editor.cc/), etc. but I recommend using Visual Studio Code because of its features and extensions that can help you vibe code and create beautiful websites.

---

## Tools and Technologies

- **[React](https://reactjs.org/)**: A JavaScript library for building user interfaces.
- **[Vite](https://vitejs.dev/)**: A build tool that provides a fast development experience for modern web projects.
- **[Tailwind CSS](https://tailwindcss.com/)**: A utility-first CSS framework for rapidly building custom user interfaces.
- **[Git](https://git-scm.com/)**: A version control system to manage your code and collaborate with others.
- **[GitHub](https://github.com)**: A platform for hosting and collaborating on Git repositories.
- **[Figma](https://www.figma.com/)**: A design tool for creating wireframes, mockups, and prototypes.

---

## AI Tools [Edited by AI]

Choose the right AI tools to help you with your coding and design process. Some popular AI tools for web development include:

- **[GitHub Copilot](https://copilot.github.com/)**: An AI-powered code completion tool that helps you write code faster and with fewer errors.
- **[Claude by Anthropic](https://www.anthropic.com/claude)**: An AI assistant that can help you with coding, design, and other tasks.
- **[Google Gemini AI](https://ai.google.dev/gemini)**: A suite of AI tools that can assist you with various aspects of web development, including code generation and design assistance.

> [!NOTE]
> I personally use Google Gemini and Claude. Claude's free tier is not generous, so use it wisely. Google Gemini is more generous and can be used for a variety of tasks, including code generation, design assistance, and more.

> [!TIP]
> Use Gemini for initial code generation and design assistance, Once you have the basic build and interactive website, you can zip the file and upload it to Claude. Also, use any extensions tools to extract your chat with Google Gemini [extension](https://chromewebstore.google.com/detail/savechat-for-gemini-expor/blndbnmpkgfoopgmcejnhdnepfejgipe).

> [!TIP]
> Don't just start with coding right away, Plan your website and design with AI Tools, once everything is explained to the AI, and the context is clear, then you can start coding. This will save you a lot of time and effort in the long run.

---

## Installing dependencies [Edited by AI]

Once you have your development environment set up, it's time to install the necessary dependencies for your project. You can use npm or yarn to install the dependencies. For example, to create a new React project with Vite and Tailwind CSS, you can run the following commands:

```bash
npm create vite@latest my-react-app -- --template react
cd my-react-app
npm install
```

After installing the dependencies, you can start the development server by running:

```bash
npm run dev
```

This will start the development server and you can view your website at http://localhost:3000.

---

## Setting up Tailwind CSS [Edited by AI]

Installing Tailwind CSS v4 with React and Vite:

```bash
npm install tailwindcss @tailwindcss/vite
```

**Configure the Vite Plugin**

Open your `vite.config.js` file and add the Tailwind CSS plugin:

```javascript
import { defineConfig } from 'vite'
import react from '@vitejs/plugin-react'
import tailwindcss from '@tailwindcss/vite' // [!code ++]

export default defineConfig({
  plugins: [
    react(),
    tailwindcss(), // [!code ++]
  ],
})
```

Now the dependecies are installed and the folder structure is ready. The folder structure should look like this:

```
my-react-app/
├── node_modules/
├── public/
├── src/
│   ├── App.jsx <-- This the the main component of your website. You can create other components and import them here.>
│   ├── index.css <-- This is where you can import your Tailwind CSS styles. You can also add your custom styles here.>
│   └── main.jsx <-- This is the entry point of your application. It renders the App component to the DOM.>
├── .gitignore
├── index.html
├── package.json
├── vite.config.js <-- This is where you configure your Vite plugins and Tailwind CSS is also loaded from here in v4.>
└── README.md
```

**Import Tailwind CSS in your `index.css` file**

```css
@import "tailwindcss";
```

Now you can use Tailwind CSS classes in your components. For example, you can create a simple button component like this:

```jsx
function Button() {
  return (
    <button className="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded">
      Click me
    </button>
  );
}
```

And you're done! You can now start building your website with React, Vite, and Tailwind CSS.

> [!TIP]
> You can also use Tailwind CSS plugins to add additional functionality to your website. Some popular plugins include:
> - [Tailwind CSS Forms](https://github.com/tailwindlabs/tailwindcss-forms): A plugin that provides better default styles for form elements.
> - [Tailwind CSS Typography](https://github.com/tailwindlabs/tailwindcss-typography): A plugin that provides beautiful typographic defaults for prose content.
> - [Tailwind CSS Aspect Ratio](https://github.com/tailwindlabs/tailwindcss-aspect-ratio): A plugin that provides utilities for controlling the aspect ratio of elements.
> 
> These plugins can help you build more complex and beautiful websites with Tailwind CSS. You can find more plugins on the [Tailwind CSS website](https://tailwindcss.com/docs/plugins).

---

## Planning Folder Structure [Edited by AI]

Before starting to code, it's important to plan your folder structure. This will help you to keep your code organized and maintainable. A good folder structure will also make it easier for you to find and update your code in the future. A common folder structure for a React project looks like this:

```
my-react-app/
├── node_modules/
├── public/ <-- This is where you can put your static assets like images, fonts, etc.>
├── src/
│   ├── components/ <-- This is where you can create your reusable components. You
│   │   ├── Hero.jsx
│   │   ├── Navbar.jsx
│   │   ├── Footer.jsx
│   │   └── ... <-- You can create as many components as you need and import them in your App.jsx file.>
│   ├── Pages/
│   │   ├── Home.jsx
│   │   ├── About.jsx
│   │   ├── Contact.jsx
│   │   ├── Privacy.jsx
│   │   └── ... <-- You can create as many pages as you need and import them in your App.jsx file.>
│   ├── App.jsx <-- This is the main component of your website. You can import all your components and pages here and render them.>
│   ├── index.css <-- This is where you can import your Tailwind CSS styles. You can also add your custom styles here.>
│   └── main.jsx <-- This is the entry point of your application. It renders the App component to the DOM.>
├── .gitignore
├── index.html
├── package.json
├── vite.config.js <-- This is where you configure your Vite plugins and Tailwind CSS is also loaded from here in v4.>
└── README.md
```

This is just a basic folder structure, you can modify it according to your needs and preferences. The important thing is to keep your code organized and maintainable. You can create separate folders for components, pages, styles, assets, etc. to keep everything organized.

Always keep the folder structure organized and clean. This will help you and others understand the code better and make it easier to maintain and update in the future. You can create separate folders for components, styles, assets, etc. to keep everything organized.

---

## Setting up CSS Variables [Edited by AI]

It's a good practice to use CSS variables for your colors, fonts, and other design tokens. This will make it easier to maintain and update your styles in the future. You can define your CSS variables in your index.css file like this:

```css
@import "tailwindcss";

@theme {
  --color-primary: #007bff;
  --color-secondary: #6c757d;
}
```

You can then use these CSS variables in your components and styles like this:

```jsx
<div style={{ backgroundColor: 'var(--primary-color)' }}>
  This is a styled component.
</div>
```

This will make it easier to maintain and update your styles in the future. If you want to change the primary color, you can just update the CSS variable in one place and it will be reflected throughout your website.

---

## Building Your Website: Tips & Best Practices

> [!TIP]
> Always build top to bottom, start with the Hero Section, then the Navbar, then the About Section, and finally the Footer. This will help you to focus on one section at a time and make it easier to debug and test your code.

> [!TIP]
> After the basic website is ready, immediately push it to Github. This will help you keep track of your changes and also allow you to have version control for you project. This would help you to revert back to previous version if something goes wrong. If you're working in a team, this will allow you to share your code with other and add them as collaborators to your repository. You can also use GitHub Pages to host your website for free.

Once the persona is set and the context is provided, You can give this specific prompt to the AI tool. I personally use this prompt, this will create the starting point for the website and then you can start building on top of it and adding more features and components as you go along.

This is my own website which I've built with Claude. You can check it out here: [Nowehere Fast](https://nowhere-fast.vercel.app/)
You can find the prompt I used to build this website here: [Nowhere Fast Prompt](./nowhere-fast-prompt.md)

> [!NOTE]
> This was just the initial prompt to guide the AI to generate the website, to see the whole chat you can use this [link](https://claude.ai/share/e9f67e3b-2e5b-489f-aad0-3dcf86e59876). Once you get the initial code, start adding components and features one by one. Don't try to do everything at once, this will help you to focus on one thing at a time and also make it easier to debug and test your code.

I used Claude to generate the whole website in this case, but you can also use Google Gemini for the initial code generation and then switch to Claude for any further improvements and optimizations.

---

## Debugging the Website

Once the basic website is ready, there will be a lot of bugs and issues which you will need to fix manually. This is where your coding skills and knowledge will come into play. You can use the AI tools to help you with debugging and optimizing your code, but always make sure to understand the code and the logic behind it before using it in your projects. You can also use browser developer tools to inspect the elements and debug any issues that may arise.

> [!TIP]
> Always use the Console and Network tabs in the browser developer tools to check for any errors or issues with your code. 90% of the bugs can be fixed by just checking the console, if you're an experienced developer, you can fix the bugs by yourself, but if you're a new developer/don't know any coding, just copy the console error and paste it in the AI Tool of your choice, and the AI tool will give you the full fixed file which you can copy and paste in your project.

---

## Deploying the Website

Now, that you have your website ready with all the bugs fixed and everything working perfectly, it's tome to deploy your website and make it live. You can use platforms like Vercel, Netlify, GitHub Pages, etc. to deploy your website for free. These platforms provide easy integration with GitHub, so you can just push your code to GitHub and connect your repository to the deployment platform. Once connected, the platform will automatically build and deploy your website whenever you push new changes to the repository.

> [!TIP]
> I personally use Vercel for deployment, it's very easy to use and provides a lot of features for free. You can also use Netlify, it's also a great platform for deployment. Both platforms provide continuous deployment, so you can just push your code to GitHub and the platform will take care of the rest.

### Steps to Deploy (Vercel)

1. Push your code to GitHub.
2. Go to Vercel and sign up for an account if you don't have one already.
3. Click on "New Project" and select your GitHub repository.
4. Follow the prompts to configure your deployment settings (you can usually leave these as default for a React + Vite project).
5. Click "Deploy" and wait for the deployment process to complete. Once it's done, you will get a live URL for your website. You can share this URL with others and also use it for your portfolio or any other purpose.

---

### Steps to Deploy (Netlify)

1. Push your code to GitHub.
2. Go to Netlify and sign up for an account if you don't have one already.
3. Click on "New site from Git" and select your GitHub repository.
4. Follow the prompts to configure your deployment settings (you can usually leave these as default for a React + Vite project).
5. Click "Deploy site" and wait for the deployment process to complete. Once it's done, you will get a live URL for your website. You can share this URL with others and also use it for your portfolio or any other purpose.

---

### Steps to Deploy (GitHub Pages)

1. Push your code to GitHub.
2. Go to your repository on GitHub and click on "Settings".
3. Scroll down to the "GitHub Pages" section and select the branch you want to deploy from (usually "main" or "master").
4. Click "Save" and wait for the deployment process to complete. Once it's done, you will get a live URL for your website (usually in the format `https://yourusername.github.io/yourrepository`). You can share this URL with others and also use it for your portfolio or any other purpose.

> [!NOTE]
> Use GitHub Pages if you want a simple and free hosting solution for your website, but keep in mind that it has some limitations (e.g., it only supports static sites, it does not support server-side rendering, etc.). If you need more features and flexibility, I recommend using Vercel or Netlify for deployment.

---

## 🚀 Show Off Your Vibe

Did you build something awesome using this guide? I want to see it!

* **Star this repo** if it helped you out.
* Open an Issue/PR if you want to contribute improvements to this guide or share your own tips and tricks. I'll personally review and merge every single one.
* Tag me on [Twitter/X](https://x.com/perhaps_aadi) with screenshots of your live site.
* Open an Issue to submit your site to the "Hall of Fame" section!

Keep building, keep iterating, and keep the vibe alive.

---

*Thank You*

***Nighteye***

---

## Table of Contents

1. [HOW TO VIBE CODE AND CREATE BEAUTIFUL WEBSITES](#how-to-vibe-code-and-create-beautiful-websites)
2. [Prerequisites](#prerequisites)
3. [Designing your website](#designing-your-website)
   - Analyzing Designs
   - Creating Wireframes
4. [Setting up your development environment](#setting-up-your-development-environment)
5. [Tools and Technologies](#tools-and-technologies)
6. [AI Tools](#ai-tools-edited-by-ai)
7. [Installing dependencies](#installing-dependencies-edited-by-ai)
8. [Setting up Tailwind CSS](#setting-up-tailwind-css-edited-by-ai)
9. [Planning Folder Structure](#planning-folder-structure-edited-by-ai)
10. [Setting up CSS Variables](#setting-up-css-variables-edited-by-ai)
11. [Building Your Website: Tips & Best Practices](#building-your-website-tips--best-practices)
12. [Debugging the Website](#debugging-the-website)
13. [Deploying the Website](#deploying-the-website)
    - [Steps to Deploy (Vercel)](#steps-to-deploy-vercel)
    - [Steps to Deploy (Netlify)](#steps-to-deploy-netlify)
    - [Steps to Deploy (GitHub Pages)](#steps-to-deploy-github-pages)
14. [🚀 Show Off Your Vibe](#-show-off-your-vibe)