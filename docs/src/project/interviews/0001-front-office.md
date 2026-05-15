# Interview 0001: Front Office

## Purpose

This interview explores front office workflows.

The goal is to understand how staff reason about bookings, availability, check-in, check-out, room status, and guest-facing operational pressure.

This interview should help identify generalized workflow problems that may later inform booking, availability, room lifecycle, and operational visibility requirements.

## Focus Areas

- Booking and availability
- Check-in and check-out
- Room status visibility
- Guest-facing coordination
- Late arrivals, cancellations, and no-shows
- Common front office pain points

## Questions

### Workflow

- What does a typical front office shift look like at a high level?
- Which tasks happen most frequently during a shift?
- Which moments are usually most time-sensitive or stressful?
- Which roles does front office need to coordinate with most often?

### Booking and Availability

- How do staff reason about whether a room is available?
- What can make availability unclear or difficult to trust?
- What is the difference between a room being unbooked and a room being ready?
- What kinds of booking or room assignment mistakes are most disruptive?
- How does front office coordinate with group reservations?
- What information from group reservations is important before guest arrival?

### Check-in and Check-out

- What information is needed before a guest can check in smoothly?
- What usually happens when a guest checks out?
- Which room status changes matter around check-in and check-out?
- What can go wrong during arrival or departure workflows?

### Exceptions

- How do late arrivals affect operations?
- How do cancellations or no-shows affect room planning?
- What kinds of last-minute changes create coordination problems?
- How are unclear or conflicting room states usually resolved conceptually?

### Visibility

- What information should front office be able to see quickly?
- Which information is often missing, delayed, or unreliable?
- Which operational problems would be easier to handle with better visibility?

## Follow-up Prompts

- Is this frequent, severe, or both?
- Which roles are involved?
- What information is missing at that moment?
- What happens if this process fails?
- Can this be described without naming a specific system, hotel, guest, or employee?

## Generalized Findings

### Shift Work and Operational Rhythm

#### Front office responsibilities vary strongly by shift

Front office work is not one uniform workflow. Morning, late, and night shifts have different dominant tasks, coordination needs, and operational pressure points.

#### Shift handovers frame front office work

Front office work is structured around receiving information from the previous shift and passing relevant information to the next shift or department. Handover quality directly affects continuity of operations.

#### Morning shift connects checkout, billing, group preparation, and housekeeping coordination

The morning shift is closely tied to departures, billing-related tasks, group preparation, and passing room-preparation information to housekeeping.

#### Late shift is dominated by check-in and guest-facing interruptions

The late shift is primarily shaped by arrivals and check-ins, but staff must also handle interruptions, questions, and unexpected guest requests during the same flow.

#### Night shift combines required on-site presence with day-closing responsibilities

The night shift exists both for operational/legal presence and for the day-closing process. This makes it a distinct workflow that should be explored separately.

---

### Guest-Facing Pressure and Interruptions

#### Longer guest requests quickly create queue pressure

When one guest interaction takes longer than expected, waiting guests accumulate quickly. This creates pressure on staff even when the underlying task is routine.

#### Simple self-service checkout options may still fail without guest attention or guidance

Even when checkout is designed to be simple, guests may not notice or understand the self-service path. This can create unnecessary queues and frustration.

#### Check-in pressure increases when guest, billing, or registration data must be collected manually

Check-in slows down when staff must manually collect or re-enter guest details, billing information, company information, or mandatory registration data during the guest interaction.

#### Cash closing competes with active guest service

Cash closing requires concentration and timing, but front office staff may still need to serve guests at the same time. This creates a conflict between financial accuracy and immediate service.

#### Interruptions during cash closing can force repeated restart work

When cash closing is interrupted by guest service, staff may need to pause, restart, or re-check parts of the process. This increases stress and creates opportunities for mistakes.

---

### Coordination, Handover, and Decision Authority

#### Front office coordinates with housekeeping, reservations, sales, supervisors, and management

Front office work depends on several other roles and departments. Coordination covers room preparation, group bookings, corporate information, exception handling, and escalation.

#### Housekeeping handover carries room-preparation and stay-continuation information

The handover to housekeeping includes information such as special room setup, occupancy preparation, stay extensions, and rooms that should not be cleaned as departures.

#### Reservations handover carries group, payment, and service-inclusion information

Reservations provide important context for group arrivals, payment handling, deposits, billing responsibility, and included services.

#### Corporate contract and billing information must be reliable during guest-facing decisions

Front office staff need reliable information about corporate agreements, billing arrangements, and cost coverage while interacting with guests.

#### Supervisors and department leads support exception, goodwill, and revenue-impacting decisions

Some decisions require escalation because they affect revenue, policy exceptions, or goodwill toward guests. Front office staff rely on supervisors or department leads for these cases.

#### Missing, late, or inconsistent handover information creates operational uncertainty

When important information is missing, delayed, or inconsistent, front office staff must resolve uncertainty during live operations, often while the guest is present.

#### Contradictory staff decisions can undermine front office authority and guest trust

When staff give conflicting answers or override each other informally, guests may lose trust in the original decision and front office authority is weakened.

---

### Availability, Room Status, and Room Readiness

#### Bookable availability and physical room readiness are separate concepts

A room can be available for sale without being physically ready for a guest. Availability, cleanliness, assignment, and readiness are related but distinct concerns.

#### Different system views answer different availability questions

Staff use different system views depending on whether they want to check general availability, availability by category, future availability, or bookable rates.

#### Room status uncertainty usually comes from communication gaps rather than availability calculation

Availability itself may be clear in the system, but uncertainty appears when room status updates or handover information are inconsistent.

#### Cleanliness status determines whether an unbooked room is usable

An unbooked room is not automatically usable. It must also have the correct cleanliness or readiness status before it can be assigned confidently.

#### Out-of-order rooms reduce sellable availability

Rooms marked as out of order are removed from normal availability and are not treated as sellable capacity.

#### Out-of-service rooms may remain counted as available while not being directly assignable

Some rooms may still appear in availability but cannot be assigned directly because they require minor service or follow-up before use.

#### Temporary room markers support operational flexibility

Temporary markers allow staff to identify rooms for special operational purposes, such as specific preparation types, guest requests, or internal coordination.

#### Room preparation differs between single and double occupancy

The same physical room may require different preparation depending on whether it is used for single or double occupancy. This affects housekeeping effort and operational planning.

#### Room status descriptions are needed to explain why rooms are blocked or restricted

When a room is unavailable, restricted, or marked for service, staff need enough explanation to understand whether and how it can be used.

---

### Booking, Assignment, and Pre-Arrival Preparation

#### Multi-room bookings create additional splitting and assignment work

Bookings involving multiple rooms may require extra work to separate reservations, assign names, and handle individual room details.

#### Front office and reservations may use different booking workflows

Different departments may have different workflows or system knowledge for creating and managing bookings, especially group or multi-room bookings.

#### Limited training across booking workflows increases operational friction

When front office staff are expected to handle certain booking cases without the same workflow knowledge as reservations, tasks become slower and more error-prone.

#### Overbooking and late stay extensions can create negative availability

Availability conflicts can occur when the property is overbooked or when existing guests are extended despite limited future capacity.

#### System warnings can be overridden during availability conflicts

The system may warn about missing availability, but staff can still override or continue the action. This creates a gap between system warning and operational prevention.

#### Room assignment depends on stay length, guest needs, occupancy, and room quality

Room assignment is not only about finding any free room. Staff consider stay length, guest preferences, occupancy setup, and perceived room quality.

#### Pre-assigned rooms are neither simply free nor occupied

A room can be physically free but already assigned to a future arrival. This creates an intermediate state that matters for assignment logic.

#### Arrival reports are used to prepare upcoming guest stays

Staff use arrival reports to inspect upcoming arrivals and identify preparation tasks before guests arrive.

#### Notes, traces, alerts, and reports carry operationally relevant arrival information

Important arrival information can be distributed across notes, traces, alerts, and reports. These sources influence preparation and check-in decisions.

#### Special requests must be identified and handled before late arrival

Some guest requests must be prepared before the guest arrives, especially when the responsible department may no longer be available later in the day.

#### Arrival preparation creates downstream tasks for housekeeping

Front office preparation often produces housekeeping tasks, such as special room setup, occupancy setup, or awareness of stay continuations.

#### Multilingual or inconsistent note wording complicates preparation

Special requests and notes may appear in different languages or wording variants, which makes systematic preparation harder.

---

### Group Reservations, Corporate Context, and Payment Responsibility

#### Group bookings require stronger payment, cancellation, and guarantee handling

Group bookings carry higher financial risk than individual bookings, so payment guarantees, deposits, and cancellation conditions become more important.

#### Self-payer status is critical for group check-in

For group arrivals, staff need to know whether guests pay individually or whether costs are covered centrally.

#### Included services must be clear before guest arrival

Staff need to know which services are included in a booking or group arrangement, such as breakfast, parking, or other extras.

#### Corporate billing and cost coverage require reliable reference information

Front office staff need reliable information about which companies or partners have billing arrangements and what those arrangements include.

#### Missing contract or corporate account visibility creates front office risk

If corporate or contract information is not easily available, staff may have to make guest-facing decisions without being able to verify claims.

#### Ambiguous cost coverage creates conflict during check-in or checkout

When it is unclear whether services are covered by a company, group, or guest, front office staff may have to resolve the conflict directly with the guest.

---

### Check-in, Checkout, and State Transitions

#### Booking state and room state are separate state models

Bookings and rooms have separate lifecycles. A booking can change state independently from the physical room status.

#### Booking lifecycle includes arrival, in-house, departure, cancellation, and no-show states

The booking lifecycle includes multiple operational states that determine what actions are available and how the booking is handled.

#### Some booking actions become available only after check-in

Certain actions, such as billing-related operations, may only become available after a booking is checked in.

#### Checkout can be simplified when payment and scheduled departure are handled earlier

If payment is handled at check-in and checkout can be scheduled, departure can require less active front office work.

#### Room cleanliness state may lag behind booking check-in state

A room may remain marked as clean for a period after check-in, especially when online check-in or delayed physical arrival is possible.

#### Online check-in creates ambiguity between assigned and physically occupied rooms

When guests can check in online before physically arriving, the system must distinguish between an assigned room and a room that has actually been entered or used.

#### Guest key access, booking state, and physical occupancy can diverge

A guest may receive access to a room even if the booking state is not updated correctly. This creates risk because system state and real-world occupancy no longer match.

---

### Exceptions, Recovery, and Failure Modes

#### No-show handling is tied to the day-closing process

Bookings that remain in arrival state during day closing may become no-shows. This makes day closing an important boundary in the booking lifecycle.

#### Late arrivals can delay day-closing decisions

If a guest is expected to arrive late, staff may delay the day-closing process to avoid incorrectly marking the booking as a no-show.

#### A guest can physically arrive without being correctly checked in

Operational shortcuts or interruptions can result in a guest receiving access without the booking being moved into the correct checked-in state.

#### Incorrect no-show handling can make an occupied room appear available

If a physically occupied room is marked as no-show, the system may treat it as available even though a guest is already using it.

#### Missed booking confirmations can leave guests without a reservation

If a booking request or accepted offer is not processed, a guest may arrive expecting a room even though no reservation exists.

#### Out-of-order rooms can become emergency fallback capacity

Rooms that are normally blocked may still be considered as last-resort fallback capacity during operational recovery.

#### Non-guaranteed bookings can be displaced during operational recovery

When availability conflicts occur, non-guaranteed bookings may be treated as lower priority than guests whose booking failure was caused internally.

#### Manual recovery decisions often balance guest impact, policy, and available fallback capacity

When something goes wrong, staff must balance policy, fairness, guest impact, and remaining room options to find an acceptable recovery path.

---

### Same-Day Changes and Downstream Operational Effects

#### Last-minute occupancy changes affect room preparation

When guests arrive with a different occupancy than expected, room setup and service assumptions may no longer match the actual need.

#### Additional guests require reservation updates and service adjustments

Adding an extra person can require updates to the reservation, pricing, breakfast, city tax, bedding, towels, and room preparation.

#### Front office may need to compensate for unavailable housekeeping support

When housekeeping is no longer available, front office staff may need to handle room-preparation issues themselves.

#### Late breakfast additions affect food and beverage staffing and supply planning

Breakfast decisions made during check-in can significantly change the expected breakfast volume for the next day.

#### Same-day service changes can create downstream operational pressure

Short-notice service changes can affect other departments, staffing plans, supplies, and guest-facing service quality.

---

### Visibility and Information Needs

#### Front office needs fast access to booking context during check-in

Check-in depends on quickly understanding relevant booking information without searching through too many places.

#### Payment status and cost coverage must be visible before guest interaction

Staff need to know whether a booking is paid, unpaid, guaranteed, covered by a company, or paid by the guest before or during check-in.

#### Stay length influences room assignment decisions

The expected length of stay affects which room staff prefer to assign, because poor assignments can create later room moves.

#### Guest type and travel purpose affect billing and handling decisions

Whether a stay is business-related, private, corporate, or group-related influences billing, documentation, and guest handling.

#### Breakfast, parking, and included services must be easy to verify

Operationally relevant extras and included services must be visible enough for staff to avoid disputes or incorrect charges.

#### Important operational information may exist in the system but still be hard to notice

The issue is not always missing data. Sometimes the data exists, but it is distributed, hidden, inconsistently formatted, or not visible at the right moment.

#### Staff often rely on accumulated workflow knowledge to notice relevant information quickly

Experienced staff may process important information almost automatically, but this knowledge is implicit and may not be obvious to new staff or system designers.
