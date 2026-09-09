# AH Web

`ah_web` is the canonical repository for simple public one-off webpages.

## Publishing model

GitHub Pages publishes the `main` branch from the repository root.

Each page normally lives in its own folder:

```text
ah_web/
├── page-one/
│   └── index.html
├── page-two/
│   └── index.html
└── assets/
    └── ah-web.css
```

A folder named `example-page` is published at:

```text
https://allanhewitt.github.io/ah_web/example-page/
```

Committing changes to `main` triggers GitHub Pages to republish automatically.

## House style

The canonical visual language is **AH Web Style v1**.

Read:

- `STYLE_GUIDE.md` for design principles and conventions.
- `assets/ah-web.css` for the shared implementation.
- `templates/standard-page.html` for the normal starting structure.

New pages should use the shared stylesheet unless there is a clear reason to depart from it.

The original reference implementation is `b1408-guide/index.html`.

## Working convention

For a new one-off page:

1. Create a short, stable folder slug.
2. Start from `templates/standard-page.html`.
3. Use `../assets/ah-web.css` for the shared style.
4. Add page-specific CSS only when the content genuinely needs it.
5. Keep published prose free of em dashes.
6. Commit to `main` and allow GitHub Pages to redeploy.
