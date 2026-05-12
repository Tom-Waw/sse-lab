# Scope

## Purpose

This document defines the initial scope boundaries for `sse-lab`.

The scope is intentionally limited. The project uses hospitality operations as a realistic engineering domain, but it does not attempt to build a complete hotel management product.

Scope decisions should help keep the project focused, reviewable, and useful as a software systems engineering portfolio.

## Initial In-Scope Areas

### Room Inventory

The system may model rooms as operational resources.

Initial room-related concepts may include:

- room identifier;
- room type or category;
- capacity;
- floor or location metadata;
- operational status.

### Booking and Availability

The system may model booking and availability workflows.

Initial booking-related concepts may include:

- availability search;
- booking creation;
- booking cancellation;
- booking status;
- check-in and check-out dates;
- prevention of double booking;
- idempotent booking requests.

### Room Lifecycle

The system may model room state transitions.

Example states may include:

- available;
- reserved;
- occupied;
- dirty;
- cleaning;
- inspection;
- out of service.

The exact state model should be refined during domain analysis.

### Housekeeping Workflow

The system may model operational tasks created from room lifecycle events.

Initial housekeeping-related concepts may include:

- task creation after checkout;
- task priority;
- task assignment;
- task completion;
- task status;
- operational delays.

### Staff Assignment and Scheduling

The system may model simple staff assignment and scheduling.

Initial staff-related concepts may include:

- staff availability;
- shift windows;
- workload;
- floor or area assignment;
- naive and improved assignment strategies.

This area should start simple and evolve only after the core booking and room lifecycle workflows are understood.

### Operational Dashboard

The system may expose operational views for understanding hotel state.

Initial dashboard concepts may include:

- current occupancy;
- rooms by state;
- open housekeeping tasks;
- upcoming check-ins and check-outs;
- operational delays;
- worker or queue health once asynchronous processing exists.

## Engineering In-Scope

The project should support engineering work around:

- modular backend architecture;
- persistence and data modeling;
- state transitions and invariants;
- transactional consistency;
- asynchronous processing;
- feature flags for architecture variants;
- caching and read models;
- background workers;
- load testing and benchmarking;
- structured logging, metrics, and tracing;
- reproducible local development;
- infrastructure automation;
- documentation of architectural trade-offs.

## Initial Out-of-Scope Areas

The initial system will not include:

- real payment processing;
- invoicing or accounting;
- tax handling;
- channel-manager integrations;
- third-party booking platform integrations;
- real guest messaging;
- email or SMS delivery to real users;
- loyalty programs;
- housekeeping mobile apps;
- full HR management;
- payroll;
- legal compliance workflows;
- real hotel, guest, employee, employer-specific, or proprietary system data;
- advanced AI features;
- a complete feature flag platform;
- production deployment for real hotel use.

## Architecture Out-of-Scope for the Initial Phase

The initial phase will not start with:

- microservices;
- distributed transactions;
- Kubernetes-only development;
- complex event streaming infrastructure;
- multi-region deployment;
- advanced search infrastructure;
- external AI services;
- real-time collaboration features.

These topics may be considered later only if they are justified by project goals, measurements, or documented architectural decisions.

## Scope Management Principles

The project should prefer depth over breadth.

A small number of workflows implemented thoughtfully is more valuable than a broad but shallow hotel management clone.

New features should be accepted only if they support at least one of the following goals:

- clarify the hospitality operations domain;
- demonstrate a meaningful architecture decision;
- enable a measurable engineering experiment;
- improve observability, reliability, or operability;
- improve the project’s value as a portfolio-quality engineering system.

## First Scope Boundary

The first implementation milestone should focus on:

- room inventory;
- naive availability search;
- booking creation;
- booking cancellation;
- basic room lifecycle states;
- tests around booking consistency assumptions.

Housekeeping, staff assignment, asynchronous processing, caching, and advanced observability should follow after the baseline has been established.
