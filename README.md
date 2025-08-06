# Karross Documentation

This repository contains the source files for the Karross framework documentation.

- Written in Markdown
- Built using [MkDocs](https://www.mkdocs.org/)
- Deployed to: [https://karross.github.io](https://karross.github.io)

## How to contribute and run your changes locally

First, clone the repository:

```bash
git clone git@github.com:Karross/docs.git
cd docs
```

Install mkdocs and serve the doc.
```bash
pip install mkdocs
mkdocs serve
```

Visit [http://127.0.0.1:8000/](http://127.0.0.1:8000/) in your browser.

When satisfied, open a merge request.

## How to deploy for owners

First, pull the last changes for this repository

```bash
git pull
```

Then clone the repository of the documentation website at the same level.

```bash
cd ..
git clone git@github.com:Karross/karross.github.io.git
cd karross.github.io
```

Generate the static website in the "site" directory of the "docs" repository and deploy it online.

```bash
mkdocs gh-deploy --config-file ../docs/mkdocs.yml --remote-branch main
```
