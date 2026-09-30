# Initial import adjustments

Date: September 30, 2026. Source snapshot: see `SOURCE_PROVENANCE.md`.

The imported MkDocs configuration and example manifest point to the upstream repository and `master`/`dev` branches. Those links must target this repository's `main` branch so readers can access the files actually published here. Update the example validator to read a repository URL from the manifest, preserving the inherited source and runner correspondence checks. The manifest's historical audit date is retained as provenance, not presented as a new audit.

The imported link checker skips two historical exceptions, and the navigation references a missing JSON-RPC page. Resolve the missing homepage link, remove the absent navigation destination and remove the checker exceptions. No node software or example transaction behavior is changed. Verify the updated manifest and URLs, JavaScript syntax and existing example tests, local documentation links and a strict MkDocs build.

Inherited trailing whitespace and empty EOF lines were normalized; explicit Markdown hard breaks were retained using backslashes.

Four malformed inherited SDK page titles were corrected for readable navigation.
