# Requirements Engineering

## Purpose

This document defines how requirements will be discovered, generalized, evaluated, and translated into project work.

It describes the process, not the actual requirements.

The goal is to keep requirements useful, scoped, and connected to engineering decisions without creating heavyweight project paperwork.

## Principles

Requirements engineering in `sse-lab` follows these principles:

- Capture generalized problems and workflows, not confidential real-world details.
- Describe stakeholder needs before implementation ideas.
- Keep requirements aligned with the project vision and scope.
- Prefer small, testable, reviewable requirements.
- Distinguish domain requirements from architecture experiments.
- Accept complexity only when it supports measurable engineering value.
- Use requirements to guide issues, tests, ADRs, and experiment plans.

## Input Sources

Requirements may be informed by:

- stakeholder analysis;
- generalized conversations with a hospitality practitioner;
- project vision and scope;
- ADRs;
- public domain knowledge about hospitality operations;
- implementation feedback;
- experiment results.

Requirements must not be based on:

- confidential hotel, guest, employee, employer, vendor, or proprietary system information;
- screenshots or direct descriptions of a specific commercial hotel system;
- real guest or employee data;
- reverse-engineered vendor behavior.

## Interview Findings

Interview transcripts are private and are not stored in the repository.

Each interview artifact may contain generalized findings after the conversation has been processed. These findings are source-near notes, not committed requirements.

Cross-interview synthesis, requirement candidates, roadmap items, and architecture decisions are derived only after findings from multiple perspectives have been compared.

## Requirements Workflow

Requirements should follow a lightweight workflow:

1. Gather input from approved sources.
2. Extract generalized findings.
3. Link findings to stakeholder concerns or project goals.
4. Convert relevant findings into requirement candidates.
5. Check candidates against scope and non-goals.
6. Classify and prioritize accepted candidates.
7. Translate accepted requirements into issues, tests, documentation tasks, ADRs, or experiment plans.
8. Validate requirements through implementation, review, tests, or measurements.

This workflow should remain practical. It exists to support disciplined engineering, not to create process overhead.

## Requirement Categories

Requirements may be classified as:

| Category      | Meaning                                                                                      |
| ------------- | -------------------------------------------------------------------------------------------- |
| Functional    | Domain behavior the system should support                                                    |
| Quality       | Performance, reliability, usability, maintainability, observability, or security expectation |
| Constraint    | Technical, ethical, scope, or project limitation                                             |
| Architecture  | Requirement that affects system structure or design decisions                                |
| Experiment    | Requirement used to compare naive and improved approaches                                    |
| Documentation | Required explanation, ADR, report, runbook, or project artifact                              |

## Prioritization

Requirements should be prioritized using simple categories:

| Priority     | Meaning                                          |
| ------------ | ------------------------------------------------ |
| Baseline     | Needed for the first useful system version       |
| Experiment   | Enables measurable architecture comparison       |
| Later        | Useful, but not needed for the current milestone |
| Out of scope | Not aligned with current project boundaries      |

Prioritization should consider:

- alignment with project vision and scope;
- stakeholder relevance;
- feasibility for one engineer;
- testability or measurability;
- portfolio value;
- risk of scope creep;
- dependency on external systems or confidential information.
