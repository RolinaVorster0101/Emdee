# Emdee

A clean, distraction-free Markdown reader that runs entirely in your browser — no build step, no server, no dependencies. Open the file, add your `.md` notes, and read.

**🟢 Live:** [emdee.rvor.co.za](https://emdee.rvor.co.za/)

## Features

- **Zero dependencies** — a single self-contained `.html` file. No CDN scripts, no external fonts, no network requests of any kind.
- **Drag-and-drop or file picker** — add one or more `.md` files at a time, straight from your computer.
- **Hand-written Markdown parser** — supports headings, bold/italic/strikethrough, links, images, inline code, fenced code blocks, blockquotes, ordered/unordered/task lists, tables, and horizontal rules.
- **Auto-generated table of contents** with scroll-spy highlighting, so the sidebar always shows where you are in the document.
- **File library** — every file you add stays listed in the sidebar; switch between them instantly, or step through with Previous/Next.
- **Remove files** individually with the × on each row, without reloading the app.
- **Word count & reading time** shown for whichever file is open.
- **Fully responsive** — a proper slide-in drawer navigation on mobile, not just a squashed sidebar.
- **Installable** — carries a manifest and app icon so it can be added to your desktop as a standalone app window (see below).
- **100% local** — nothing you open is ever uploaded anywhere. Everything renders client-side.

## Getting started

No installation required.

1. Download `emdee.html`.
2. Open it in any modern browser (Chrome, Edge, Firefox, Safari).
3. Click **+ Add another .md file**, or drag a `.md` file anywhere onto the page.

That's it — there's no build process, no `npm install`, no dependencies to fetch.

### Installing it as a desktop app

Emdee ships with an embedded web manifest and icon, so it can be installed like a native app:

- **Chrome / Edge (instant, no hosting needed):** open `emdee.html` → menu (**⋮**) → **More tools → Create shortcut** → check **"Open as window"**. This launches Emdee in its own app window with its icon, straight from the local file.
- **Full PWA install prompt:** host the file over `http://` or `https://` (e.g. GitHub Pages, Netlify) and the browser's native "Install" prompt will pick up the manifest automatically.

## Tech stack

Plain HTML, CSS, and vanilla JavaScript — nothing else. No frameworks, no libraries, no package manager. The Markdown-to-HTML conversion is a small hand-written parser rather than a third-party dependency, which is what keeps the whole app to a single portable file.

## Project structure

```
emdee.html   → the entire application (markup, styles, and logic in one file)
```

## Browser support

Any evergreen browser with standard ES5+ JavaScript and CSS Grid/Flexbox support. No transpilation or polyfills are used.

## Privacy

Emdee makes no network requests. Files you open are read locally via the browser's File API and never leave your machine.

---

## License

All rights reserved. This is a private, personal project. Source is not licensed for reuse, modification, or redistribution.

## Author

**Rolina Vorster** — Full-Stack Developer & Visual Experience Designer
[LinkedIn](https://www.linkedin.com/in/rolina-vorster) | [GitHub](https://github.com/RolinaVorster0101)
