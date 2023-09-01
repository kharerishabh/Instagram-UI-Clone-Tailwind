# How to initialize the Tailwind in HTML
- npm install -D tailwindcss
- npx tailwindcss init

# In tailwind config file
- module.exports = {
  content: ["./src/**/*.{html,js}"],
  theme: {
    extend: {},
  },
  plugins: [],
}

# Create new file input.css
- @tailwind base;
- @tailwind components;
- @tailwind utilities;

# To Track what we are changing in the code Tailwind want the CLI build process to keep track.
- npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch

# Adding tailwind Form by package
- npm install -D @tailwindcss/forms

# then add the plugin to your tailwind.config.js
- plugins: [
    require('@tailwindcss/forms'),
    // ...
  ],

# Icons From Heroicons form Tailwind
- for heroicons site

# Require Scrool bar from Tailwind Css.
- npm install --save-dev tailwind-scrollbar
- In tailwind.config file - plugins: [
    // ...
    require('tailwind-scrollbar'),
],

