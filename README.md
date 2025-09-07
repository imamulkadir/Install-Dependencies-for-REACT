# Mega Install

`npm install tailwindcss @tailwindcss/vite react-router-dom localforage match-sorter sort-by daisyui@latest`

`npm install -D prettier prettier-plugin-tailwindcss tailwindcss postcss autoprefixer @tailwindcss/vite@latest`

in root/

```.prettierrc
{
"plugins": ["prettier-plugin-tailwindcss"]
}
```

```
@import "tailwindcss";
@plugin "daisyui";
```

tailwind.config.js

```
/** @type {import('tailwindcss').Config} */
export default {
  darkMode: "class",
  content: ["./src/**/*.{js,jsx,ts,tsx}"],
  theme: { extend: {} },
  corePlugins: {
    preflight: true,
  },
  plugins: [],
};
```

```Mega Install Packages
┌─────────────────────┐
│      Styling        │
├─────────────────────┤
│ tailwindcss         │ <- Utility-first CSS framework
│ daisyui             │ <- Prebuilt UI components for Tailwind
│ @tailwindcss/vite   │ <- Tailwind plugin for Vite
│ postcss             │ <- CSS processor (used by Tailwind)
│ autoprefixer        │ <- Adds vendor prefixes to CSS
└─────────────────────┘
```
```
┌─────────────────────┐
│ Routing │
├─────────────────────┤
│ react-router-dom │ <- React routing library
└─────────────────────┘

┌─────────────────────┐
│ Storage │
├─────────────────────┤
│ localforage │ <- Browser storage abstraction
├─────────────────────┤
│ match-sorter │ <- Sort/filter lists by string matching
│ sort-by │ <- Sort arrays of objects by properties
└─────────────────────┘

┌──────────────────────────────┐
│ Dev Tooling │
├──────────────────────────────┤
│ prettier │ <- Code formatter
│ prettier-plugin-tailwindcss │ <- Auto-sort Tailwind classes
└──────────────────────────────┘
```
