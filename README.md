# Transportation Intelligence Lab Website

This repository contains the source for the Transportation Intelligence Lab website, built with the
al-folio Jekyll theme and customized for a research group website.

## Local Preview

Install dependencies once:

```bash
bundle install
```

Build the site:

```bash
bundle exec jekyll build
```

Serve locally:

```bash
bundle exec jekyll serve
```

## Deployment

The site is configured for GitHub Pages at:

```text
https://scottlzh.github.io/scottlzh/
```

Pushes to `main` trigger the deployment workflow, which builds the Jekyll site
and publishes the generated `_site` output to the `gh-pages` branch.
