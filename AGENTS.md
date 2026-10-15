# Repository Guidelines

## Project Structure & Module Organization

This repository is a single-page static website. `index.html` contains the page content and inline SVG illustrations; `style.css` contains all layout, color, and responsive rules. Store image assets in `assets/` and reference them with relative paths, as the logo does (`assets/TPCT-logo.png`). `README.md` covers setup and project files. There is currently no JavaScript, build configuration, or test directory.

## Build, Test, and Development Commands

No install or build step is required. Open `index.html` in a browser for a quick preview, or run `python3 -m http.server 8000` from the repository root and visit `http://localhost:8000/`. The local server makes relative asset paths behave like they will on a static host. Run `git diff --check` before committing to catch whitespace errors. There is no configured `npm test`, linter, or formatter command.

## Coding Style & Naming Conventions

Follow the existing four-space indentation in HTML and CSS. Use semantic HTML elements, descriptive `id` values for section anchors, and lowercase kebab-case class names such as `service-card` and `hero-description`. Keep CSS custom properties for shared colors and dimensions in `:root`. Add component styles near the related section comment and responsive overrides in the existing media-query blocks. Preserve useful accessibility attributes, visible keyboard focus, the skip link, and reduced-motion behavior when changing the page.

Use plain punctuation in all repository text. Do not use em dashes, en dashes, or emoji in documentation, interface copy, commit messages, or pull request descriptions.

## Testing Guidelines

There is no automated test framework or coverage target. For visual or content changes, preview the page at desktop and narrow mobile widths; check navigation anchors, the contact email link, logo loading, text wrapping, and keyboard focus. If you add JavaScript or tooling, include a suitable test command and document it here. Name any future tests after the behavior they verify.

## Commit & Pull Request Guidelines

Recent commits use short, imperative, sentence-style summaries (for example, `Refine organization webpage design and business messaging` and `fix header title`). Keep each commit focused on one change. In pull requests, describe the user-visible result, list manual checks performed, and include before/after screenshots for layout or styling changes. Link a related issue when one exists.
