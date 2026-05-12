# Software Systems Engineering Lab

Designing, testing, measuring, and evolving production-inspired software systems.

## Purpose

`sse-lab` is a personal software systems engineering monorepo. It acts as both a portfolio project and a learning lab for backend engineering, software architecture, infrastructure, performance engineering, observability, and software project management.

The project is not intended to be a toy application or a clone of an existing product. Its purpose is to demonstrate how a realistic system can be analyzed, designed, implemented, measured, operated, and improved over time.

The project intentionally uses a domain outside my professional document-analysis background to show that the same engineering discipline can be applied to a new real-world problem space.

## Initial Domain: Hospitality Operations

`sse-lab` uses hospitality operations as its initial system domain.

The project models selected hotel operations workflows, such as room inventory, booking and availability, room lifecycle management, housekeeping workflows, staff assignment, and operational dashboards.

The goal is not to build a complete commercial hotel management system. The hospitality domain was selected because it combines understandable real-world workflows with meaningful engineering challenges: booking consistency, lifecycle state management, workflow automation, caching, asynchronous processing, scheduling, and operational visibility.

The domain is grounded in real operational pain points from hospitality work, while still being modeled as a generalized and independent system. Informal conversations with a hospitality practitioner help validate assumptions and keep the requirements realistic without using confidential hotel, guest, employee, employer-specific, or proprietary system information.

## Engineering Philosophy

`sse-lab` is built around architectural evolution.

The project should start with simple, understandable implementations and then improve them deliberately based on evidence.

The core engineering loop is:

1. Build a simple implementation.
2. Identify design limitations.
3. Stress it with tests, fault scenarios, or load.
4. Capture measurements.
5. Improve the design deliberately.
6. Re-run the same tests.
7. Compare results.
8. Document the trade-offs.

## Software Project Management

`sse-lab` also demonstrates practical software project management.

Before implementation grows, the project should document its domain assumptions, stakeholders, requirements approach, scope boundaries, risks, roadmap, and architectural decisions. These artifacts should remain lightweight and useful. They should guide engineering work rather than exist as academic paperwork.

## Documentation

The published documentation site is available through [GitHub Pages](https://tom-waw.github.io/sse-lab/).

## Repository Status

This repository is in its initial planning and documentation phase.

The current focus is to define the system domain, project scope, requirements approach, and architecture baseline before implementation begins.
