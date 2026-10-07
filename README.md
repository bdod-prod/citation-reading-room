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

## Pending launch metadata

The production origin is not known yet. Canonical URLs, `og:url`, an absolute sitemap and host-specific configuration are intentionally omitted until launch.

## Rendered review — 7 October 2026

The guide and worksheet were reviewed in Chromium at desktop width, 390 px and 320 px. Links, download files, metadata, keyboard focus and absence of external runtime requests passed. Print spacing and record breaks were corrected: the worksheet now occupies two A4 pages rather than five, with no blank continuation page. Printed labels and writing rules were refined; screen styling and outbound links are unchanged. See the root `BUILD-REPORT.md` for evidence and launch status. Hosting remains pending the user's choice.
