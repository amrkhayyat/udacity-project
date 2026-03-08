# Copilot Instructions (Static Site)

## 🧠 Project Overview
This repository is a simple **static website** made of **HTML**, **CSS**, and local image assets. There is no build step, package manager, or runtime framework. The site is intended to be served as plain files (e.g., via a file:// URL or a static host).

Key files:
- `Index.html` – main landing page
- `css/index.css` – site styling
- `pages/contact.html` – placeholder contact page (currently empty)
- `images/` – local assets referenced by `<img src="...">`

## 🛠️ Developer Workflow
✅ **Open and preview**
- Open `Index.html` in the browser directly or use VS Code Live Preview (configured via `.vscode/settings.json` to load `/Index.html`).

✅ **Editing**
- Keep HTML and CSS separate (HTML in `.html`, styles in `css/index.css`).
- Use **relative paths** for assets and navigation links, consistent with the existing patterns (e.g., `pages/contact.html`).

✅ **No build/tools**
- There is no `npm`, `package.json`, or other build tooling in the repo. Do not assume bundlers, preprocessors, or servers unless explicitly added.

## ✅ Coding Conventions in This Repo
- HTML uses **classic static markup** (no templating or JS frameworks).
- Navigation links are hardcoded (e.g., `href="home.html"` and `href="pages/contact.html"`). Update these with care.
- Maintain consistent indentation and minimal inline styles. Most styling should be in `css/index.css`.

## 🔎 What to Watch For (Known Gaps)
- `pages/contact.html` is empty; adding content here is expected when expanding the site.
- The main page has placeholder card markup (`<img src="...">`, `Card title`, etc.) — these are intended to be replaced with real assets and text.

## 📌 How to Contribute (for Agents)
When making changes:
1. Reference the core HTML structure in `Index.html` and keep the `<link rel="stylesheet" href="css/index.css">` in place.
2. Add content to `pages/contact.html` using consistent structure to `Index.html` (sections + semantic elements).
3. Keep image paths relative to the HTML file referencing them.

---

If any parts of the site behavior are unclear (navigation structure, intended responsive behavior, design goals), ask for clarification so the edits match the author’s intent.