# TP Care Technology

Source for the TP Care Technology website. The single-page site introduces the company's software development, IT solutions, and healthcare technology services, and provides a contact email.

## Run locally

No dependencies or build step are required. From the repository root, run:

```sh
python3 -m http.server 8000
```

Open `http://localhost:8000/` in a browser. You can also open `index.html` directly for a quick preview.

## Project files

- `index.html`: page content, navigation, and inline SVG artwork.
- `404.html`: custom not-found page for GitHub Pages.
- `style.css`: visual styles and responsive layouts.
- `assets/TPCT-logo.png`: site logo.
- `AGENTS.md`: contributor guidelines.

## Making changes

Edit `index.html` for copy and structure, and `style.css` for appearance. Keep asset links relative so the site works from the repository root on a static host. After changes, check the page at desktop and mobile widths, verify navigation links and the contact email, then run `git diff --check`.

There is currently no automated test suite or package manager configuration.
