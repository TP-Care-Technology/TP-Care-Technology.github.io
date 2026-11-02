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
- `robots.txt` and `sitemap.xml`: crawler guidance for the GitHub Pages URL.
- `style.css`: visual styles and responsive layouts.
- `assets/TPCT-logo.png`: site logo.
- `AGENTS.md`: contributor guidelines.
- `CHANGELOG.md`: record of website changes.

## Making changes

Edit `index.html` for copy and structure, and `style.css` for appearance. Keep asset links relative so the site works from the repository root on a static host. After changes, check the page at desktop and mobile widths, verify navigation links and the contact email, then run `git diff --check`.

There is currently no automated test suite or package manager configuration.

## Search visibility

The homepage canonical URL, organization data, and sitemap currently use `https://tp-care-technology.github.io/`. When a custom domain is launched, update all three to the new public URL.

To monitor indexing, add the published URL as a URL-prefix property in Google Search Console, verify ownership using the method offered for your account, submit `https://tp-care-technology.github.io/sitemap.xml`, and inspect the homepage URL. Review search queries and clicks before deciding which service needs a dedicated page.
