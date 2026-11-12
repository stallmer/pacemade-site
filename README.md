# pacemade.app

The public website for Pacemade: a landing page, support, and privacy policy. Plain HTML and CSS, no build step and no JavaScript.

## Layout

```
index.html           Landing page
support/index.html   Support and FAQ
privacy/index.html   Privacy policy
schema/plan-v1.json  The plan JSON Schema (copy of pacemade/schema/pacemade-plan.schema.json)
assets/              Stylesheet, icons, app screenshots
credits/             Open source credits (Phosphor Icons MIT notice for the app icon runner)
CNAME                Custom domain for GitHub Pages
404.html, robots.txt, sitemap.xml
```

## Preview

```
python3 -m http.server 8000
```

Then open http://localhost:8000. Links use root-relative paths (`/support/`), so preview from this folder's root.

## Keeping it in sync

- `support/` and `privacy/` mirror the text of the Pacemade Support Page and Privacy Policy notes in the Obsidian vault (`07 - Pacemade`). Change both together.
- `schema/plan-v1.json` must match `schema/pacemade-plan.schema.json` in the app repo.
- Update the screenshots in `assets/` when the app's screens change.
- Update the privacy policy before shipping any feature that touches user data.
