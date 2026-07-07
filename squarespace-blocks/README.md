# Squarespace code blocks (Phase C)

Paste-ready HTML for the two custom sections that native Squarespace
blocks can't do. Everything else in the redesign is native Squarespace.

## Files
- `1-scent-band.html` — the dark "one scent, three ways" band. Static, no JS.
- `2-ceramics-gallery.html` — the dark ceramics gallery grid + click-to-open
  lightbox. Includes a small script for the pop-up.

## How to use
1. In the Squarespace page editor, add a **Code Block** where you want the
   section, and paste the whole file contents in.
2. Ceramics only: if the pop-up doesn't open, move the `<script>…</script>`
   from the bottom of the block into **Settings → Advanced → Code Injection →
   Footer**. (Squarespace sometimes strips scripts inside code blocks.)
3. Ceramics only: give your "Commissioning a piece" section the anchor/block
   ID `pda-commission` so the "Commission Your Own Piece" button scrolls to it.
   If it can't find it, the button opens an email instead — still works.

## Before launch
The image URLs currently point at the GitHub Pages mockup
(danieldiazrn.github.io/...), which is fine for testing. For production,
re-upload the images to Squarespace and swap the URLs to the Squarespace-hosted
versions so the site doesn't depend on the GitHub repo staying up.

All CSS classes are prefixed `pda-` so they won't collide with Squarespace's
own styles.
