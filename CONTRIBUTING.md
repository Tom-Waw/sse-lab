# Contributing

`sse-lab` is developed as a long-lived software systems engineering lab. Contributions should be small, reviewable, intentional, and aligned with the project’s purpose as a portfolio-quality engineering system.

The repository should demonstrate disciplined software engineering, not only feature delivery.

## Development Principles

- Prefer simple, understandable solutions before introducing complexity.
- Avoid premature abstraction and premature service extraction.
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
- Keep the scope small enough to review confidently.

## Documentation

Documentation is part of the product.

Use documentation to explain:

- Project purpose, scope and requirements
- System boundaries
- Architectural decisions
- Operational assumptions
- Experiment design
- Performance measurements
- Trade-offs and limitations

Documentation should be useful to future contributors, reviewers, and interviewers. Avoid documentation that does not help explain or improve the system.

## Security

- Keep secrets out of version control.
- Use `.env.example` for documented configuration.
- Prefer secure defaults.
- Document authentication and authorization boundaries as they evolve.
