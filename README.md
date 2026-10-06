# seminar-3d-rendering-comaputational-art-2026

Seminar Landing Page for the Software Prototypes of the 2026 3D Rendering & Computational Art seminar at the research group of Computer Graphics Systems, Hasso Plattner Institute and Digital Engineering Faculty, University of Potsdam.

## Build

Install the locked dependencies and generate the production site in `build/`:

```sh
npm ci
npm run build
```

Pug 3 templates use `@webdiscus/pug-loader`. Project URLs in
`source/data/projects.yaml` are strings; use `"#"` for placeholders and `[]` for
empty contributor lists.

## Publish to GitHub Pages

```sh
npm run publish
```

This rebuilds the site and, only if the build succeeds, publishes `build/` to the
`gh-pages` branch of the `origin` remote. Configure GitHub Pages to serve that
branch from its root directory. Asset URLs are relative so the site can be served
under the repository path.
