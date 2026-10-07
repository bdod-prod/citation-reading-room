# Citation Reading Room

A static editorial guide by Alex Rostovtsev for checking whether a source page actually supports the specific answer claim beside it.

## File structure

- `public/index.html` — complete guide, fictional worked examples, source-type notes, resources and author section.
- `public/worksheet.html` — blank printable source-check worksheet.
- `public/resources/worksheet.md` — downloadable Markdown worksheet with matching fields.
- `public/404.html` — noindex fallback page.
- `public/robots.txt` — allows crawling.
- `public/assets/styles.css` — local site and print styles.
- `public/assets/favicon.svg` — local favicon.

## Preview locally

```bash
python3 -m http.server 8000 --directory public
```

Open `http://localhost:8000/`. There is no JavaScript and no build step.

## Editing

Edit the HTML and Markdown directly. The Morrow Coworking passages and reserved `.example` URLs are fictional and should remain clearly labelled if replaced.

## Production configuration

Production base URL: `https://citation-reading-room.onrender.com/`.

Render Static Site `srv-db3a62l9fdbs73afpejg` serves `public/` from the `main` branch of `bdod-prod/citation-reading-room`. Its command is `test -f public/sitemap.xml`, a publication check that does not build or transform the site. The public-repository connection uses manual deployment from the Render dashboard; it does not grant Render access to other repositories.

Canonical and Open Graph URLs use this origin; the sitemap lists the guide and printable worksheet. Root-aware links keep the fallback page styled when it is served at a nested missing path. No SPA rewrite is configured.

## Rendered review — 7 October 2026

The guide and worksheet were reviewed in Chromium at desktop width, 390 px and 320 px. Links, download files, metadata, keyboard focus and absence of external runtime requests passed. Print spacing and record breaks were corrected: the worksheet now occupies two A4 pages rather than five, with no blank continuation page. Printed labels and writing rules were refined; screen styling and outbound links are unchanged. See the root `BUILD-REPORT.md` for evidence and launch status. The user selected Render Static Sites in the existing Google-linked workspace.
