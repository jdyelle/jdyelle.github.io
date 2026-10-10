# jeremy.yelle.dev

Personal site, CV, and tutorials. Built with Jekyll on GitHub Pages using a custom, theme-free layout.

## Layout

- `_config.yml`: site settings, author info, and the nav (`nav:`)
- `_layouts/`, `_includes/`, `assets/`: hand-written templates, CSS (`assets/css/site.css`), and JS
- `_data/cv.yml`: CV content (the `/cv/` page renders from this)
- `_data/adventures.yml`: trail log entries; add photos to `assets/img/adventures/`
- `Tutorials/`: tutorials (URLs are unchanged)

## Preview locally

With Docker (no Ruby install needed):

```sh
mkdir -p ~/.cache/jekyll-bundle
docker run --rm -u $(id -u):$(id -g) -e HOME=/tmp -e BUNDLE_PATH=/bundle \
  -v ~/.cache/jekyll-bundle:/bundle -v "$PWD":/srv/jekyll -p 4000:4000 \
  jekyll/jekyll:4.2.2 sh -c "bundle install --quiet && bundle exec jekyll serve --host 0.0.0.0"
```

Then open http://localhost:4000.
