# Hemendra Singh Rajawat | Personal Portfolio & Blog

[![Hugo](https://img.shields.io/badge/Static%20Site-Hugo-orange.svg)](https://gohugo.io/)
[![Theme](https://img.shields.io/badge/Theme-PaperMod-blue.svg)](https://github.com/adityatelange/hugo-PaperMod)
[![Deploy Hugo site to Pages](https://github.com/hemendrarajawat/hemendra.in/actions/workflows/hugo.yml/badge.svg?branch=main)](https://github.com/hemendrarajawat/hemendra.in/actions/workflows/hugo.yml)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

This repository contains the source code for my personal website and blog: **[hemendra.in](https://hemendra.in)**.

The site is a professional hub where I document my journey as a **Salesforce & TensorFlow Certified Developer**, showcase my projects, and share technical insights on enterprise development and Machine Learning.

---

## 🚀 Technologies Used

* **Framework:** [Hugo](https://gohugo.io/) (Static Site Generator)
* **Theme:** [hugo-PaperMod](https://github.com/adityatelange/hugo-PaperMod)
* **Deployment:** GitHub Actions & GitHub Pages
* **Search:** Fuse.js (Built-in PaperMod search)
* **Styling:** PostCSS / SCSS

---

## ✨ Key Features

* **Blog:** Articles on Salesforce development, TensorFlow, and Python.
* **Projects:** Portfolio of ML models and custom Salesforce components.
* **Archive:** Yearly organized post history for easy navigation.
* **Search:** Real-time, fast client-side search.
* **RSS Feed:** Stay updated via [hemendra.in/index.xml](https://hemendra.in/index.xml).
* **Mode:** Automatic Dark/Light mode switching.

---

## 🛠️ Local Development

### Prerequisites

- **Hugo (Extended)** — required for the SCSS/PostCSS pipeline. Install with Homebrew:

```bash
brew install hugo
```

- **Git** — for cloning the repo and initializing submodules.
- **Node.js & npm** — optional; only needed if you edit or rebuild the site's SCSS/JS assets.

### Setup

1. Clone the repository and initialize submodules:

```bash
git clone --recurse-submodules https://github.com/hemendrarajawat/hemendra.in.git
cd hemendra.in
git submodule update --init --recursive
```

2. (Optional) Install Node dependencies and build assets if you change CSS/JS:

```bash
npm install
# Example asset build (check package.json for exact script):
npm run build
```

3. Run the local development server (shows drafts):

```bash
hugo server -D
```

4. Build for production:

```bash
hugo --minify
```

5. Production preview locally (useful to test `baseURL` and minification):

```bash
hugo server --bind 0.0.0.0 -D --baseURL "http://example.org/"
```

Notes:

- If you don't use the asset pipeline, skip the Node/npm steps.
- Replace `npm run build` with the exact script name from `package.json` if different.

---

## 📂 Project Structure

- `archetypes/`: Content archetypes used when creating new posts.
- `content/`: Markdown files for blog posts, pages, projects, and experience entries.
- `assets/`: Source assets (SCSS, JS) processed by Hugo Pipes or external tooling.
- `layouts/`: Template overrides and custom layouts for the site.
- `static/`: Static files served as-is (images, PDFs, favicons, robots.txt).
- `themes/`: Theme source (PaperMod) — usually kept as a submodule.
- `public/`: Generated site output after running `hugo` (build artifact).
- `config.yml`: Site configuration and params.
- `package.json` (optional): Node build scripts and dependencies for asset tooling.

---

## 📄 License

This repository is released under the MIT License — see [LICENSE](LICENSE) for the full text.

You are welcome to reuse the site's code, layout, and assets for your own projects. Please do not republish or reuse personal content (blog posts, personal images) without permission from the owner.

---

**[Visit hemendra.in →](https://hemendra.in)**