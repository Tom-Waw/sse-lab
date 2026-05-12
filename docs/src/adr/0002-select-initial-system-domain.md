# ADR 0002: Select Hospitality Operations as Initial System Domain

## Status

Accepted

## Context

`sse-lab` is a software systems engineering lab and portfolio project. Its purpose is to demonstrate architectural reasoning, backend engineering, performance measurement, observability, infrastructure automation, software project management, and deliberate system evolution.

The project needs an initial domain that is realistic enough to create meaningful engineering problems, but small enough to be implemented incrementally by one engineer.

The domain should also complement existing professional experience rather than duplicate it.

## Decision

`sse-lab` will use **hospitality operations** as its initial system domain.

The system will model selected hotel operations workflows, such as:

- room inventory;
- booking and availability;
- room lifecycle management;
- housekeeping workflows;
- staff assignment and scheduling;
- operational dashboards.

The goal is not to build a complete commercial hotel management product. The domain is used as a realistic vehicle for exploring production-inspired backend architecture, infrastructure decisions, software project management, and measurable system evolution.

## Alternatives Considered

### Document Analysis Platform

A document analysis platform would provide strong opportunities for ingestion pipelines, asynchronous processing, search, OCR, NLP, caching, and observability.

This option was rejected because it overlaps too closely with existing professional experience. The project should expand the demonstrated skill set instead of recreating a familiar domain, and it should avoid unnecessary concerns around confidentiality or reuse of professional knowledge.

### Media Infrastructure Platform

A media infrastructure platform could demonstrate upload handling, object storage, asynchronous processing, feed generation, caching, and backpressure.

This option was rejected because its core architecture is structurally similar to document-processing pipelines: upload, process, transform, store, and serve. It is also a common portfolio domain and would be less differentiated.

### Logistics Dispatch Platform

A logistics dispatch platform would provide strong opportunities for event-driven architecture, assignment algorithms, optimization, simulation, and operational dashboards.

This option remains a strong future inspiration, especially for scheduling and assignment problems. It was not selected as the initial domain because hospitality operations provides a more personal and immediately understandable real-world context.

### Feature Flag and Experimentation Platform

A feature flag and experimentation platform would demonstrate low-latency rule evaluation, caching, event ingestion, rollout safety, and analytics.

This option was not selected as the primary domain. Feature flags will instead be used as a cross-cutting mechanism to compare naive and improved implementations inside `sse-lab`.

## Rationale

Hospitality operations provides a strong balance between product realism and architecture depth.

A hotel operations system appears simple at first, but introduces non-trivial engineering problems, including:

- preventing double bookings under concurrent requests;
- modeling booking, room, and housekeeping state transitions;
- balancing strong consistency for bookings with eventual consistency for operational dashboards;
- moving selected workflows from synchronous processing to asynchronous workers;
- improving availability search, staff assignment, and operational visibility over time.

The domain is understandable to recruiters and reviewers, while still giving senior engineers enough depth to evaluate architectural decisions.

It also supports practical software project management activities such as stakeholder analysis, requirements engineering, scope definition, risk analysis, and roadmap planning without requiring confidential industry data.

Hospitality operations was also selected because it provides a personally motivated and realistically grounded domain while still allowing requirements to be generalized without using confidential industry data.

## Consequences

The project will initially be organized around hospitality operations concepts such as rooms, bookings, room states, housekeeping tasks, staff members, shifts, and operational events.

The system should start with a simple modular architecture. More advanced mechanisms such as queues, caches, read models, worker scaling, optimized scheduling, and Kubernetes deployment should be introduced only after simpler baselines have been implemented and measured.

Future documentation should capture both naive and improved designs, including why each improvement was introduced and which trade-offs it created.

## Trade-offs

Choosing hospitality operations favors product realism, transactional correctness, workflow architecture, and project-management practice over media processing, AI pipelines, or pure infrastructure systems.

The domain may look like a CRUD application if implemented poorly. To avoid this, the project must focus on workflows, invariants, measurements, and architectural evolution rather than basic entity management.

The domain is broad, so the project must remain intentionally scoped and avoid trying to build a complete hotel management suite.

## Non-goals

The initial system will not:

- become a complete commercial hotel management platform;
- implement payments, invoicing, accounting, channel-manager integrations, or real guest communication integrations;
- model every hotel department or hospitality workflow;
- start as a microservice architecture;
- require Kubernetes to run locally;
- implement a full feature flag platform;
- include expensive AI features or external AI dependencies;
- duplicate document analysis or media-processing pipeline work from existing professional experience;
- include real hotel, guest, employee, employer-specific, or confidential operational data.

## Related Follow-up Work

This ADR only selects the initial system domain.

Further details should be documented separately, including:

- project vision and scope;
- stakeholder analysis;
- requirements engineering approach;
- initial domain model;
- architecture baseline;
- roadmap and milestones;
- measurable architecture experiments.
