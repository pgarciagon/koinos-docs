# Project context

Read `README.md`, `CONTRIBUTING.md` and `SOURCE_PROVENANCE.md` before making changes.

This repository maintains English Koinos documentation as an independent community edition. It is linked from the producer-node coordinator at https://github.com/pgarciagon/koinos_legacy_node.

## Documentation rules

- Write all documentation and local project notes in English.
- Preserve upstream licenses, attribution and immutable source references.
- Keep architectural service behavior in `docs/architecture/` and operational procedures in `docs/nodes/`.
- Expand technical references using `maintenance/templates/service-reference.md`.
- Before changing a technical claim, identify the relevant source repository, tag or full commit and compatible protocol baseline. Refresh volatile facts.
- Update `maintenance/source-baselines.json` when reviewing or changing a service baseline. Set a review date only when the review was actually performed; describe its scope and remaining gaps.
- Distinguish source inspection, documentation builds, runtime tests and actual deployments. Inherited documents and successful builds do not establish producer readiness.
- Keep unreviewed material under ignored `drafts/`. Review claims and adapt the content before promoting it to public pages.
- Do not publish private project content, local machine paths, credentials, keys or personal operational data.
- Check links and run `mkdocs build --strict` for documentation changes. Run the example validation appropriate to any changed examples.
- Repository maintenance does not authorize transactions, node configuration changes, producer activation or deployments.

## Continuation point

The initial content is an imported snapshot, not a new technical audit. The detailed reference template defines the intended expansion of the 11 service pages. Track missing coverage with issues and submit reviewable changes through pull requests. Build checks and inherited example checks run in GitHub Actions; no website deployment is configured.
