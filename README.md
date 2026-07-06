# Curtin ML Group — Handbook

Source for the group handbook site, built with [MkDocs Material](https://squidfunk.github.io/mkdocs-material/).

## Preview locally
```bash
pip install -r requirements.txt
mkdocs serve        # then open http://127.0.0.1:8000
```

## Edit
Pages are Markdown files in `docs/`. Edit a page and open a pull request. On merge to `main`, the site republishes automatically.

## Publish
Pushes to `main` build and deploy the site via GitHub Actions (`.github/workflows/pages.yml`).
To turn the public site on: **repo Settings → Pages → Source: GitHub Actions**.
