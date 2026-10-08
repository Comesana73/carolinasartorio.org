# carolinasartorio.org

Personal website of Carolina Sartorio. Plain HTML and CSS — no build step. GitHub Pages serves the files as they are.

## Pages

- `index.html` — home (bio, books, recent papers)
- `books.html` — books, with symposia and reviews
- `papers.html` — all papers, filterable by topic and searchable
- `style.css` — all styling (light and dark mode)

## Adding a paper

In `papers.html`, copy an existing `<li class="paper">` block into the right year's section (or copy a whole `<section class="year-group">` for a new year), then edit the title, link, venue, and description.

- `data-topics` sets which topic buttons show the paper, separated by `|` (for example `causation|free will`).
- `data-search` is the lowercase text the search box looks through; put the title and journal there.

To feature it on the home page, also replace one of the four papers under "Recent papers" in `index.html`.

## PDFs

Paper PDFs currently link to her Rutgers site. To host them here instead, add a `papers/` folder with the PDFs and change the links to `papers/Filename.pdf`.

## Custom domain (carolinasartorio.org)

1. At the domain registrar, add four `A` records for the bare domain pointing to `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`, and a `CNAME` record for `www` pointing to `comesana73.github.io`.
2. In this repo: Settings → Pages → Custom domain → `carolinasartorio.org` → Save. Tick "Enforce HTTPS" once it becomes available.
