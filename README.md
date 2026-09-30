# Koinos documentation — community edition

[Public repository](https://github.com/pgarciagon/koinos-docs)

This repository is the maintained home for English Koinos architecture, microservice references and node operator documentation. It starts with the consolidated documentation snapshot recorded in [SOURCE_PROVENANCE.md](SOURCE_PROVENANCE.md) and preserves its MIT license. It is independently maintained and does not represent an official Koinos release or endorsement.

## Read the documentation

- [Architecture overview](docs/architecture/index.md)
- [Microservices overview](docs/architecture/microservices.md)
- [Internal messaging](docs/architecture/interprocess-communication.md)
- [Node operators](docs/nodes/index.md)
- [Maintenance and review status](docs/maintenance.md)

The initial reference set covers Chain, Block Store, P2P, Mempool, Transaction Store, Block Producer, JSON-RPC, gRPC, REST, Contract Meta Store and Account History. RabbitMQ and the shared messaging contracts are covered in the internal messaging chapter. The inherited developer, contract and ecosystem chapters are retained for context and cross-references.

## Preview and build

Use Python 3.12 and Node.js 22 for the same environment as CI:

```bash
python3 -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
npm ci --ignore-scripts
npm run docs:links
npm run examples:verify
npm run examples:syntax
mkdocs build --strict
mkdocs serve
```

The preview is available at `http://127.0.0.1:8000/`. The generated static site is written to `site/`, which is ignored by Git. Repository publication does not imply deployment of a hosted website.

## Improve the references

Follow [CONTRIBUTING.md](CONTRIBUTING.md), the [service reference template](maintenance/templates/service-reference.md) and the [source baseline record](maintenance/source-baselines.json). Use issues for missing coverage and pull requests for reviewed changes. Record the exact source revision, verification date, evidence and remaining uncertainty whenever a technical claim changes.

Unreviewed source drafts remain local under ignored `drafts/`; they are excluded from both Git and the site. Private project material must not be copied into this repository. Architectural behavior belongs in service references; operational commands, configuration, ports, backup and recovery belong in Node Operators.

The [producer-node coordinator](https://github.com/pgarciagon/koinos_legacy_node) maintains software inventories, improvement proposals, implementation references and deployment evidence separately.

## License

See [LICENSE.md](LICENSE.md) and [SOURCE_PROVENANCE.md](SOURCE_PROVENANCE.md) for inherited copyright and attribution.
