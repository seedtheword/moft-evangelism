# Messenger of Truth — Evangelism Stand Landing Page

A single-page landing site for MOFT Church's Lake Stevens evangelism stand. People at the stand scan a QR code on the table cloth or a printed sign and land here. They get three clear actions:

1. Take the community survey (Google Forms)
2. Submit a prayer request (mailto)
3. Visit the main church website (https://messengeroftruth.org/)

## What's in here

- `index.html` — the entire site. One file. No build step.
- `assets/images/` — empty for now. Add MOFT photos here if you want to swap the inline SVG cross for the real logo file.

## How it's hosted

GitHub Pages, free tier, no build step.

1. Push this repo to GitHub.
2. Repo Settings → Pages → Source: `Deploy from a branch` → Branch: `main` → folder: `/ (root)` → Save.
3. Wait ~1 minute. The site is live at `https://<your-username>.github.io/moft-evangelism/`.
4. Generate a QR code pointing to that URL. Print it on the tablecloth or sign.

## Customizing

Everything you'd want to edit lives in `index.html`. The most common edits:

| What | Find this in `index.html` |
|---|---|
| Survey link | the `href` on the first `<a class="action--primary">` |
| Prayer request email | the `mailto:` on the second `<a class="action">` |
| Main church URL | the `href` on the third `<a class="action">` |
| Stand address | the `<p class="stand-info__address">` block |
| Page colors | the `:root` CSS variables at the top of the `<style>` block |
| Verse | the `<blockquote>` near the bottom |

## Forking

If MOFT wants to host this on their own GitHub later, the repo is self-contained — no external dependencies beyond Google Fonts (loaded over CDN). They fork, change the survey link if it ever rotates, and re-publish under their own Pages URL. The page itself never needs to change.

## License

Page content (copy, structure, design) is released for MOFT's use. Cormorant Garamond and Inter are loaded from Google Fonts (Open Font License). The cross-mark SVG is original and free to use.
