# Service reference template

Use this template to expand a service page. Write verified facts in the public page; track missing investigations in an issue or local draft rather than filling gaps with assumptions. Retain introductory explanations so readers can progress into implementation details.

## Purpose and boundaries

Explain responsibilities, authoritative decisions, derived data and exclusions.

## Dependencies and startup behavior

Document internal dependencies, RPC inputs, required schemas, initialization, catch-up, readiness and shutdown behavior. Distinguish Compose startup order from application readiness. Link to operator setup procedures.

## RPC interfaces

For each relevant method, record the request and response schemas, caller, side effects, error behavior and source definitions. Cite the exact service and protocol commits. Distinguish internal RPC from externally exposed APIs.

## Events and messaging

List consumed and emitted events, exchanges, routing keys, payloads and handling behavior. Document ordering, delivery, retries or idempotency only when established by source or tests.

## Persistent state and consistency

Describe the storage engine, data ownership, schema, forks, irreversible state, rebuildability and recovery constraints. Link operational backups and restore procedures to Node Operators.

## Failure behavior

Explain dependency outages, timeouts, reconnection, stalls, partial progress and observable symptoms. Distinguish a running process from useful service availability.

## Resource use and security boundaries

Record permissions and trust boundaries. Include resource or performance figures only with a reproducible measurement, environment and version. Keep credentials, producer keys and machine-specific data out of examples.

## Verification and limitations

State what source was inspected, what tests were actually run, their dates and results, and what remains unverified. Distinguish fixtures, isolated runtime checks and production evidence.

## Versioned sources

Link the service commit, matching protobuf revision, integration configuration, tests and relevant issue or PR. Update the central baseline record after a substantive review.
