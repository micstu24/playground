# Michelle Stunkard — Playground Site

A personal site blending GTM ops work, learning Claude, and life outside of work
(arts &amp; crafts, family). Built as static HTML/CSS/JS — no build tools required.

## Structure

```
index.html                          → homepage (hero, about, Playground feed, toolkit)
projects/
  martech-roi-audit.html            → first real project page (filled out, needs your details)
  coming-soon.html                  → placeholder every unwritten card currently links to
  template.html                     → blank copy of the project page layout for new write-ups
```

## What's real vs. placeholder right now

- The **MarTech Stack ROI Audit** page has the real layout and structure, but the body
  content is bracketed placeholder text — `[Replace with real detail: ...]`. Fill that in
  with your actual audit process and numbers.
- Every other card on the homepage links to `coming-soon.html` for now.

## Adding a new project page

1. Copy `projects/template.html` to a new file, e.g. `projects/funnel-anomaly-diagnosis.html`.
2. Fill in the title, stamp/tag color (`.stamp` classes: default blue = Work, `.claude` = amber,
   or add `.art` / `.mom` variants by copying the color values from `index.html`'s `:root`).
3. Replace the bracketed placeholder sections with real content.
4. In `index.html`, find the matching card and change its link from `projects/coming-soon.html`
   to your new file.

## Next steps in Claude Code

1. Open this folder in Claude Code.
2. Run `git init` and commit, so you have version history as you keep adding to it.
3. Deploy for free with Vercel, Netlify, or GitHub Pages — any of them will auto-deploy
   from a git repo with no config needed for a static site like this.
4. Optional: connect a custom domain once you're happy with it.

## Privacy note

`index.html` and every page in `projects/` have a `<meta name="robots" content="noindex, nofollow">`
tag, so none of this gets indexed by search engines while you're still building. Remove that
tag from a page whenever you're ready for it to be discoverable.
