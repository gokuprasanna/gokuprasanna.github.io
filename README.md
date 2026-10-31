# Prasanna Vijayaraghavan

Personal academic website built with Jekyll and hosted with GitHub Pages.

- Research profile: [ORCID](https://orcid.org/0000-0002-6036-651X)
- Publications: [Google Scholar](https://scholar.google.com/citations?user=f74k65cAAAAJ)

## Local preview

Install Ruby and Bundler, then run:

```sh
bundle install
bundle exec jekyll serve
```

Open `http://localhost:4000` to preview the site.

## Updating the site

- Personal details and links: `_config.yml`
- Page content: `_pages/`
- Education: `_data/pi.yml`
- Publications: `assets/ref.bib`
- Profile photo: `images/`

## Publishing

The GitHub Actions workflow in `.github/workflows/deploy.yml` builds and deploys
the site when changes are pushed to `main`. In the repository's **Settings >
Pages**, set the source to **GitHub Actions**.

## Credits

This site is built on the
[academic-website-template](https://github.com/sbryngelson/academic-website-template)
by Spencer Bryngelson, used under the MIT License (see `LICENSE`).
