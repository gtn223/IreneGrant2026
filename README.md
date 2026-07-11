# Irene & Grant — Animated Wedding Invitation

A web-based wedding invitation. Tall ornate gates — joined by a white wax seal
bearing the couple's gold IG monogram — swing open in 3D toward the viewer to
reveal a full-height carousel of the invitation cards, over a softly blurred
gradient from light purple into deep forest green.

## Single self-contained file
`index.html` contains everything embedded inside it — the gate images, the three
invitation cards, the blurred gradient background, and the IG monogram logo. No
separate `assets` folder is needed to run it. Just open or upload the one file.

## Features
- A white circular **seal** with the gold IG logo, split into two halves — one
  embedded in each gate on the same 3D plane — so it opens perfectly evenly with
  the gate animation (the seam runs exactly down the middle).
- Tall gates sized to the carousel: when they open, the revealed card lands in
  the same full-height footprint.
- 3D gate opening (tap, click, Enter/Space).
- Softly blurred background gradient: light purple at the top flowing down into
  deep forest greens, with a slow drifting depth layer. No butterflies.
- White "Tap to open" button centered under the names.
- Auto-advancing carousel: arrows, dots, swipe, ← → keys.
- **RSVP** button links directly to
  <https://www.zola.com/wedding/ireneandgrant2026> (new tab).

## Preview locally
Double-click `index.html`, or run a static server:
```bash
python3 -m http.server 8000   # http://localhost:8000
```

## Host on GitHub Pages
1. Create a repo, e.g. `irene-and-grant`.
2. Upload **`index.html`** (that single file is all you need).
3. Repo → **Settings → Pages** → Source: Deploy from a branch → Branch `main`,
   folder **/ (root)** → Save.
4. Live in ~1 min at `https://YOUR-USERNAME.github.io/irene-and-grant/`.

## Customize
- **RSVP link:** search the Zola URL in `index.html`.
- **Background colors/blur:** the `#base` gradient stops in the background SVG
  and the `filter:blur(...)` on `.garden-bg`.
- **Seal size:** the `--seal` variable at the top of the CSS.
- **Gate/carousel height:** the shared `height`/`max-height` on `.gate-wrap`
  and `.carousel`.
