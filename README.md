# ✨ Nikita's Sky — Personal Bookmark Dashboard

A beautiful, fully offline personal bookmark manager built as a single HTML file. No server, no dependencies, no install — just open it in a browser.

![License](https://img.shields.io/badge/license-Proprietary-red?style=flat-square)
![HTML](https://img.shields.io/badge/built%20with-HTML%20%2F%20CSS%20%2F%20JS-e91e8c?style=flat-square)
![No Dependencies](https://img.shields.io/badge/dependencies-none-brightgreen?style=flat-square)

---

## Features

- **Add bookmarks** — save title, URL, category, and optional notes via a clean modal dialog
- **Edit & delete** — update any bookmark in place or remove it with a single click
- **Delete all** — clear everything with one confirmation click
- **Search** — instant real-time filtering by title, category, or notes
- **Category filters** — pill buttons auto-generated from your categories; click to filter
- **Import bookmarks** — import your browser's exported `.html` bookmark file, including deeply nested folder hierarchies (folder → subfolder → sub-subfolder → …). Folder names become categories.
- **Export bookmarks** — download a standard Netscape-format `.html` file you can import into Chrome, Firefox, or Edge
- **Dark / Light theme** — toggle with one click; respects your system preference on first load; choice is saved
- **localStorage persistence** — all bookmarks survive page refreshes and browser restarts
- **Favicon icons** — auto-fetched per domain so cards look polished
- **Responsive** — works on mobile with a single-column layout
- **Zero dependencies** — one `.html` file, no npm, no bundler, no CDN

---

## Quick Start

1. Download [`bookmark.html`](./bookmark.html)
2. Open it in any modern browser (Chrome, Firefox, Edge, Safari)
3. That's it — your bookmarks are stored locally in your browser

---

## Importing Browser Bookmarks

**Chrome**
> Menu (⋮) → Bookmarks → Bookmark Manager → Menu (⋮) → Export bookmarks

**Firefox**
> Bookmarks → Manage Bookmarks → Import and Backup → Export Bookmarks to HTML

**Edge**
> Menu (⋯) → Favorites → Manage favorites → ⋯ → Export favorites

Then click **Import** in the dashboard and pick the exported file. Folder structure is preserved — each folder becomes a category, and the full path (e.g. `Work › Dev Tools › Frontend`) is stored in the Notes field for deep nests.

---

## Exporting Your Bookmarks

Click **Export** in the header. A `nikitas-sky-bookmarks.html` file downloads, grouped by category, importable back into any browser.

---

## Tech Stack

| Layer | Detail |
|---|---|
| Markup | Semantic HTML5 |
| Styling | Pure CSS with custom properties (variables) for theming |
| Logic | Vanilla JavaScript (ES5-compatible, no transpiler needed) |
| Storage | `localStorage` (key: `bm_bookmarks_v1`) |
| Icons | Google Favicon API (`https://www.google.com/s2/favicons`) |
| Fonts | System font stack (`-apple-system`, `Segoe UI`, `sans-serif`) |

---

## Folder Structure

```
nikitas-sky/
├── bookmark.html   # The entire app — HTML + CSS + JS in one file
├── README.md
└── LICENSE
```

---

## License

© 2025 Nikita. All rights reserved.

This project is licensed under a **Proprietary License** — personal use is free, but selling or sublicensing requires purchasing a commercial license. See [LICENSE](./LICENSE) for full terms.
