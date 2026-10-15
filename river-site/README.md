# River project documentation site

A static HTML, CSS, and JavaScript website. No npm dependencies or build step is required to serve it.

## Run locally

1. Extract this ZIP.
2. Open a terminal in the extracted folder.
3. Run: python -m http.server 8000 --directory dist
4. Open http://localhost:8000

On Windows, use `py` instead of `python` if needed.

Use a local server: links begin with `/` and are designed for the website root.

## Edit

- dist/index.html: project overview
- dist/projects/: individual documentation pages
- dist/about.html: About page
- dist/style.css: styling and responsive layouts
- dist/app.js: search, filters, and mobile navigation
- dist/projects.json: exported project data (not loaded dynamically)
- build.py: generator containing project content and page templates

To regenerate the pages, run `python build.py`. Regeneration replaces generated files, so make content/template edits in build.py if using the generator.

For hosting, upload the contents of dist/ to the root of a static website. Google Fonts are loaded remotely, with local font fallbacks.
