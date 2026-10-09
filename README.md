# Mousehold Cat Café

A cat-café concept and creative project. **Mousehold** is the lead brand; **Mousehold Cat Café**
makes the idea clear. The name plays on "mouse" + "household" and evokes a cozy sanctuary.

**Live:** https://mousehold.cafe/ — currently a placeholder page.

## Status

Early. This repo holds a static placeholder while the first real piece gets decided.
Nothing here is a commitment to a launch scope, a location, or a schedule.

## Possible directions

Captured as ideas, not deliverables:

- **The Cats** — profiles, photos, personalities, favorite things, and stories.
- **Virtual Café** — cozy online rooms where visitors spend time with different cats.
- **Cat of the Week** — a chosen cat, written up.
- **Menu Lab** — invented café drinks and treats, with visitor votes.
- **Mousehold Journal** — drawings, logo experiments, décor concepts, progress.
- **Adoption Corner** — adoptable cats via local shelters.

## Structure

```
index.html   # placeholder page, single file, no dependencies or build step
.nojekyll    # serve files as-is; skip GitHub's Jekyll processing
CNAME        # GitHub Pages custom domain (mousehold.cafe)
assets/      # images used by the page:
             #   sleeping-kitten.webp   kitten resting on top of the card
             #   kitten-eyes-open.webp  layered over it; he is mostly awake, blinks, and dozes briefly
             #   kitten-tail.webp       80-frame sprite sheet (10 x 8); his tail sways under the card
             #   mouse-run.webp         24-frame sprite sheet (6 x 4); the mouse that runs to its hole
             #   cat-pattern.webp       tiled page background of cat outlines (cat-pattern-dark.webp in dark mode)
             #   mousehold-logo.svg     the logo, used as the page title at 75% of the page width
             #                          (mousehold-logo-light.svg in dark mode); traced from the logo PNG
```

## Local preview

No build step. Open `index.html` directly, or serve it:

```sh
python3 -m http.server 8000
# → http://localhost:8000
```

## Deploy

GitHub Pages serves `main` at the repo root. Pushing to `main` publishes.

## Domain

`mousehold.cafe` is registered at Namecheap, with DNS on Cloudflare. Two DNS-only CNAME records
(`@` and `www`) point to `yuxt.github.io`. The `CNAME` file sets the GitHub Pages custom domain,
HTTPS is enforced, and `www.mousehold.cafe` redirects to `mousehold.cafe`.
