# Toronto Preview Release Evidence

This file records the latest verified Toronto preview deployment and preserves prior release checkpoints for traceability.

## Latest verified commercial-parity release — September 4, 2026

### Immutable release source

- Source repository: `JeremyHennessy/TowerSignal`
- Exact source commit: `19b5bfb094b9e15bab6900b409dd5e8c4078384d`
- Preserved source branch: `release/toronto-20260904-ny-parity`
- Main Toronto parity data-finalization run: `33890058632` — `success`
- Combined source CI run: `33893632300` — `success`
- Combined CI passed frontend dependency install, lint, TypeScript, all frontend tests, complete Python regression, and production build.

### Toronto market payload now deployed

The commercial-parity release intentionally expands the Toronto payload while preserving the evidence boundary.

- Canonical Toronto properties: `13,380`
- Documentary-confirmed tower properties: `47`
- Official source families: `16`
- Property/source links: `40,060`
- Source-backed relationship edges: `6,344`
- True Toronto cooling-tower market denominator: `UNKNOWN_DENOMINATOR`

The release includes the recovered building-permit universe and the post-recovery exact-address TOBids relationship at `40 College St`, document `3704322859`, supplier `1246175 Ontario Limited o/a Active Mechanical Services`. That relationship is represented only as `SUCCESSFUL_BIDDER_AT_PROPERTY`; no owner, contractor, tower, compliance or operating-status inference is created from the award row.

Active and cleared building-permit joins remain timing/context evidence only. Permit recovery does not promote tower status or create organization relationships.

### New Toronto product workspaces

The isolated Toronto preview now exposes Toronto-native commercial workspaces beneath the verified Toronto header:

- `Market` — existing canonical property explorer, source-specific filters, Table/Map, source coverage and evidence drawer.
- `Benchmarking` — aggregate Ontario EWRB market context only.
- `Prospects` — source-backed commercial attention ranking with an explicit non-regulatory/non-compliance boundary.
- `Opportunities` — confirmed-tower/mechanical-permit, project timing, planning/development, relationship-gap, multi-source and environmental/health queues.
- `Companies` — source-backed organization aggregation.
- `Portfolios` — multi-property organization groups using explicit allowed relationship roles only.
- `Watchlist` — browser-local saved-property workflow; it does not enable the shared New York workflow/auth backend.
- `Sources` — source-level counts, match rates, limits and official links.

Prospects, Opportunities and Watchlist can export CSV. Companies and Portfolios can export account CSVs. Property rows can copy a lead summary containing the canonical property ID, evidence status, source families, explicit organization relationships and a verification caveat.

Toronto does not expose a fake `Monitor` workspace. New York Monitor is based on real change-history events; Toronto will add that surface only after a validated snapshot-to-snapshot event feed exists.

### Aggregate Ontario EWRB context

The Ontario EWRB warehouse reporting-year normalization was repaired so the resource named `2022` is not incorrectly relabelled by a later publication/update year.

The deployed `public/data/toronto-ewrb-market.json` contract is deliberately `TORONTO_AGGREGATE_ONLY`:

- Published Toronto reporting rows: `11,595`
- Reporting years: `2018` through `2024`
- Property-level EWRB links: `0`
- Tower-evidence effect: `NONE`
- Relationship effect: `NONE`

The public Ontario disclosure does not contain civic street address or assessment roll number. EWRB ID, city and postal FSA are insufficient for deterministic TowerSignal property identity, so the preview uses EWRB only for Toronto-wide annual volume, property-type mix, postal-FSA mix, data-quality-check and Energy Star availability context.

### Verified Pages deployment

- Wrapper commit that introduced the immutable verified-artifact deployment: `7e732e512b0c516b0e1522cf63b444e66a520d98`
- Workflow: `Deploy Verified Toronto Parity Artifact`
- Workflow run: `33894400517`
- Build conclusion: `success`
- Pages deploy conclusion: `success`
- GitHub Pages artifact ID: `9945178428`
- Artifact digest: `sha256:e5a8f34448ca2a5bd48c7cc220f4af738aef54f1475b19f90e678c80042116f5`
- Live URL: `https://jeremyhennessy.github.io/TowerSignal-Toronto-Preview/`
- Canonical route: `https://jeremyhennessy.github.io/TowerSignal-Toronto-Preview/#/toronto`

The verified-artifact deploy proves the committed market counts, TOBids/permit/EWRB regression contracts, Toronto parity frontend tests, lint, TypeScript, exact Vite build, isolated route guard and New York handoff before deployment.

A separate strict reproducibility deployment, run `33893892181`, is pinned to the same exact source commit and regenerates the Toronto market payload before repeating strict source-action, semantic, row-resolution and final-evidence validation. It remains a reproducibility check and cannot introduce an older source version because it is pinned to the same release SHA.

### Live browser acceptance evidence

- Workflow: `Toronto Preview Live Parity Audit`
- Workflow run: `33894057100`
- Conclusion: `success`
- Audit artifact ID: `9945238996`
- Audit artifact digest: `sha256:8549964a67f98aaac0875c1071d8148ceaee7c5915fddf4f294b961800429d41`

The audit waited until the new `Benchmarking` workspace and the exact aggregate EWRB contract were visible on public Pages before recording evidence. It then passed all of the following against the live application:

- Toronto Market desktop at 1440×1000.
- Toronto Market iPhone viewport at 390×844.
- Benchmarking.
- Prospects desktop and iPhone viewport.
- Opportunities.
- Companies.
- Portfolios.
- Watchlist.
- Sources.
- Internal Toronto Map view.
- Property detail drawer.
- Bare-root redirect to `#/toronto`.
- Legacy `#/prospect` redirect to `#/toronto`.
- New York external handoff.
- No HTTP 4xx/5xx responses in audited flows.
- No failed browser requests in audited flows.
- No page-level horizontal overflow; both iPhone captures reported `scrollWidth == viewportWidth == 390`.
- No `Intelligence workspace unavailable`, dataset request failure or `Failed to fetch` state.
- The New York destination returned successfully and did not reproduce the historical QA-harness false positive.

The audit intentionally checks unavailable NY/NYC/NYS controls only inside the Toronto top header. The new Toronto-native workspace buttons are expected and are not treated as forbidden shared-app navigation.

## Prior verified UI/navigation checkpoint — September 4, 2026

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

That release was a UI/navigation repair. The Toronto market payload was not changed.

- File: `public/data/toronto-market.json`
- Size: `34,185,287` bytes
- Git blob: `50d6a69eea62550bad0066ae879bb799b06fd0c9`
- SHA-256: `ca27946af79c6624a7dd0fa893f0877b267352671d3468c7aad29fb8e1030a03`

### Corrected live browser acceptance evidence

- Workflow run: `33880360312`
- Job: `101047239666`
- Conclusion: `success`
- Audit artifact ID: `9939634626`
- Audit artifact digest: `sha256:04c632b7afc110284ef31e14424102b1eebe3e0c6982c744921a894b10a19ec5`

That checkpoint removed unavailable NYC/NYS header routes, guarded bare/legacy hashes to `#/toronto`, disabled the shared workflow/auth initializer in preview mode, fixed 390-pixel filter overflow and verified the standalone New York link.

### QA-harness false positive resolved

An earlier New York screenshot showed `Failed to fetch`. Investigation proved that was caused by the audit harness, not the New York application: Playwright had been configured with a global `Cache-Control: no-cache` extra HTTP header, which was also injected into the cross-origin Neon session request. Neon correctly rejected that non-allowed preflight header.

The browser diagnostic was rerun without the injected header. Run `33880082252` confirmed the production New York sign-in page did not show `Failed to fetch`, the app session request returned HTTP 200, and direct in-page Neon auth fetches returned HTTP 200. The temporary candidate that would have hidden the New York link was discarded and never deployed.

## Prior verified release — September 3, 2026

- Source commit: `a535195e32eb2be7397eafd709ec0eba013e6890`
- Preserved source branch: `release/toronto-20260903-a535195`
- Wrapper commit: `a2c196a06fb269f01c487e9ea14e8d8abd57a0c7`
- Workflow run: `33775765172`
- GitHub Pages artifact ID: `9903471373`
- Artifact digest: `sha256:06e7da940eb3ddd8891e49ffd24511e0ea87a4bed1c7e30cbf360ead04d95d0a`
- Deployment conclusion: `success`

## Known Toronto data limitations retained

- No defensible public denominator for the total installed Toronto cooling-tower population has been established; true market coverage remains unknown.
- Application Information Centre supporting-document transport is blocked by browser-generated reCAPTCHA, so the application does not claim a completed AIC supporting-document corpus.
- Construction Act publication sources currently require permission/reuse authorization for the desired ingestion path.
- The remaining unresolved municipal property identities remain explicitly unresolved rather than force-matched.
- Aerial screening remains weak-label visual similarity only and does not upgrade tower confirmation.
- Ontario public EWRB disclosure is aggregate context only until a lawful independent address-bearing bridge is available.
