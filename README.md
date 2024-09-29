# TailwindProps

## What is this?

A CSS library of predefined variable names similar to TailwindCSS naming and similar to OpenProps system with minor deviations.

## Why did I make this?

I was using TailwindCSS and sometimes Open Props in my projects before. I liked Tailwind and the units and colors were perfect but I felt like the HTML was too messy, I liked Open Props too but I was used with the naming and units of TailwindCSS classes. With this, it is similar to Open Props but using tailwind-like naming and units.

## What does it help you with?

It's basically a design system and it helps you write more consistent code.

## How does it compare with other tools?

Using TailwindCSS @apply feature is almost the same but you need to do much more config and it could be inconsistent as sometimes you can mix Tailwind and Sass. Using Open Props is pretty similar too but it doesn't have all of the units and naming of TailwindCSS

## Who can use this and take advantage of it?

Literally anyone who is writing CSS or using a CSS framework. From inline styles, to Sass, and Tailwind arbitrary values

## Usage

### Option 1 (NPM Package)

1. Install the npm package `npm i geomydas/tailwindprops`
2. Link or import the CSS file that you need inside `node_modules/@geomydas/tailwindprops/`

```
<link rel="stylesheet" href="/node_modules/@geomydas/tailwindprops/src/minified-main.css">
```

```
@import url('/node-modules/@geomydas/tailwindprops/src/minified-main.css')
```

### Option 2 (Unpkg CDN)

1. Add this line inside your `<head>` or either `@import` in your CSS

```
<link
  rel="stylesheet"
  href="https://unpkg.com/@geomydas/tailwindprops@1.0.8/src/minified-main.css"
/>
```

```
@import url("https://unpkg.com/@geomydas/tailwindprops@1.0.8/src/minified-main.css")
```

2. Et viola!

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
    "**/.git",
    "**/.svn",
    "**/.hg",
    "**/CVS",
    "**/.DS_Store",
    "**/node_modules",
    "**/bower_components",
    "**/tmp",
    "**/dist",
    "**/tests"
  ],
```

8. Et voila!


## Optimizing for Production

All of the variables take up atleast 600+ lines of code and is 14kb minified without Gzip nor Brotli compression. You can use PurgeCSS to remove all of the unused variables since TailwindProps doesn't have a just-in-time feature at the moment. Just use their docs instead of a guide here. 


## Demo Usage

**Tailwind Version**

```
<div class="w-full bg-red-400 h-full font-bold"> </div>
```

**TailwindProps Version**

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

- Use TailwindCSS classes as variables instead of @apply
- Less config
- Framework agnostic
- Best of both worlds (Tailwind & OpenProps)

More features will be coming! Feel free to contribue by either making an issue or a pull request. Any suggestions, feedback, roasts are welcome!

## To-do

- [x] Complete all variables
- [ ] Make a website
- [x] Make NPM package
- [x] Write better docs
- [ ] Get first contributor
- [ ] Test for performanced compared to Tailwind, OpenProps, and TailwindProps
- [x] Make more stuff consistent
