# yihshe.github.io

Personal website of Yihang She, built with [Academic Pages](https://github.com/academicpages/academicpages.github.io) (Jekyll) and hosted on GitHub Pages. The site is a single page plus header links; pushing to `master` redeploys it automatically.

## Where to edit things

| What | File |
|---|---|
| Homepage content (about, research, publications, news) | `_pages/about.md` |
| Header links (Publications → Google Scholar, CV, News → LinkedIn) | `_data/navigation.yml` |
| Sidebar profile (name, photo, email, social icons) | `author:` section of `_config.yml` |
| Site title / description | top of `_config.yml` |
| CV and other PDFs | `files/` |
| Profile photo and favicons | `images/` |

### Common tasks

- **Update the CV**: drop the new PDF into `files/`, then update the CV URL in `_data/navigation.yml` (and remove the old PDF).
- **Add publication links (paper / slides / talk / poster)**: in `_pages/about.md`, each publication entry has an HTML comment containing placeholder links — replace `GDRIVE_LINK` / `YOUTUBE_LINK` / `ARXIV_LINK` with the real URLs and move the links outside the `<!-- -->` markers so they show.
- **Add a publication**: copy one of the existing entries in the *Selected Publications* section of `_pages/about.md`.

Everything else (`_layouts/`, `_includes/`, `_sass/`, `assets/`) is theme machinery and rarely needs touching.

## Preview locally

With Ruby/Bundler:

```bash
bundle install
bundle exec jekyll serve -l -H localhost
# open http://localhost:4000
```

Or with Docker:

```bash
docker compose up
```
