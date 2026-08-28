# Yena Choi — academic portfolio

Personal academic website built on the [al-folio](https://github.com/alshedivat/al-folio) Jekyll theme.

## Before you deploy

A few things are still placeholders — search the repo for `YOUR_GITHUB_USERNAME` and `TODO` and fill these in:

- **`_config.yml`** — set `url` (and `baseurl` if this isn't a `<username>.github.io` repo) to match where you deploy.
- **`_data/socials.yml`** — set `github_username` (LinkedIn is already filled in); optionally add `scholar_userid`, `orcid_id`.
- **`_data/repositories.yml`** — add your GitHub username under `github_users`, and any more `mirage-cikm` (or other) repos you want shown under `github_repos`.
- **`_news/*.md`** — the announcement dates are placeholders; adjust to the real dates.
- **`_data/cv.yml`** — real CV data (education, experience, awards, publications) is filled in and the CV page is enabled. Note: this theme only gives rich date/location/highlight formatting to a section literally named `Experience` (it also merges in `Volunteer`) — any other custom section name falls back to a bare-bones renderer, so all experience-type entries live under that one `Experience` list, sorted by date.

## Local preview

```bash
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000.

## Deploying to GitHub Pages

1. Create a new GitHub repository (name it `<your-username>.github.io` to serve at the domain root, or anything else for a project site).
2. Push this folder's contents to that repository's `main` branch.
3. In the repo's **Settings → Pages**, set the source to **GitHub Actions** (the included `.github/workflows/deploy.yml` handles the build).
4. Push — the site builds and deploys automatically within a few minutes.

## Adding publications

Edit `_bibliography/papers.bib` — each `@inproceedings`/`@article` entry becomes a publication card automatically. See [al-folio's customization docs](https://github.com/alshedivat/al-folio/blob/master/docs/CUSTOMIZE.md) for all supported fields (`pdf`, `code`, `slides`, `poster`, `video`, etc.).
