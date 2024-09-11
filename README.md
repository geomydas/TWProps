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

## How to use it

1. Clone this repository. `git clone git@github.com:geomydas/TailwindProps.git`
2. Either `@import` or `<link>` the CSS file that you need

```
<link rel="stylesheet" href="src/color.css">
@import url("src/color.css")
```

3. Use the variables!
4. Et voila!

## Demo Usage

Tailwind Version

```
<div class="w-full bg-red-400 h-full font-bold"> </div>
```

TailwindProps Version

```
<div> </div>

div {
    width: var(--size-full);
    height: var(--size-full);
    background-color: var(--red-400);
    font-weight: var(--font-bold);
}

```

## Advantages

- Use TailwindCSS classes as variables instead of @apply
- Less config
- Framework agnostic
- Basically a design system
- Best of both worlds (Tailwind & OpenProps)

More features will be coming soon and feel free to contribute since I'm still a noob (_i don't even know how to make a calculator in js level_). Any suggestions, feedback, roasts are welcome!

## To-do

- [ ] Complete all variables
- [ ] Make a website
- [ ] Make NPM package
- [ ] Write better docs
- [ ] Get first contributo  r
- [ ] Test for performanced compared to Tailwind, OpenProps, and TailwindProps
- [ ] Make more stuff consistent
