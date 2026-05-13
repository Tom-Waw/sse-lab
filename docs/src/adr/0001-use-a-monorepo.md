# ADR 0001: Use a Monorepo

## Status

Accepted

## Context

`sse-lab` is intended to become a production-inspired software systems engineering lab. The project may eventually include backend services, frontend applications, Rust components, infrastructure code, load tests, observability configuration, and documentation.

These parts are closely related and should evolve together. The repository should make system boundaries, integration points, and architectural trade-offs visible in one place.

## Decision

Use a monorepo for the project.

The repository will keep related services, applications, infrastructure, documentation, experiments, and supporting tooling in a single version-controlled workspace.

## Consequences

This makes it easier to keep documentation, implementation, tests, and infrastructure changes aligned.

It also makes architectural evolution easier to follow through the commit history.

The trade-off is that repository structure, tooling, and CI configuration need to stay disciplined as the project grows. Without clear boundaries, a monorepo can become difficult to navigate.

## Notes

The monorepo structure should remain lean at the beginning and evolve only when the project has a real need for additional directories, packages, or services.
