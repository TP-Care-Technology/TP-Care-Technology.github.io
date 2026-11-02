# Repository Guidelines

## Project Structure & Module Organization

This is a single-page static website. `index.html` contains content and inline SVG illustrations; `style.css` contains the theme, layout, and responsive rules. Store images in `assets/` and reference them with relative paths, as with `assets/TPCT-logo.png`. `README.md` covers setup, and `CHANGELOG.md` records notable changes. There is no JavaScript, build configuration, or test directory.

## Build, Test, and Development Commands

No install or build step is required. Open `index.html` in a browser, or run `python3 -m http.server 8000` from the repository root and visit `http://localhost:8000/`. Run `git diff --check` before committing. There is no configured test, lint, or format command.

## Coding Style & Naming Conventions

Follow the existing four-space indentation in HTML and CSS. Use semantic HTML elements, descriptive `id` values for section anchors, and lowercase kebab-case class names such as `service-card` and `hero-description`. Keep responsive overrides in the existing media-query blocks. Preserve accessibility attributes, visible keyboard focus, the skip link, and reduced-motion behavior.

Define a semantic theme in `:root` before implementing UI. Reuse its design tokens and shared styles, including `.button`, throughout the site. Do not hardcode colors, font sizes, font families, spacing, border radii, or other visual styles in individual components. Do not invent visual values when an existing token or shared component fits. If a project has no theme, ask the user to define its color scheme and required tokens before implementing UI. Keep the theme consistent across the application. Use Title Case for action button labels, such as `Save Changes`.

Use plain punctuation in all repository text. Do not use em dashes, en dashes, or emoji in documentation, interface copy, commit messages, or pull request descriptions.

## Testing Guidelines

There is no automated test framework or coverage target. For visual or content changes, preview the page at desktop and narrow mobile widths; check navigation anchors, the contact email link, logo loading, text wrapping, and keyboard focus. If you add JavaScript or tooling, include a suitable test command and document it here. Name any future tests after the behavior they verify.

## Commit & Pull Request Guidelines

Recent commits use short, imperative, sentence-style summaries (for example, `Refine organization webpage design and business messaging` and `fix header title`). Keep each commit focused on one change. In pull requests, describe the user-visible result, list manual checks performed, and include before/after screenshots for layout or styling changes. Link a related issue when one exists.

Follow the Keep a Changelog 1.1.0 format in `CHANGELOG.md`. Record each notable visitor-facing change under `## [Unreleased]` while working on `dev`. Use the relevant Added, Changed, Deprecated, Removed, Fixed, or Security heading; omit empty categories and routine internal edits. Describe completed changes rather than planned setup.

When changes are merged into `main` and published, move the released entries into a version heading with the publication date in `YYYY-MM-DD` format, and keep an empty `## [Unreleased]` heading above it. Start with version `0.1.0`, use Semantic Versioning for later releases, and tag each release with a matching `v` prefix such as `v0.1.0`. Add comparison links to the changelog when the first version is published.
