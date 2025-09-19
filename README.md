# Tailwind Css Lecture Notes 

A small collection of example HTML files and notes used while learning and teaching Tailwind CSS. The samples are intentionally simple and demonstrate Tailwind utility classes, custom arbitrary values, and the browser CDN workflow.

## Quick start — preview in a browser

- Open `index.html` (or any other `.html` file) in your browser. The examples use the Tailwind browser build via CDN so no build step is required for quick previews.
- For a local static server (recommended), run from this folder:

```bash
python3 -m http.server 8000
# then open http://localhost:8000 in your browser
```

## What you'll find here

- `index.html` — Main playground demonstrating Tailwind utility classes and arbitrary values (e.g. `w-[75%]`, `bg-[#252629]`). Uses the Tailwind browser runtime via the `<script src="https://cdn.jsdelivr.net/npm/@tailwindcss/browser@4"></script>` tag.
- `index.css` — Present for local overrides; currently empty.
- `background-color.html`, `responsive.html`, `translate-from-left.html`, `tailwindNotebooks.html` — Additional lecture/example pages exploring specific Tailwind concepts (colors, responsive utilities, transforms, notes).

## Notes on Tailwind usage in this repo

- These examples use the Tailwind "browser" build (CDN) which compiles styles in the browser at runtime. This is great for experimenting but not recommended for production due to performance and caching.
- You will see Tailwind arbitrary values (square brackets) used heavily in the examples, e.g. `p-[20px]`, `rounded-[25px]`, `text-[18px]`. These are valid and supported, but when you move to a production build with the Tailwind CLI or PostCSS, consider defining utility classes or using the config for repeatable values.

## Moving to a local Tailwind build (optional)

If you want a production-like setup with generated CSS and purge capabilities, create a Node project and install Tailwind:

```bash
# install dependencies
npm init -y
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init
```

Then configure `tailwind.config.js` and build your CSS (see the Tailwind docs for detailed steps).

## Contributing

Feel free to open issues or add simple examples. This repo is intended as a personal learning/teaching resource — keep changes small and focused.

## License

No license specified. If you plan to reuse or publish these notes, consider adding a `LICENSE` file (e.g. MIT).

---

Happy tailwinding! — Lecture notes collection
