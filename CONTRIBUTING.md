# Contributing

`sse-lab` is developed as a long-lived project. Contributions should be small, reviewable, and intentional.

## Development Principles

- Prefer simple, understandable solutions before introducing complexity.
- Keep changes focused and easy to review.
- Document architectural decisions when they matter.
- Add or update tests for meaningful behavior changes.
- Keep local setup reproducible.
- Do not commit secrets, credentials, or environment-specific configuration.
- Make trade-offs explicit when changing architecture or infrastructure.

## Commit Style

Use Conventional Commits.

Examples:

```text
docs(readme): add initial project vision
chore(repo): add editor configuration
chore(config): add environment example
feat(api): add health check endpoint
test(api): add health check integration test
ci(github): add validation workflow
docs(adr): document monorepo decision
```

## Pull Request Expectations

Before merging, changes should ideally:

- Build successfully.
- Pass formatting and linting checks.
- Pass relevant tests.
- Include documentation updates where appropriate.
- Explain trade-offs for architectural or infrastructure changes.

## Documentation

Documentation is part of the product.

Use documentation to explain:

- System boundaries
- Architectural decisions
- Operational assumptions
- Experiment design
- Performance measurements
- Trade-offs and limitations

## Security

- Keep secrets out of version control.
- Use `.env.example` for documented configuration.
- Prefer secure defaults.
- Document authentication and authorization boundaries as they evolve.
