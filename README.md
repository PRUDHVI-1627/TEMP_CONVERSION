# Temperature Converter

**Live demo:** https://temp-conversion-alpha.vercel.app/

A clean, minimal temperature conversion tool built with vanilla HTML, CSS, and JavaScript.

## Features

- Convert **Celsius → Fahrenheit** and **Fahrenheit → Celsius**
- Results rounded to one decimal place
- Subtle fade-in animation on load and a pop animation on each result
- Fully responsive card layout centered on the page

## File Structure

```
├── index.html
├── index.js
└── style.css
```

## How to Use

No installation or build step needed. Just open `index.html` in any browser.

1. Enter a temperature in the input field
2. Select a conversion direction using the radio buttons
3. Click **Convert** — the result appears instantly below

## Design

- **Fonts:** [Nunito](https://fonts.google.com/specimen/Nunito) for UI text, [Inconsolata](https://fonts.google.com/specimen/Inconsolata) for numbers and results — both loaded from Google Fonts
- **Accent color:** Cyan (`hsl(196, 90%, 48%)`)
- **Theme:** Clean and minimal with lots of white space, soft shadows, and a faint radial gradient background
- **Theming:** All colors are defined as CSS variables in `:root` inside `style.css`, making it easy to retheme

## Conversion Formulas

```
°F = (°C × 9/5) + 32
°C = (°F − 32) × 5/9
```

## Deployment

Deployed on [Vercel](https://vercel.com). To deploy your own copy:

1. Push the three files (`index.html`, `style.css`, `index.js`) to a GitHub repository
2. Import the repo on Vercel — it will detect the static site automatically
3. Hit **Deploy**

## Browser Support

Works in all modern browsers. The styled radio buttons use `appearance: none` and `:has()`, which are supported in Chrome, Firefox, and Safari (2023+).