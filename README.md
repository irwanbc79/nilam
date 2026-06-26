# IndoEssentialOil — Landing Page

Premium **patchouli (nilam) oil** exporter landing page for **[indoessentialoil.com](https://indoessentialoil.com)** — Aceh Jaya, Indonesia.

A single-file, dependency-free static site (HTML + inline CSS + vanilla JS). Bilingual **ID / EN**, fully responsive, SEO + Open Graph + JSON-LD ready.

## Structure

```
nilam/
├── index.html              # The site (self-contained, no build step)
├── assets/
│   ├── img/                # Real production photos (drums, warehouse, loading)
│   └── video/              # Real production videos
├── design-source/          # Original Claude design + full mockup (reference only)
└── README.md
```

## Local preview

```bash
cd nilam
python3 -m http.server 8080
# open http://localhost:8080
```

## Before going live — checklist

- [ ] **WhatsApp number**: edit `WA_NUMBER` in the `<script>` at the bottom of `index.html` (currently a placeholder `6285000000000`).
- [ ] **Email**: `info@indoessentialoil.com` — set up the mailbox or change the address.
- [ ] **Social links**: Instagram href is `#` — add the real profile.
- [ ] Optional: replace the SVG landscape / journey / bottle art with real photos when available (slots are in the About, Process, and Product sections).

## Notes

- The original was a Claude "design component" (`*.dc.html`) needing the `support.js` / `image-slot.js` runtime — **not deployable as-is**. This repo is the production rewrite: plain HTML, no runtime.
- `design-source/` is kept for reference and is **not** served.
- A private pricing/financial spreadsheet that was in the original ZIP was intentionally **excluded** — it must never be published.

## Deploy

Static hosting (Hostinger). Upload the contents of `nilam/` (excluding `design-source/`) to the domain web root.

🤖 Built with [Claude Code](https://claude.com/claude-code)
