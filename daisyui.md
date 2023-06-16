# How to Set Up Daisy UI with Next.js

![Daisy UI and Next.js]([https://example.com/daisy_ui_nextjs_image.png](https://images.unsplash.com/photo-1506729623306-b5a934d88b53?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80))

Are you looking to enhance the user interface of your Next.js application? Look no further than Daisy UI, a delightful CSS framework for Tailwind CSS. In this tutorial, we'll walk you through the process of setting up Daisy UI with Next.js, enabling you to create beautiful and responsive designs in no time.

## Prerequisites

Before we begin, make sure you have the following prerequisites installed on your machine:

- Node.js (v12 or higher)
- npm (Node Package Manager) or Yarn

## Step 1: Create a Next.js Application

If you haven't already, start by creating a new Next.js application using the following command:

```bash
npx create-next-app my-app
```

This command sets up a new Next.js project in a directory named `my-app`. Once the command completes, navigate to the project directory:

```bash
cd my-app
```

## Step 2: Install Tailwind CSS

Daisy UI is an extension for Tailwind CSS, so we need to install Tailwind CSS first. In your project directory, install Tailwind CSS using npm or Yarn:

```bash
npm install tailwindcss
```

or

```bash
yarn add tailwindcss
```

## Step 3: Configure Tailwind CSS

Next, we need to configure Tailwind CSS. Create a `tailwind.config.js` file in the root of your project directory and add the following content:

```javascript
module.exports = {
  purge: [],
  darkMode: false,
  theme: {
    extend: {},
  },
  variants: {
    extend: {},
  },
  plugins: [],
}
```

## Step 4: Install Daisy UI

Now it's time to install Daisy UI. In your project directory, run the following command:

```bash
npm install daisyui
```

or

```bash
yarn add daisyui
```

## Step 5: Enable Daisy UI in Tailwind CSS

To enable Daisy UI, we need to import it in our Tailwind CSS configuration. Open your `tailwind.config.js` file and update it as follows:

```javascript
module.exports = {
  purge: [],
  darkMode: false,
  theme: {
    extend: {},
  },
  variants: {
    extend: {},
  },
  plugins: [
    require('daisyui'),
  ],
}
```

## Step 6: Import Daisy UI Styles

To import the Daisy UI styles, open your `styles/globals.css` file and add the following line at the top:

```css
@import 'daisyui/dist/full.css';
```

## Step 7: Start the Next.js Development Server

You're almost there! Start the Next.js development server by running the following command in your project directory:

```bash
npm run dev
```

or

```bash
yarn dev
```

## Step 8: Test Daisy UI

Now that everything is set up, let's test Daisy UI by using its classes in your Next.js components. Open the `pages/index.js` file in your project directory and replace its content with the following code:

```jsx
import React from 'react';

const Home = () => {
  return (
    <div className="p-10">
      <h1 className="text-4xl font-bold mb-5">Welcome to My Next.js App!</h1>
      <button className="btn btn-primary">Get Started</button>
    </div>
  );
};

export default Home;
```
