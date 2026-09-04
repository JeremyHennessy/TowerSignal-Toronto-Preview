# Toronto Preview Release Evidence

This file records the latest verified Toronto preview deployment and preserves the prior release checkpoint for traceability.

## Latest verified UI/navigation checkpoint — September 4, 2026

### Deployed source

- Source repository: `JeremyHennessy/TowerSignal`
- Exact source commit: `2eea1e2d5cbf0d9cf24d2325eb3a4222806ba6ea`
- Preserved source branch: `release/toronto-20260904-ui-nav-2963934`
- Wrapper repository: `JeremyHennessy/TowerSignal-Toronto-Preview`
- Wrapper commit used for the verified UI-only Pages deployment: `dc03c2acdc8318cf80784fdb36231792b8a053a0`
- Workflow: `Deploy Toronto Preview UI Hotfix`
- Workflow run: `33878785920`
- Deployment conclusion: `success`

### Data preservation proof

This release is a UI/navigation repair. The Toronto market payload was not changed.

- File: `public/data/toronto-market.json`
- Size: `34,185,287` bytes
- Git blob: `50d6a69eea62550bad0066ae879bb799b06fd0c9`
- SHA-256: `ca27946af79c6624a7dd0fa893f0877b267352671d3468c7aad29fb8e1030a03`

The UI-hotfix workflow verifies the committed payload before the frontend build and verifies `dist/data/toronto-market.json` again after the Vite build. Both checks passed before the Pages artifact was uploaded.

### Pages artifact

- GitHub Pages artifact ID: `9938992899`
- Artifact digest: `sha256:70f9d4d4a60f61a4ac351a868c65a806bd7dd398d61642088377e99cdfc9ab9f`
- Live URL: `https://jeremyhennessy.github.io/TowerSignal-Toronto-Preview/`
- Canonical route: `https://jeremyhennessy.github.io/TowerSignal-Toronto-Preview/#/toronto`

### Navigation and runtime changes included

The isolated Toronto preview now exposes only controls that are valid for the isolated Toronto artifact. Unavailable NYC/NYS application routes are not exposed in the Toronto header. Bare-root and legacy non-Toronto hashes are guarded back to `#/toronto` before the application can request unavailable datasets.

The verified source also suppresses shared workflow/auth initialization when `VITE_TORONTO_PREVIEW=true`. This prevents the isolated Toronto preview from making an unnecessary Neon session request while leaving normal NYC/NYS workflow/auth behavior unchanged.

A Toronto-only mobile sizing fix prevents filter controls from forcing horizontal page overflow on a 390-pixel viewport.

The standalone New York link is retained. It points to `https://jeremyhennessy.github.io/TowerSignal/` and was verified in an ordinary Chromium browser context.

### Corrected live browser acceptance evidence

- Workflow: `Toronto Preview Live UI Audit`
- Workflow run: `33880360312`
- Job: `101047239666`
- Conclusion: `success`
- Audit artifact ID: `9939634626`
- Audit artifact digest: `sha256:04c632b7afc110284ef31e14424102b1eebe3e0c6982c744921a894b10a19ec5`

The corrected public audit passed all of the following against the live URLs:

- Toronto desktop at 1440×1000.
- Toronto iPhone-sized viewport at 390×844 with `scrollWidth == viewportWidth`.
- Bare preview root redirect to `#/toronto`.
- Legacy `#/prospect` redirect to `#/toronto`.
- Toronto internal Map view renders.
- A Toronto property detail drawer opens.
- No unavailable Home, Prospect, Monitor, header Map, NYS Market, NYS Changes, Opportunities, Companies, Portfolios, Workflow, market-selector, NYC search, source-health or account controls are exposed in the Toronto header.
- No HTTP 4xx/5xx responses or failed requests were observed in the verified Toronto flows.
- The New York destination returned HTTP 200, rendered TowerSignal, did not display `Failed to fetch`, and produced no failed requests in the corrected browser audit.

### QA-harness false positive resolved

An earlier New York screenshot showed `Failed to fetch`. Investigation proved that was caused by the audit harness, not by the New York application: Playwright had been configured with a global `Cache-Control: no-cache` extra HTTP header, which was also injected into the cross-origin Neon session request. Neon correctly rejected that non-allowed preflight header.

The browser diagnostic was rerun without the injected header. Run `33880082252` confirmed the production New York sign-in page did not show `Failed to fetch`, the app session request returned HTTP 200, and direct in-page Neon auth fetches returned HTTP 200. The temporary candidate that would have hidden the New York link was therefore discarded and never deployed.

### Deployment ordering / stale-run protection

A stale strict preview deployment on the prior UI source was cancelled before it could supersede the verified UI fix. The strict `Deploy Toronto Preview` workflow is now pinned to source commit `2eea1e2d5cbf0d9cf24d2325eb3a4222806ba6ea` and uses `cancel-in-progress: true` for its preview deployment concurrency group so a superseded deployment cannot later overwrite a newer verified preview.

At the time this checkpoint was recorded, strict workflow run `33878713743` was still executing its deep Toronto source-semantic validation. It uses the same corrected source commit; this file does not claim that run is complete until GitHub reports a final conclusion.

## Prior verified release — September 3, 2026

- Source commit: `a535195e32eb2be7397eafd709ec0eba013e6890`
- Preserved source branch: `release/toronto-20260903-a535195`
- Wrapper commit: `a2c196a06fb269f01c487e9ea14e8d8abd57a0c7`
- Workflow run: `33775765172`
- GitHub Pages artifact ID: `9903471373`
- Artifact digest: `sha256:06e7da940eb3ddd8891e49ffd24511e0ea87a4bed1c7e30cbf360ead04d95d0a`
- Deployment conclusion: `success`

That release passed the Toronto identity and ChemTRAC regressions, normalized-payload rebuild, strict source-action validation, strict source-semantic audit, public-notice cardinality proof, strict source-row resolution, final market/evidence-contract validation, frontend lint/typecheck/tests, isolated Pages build, and Pages deployment.

## Known Toronto data limitations retained

- No defensible public denominator for the total installed Toronto cooling-tower population has been established; true market coverage remains unknown.
- Application Information Centre supporting-document transport is blocked by browser-generated reCAPTCHA, so the application does not claim a completed AIC supporting-document corpus.
- Construction Act publication sources currently require permission/reuse authorization for the desired ingestion path.
- The remaining unresolved municipal property identities remain explicitly unresolved rather than force-matched.
- Aerial screening remains weak-label visual similarity only and does not upgrade tower confirmation.
