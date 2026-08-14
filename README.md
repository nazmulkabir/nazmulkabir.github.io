# nazmulkabir.com

Personal academic website of [Md Nazmul Kabir Sikder](https://nazmulkabir.com), built with
[Jekyll](https://jekyllrb.com/) on the [academicpages](https://github.com/academicpages/academicpages.github.io)
template (MIT licensed — see `LICENSE`).

## Structure

| Path             | Contents                                                        |
| ---------------- | --------------------------------------------------------------- |
| `_pages/`        | Top-level pages: about (home), publications, portfolio, people, CV |
| `_publications/` | One Markdown file per publication                                 |
| `_posts/`        | News items, surfaced at `/year-archive/`                          |
| `_portfolio/`    | Project entries                                                   |
| `_talks/`        | Empty — unlinked in nav until content is added                    |
| `_teaching/`     | Empty — unlinked in nav until content is added                    |
| `media/`         | Images and publication PDFs (paths preserved from the old site)   |
| `cv/`            | Resume PDFs                                                       |
| `projects-html/` | Standalone long-form project write-ups linked from the portfolio  |
| `_config.yml`    | Site settings, author profile, publication categories             |
| `_data/navigation.yml` | Header navigation                                           |

## Local development

Requires Ruby. With Bundler:

```bash
bundle install
bundle exec jekyll serve --livereload
```

Then open <http://localhost:4000>.

Or with Docker (no Ruby install needed):

```bash
docker compose up
```

## Deployment

`.github/workflows/deploy-pages.yml` builds the site on every push and pull request.
It **deploys to GitHub Pages only from `main`** — pushes to other branches build for
verification without touching the live site.

The `CNAME` file pins the custom domain to `nazmulkabir.com`.

## Adding content

- **Publication** — add `_publications/YYYY-MM-DD-slug.md` with a `category` of
  `books`, `manuscripts`, `conferences`, `chapters`, or `theses` (defined in `_config.yml`).
- **News** — add `_posts/YYYY-MM-DD-slug.md`.
- **Project** — add `_portfolio/slug.md`.
- **Talks / Teaching** — add files to `_talks/` or `_teaching/`, then uncomment the
  matching entries in `_data/navigation.yml`.
