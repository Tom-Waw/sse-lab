# Interview Guide 0003: Night Shift

## Purpose

This interview explores night shift and night audit workflows.

The goal is to understand how hospitality operations handle late arrivals, no-shows, unresolved room states, date boundaries, reconciliation, and daily reporting.

This interview should help identify generalized workflow problems that may later inform temporal modeling, scheduled jobs, reporting, reconciliation, and auditability requirements.

## Focus Areas

- Late arrivals
- No-shows
- End-of-day operations
- Date-boundary workflows
- Reconciliation
- Reporting
- Operational handover to the next day

## Questions

### Workflow

- What makes night shift different from day shift?
- Which tasks usually happen during the night?
- Which operations need to be completed before the next day starts?
- What information does night shift need from earlier shifts?

### Late Arrivals and No-shows

- How do late arrivals affect operations conceptually?
- How are no-shows handled at a high level?
- What room or booking states become unclear during these cases?
- What problems can carry over into the next day?

### Date Boundaries

- How should we think about the “hotel day” compared with the calendar day?
- Which workflows depend on a day boundary?
- What needs to be reconciled before the next operational day?
- What can go wrong if date-boundary operations are unclear?

### Reporting and Reconciliation

- Which summaries or reports are useful during night operations?
- What needs to be checked or reconciled?
- Which inconsistencies are important to notice early?
- What information should be available for the next shift?

### Handover

- What does the next shift need to know?
- Which unresolved issues should be visible?
- What makes handover difficult or error-prone?

## Follow-up Prompts

- Is this a recurring workflow or a rare exception?
- Which state needs to be correct for the next day?
- What happens if this is missed?
- Which information should be auditable?
- Can this be described without referencing a specific workplace process?

## Expected Insights

This interview may produce generalized findings about:

- temporal modeling;
- no-show handling;
- late check-in workflows;
- scheduled jobs;
- reconciliation;
- operational reports;
- audit trails;
- shift handover.
