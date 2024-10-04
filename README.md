# TajilwindProps

## What is this?

A CSS library of predefined variable names similar to TailwindCSS naming and similar to OpenProps system with minor deviations from the naming scheme.

## Why did I make this?

I was using Tailwind in some of my projects, and Open Props in my project before. I liked Tailwind and the naming and units were perfect but I felt like the HTML was too messy. I liked Open Props too but I preferred the naming and units of Tailwind. With this, it is the same concept as Open Props but with Tailwind's naming and units

## What does it help you with?

It forces you to write more consistent code using variables instead of using magic numbers.

## How does it compare with other tools?

Using Tailwind's @apply feature is quite similar but you have to do more config. @apply isn't reccomended either and might be deprecated in the future. Using Open Props is similar too but it doesn't have the naming and units of Tailwind

## Who can use this and take advantage of it?

Anyone who is writing CSS. Inline styles, Sass, Tailwind arbitrary values, etc.

## Browse CDN

- [https://unpkg.com/twprops/](https://unpkg.com/twprops/)

## Usage

### Option 1 (NPM Package)

1. Install the npm package `npm i twprops`
2. Import the CSS file you need inside `node_modules/twprops/`

   ```
   @import "/node_modules/twprops/"
   ```

### Option 2 (NPM Package + PostCSS JIT Props)

1. Install PostCSS JIT Props

```
npm install postcss-jit-props
```

2. Add the following lines of code inside your `postcss.config.js`

```
// postcss.config.js

```

### Option 3 (Unpkg CDN)

1. Add this line in your CSS

```
@import "https://unpkg.com/twprops/twprops.min.css"
```

## Tooling & Autocomplete _(VSCode Only!)_

1. Install this [extension](https://marketplace.visualstudio.com/items?itemName=vunguyentuan.vscode-css-variables).
2. Go inside the extensions tab (Ctrl + Shift + X).
3. Find the extension.
4. Click on the settings icon (cog) and a modal will appear.
5. Click "Extension Settings".
6. Go to "CSS Variables: Blacklist Folders" and open it inside `settings.json`.
7. Delete the line that contains `node_modules` inside the array.

   ```
   "cssVariables.blacklistFolders": [
      // Some stuff here
      "**/node_modules",
      // Some stuff here also
   ],
   ```

## Optimizing for Production

All of the variables take up atleast 600+ lines of code and is 14kb minified without Gzip nor Brotli compression. You can use PurgeCSS to remove all of the unused variables since TailwindProps doesn't have a just-in-time feature at the moment. Just use their docs instead of a guide here.

## Demo Usage

### Tailwind Version

```

<div class="w-full bg-red-400 h-full font-bold"> </div>
```

### TailwindProps Version

```
<div> </div>

div {
    width: var(--spacing-full);
    height: var(--spacing-full);
    background-color: var(--red-400);
    font-weight: var(--font-bold);
}
```

## Advantages

- Less config
- Framework agnostic
- Best of both worlds! (Tailwind & OpenProps)

## To-do

- [x] Complete all variables
- [ ] Make a website
- [x] Make NPM package
- [x] Write better docs
- [ ] Get first contributor
- [ ] Test for performanced compared to Tailwind, OpenProps, and TailwindProps
- [x] Make more stuff consistent
