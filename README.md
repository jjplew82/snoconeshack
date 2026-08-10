# Sno Cone Shack — Website

One file, no build step: `index.html` is the entire site (HTML, CSS, and JS
all inline). Push it to a repo and turn on GitHub Pages, and you're live.

## To go live with GitHub Pages
1. Create the repo and add `index.html` to the root.
2. In the repo, go to **Settings → Pages**.
3. Under "Build and deployment," set Source to **Deploy from a branch**,
   branch `main`, folder `/ (root)`.
4. Save — GitHub gives you a URL in a minute or two.

## What to edit as things change

| What | Where in `index.html` | Search for |
|---|---|---|
| Flavors | Menu section | `Today's Flavors` |
| Weekly schedule / stops | Find Us section | `EDIT ME: this week's real stops` |
| Instagram / Facebook links | Find Us section | `EDIT ME: point these at your real accounts` |
| Trailer photos | Gallery section, once you have real shots | `EDIT ME: once you have real photos` |
| Booking form destination | Bottom of the file, in the `<script>` | `EDIT ME: wire this up to a real backend` |

## The booking form
Right now the form shows a "thanks, not wired up yet" message and doesn't
actually send anywhere. Easiest ways to make it real, no server needed:
- **Formspree** (formspree.io) — free tier, just point the form's `action`
  at the endpoint they give you.
- **Netlify Forms** — if you end up hosting on Netlify instead of GitHub
  Pages, add `netlify` as a form attribute and it works automatically.

## Photos
The gallery section currently has four dashed placeholder boxes. Once the
trailer's decorated for a wedding, a coffee bar, etc., add an `images/`
folder next to `index.html`, drop the photos in, and swap each placeholder
`<div class="gallery-slot">...</div>` for an `<img src="images/your-photo.jpg" alt="...">`.

## Brand assets
The logo, sign, and coin designs from the branding round live alongside
this in case you want them for print or social: the badge/sign HTML files
and the print-ready sign and coin JPGs.
