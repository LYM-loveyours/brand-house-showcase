# Local validation — 1 October 2026

- Production static export: PASS, 13 content routes plus 404.
- TypeScript: PASS (`npm run typecheck`).
- Playwright: **32 passed**, 2 intentionally skipped duplicate mobile invocations of the dedicated desktop Firefox/WebKit test. No failing tests.
- Chromium: all 13 routes at 1440 × 1000 and 390 × 844; one heading, no horizontal overflow, no page errors or failed assets; axe WCAG 2 A/AA and 2.1 AA checks passed on those pages.
- Chromium desktop/mobile: menu/index navigation, native form validation, cleared fields, zero POST requests and no local/session storage writes.
- Firefox and WebKit: keyboard skip link, contact navigation, non-sending form completion and reduced-motion behaviour. On macOS WebKit, Option+Tab is used to include links in keyboard navigation.
- GitHub Pages subpath: `npm run build:pages` and `npm run test:pages` PASS. Verified `/brand-house-showcase/` home → index → label navigation, scripts, imagery and fonts locally. Root build restored afterwards.
- Dependency audit: zero known vulnerabilities in the local npm audit result.
- Visual inspection: desktop/mobile homepage and label viewport captures, desktop index and statement captures under `docs/screenshots/`.

The checks use local production output. Hosted GitHub Actions/Pages, physical devices, assistive-technology user testing, exhaustive keyboard journeys and field performance are unverified. Automated accessibility checks are not a full accessibility audit. The workflow is configured with read-only repository permissions and does not publish.

No real enquiry delivery exists or was tested. No repository, hosting or profile changes are made by this project. The publication decision is separate.
