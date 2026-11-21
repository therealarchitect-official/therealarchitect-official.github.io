# Project Overview: TheRealArchitect — Three Separate Visual Portfolios

This is the official portfolio site for **TheRealArchitect**, built as plain static HTML, CSS, and JavaScript (no frameworks, no build step). It is intentionally **not** a terminal/CRT/command-prompt interface — that direction was abandoned. The site is three separate pages, each with its own visual identity:

1. **`index.html` — Main portfolio (the original design, source of truth)**
   - Light "paper and ink" aesthetic: `#f2f0e9` background, `#20231f` ink, `#e44d32` accent.
   - Fonts: **Londrina Solid** (display) and **Righteous** (body) from Google Fonts.
   - Keep its existing content and working interactions intact: the category tabs (Concepts / Games / Repositories), the "Gamify The Portfolio" Boredom Slasher game window, and the Projects page links.
   - This page links to the two other portfolios via the nav and the "Two more worlds" section.

2. **`geometry-dash.html` — Geometry Dash portfolio (RealArchitectGD)**
   - Energetic game-world styling: dark teal night background, glowing cyan/gold neon, pixel fonts (**Press Start 2P**, **VT323**), geometric cube motifs.
   - Sections: Levels & IDs (placeholders until real level names/IDs exist), Collabs, plus a link to the Geometry Dash Web preview.
   - **Credit Geometry Dash Web to GDColon.**

3. **`munet-dash.html` — Munet Dash portfolio (ArchitectMunet)**
   - Playful pastel look (lavender/pink/gold, rounded shapes, Fredoka font) — must stay visually distinct from both other pages.
   - Features the fan-made Munet Dash Web project, custom assets, and a prominent playable-preview link.
   - **Credit Munet Dash to Munetios, and Munet Dash Web to TheRealArchitect.**

## Placeholders & Verified URLs
- Only use URLs that exist in this repository (e.g. the Boredom Slasher page, the ZenithOS Figma site, the GitHub org).
- The `geometry-dash-web` and `munet-dash-web` GitHub Pages URLs are **placeholders** (they are referenced in the repo but are not live). They are clearly marked in the pages — swap them for real URLs when the projects ship.
- Do not invent level names, Geometry Dash level IDs, collaborators, or external URLs (including GDColon's Geometry Dash Web URL).

## Shared Rules
- Navigation must connect all three portfolios (and `projects.html`) so every page is reachable.
- Keep everything plain HTML/CSS/JS, mobile-friendly (test ~360px widths), and accessible (landmarks, `aria-current`, focus outlines, `prefers-reduced-motion`, alt/aria-labels for decorative art).
- No terminal UI, command prompts, or CRT scanline styling anywhere in these three portfolios.
- `favicon.png` is the TRA pixel favicon — keep it linked in `<head>`.
