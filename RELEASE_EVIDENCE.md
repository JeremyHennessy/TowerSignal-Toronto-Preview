# Toronto Preview Release Evidence

This file records the verified Toronto preview deployment completed on September 3, 2026. It documents the deployed application state; later documentation-only commits in this wrapper repository do not change the deployed Pages artifact because the deployment workflow is path-scoped to `.github/workflows/deploy-pages.yml`.

## Deployed source

- Source repository: `JeremyHennessy/TowerSignal`
- Exact source commit: `a535195e32eb2be7397eafd709ec0eba013e6890`
- Preserved source release branch: `release/toronto-20260903-a535195`
- Wrapper repository: `JeremyHennessy/TowerSignal-Toronto-Preview`
- Wrapper commit used for the Pages build: `a2c196a06fb269f01c487e9ea14e8d8abd57a0c7`
- Workflow: `Deploy Toronto Preview`
- Workflow run: `33775765172`

## Verification and deployment

The workflow completed successfully. Its build job passed the Toronto identity and ChemTRAC regressions, normalized-payload rebuild, strict source-action validation, strict source-semantic audit, public-notice cardinality proof, strict source-row resolution, final market/evidence-contract validation, frontend lint/typecheck/tests, and isolated Pages build before upload.

The deployment job then published the generated Pages artifact successfully.

- GitHub Pages artifact ID: `9903471373`
- Artifact digest: `sha256:06e7da940eb3ddd8891e49ffd24511e0ea87a4bed1c7e30cbf360ead04d95d0a`
- Pages build version: `a2c196a06fb269f01c487e9ea14e8d8abd57a0c7`
- Deployment reported successful: `2026-09-03T16:48:42Z`
- Live URL: `https://jeremyhennessy.github.io/TowerSignal-Toronto-Preview/`
- Prospect route: `https://jeremyhennessy.github.io/TowerSignal-Toronto-Preview/#/prospect`

The transient GitHub Actions artifact is not the release identity. The immutable source commit, wrapper build commit, workflow run, and recorded artifact digest above are the durable evidence for the deployed release.

## Known limitations retained in the release

- No defensible public denominator for the total installed Toronto cooling-tower population has been established; true market coverage remains unknown.
- Application Information Centre supporting-document transport is blocked by browser-generated reCAPTCHA, so the application does not claim a completed AIC supporting-document corpus.
- Construction Act publication sources currently require permission/reuse authorization for the desired ingestion path.
- The remaining unresolved municipal property identities remain explicitly unresolved rather than force-matched.
- Aerial screening remains weak-label visual similarity only and does not upgrade tower confirmation.
