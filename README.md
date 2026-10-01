# Forme House

**[Explore FORME HOUSE live](https://lym-loveyours.github.io/brand-house-showcase/)**


A fictional brand-house experience by **Love Yours Media**. Adapted from prior studio work, this study explores how a confident editorial system can support five distinct identities.

![Forme House desktop preview](docs/screenshots/home-desktop.png)

## Explore the work

Thirteen routes: the homepage, label index, five label stories, an about page, a journal and three articles, and a browser-only enquiry demonstration. A custom 404 completes the experience.

The design combines oversized typography, a precise grid, warm textile imagery and a rust accent. The five fictional labels use different type treatments within the same navigation and layout system. Responsive layouts, keyboard access and reduced-motion preferences are built in.

## Run locally

Requirements: Node.js 22 or newer, npm, Python 3 for the local static preview.

```sh
npm ci
npm run build
npm run preview
```

Open http://127.0.0.1:9404/. Development mode: `npm run dev`.

```sh
npm run typecheck
npx playwright install chromium firefox webkit
npm test
npm audit
```

The production build is a static export in `out/`. `npm run build` targets a domain root. For the proposed GitHub Pages repository path, run `npm run build:pages` followed by `npm run test:pages`; this sets `/brand-house-showcase` consistently for navigation, scripts, imagery and fonts. Publish that output only after approval. Re-run `npm run build` to restore the root preview. No hosting or publication is included.

## Demonstration boundaries

Forme House and its five labels are fictional identities, with no affiliation to real businesses intended. The articles are illustrative design writing. No client results, trading history, licences, credentials or supplier relationships are claimed.

The form has no API, email transport or database. JavaScript validates entries, clears the fields and displays a truthful completion message. Use fictional information. There is no analytics or tracking integration, and all fonts and imagery are served locally.

## Build and attribution

Next.js / React / TypeScript; authored CSS; static export; Playwright and axe checks. This version re-expresses a previous studio layout direction with newly written fictional content and a reduced dependency surface. No private Git history, client marks or operational integrations are included.

See [QA](QA.md), [asset manifest](ASSETS.json), [provenance](PROVENANCE.md) and [licence](LICENSE). Automated accessibility checks cover a subset of accessibility requirements; they are not a certification.

[Love Yours Media](https://loveyoursmedia.com)
