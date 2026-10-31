# Kangxian Xie · Personal website

Academic homepage: https://kangxian97.github.io

A static Jekyll website hosted on GitHub Pages. The main pages use a shared, responsive layout with no JavaScript or frontend build step.

## Editing content

- `_pages/about.md`: biography, research aspiration, latest work, and news.
- `_publications/`: publication metadata and detail pages. `project_name: CoWTalk` selects the featured homepage paper.
- `_pages/cv.md`: education and research experience.
- `_teaching/`: course records.
- `_config.yml`: name, affiliation, contact information, and site metadata.
- `_layouts/academic.html` and `assets/css/academic.css`: shared page structure and styling.
- `_includes/publication-entry.html`: publication lists shared by the homepage, publications page, and CV.
- `images/research/README.md`: research figure provenance.

Existing publication and teaching permalinks are retained. Publication lists are generated from the same collection and sorted by date.

## Local preview

With Ruby and Bundler available:

```sh
bundle install
bundle exec jekyll serve --host 127.0.0.1 --port 4173
```

Open http://127.0.0.1:4173/. Use the Jekyll server for preview: it supports the extensionless URLs used by GitHub Pages.

To check the production build:

```sh
JEKYLL_ENV=production bundle exec jekyll build
```

Build output, dependencies, local working materials, and the original research PDF are ignored by Git. The `local/` and `vendor/` directories are also excluded from the published site.

## Credits

This repository was originally based on [AcademicPages](https://github.com/academicpages/academicpages.github.io), built on the Minimal Mistakes Jekyll theme. The legacy layouts and assets remain available. See `LICENSE` for the original license.
