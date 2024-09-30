# List of Variables

## Sizing

Same as their TailwindCSS counterparts but changes in the name

For example, `w-40` is `width: var(--spacing-40)`.

Dots `.` and slashes are equivalent to 1 and 2 under scores.

```
w-1.5
width: var(--spacing-1_5)

```

```
w-1/2
width: var(--spacing-1__2)
```

The only thing we changed is that `w-screen` and `h-screen` is now `var(--spacing-screen-w)` and `var(--spacing-screen-h)`

All of the units can be found [here](https://tailwindcss.com/docs/width), [here](https://tailwindcss.com/docs/max-width) and [here](https://tailwindcss.com/docs/height)

