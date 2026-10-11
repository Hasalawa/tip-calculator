# Tip Calculator

[![CI/CD](https://github.com/Hasalawa/tip-calculator/actions/workflows/deploy.yml/badge.svg)](https://github.com/Hasalawa/tip-calculator/actions/workflows/deploy.yml)

**Live demo:** https://hasalawa.github.io/tip-calculator/

A clean, single-page tip calculator built with plain HTML, CSS and JavaScript. Enter a bill, pick a tip percentage, and see the tip and total update instantly. Built with [Cursor](https://cursor.com) for MLH Global Hack Week: Hacktoberfest (Challenge 1: Build a Mini App with Cursor).

## Features

- **Live results:** tip amount and total update as you type
- **Quick tip presets:** one-tap buttons for 10%, 15%, 18%, 20% and 25%, or enter any custom percentage
- **Split the bill:** divide the total between 2 to 50 people and see what each person pays
- **Dark mode:** toggle between light and dark themes; your choice is remembered, and it follows your system preference by default
- **Responsive and accessible:** works on desktop and mobile, with keyboard focus styles and ARIA labels

## Getting started

No build step or dependencies are needed.

1. Clone the repository:
   ```bash
   git clone https://github.com/Hasalawa/tip-calculator.git
   cd tip-calculator
   ```
2. Open `index.html` in your browser (double-click it, or run `open index.html` on macOS / `start index.html` on Windows).

## How to use

1. Type the **bill amount**.
2. Choose a **tip percentage** with a preset button or type your own.
3. (Optional) Click **Split the bill** and set the number of people.
4. Read the **tip amount**, **total**, and **per-person** amount in the results panel.
5. Use the sun/moon button in the top-right corner to switch themes.

## Tech stack

- HTML5
- CSS3 (custom properties for theming)
- Vanilla JavaScript (no frameworks)
- Google Fonts: Fraunces and Outfit

## Project structure

```
tip-calculator/
├── .github/workflows/deploy.yml   # CI/CD: lint + deploy to GitHub Pages
├── index.html                     # markup, styles and logic in a single file
└── README.md
```

## CI/CD

A GitHub Actions workflow (`.github/workflows/deploy.yml`) runs on every push and pull request to `main`:

1. **Test:** lints `index.html` with HTMLHint
2. **Deploy:** if the lint passes on `main`, the site is published to GitHub Pages automatically

## How Cursor helped

Cursor generated the initial scaffold of the app from a short prompt and then helped me iterate: adding the dark mode toggle and the split-the-bill feature, and fixing issues along the way.

## License

Free to use and modify.