# Source provenance

Import date: September 30, 2026.

The initial public documentation, assets, executable examples and validation tools were copied from the consolidated Koinos documentation working branch `codex/update-four-chapters-docs`, at full commit `9178aa7f38cd94b7aaf8309ab58bcb8bc5dec362`. That working project uses https://github.com/koinos/koinos-docs.git as its upstream remote; the recorded working commit is not asserted to be merged or publicly available upstream.

This repository starts with a fresh Git history. The local source history, unreviewed drafts and internal planning reports were not published. The original MIT license and Koinos Group copyright are retained in [LICENSE.md](LICENSE.md). New maintenance documentation and repository configuration were added for this community edition.

The upstream [koinos-docs README](https://github.com/koinos/koinos-docs) marks that repository deprecated and redirects contributors to `koinos/koinos/docs`. The target path returned HTTP 404 when checked on September 30, 2026. This independently maintained repository does not claim to replace an official publication channel.

## Technical baselines

The imported service pages cite full source commits and `koinos-proto` v2.6.0. Their integration topology references `koinos/koinos` commit `821674672e699bf56e94d7c0e8bce122e83d1482`. The coordinator's September 30 inventory uses a different integration revision, `b05b8337d0a8d09748f9c2d1faef810ee2f5de28`; compare configurations before reconciling these baselines.

[maintenance/source-baselines.json](maintenance/source-baselines.json) records each imported service reference and its cited source revision. Review dates initially remain unset because creation of this repository did not perform a new behavioral audit. Importing a document, building its site and validating links do not establish that its procedures were executed or that a node is ready to produce.
