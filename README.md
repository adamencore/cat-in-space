# Cat in Space — Deployment Kit

A hand-drawn space arcade game. One self-contained HTML file with everything inlined (sprites, backgrounds, fonts via Google Fonts).

## What's in this folder

- **`cat-in-space.html`** — The whole game. Open it in any browser. ~3.35 MB.
- **`favicon-32.png`** — Standalone favicon. The HTML already has this inlined, but you may want it as a file for some hosts.
- **`apple-touch-icon.png`** — Standalone Apple touch icon (180×180). Same deal.
- **`icon-192.png` / `icon-512.png`** — App icons for PWA / "Add to Home Screen."

The HTML file is the only file you actually need to deploy. The PNGs are extras in case a host wants standalone icon files.

## Test it locally first

Just double-click `cat-in-space.html`. It runs in any modern browser with zero setup. Works offline once loaded.

## Deploy options (pick one)

### Option 1: Netlify Drop (easiest, free, ~30 seconds)
1. Go to https://app.netlify.com/drop
2. Drag `cat-in-space.html` (or this whole folder) onto the page
3. You'll get a random URL like `https://glittering-cat-9af2c1.netlify.app`
4. Share that URL with playtesters
5. Optional: rename the URL in site settings → "Change site name" to something like `playcatinspace`

### Option 2: Netlify under adamrecordmusic.com
If you want it as `adamrecordmusic.com/cat-in-space`:
1. In your existing Netlify site's repo, create a folder `cat-in-space/`
2. Put `cat-in-space.html` inside, renamed to `index.html`
3. Commit and push — Netlify auto-deploys
4. Visit `adamrecordmusic.com/cat-in-space`

### Option 3: GitHub Pages
1. Create a new repo, e.g. `cat-in-space`
2. Add `cat-in-space.html` renamed to `index.html`
3. Settings → Pages → Source: deploy from main branch
4. URL: `https://YOUR_USERNAME.github.io/cat-in-space`

### Option 4: Anywhere else
Upload the HTML to any static host. The file is fully self-contained. No build step, no env vars, no server-side logic.

## Soft-launch notes

The current build has these soft-launch defaults baked in:

- **`<meta name="robots" content="noindex" />`** — Search engines won't index it. Safe to share a link without it showing up in Google.
- **No-cache headers** — Testers will get the freshest version every load. Important during iteration; you'll want to remove this for the public launch (cache makes loads instant on return visits).

When you're ready to go fully public, ask me to flip both of those.

## Playtest checklist

A few things worth gathering from testers:

- **Device:** iPhone model / Android model, browser used
- **First impression:** Did they figure out the donuts-are-good rule without being told?
- **Difficulty curve:** What level did they reach? Did it feel fair, too hard, too easy?
- **The cat size:** Big enough? Too big?
- **The miss penalty:** Did −25 feel right, or annoying?
- **Bugs:** Anything weird with touch controls, flickering, layout on their device

## Iterating

When you want changes, send me your feedback + this HTML file (or just describe what you want changed). I have the source — I can rebuild quickly and hand you a new HTML to drop in. Same filename means same URL → testers just refresh.

---

Built with Adam's art. Have fun.
