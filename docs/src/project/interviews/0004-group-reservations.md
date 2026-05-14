# Interview Guide 0004: Group Reservations

## Purpose

This interview explores group reservation workflows.

The goal is to understand how group bookings, room blocks, reservation changes, and email-driven coordination can affect booking and availability assumptions.

Group reservations are important for early domain discovery, even if implementation remains later scope.

This interview should help identify generalized workflow problems that may later inform booking models, availability calculations, reservation holds, batch changes, and coordination boundaries.

## Focus Areas

- Group bookings
- Room blocks and allotments
- Email-driven reservation requests
- Booking changes and cancellations
- Coordination with front office
- Availability impact
- Scope boundaries

## Questions

### Workflow

- What kinds of requests usually reach group reservations?
- How does a group reservation differ from an individual booking?
- Which steps happen before a group reservation is confirmed?
- Which roles or departments need to be involved?

### Availability and Room Blocks

- How do group reservations affect room availability?
- What does it mean to hold or block rooms for a group?
- What can go wrong if blocked rooms are not updated correctly?
- How are changes to group size handled conceptually?

### Email and Communication

- What role do emails play in group reservation work?
- What information is usually needed before a request can be processed?
- What causes back-and-forth communication or delays?
- Which information needs to be visible to other departments?

### Changes and Exceptions

- How do cancellations, partial cancellations, or date changes affect operations?
- What happens when a group request conflicts with existing availability?
- What kinds of mistakes are most disruptive in group reservation workflows?
- Which issues are discovered late and create operational pressure?

### Coordination

- How does group reservations coordinate with front office?
- Which information does front office need before group arrival?
- Which information does management need?
- Are there handoffs to housekeeping, food and beverage, or other departments?

### Scope Boundaries

- Which parts of group reservation work are essential to understand availability?
- Which parts are too broad for the initial system?
- Which parts are mostly communication or sales workflow rather than core hotel operations?

## Follow-up Prompts

- Is this frequent, severe, or both?
- Is this specific to one workplace or a general hospitality pattern?
- Which state needs to be visible to other roles?
- Does this affect actual availability or only planning?
- Can this be generalized without describing a specific customer, company, hotel, or system?

## Expected Insights

This interview may produce generalized findings about:

- group booking workflows;
- room blocks and holds;
- availability impact;
- batch booking changes;
- email-driven coordination;
- handoffs to front office and management;
- future scope boundaries.
