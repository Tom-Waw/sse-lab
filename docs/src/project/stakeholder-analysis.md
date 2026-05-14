# Stakeholder Analysis

## Purpose

This document identifies the relevant stakeholder groups and explains how their concerns influence requirements, scope, quality attributes, and architecture decisions.

The goal is not to model a real hotel organization completely. The goal is to use stakeholder perspectives to derive realistic engineering priorities for a hospitality operations system.

This analysis should help keep the project focused on meaningful workflows, measurable architecture decisions, and practical software project management.

## Analysis Scope

The stakeholder analysis includes two kinds of stakeholders:

1. **Domain stakeholders** who would exist in a real hospitality operations environment.
2. **Project stakeholders** who matter because the repository is also a public engineering portfolio.

The analysis is intentionally generalized. It must not include confidential hotel, guest, employee, employer-specific, vendor-specific, or proprietary system information.

## Stakeholder Categories

### Primary Domain Stakeholders

Primary domain stakeholders represent the core operational workflows that the system may model early.

| Stakeholder            | Main interest                                                                               |
| ---------------------- | ------------------------------------------------------------------------------------------- |
| Front Office staff     | Fast and correct booking, availability, check-in, check-out, and room status information    |
| Housekeeping staff     | Clear tasks, priorities, room readiness status, and manageable workload                     |
| Night shift staff      | No-show handling, late arrivals, daily reconciliation, and reporting across date boundaries |
| Operations coordinator | Coordination across front office, housekeeping, maintenance, and management                 |
| Hotel management       | Occupancy, staffing, operational bottlenecks, reporting, and service quality                |
| Guests                 | Correct booking, smooth arrival, room readiness, and reliable service                       |

### Secondary or Future Domain Stakeholders

Secondary stakeholders may be relevant for early discovery, but they should not drive the initial implementation.

| Stakeholder               | Main interest                                                                                           |
| ------------------------- | ------------------------------------------------------------------------------------------------------- |
| Group reservations        | Group bookings, room blocks, email-driven requests, booking changes, and coordination with front office |
| Maintenance staff         | Rooms out of service, repair tasks, and impact on availability                                          |
| Staff scheduler           | Shift planning, workload balance, staff availability, and assignment constraints                        |
| Revenue manager           | Occupancy, pricing, forecasting, and overbooking strategy                                               |
| External booking channels | Integration boundaries, inventory synchronization, and booking updates                                  |
| Accounting / finance      | Invoicing, payment reconciliation, taxes, and financial reporting                                       |

### Project Stakeholders

Project stakeholders are concerned about the repository and the code itself.

| Stakeholder                  | Main interest                                                                                         |
| ---------------------------- | ----------------------------------------------------------------------------------------------------- |
| Maintainer / portfolio owner | Feasible scope, learning value, senior-level portfolio signal, maintainability, and project coherence |
| Future contributors          | Clear structure, reproducible setup, contribution guidance, tests, and documentation                  |
| Recruiters / hiring managers | Understandable project purpose, visible engineering maturity, and credible portfolio value            |
| Senior engineer reviewers    | Architecture decisions, trade-offs, correctness, measurements, operational thinking, and code quality |
| Demo users                   | A smooth way to understand, run, inspect, or evaluate the project                                     |

### Operational and Governance Stakeholders

Operational stakeholders represent concerns that would matter when running or reviewing the system.

| Stakeholder              | Main interest                                                                             |
| ------------------------ | ----------------------------------------------------------------------------------------- |
| System operator          | Reliability, deployment, observability, incident diagnosis, and recovery                  |
| Data/privacy stakeholder | Safe data handling, synthetic data, anonymization, and no use of confidential information |
| Security reviewer        | Secure defaults, authentication boundaries, authorization boundaries, and secret handling |

## Influence and Interest

This classification helps decide how much each stakeholder perspective should influence early project work.

| Stakeholder                  |      Interest |     Influence | Engagement approach                                                                   |
| ---------------------------- | ------------: | ------------: | ------------------------------------------------------------------------------------- |
| Maintainer / portfolio owner |          High |          High | Drives project direction, scope, quality bar, and prioritization                      |
| Front Office staff           |          High |        Medium | Core workflow perspective for booking, availability, and room state                   |
| Housekeeping staff           |          High |        Medium | Core workflow perspective for room readiness and task flow                            |
| Hotel management             |          High |        Medium | Provides reporting, staffing, and operational visibility concerns                     |
| Senior engineer reviewers    |          High |        Medium | Require visible architecture reasoning, trade-offs, and measurements                  |
| System operator              |          High |        Medium | Drives observability, deployment, reliability, and runbook concerns                   |
| Operations coordinator       |        Medium |        Medium | Connects cross-team workflow and escalation concerns                                  |
| Night shift staff            |        Medium |        Medium | Introduces reconciliation, scheduled jobs, date boundaries, and reporting concerns    |
| Group reservations           |        Medium |        Medium | Important for understanding group bookings, room blocks, and availability assumptions |
| Recruiters / hiring managers |        Medium |        Medium | Need clear project story, accessible README, and understandable demo value            |
| Future contributors          |        Medium |           Low | Need documentation, local setup, tests, and contribution guidance                     |
| Demo users                   |        Medium |           Low | Need a fast path to understand and inspect the system                                 |
| Guests                       |        Medium |           Low | Represent service expectations, but are not direct system users initially             |
| Data/privacy stakeholder     |        Medium |           Low | Ensures safe, generalized, and synthetic data use                                     |
| Security reviewer            |        Medium |           Low | Ensures secure defaults and clear auth boundaries as they evolve                      |
| Maintenance staff            | Low initially | Low initially | Relevant when out-of-service room workflows are modeled                               |
| Staff scheduler              |  Medium later |  Medium later | Relevant when staff scheduling becomes an active workstream                           |
| Revenue manager              | Low initially | Low initially | Relevant for later pricing or forecasting work                                        |
| External booking channels    | Low initially | Low initially | Relevant for integration design, but out of initial scope                             |
| Accounting / finance         | Low initially | Low initially | Relevant for real products, but payments and invoicing are out of scope               |

## Key Stakeholder Relationships and Tensions

Stakeholder relationships reveal where requirements and architecture trade-offs are likely to appear.

| Relationship                                     | Tension or coordination need                                                                                          | Engineering implication                                                        |
| ------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------ |
| Front Office staff ↔ Guests                      | Guests expect fast check-in and correct booking information; front office needs reliable availability and room status | Booking correctness, fast availability search, clear room state model          |
| Group reservations ↔ Front Office staff          | Group bookings and changes affect availability, room planning, and guest arrival preparation                          | Reservation holds, room blocks, booking state model, availability assumptions  |
| Front Office staff ↔ Housekeeping staff          | Front Office needs rooms ready; housekeeping needs realistic priorities and workload visibility                       | Room lifecycle states, housekeeping task workflow, operational dashboard       |
| Front Office staff ↔ Night shift staff           | Late arrivals, no-shows, and date-boundary operations must be handled consistently                                    | Scheduled jobs, booking state transitions, audit trail, reconciliation reports |
| Housekeeping staff ↔ Operations coordinator      | Tasks may need reprioritization during high occupancy or staff shortages                                              | Task prioritization, reassignment, workflow visibility                         |
| Operations coordinator ↔ Maintenance staff       | Rooms may become unavailable and affect bookings, housekeeping, and room readiness                                    | Out-of-service states, availability impact, operational events                 |
| Hotel management ↔ Operational staff             | Management wants efficiency and visibility; staff need realistic workload and clear instructions                      | Reporting, workload metrics, task status, escalation paths                     |
| Maintainer ↔ Portfolio reviewers                 | The project must be feasible for one engineer but still show senior-level engineering depth                           | Small increments, ADRs, experiment reports, clear scope boundaries             |
| System operator ↔ Developers                     | Operational issues must be diagnosable and recoverable                                                                | Structured logs, metrics, traces, health checks, runbooks                      |
| Data/privacy stakeholder ↔ Requirements analysis | Requirements should be realistic without exposing confidential or personal data                                       | Generalized findings, synthetic data, privacy boundaries                       |
| Architecture goals ↔ Scope control               | Advanced architecture is valuable, but overbuilding weakens focus                                                     | Naive-first implementation, feature flags, measurable improvements             |

## Project Implications

This analysis creates several high-level implications.

- Booking, availability, room state, and housekeeping should be treated as core early domain areas.
- Group reservations should be explored early because it affects booking and availability assumptions, but implementation should remain later scope.
- Staff scheduling, maintenance, revenue management, accounting, and external integrations should remain secondary or future concerns.
- The project should explicitly balance domain realism with portfolio feasibility.
- Documentation should make stakeholder-driven decisions visible without pretending to be a commercial rollout.
- Architecture work should focus on workflows, correctness, observability, and measurable evolution rather than broad feature coverage.
- All real-world input must be generalized and must avoid confidential or employer-specific information.

## Out-of-Scope Stakeholders for the Initial Phase

Some stakeholders are relevant to real hotel systems but should not influence the initial implementation.

| Stakeholder                   | Reason for exclusion from initial scope                    |
| ----------------------------- | ---------------------------------------------------------- |
| Payment providers             | Real payment processing is out of scope                    |
| Tax authorities               | Tax handling and compliance are out of scope               |
| Accounting departments        | Invoicing and financial reporting are out of scope         |
| Loyalty program managers      | Loyalty features are outside the project focus             |
| Marketing teams               | Campaigns and guest engagement are out of scope            |
| Third-party booking platforms | External integrations are out of scope initially           |
| Hardware vendors              | Hardware integration is out of scope                       |
| Real hotel IT departments     | The system is not intended for production hotel deployment |

These stakeholders may be referenced in future architecture discussions only when they help clarify boundaries or integration trade-offs.

## Maintenance Notes

This document should evolve as requirements analysis progresses.

Updates should be made when:

- new stakeholder perspectives are discovered;
- scope changes affect stakeholder priorities;
- requirements interviews reveal new generalized findings;
- architecture decisions change stakeholder impact;
- the project adds new workflow areas.
