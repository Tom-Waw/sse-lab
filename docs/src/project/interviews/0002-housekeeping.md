# Interview 0002: Housekeeping

## Purpose

This interview explores housekeeping workflows and room readiness.

The goal is to understand how rooms move from occupied or dirty to ready, how housekeeping work is discovered and prioritized, and where coordination problems appear.

This interview should help identify generalized workflow problems that may later inform room lifecycle, housekeeping task, staff assignment, and operational dashboard requirements.

## Focus Areas

- Room readiness
- Room state transitions
- Housekeeping task discovery
- Task prioritization
- Workload visibility
- Special room preparation
- Coordination with front office and shift leads

## Questions

### Workflow

- What does a typical housekeeping workflow look like at a high level?
- How does housekeeping know which rooms need work?
- What information is needed before starting a room?
- How does the workflow differ between stayover rooms, departure rooms, and rooms prepared for arrival?

### Room Readiness

- What does it mean for a room to be ready?
- What can cause a room to be physically free but not ready?
- Which room states are important for staff to distinguish?
- How do staff know whether a room is dirty, clean, inspected, blocked, or ready?
- How are out-of-order or out-of-service rooms handled from the housekeeping side?

### Task Coordination

- How are housekeeping tasks usually prioritized?
- What makes a room urgent?
- How are changes in priority communicated?
- What information from front office is most important before cleaning or preparing rooms?
- How are special requests or occupancy changes communicated?

### Workload

- What makes housekeeping workload feel balanced or unbalanced?
- Which constraints matter when assigning work?
- How are interruptions or unexpected tasks handled?
- How do single and double occupancy preparations affect housekeeping work?
- What information would help staff plan work better?

### Handoffs

- How does housekeeping communicate room readiness to front office?
- What happens when front office needs a room urgently?
- What kinds of handoff problems create delays?
- What happens when the room status in the system does not match what housekeeping finds in the room?

## Follow-up Prompts

- Is this a normal part of the workflow or an exception?
- Which roles depend on this information?
- What happens if the room state is wrong?
- What information would prevent confusion?
- How is this communicated today?
- Who is allowed to make or override this decision?
- Can this be generalized without describing a specific employer process?

## Generalized Findings

### Housekeeping Workflow and Work Allocation

#### Housekeeping starts with a front office handover

Housekeeping begins by receiving relevant operational information from front office, especially special requests, expected room needs, occupancy setup, and anything that affects room preparation.

#### Housekeeping work is allocated by floor, workload, and expected room needs

Housekeeping work is distributed based on floors, the number of rooms to clean, expected arrivals, and the practical effort required on each floor.

#### Housekeeping leadership assigns work while cleaners execute assigned room lists

Housekeeping work is coordinated by a lead or responsible role that distributes room lists, while cleaners usually work from assigned tasks rather than managing the full operational picture themselves.

#### Housekeeping distinguishes departure rooms, stayover rooms, and arrival preparation

Housekeeping work differs depending on whether a room is a departure, a stayover, or a room being prepared for an arriving guest. These categories affect cleaning scope and urgency.

#### Housekeeping may prioritize only the rooms needed for expected arrivals

When cleaning capacity is limited, housekeeping may not need to clean every dirty room immediately. The immediate target can be the number and type of rooms required for expected arrivals.

#### Housekeeping ends with a structured handover back to front office

At the end of the housekeeping workflow, front office receives updated information about cleaned rooms, skipped rooms, defects, special preparations, and available extras.

#### Housekeeping reports cleaned rooms, skipped rooms, special setups, defects, and floor-level extras

The handover includes operational details that front office may need later, such as rooms that were not cleaned, rooms with special setups, defects found during cleaning, and extra bedding or supplies stored on specific floors.

---

### Room Readiness and Lifecycle States

#### A room is ready only after cleaning, restocking, and quality checking

A room is not ready merely because the previous guest has left. It must be cleaned, restocked with expected items, and checked before it can be confidently released.

#### Physically free rooms are not necessarily ready for assignment

A room can be empty but still unusable for a new guest because it has not yet been cleaned, checked, restocked, or released.

#### Departure and stayover rooms require different cleaning scopes

Departure rooms require a full reset for the next guest, while stayover rooms usually receive a lighter service depending on guest presence and service rules.

#### Long-empty rooms may need refresh work even when marked clean

A room that has been unused for a longer period may still need airing, dusting, water flushing, or other refresh work even if it is technically marked as clean.

#### Long-unused clean rooms are hard to identify systematically

Housekeeping may not have system support for identifying rooms that have been empty long enough to require refresh work, making this condition harder to detect systematically.

#### Housekeeping distinguishes occupancy, cleanliness, inspection, and repair-related states

From the housekeeping perspective, room readiness depends on multiple dimensions: whether the room is occupied, whether it has been cleaned, whether it has been checked, and whether defects or repairs affect usability.

---

### Capacity Planning and Prioritization

#### Housekeeping planning depends on forecasted room workload

Housekeeping capacity is planned against expected room workload, especially forecasted departures, stayovers, and arrivals.

#### Housekeeping capacity planning depends on staffing, expected workload, and provider coordination

The ability to complete all required rooms depends on available cleaners, expected workload, and whether staffing is handled internally or through an external provider.

#### Unexpected staff shortages force capacity-based prioritization

When fewer cleaners are available than expected, housekeeping may need to decide which rooms are truly required for the day and which work can be deferred.

#### Workload distribution depends on both room count and floor distribution

The number of rooms alone is not enough to understand workload. Distribution across floors matters because some floors may have more departures, stayovers, or room types than others.

#### Prepared clean inventory becomes critical as check-in time approaches

As official check-in time approaches, front office needs enough clean and released rooms to handle arriving guests. Lack of clean inventory creates immediate operational pressure.

#### Stayover rooms can become urgent when guests leave the room late

Stayover rooms can become urgent when guests remain in the room for much of the day and later request cleaning while housekeeping is already progressing through planned work.

#### Pre-assigned rooms with special requests are high priority

Rooms linked to special requests, such as baby beds or specific room wishes, become high priority because front office may not be able to simply assign another room.

#### Front office priority changes are communicated outside the core system

When front office urgently needs a room or changes priorities, this is communicated through informal or external channels rather than through a dedicated prioritization mechanism in the core system.

---

### Special Preparation and Occupancy Setup

#### Special requests are communicated through handover information

Special preparation needs, such as baby beds, extra bedding, or other room-specific requests, are passed to housekeeping through handover information.

#### Baby beds and similar fixed-room requests create hard assignment constraints

Some special requests bind preparation to a specific room. Once that room has been prepared for the request, changing the assignment becomes harder.

#### Connection bookings must be communicated to avoid incorrect departure cleaning

If a guest has a follow-up booking and remains in the same room, housekeeping must know this. Otherwise the room may appear as a departure even though it should be treated as a stayover.

#### Occupancy setup determines bedding, towels, and preparation effort

The number of expected occupants determines how many bedding sets, towels, and related room items are required.

#### Single and double occupancy preparation affects labor and laundry cost

Preparing rooms for double occupancy requires more bedding, towels, laundry, and handling effort than single occupancy. This creates a cost and workload difference.

#### Housekeeping tries to reuse already prepared occupancy setups when possible

To avoid unnecessary work, housekeeping prefers to use rooms that are already prepared in the required occupancy setup instead of changing prepared rooms again.

#### Temporary room markers are used to group operationally relevant rooms

Temporary markers can help group rooms that share a temporary operational meaning, such as rooms already prepared for a certain occupancy setup.

#### Generic temporary room markers can become ambiguous without shared context

A generic marker only works when all involved staff understand what it means in the current situation. Without shared context, the marker does not explain itself.

#### Bed-size and room-category mix affects whether prepared rooms match arriving guests

It is not enough to prepare the right number of double rooms. The prepared room mix must also match expected bed sizes or room categories, otherwise front office may face assignment conflicts.

---

### Quality Control, Defects, and Supplies

#### Cleaned rooms are inspected before being released

Rooms are checked after cleaning before they are marked as clean or ready. This creates a quality gate between cleaning work and operational release.

#### Quality control helps compensate for fatigue and inconsistent cleaning quality

Cleaning many rooms is physically demanding, and quality may decline over time. Inspection helps catch issues before guests receive the room.

#### Housekeeping identifies defects during cleaning and inspection

Because housekeeping enters and checks rooms directly, it is often the first role to notice broken, missing, dirty, or unsafe items.

#### Housekeeping helps classify defects by operational severity

Housekeeping may judge whether an issue is minor and fixable by staff, requires maintenance, or makes the room unsuitable for guest use.

#### Defect reasons must be visible for restricted rooms

When a room is blocked, restricted, or marked for service, staff need to know the reason so they can judge urgency, responsibility, and whether the room can be released again.

#### Defects are communicated through maintenance or technician lists

Defects discovered in rooms are passed to maintenance through a dedicated list or similar coordination mechanism.

#### Housekeeping records lost-and-found items

Housekeeping handles lost property discovered during cleaning and records relevant details such as room, date, and item type.

#### Housekeeping supervisors monitor supplies, cleaning materials, and department stock

Housekeeping leadership is also responsible for ensuring that cleaning materials, consumables, and department supplies are available.

---

### Handover, System Access, and Status Updates

#### Housekeeping derives work from system-generated departure and stayover lists

The system provides the basis for housekeeping work by listing departures and stayovers, which are then used to create room work assignments.

#### Housekeeping system access is limited for privacy and operational simplicity

Housekeeping does not need the same level of guest and booking information as front office. Access is limited to protect privacy and keep the workflow focused.

#### Cleaners may work from assigned room lists instead of direct system access

Individual cleaners may not interact with the system directly. Instead, they receive assigned room lists and report progress or completion through supervisors or communication channels.

#### Housekeeping benefits from privacy-safe arrival-category information

Housekeeping may need to know what kinds of rooms are required for arrivals, but not necessarily personal guest details. This creates a need for privacy-safe operational visibility.

#### Front office depends on housekeeping to mark rooms clean in time

Front office can only confidently assign and check in guests once rooms are marked clean or otherwise confirmed ready.

#### Room-readiness updates may lag behind physical inspection

A room may already be physically checked and ready before its status is updated in the system, especially if the responsible person must return to an office or system access point first.

#### Front office may override dirty-room warnings when housekeeping confirms readiness

If housekeeping confirms that a room is clean but the system has not been updated yet, front office may still use the room by relying on direct confirmation.

#### Operational flexibility depends on trusted communication between front office and housekeeping

The system state is important, but live operations also rely on trust between departments when urgent decisions are needed.

#### Missing occupancy setup information causes preparation mismatches

If housekeeping does not receive accurate occupancy information, rooms may be prepared with the wrong bedding, towels, or setup.

#### Missing bed-size or room-category information causes assignment conflicts

If housekeeping prepares the wrong mix of room categories or bed sizes, front office may not have suitable clean rooms for arriving guests.

#### Missing connection-booking information causes unnecessary or incorrect cleaning work

When follow-up stays are not communicated, housekeeping may treat an occupied or continuing room as a departure, causing confusion and extra work.

---

### State Mismatches, Exceptions, and Recovery

#### System room status can differ from physical room condition

The room status shown in the system may not always match the real physical state of the room.

#### Rooms can be marked clean incorrectly through housekeeping error

A room can be accidentally marked clean even though it is still dirty, usually due to human error during status updates.

#### Rooms can remain marked dirty even when physically unused

A room can remain marked dirty even if it was not actually used, for example after online check-in, no physical arrival, or certain room-move situations.

#### Room moves can leave room cleanliness state incorrect if handled too quickly

During room moves, staff may accidentally choose the wrong cleanliness outcome for the original room, leaving the system state inaccurate.

#### Online check-in can create room-status ambiguity

Online check-in can make it unclear whether a room has only been assigned digitally or physically entered and used by a guest.

#### Status mismatches require recent room history to be understandable

When system status and physical room condition differ, staff need a way to understand what recently happened to the room in order to resolve the mismatch.

#### Out-of-service rooms can be released when housekeeping confirms the issue is resolved

Rooms with minor service issues may be returned to normal use once housekeeping confirms the issue has been handled.

#### Out-of-order rooms require controlled repair confirmation before release

Rooms with serious defects require stronger confirmation before being released, especially when external repair or safety-relevant work is involved.

#### Early arrivals create pressure before official check-in time

Guests may arrive before official check-in time, creating pressure to provide rooms earlier than planned.

#### Limited luggage storage can increase pressure to release rooms early

When many early arrivals want to store luggage, front office may prefer to check guests in earlier if clean rooms are available.

#### Unexpected tasks and guest complaints disrupt planned housekeeping flow

Guest complaints, new requests, incidents, and short-notice changes can interrupt the planned room-cleaning sequence.

#### Incidents and workplace accidents require separate reporting

Workplace incidents or injuries create additional reporting work outside the normal room-cleaning workflow.
