# Contributing

All documentation is maintained in English. Open an issue for missing coverage, an unclear claim or a proposed baseline update. Include the affected service, page and target version.

## Propose a change

1. Create a branch from `main`.
2. Read the affected service source at an exact tag or full commit and check its dependencies and protocol definitions.
3. Update the relevant page using the [service reference template](maintenance/templates/service-reference.md). Keep operations in Node Operators and link to them from architecture pages.
4. Cite immutable source URLs close to the claims they support. Record changes to the baseline, actual review date, review scope and unresolved questions in [source-baselines.json](maintenance/source-baselines.json).
5. Run the checks below and describe the evidence in a pull request. A documentation build establishes rendering and structure, not node or consensus behavior.

## Validation

With Python dependencies installed and Node.js 22 available:

```bash
npm ci --ignore-scripts
npm run docs:links
npm run examples:verify
npm run examples:syntax
mkdocs build --strict
```

For changes to executable examples, also run the relevant example tests. For changes to node procedures, review the target integration configuration and use isolated test data where execution is necessary. Never infer production readiness from a local build or a source-only review.

Inspect changed pages in the local MkDocs preview. Check tables, diagrams, code blocks, navigation and narrow layouts. CI stores the built site as an artifact for review.

## Public content and drafts

`docs/` contains published documentation. The ignored local `drafts/` directory is working material; it is not part of the public repository or website. Adapt and verify useful historical concepts before publication. Do not copy private Knodel content or local machine information.

Consensus-sensitive descriptions require careful source review and, where source does not establish intended behavior, review by the relevant maintainers. Explicitly describe what remains unverified.

## License

Contributions are licensed under the repository's [MIT license](LICENSE.md). Preserve inherited attribution and identify the origin and license of any new external material.
