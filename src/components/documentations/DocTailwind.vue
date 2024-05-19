<template>
  <div>
    <p class="text-xl font-bold">Tailwind Setup</p>
    <div class="container flex py-2">
      <div class="w-2/6">
        <p class="font-bold">Step 1 : Install Tailwind CSS</p>
        <p>
          Install tailwindcss and its peer dependencies, then generate your
          <span class="font-bold">tailwind.config.js</span> and
          <span class="font-bold">postcss.config.js</span> files.
        </p>
      </div>
      <div
        class="container w-3/6 border-2 text-white rounded-lg bg-gray-800 flex flex-col"
      >
        <div class="p-2 border-b-2 border-sky-300 text-sky-300">
          <p class="text-sm font-semibold">Terminal</p>
        </div>
        <div class="py-2">
          <code class="terminal flex flex-col">
            <span>npm install -D tailwindcss postcss autoprefixer</span>
            <span>npx tailwindcss init -p</span>
          </code>
        </div>
      </div>
    </div>
    <div class="container flex py-2">
      <div class="w-2/6">
        <p class="font-bold">Step 2 : Configure your template paths</p>
        <p>
          Add the paths to all of your template files in your
          <span class="font-bold">tailwind.config.js</span> file.
        </p>
      </div>
      <div
        class="container w-3/6 border-2 text-white rounded-lg bg-gray-800 flex flex-col"
      >
        <div class="p-2 border-b-2 border-sky-300 text-sky-300">
          <p class="text-sm font-semibold">tailwind.config.js</p>
        </div>
        <div class="py-2">
          <code class="flex flex-col">
            <span class="pl-2"
              >/** @type {import('tailwindcss').Config} */
            </span>
            <span class="pl-2"> export default { </span>
            <span class="pl-6 border-sky-400 border-l-4 bg-sky-300/15">
              content: [
            </span>
            <span class="pl-10 border-sky-400 border-l-4 bg-sky-300/15">
              "./index.html",
            </span>
            <span class="pl-10 border-sky-400 border-l-4 bg-sky-300/15">
              "./src/**/*.{js,ts,jsx,tsx}",
            </span>
            <span class="pl-6 border-sky-400 border-l-4 bg-sky-300/15">
              ],
            </span>
            <span class="pl-6"> theme: { </span>
            <span class="pl-10"> extend: {}, </span>
            <span class="pl-6"> }, </span>
            <span class="pl-6"> plugins: [], </span>
            <span class="pl-2"> } </span>
          </code>
        </div>
      </div>
    </div>
    <div class="container flex py-2">
      <div class="w-2/6">
        <p class="font-bold">
          Step 3 : Add the Tailwind directives to your CSS
        </p>
        <p>
          Add the <span class="font-bold">`@tailwind`</span> directives for each
          of Tailwind’s layers to your
          <span class="font-bold">./src/index.css</span> file.
        </p>
      </div>
      <div
        class="container w-3/6 border-2 text-white rounded-lg bg-gray-800 flex flex-col"
      >
        <div class="p-2 border-b-2 border-sky-300 text-sky-300">
          <p class="text-sm font-semibold">index.css</p>
        </div>
        <div class="py-2">
          <code class="flex flex-col">
            <span class="px-2">@tailwind base;</span>
            <span class="px-2">@tailwind components;</span>
            <span class="px-2">@tailwind utilities;</span>
          </code>
        </div>
      </div>
    </div>
    <div class="container flex py-2">
      <div class="w-2/6">
        <p class="font-bold">Step 4 : Start your build process</p>
        <p>
          Run your build process with
          <span class="font-bold">`npm run dev`</span>.
        </p>
      </div>
      <div
        class="container w-3/6 border-2 text-white rounded-lg bg-gray-800 flex flex-col"
      >
        <div class="p-2 border-b-2 border-sky-300 text-sky-300">
          <p class="text-sm font-semibold">Terminal</p>
        </div>
        <div class="py-2">
          <code class="terminal flex flex-col">
            <span>npx run dev</span>
          </code>
        </div>
      </div>
    </div>
    <div class="container flex py-2">
      <div class="w-2/6">
        <p class="font-bold">
          Step 5 : Start using Tailwind in your React project
        </p>
        <p>Start using Tailwind’s utility classes to style your content.</p>
      </div>
      <div
        class="container w-3/6 border-2 text-white rounded-lg bg-gray-800 flex flex-col"
      >
        <div class="p-2 border-b-2 border-sky-300 text-sky-300">
          <p class="text-sm font-semibold">App.jsx</p>
        </div>
        <div class="py-2">
          <code class="flex flex-col">
            <span class="pl-2">export default function App() {</span>
            <span class="pl-6">return (</span>
            <span class="pl-10 border-sky-400 border-l-4 bg-sky-300/15">
              <span>&lt;</span>
              <span class="text-pink-400">h1</span>
              <span> className="text-3xl font-bold underline"</span>
              <span>&gt;</span>
            </span>
            <span class="pl-12 border-sky-400 border-l-4 bg-sky-300/15">
              Hello world!
            </span>
            <span class="pl-10 border-sky-400 border-l-4 bg-sky-300/15">
              <span>&lt;</span><span class="text-pink-400">/h1</span><span>&gt;</span>
            </span>
            <span class="pl-6">)</span>
            <span class="pl-2"> } </span>
          </code>
        </div>
      </div>
    </div>
    <div class="container flex py-2">
      <div class="w-2/6">
        <p class="font-bold">
          Step 5 : Start using Tailwind in your Vue project
        </p>
        <p>Start using Tailwind’s utility classes to style your content.</p>
      </div>
      <div
        class="container w-3/6 border-2 text-white rounded-lg bg-gray-800 flex flex-col"
      >
        <div class="p-2 border-b-2 border-sky-300 text-sky-300">
          <p class="text-sm font-semibold">App.vue</p>
        </div>
        <div class="py-2">
          <code class="flex flex-col">
            <span class="pl-2">
              <span>&lt;</span>
              <span class="text-pink-400">template</span>
              <span>&gt;</span>
            </span>
            <span class="pl-6 border-sky-400 border-l-4 bg-sky-300/15">
              <span>&lt;</span>
              <span class="text-pink-400">h1</span>
              <span> className="text-3xl font-bold underline"</span>
              <span>&gt;</span>
            </span>
            <span class="pl-10 border-sky-400 border-l-4 bg-sky-300/15">
              Hello world!
            </span>
            <span class="pl-6 border-sky-400 border-l-4 bg-sky-300/15">
              <span>&lt;</span>
              <span class="text-pink-400">/h1</span>
              <span>&gt;</span>
            </span>
            <span class="pl-2">
              <span>&lt;</span>
              <span class="text-pink-400">/template</span>
              <span>&gt;</span>
            </span>
          </code>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
</script>

<style lang="scss" scoped>
code.terminal > span::before {
  content: ">";
  padding: 0 8px;
  color: pink;
}
</style>