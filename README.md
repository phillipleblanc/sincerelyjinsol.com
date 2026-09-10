# Sincerely Jinsol

Revived as a single-file static site (`public/index.html`), deployed with GitHub
Actions to GitHub Pages. CNAME: **jinsol.leblanc.tech**.

The 2020 Ghost "London" theme that powered the original site is preserved under
`legacy-theme/` for reference — it is not used for the live site.

## Layout

- `public/index.html` — the whole site: one HTML file with inline CSS and a
  few lines of JS (smooth scroll + photo detection).
- `public/assets/` — drop the card photos here as:
  `about.jpg`, `eat.jpg`, `play.jpg`, `mindfulness.jpg`, `love.jpg`,
  `lifestyle.jpg`, `travel.jpg` (~1200px wide looks right).
  Cards whose photo is missing render in the theme's classic big-numeral
  style automatically, so it never looks broken.
- `public/CNAME` — keeps `jinsol.leblanc.tech` wired to Pages.
- `.github/workflows/deploy.yml` — pushes to `master` publish the `public/`
  folder via `actions/deploy-pages`.

## Editing

Edit `public/index.html` and push to `master`. The section text is placeholder
copy — rewrite it in your own words directly in the HTML.
