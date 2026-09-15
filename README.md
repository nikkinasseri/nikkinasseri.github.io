# nikkinasseri.github.io

Nikki Nasseri's personal academic website — a static site (plain HTML/CSS/JS, no build step).

**Live site:** https://nikkinasseri.github.io

## How this deploys

This repo is a GitHub Pages **user site**. Every time you push to the `main` branch,
GitHub automatically rebuilds and republishes the live site — usually within about a
minute, no extra steps required.

```bash
# after editing files:
git add -A
git commit -m "Update site"
git push
```

That's it — refresh https://nikkinasseri.github.io shortly after pushing to see the change live.

## Editing locally with live preview

To see edits instantly in your browser as you save (auto-refresh), run a tiny local
server from the project folder:

```bash
cd nikkinasseri.github.io
python3 -m http.server 8000
```

Then open http://localhost:8000 in your browser. Reload the page after each save to see
changes (or use a "Live Server" extension in VS Code for automatic reload on save).

## Where to edit things

- `index.html` — all page content and structure (sections: About, Education, Research,
  Publications, Awards, Teaching, Contact).
- `css/style.css` — colors, fonts, spacing, layout. Color tokens are defined at the top
  under `:root` (light mode) and under the dark-mode media query.
- `js/script.js` — small interactive bits (mobile nav toggle, scroll-reveal animation).
- `assets/profile.jpg` — your photo (used in the hero section). Drop a new image here
  with this exact filename to swap it.
- `assets/Nikki_Nasseri_CV.pdf` — the downloadable CV linked from the "Download CV" button.

## Adding a custom domain (optional)

If you ever want e.g. `nikkinasseri.com` instead of the github.io URL, add a `CNAME` file
here with your domain, point your domain's DNS at GitHub Pages, then set it up under
your repo's Settings → Pages.
