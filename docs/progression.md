# Progression

## Overview

DurantOS started as a lightweight admin tool. It is now moving toward an internal operating system for lift-service delivery, finance control, and evidence-backed follow-through.

The direction is not “more forms.” The direction is tighter coordination between planning, field work, notifications, review, billing, receipts, and accountant handoff.

## Maintenance Coordination

Maintenance progression is becoming easier to describe in operational terms.

Recent progression includes:

- clearer separation between planning space and engineer-route ownership
- stronger maintenance-series continuity when work relates to specific lift units
- better public signal that recurring maintenance is treated as an operational command problem, not just a calendar list
- tighter visual hierarchy in the maintenance area so people can move between questions faster

Why it matters:

Recurring service work is one of the easiest places for confusion to become expensive. Clearer sequencing and ownership reduce hidden mistakes.

## Jobs And Field Delivery

The jobs workflow has moved from a simpler assigned/completed model into a clearer office-to-field chain.

Recent progression includes:

- `Engineer Standby` as a first-class job type
- invoice creation support for standby work
- explicit dispatch state on jobs instead of treating assignment as delivery
- field acknowledgement through `Accept` and `Decline`
- required decline reasons so refused jobs return to office review
- office workflow buckets for active, dispatched, declined, completed, and finished work
- undispatch support when work needs to return to dispatch planning
- completed jobs can now seed follow-on work with the same site, customer, and lift-unit context
- job-report delivery is being tightened so a fresh send is more closely tied to the latest reviewed PDF state

Why it matters:

Planning, dispatch, acknowledgement, and completion are now separate operational states instead of hidden assumptions.

## Engineer Mobile Flow

Engineer mobile flow has also been tightened.

Progression includes:

- current-job state aligned with planner state
- accepted jobs moving into the engineer workflow cleanly
- active jobs no longer lingering in planned views
- dispatch notifications reaching engineer phones through the Azure-backed notification path
- receipt uploads moving directly from the field into the shared finance queue
- native receipt scanning with document crop for cleaner evidence capture

Why it matters:

The handoff between office dispatch and field execution is becoming more reliable, and the field app is contributing directly to finance evidence rather than ending at job completion.

## Notifications And Live Runtime

The platform is moving beyond “sync when someone remembers.”

Recent progression includes:

- Azure-backed engineer device registration
- engineer dispatch notifications for mobile delivery
- realtime refresh for key operational containers
- faster propagation for jobs, quotes, invoices, and finance-adjacent records
- better queue handling during rapid consecutive edits

Why it matters:

Operational systems need both immediate awareness and reliable fallback, not just background sync.

## Customer Records And Intake

Customer data has expanded from a minimal contact record into a more commercial and operational record.

Progression includes:

- company registration number support
- payment terms support
- multiple billing recipients
- multiple job-report recipients
- separate communication and accounts contact paths
- website-originated customer intake records
- intake approval that can create both the customer record and linked service sites
- customer records now retain and surface the original intake trail more visibly inside the details view
- customer labels are getting cleaner where company and individual naming overlap

Why it matters:

The platform is increasingly using customer data for routing, billing, and document delivery, so a flat contact model is no longer enough.

## Finance Command

Finance is now a connected workflow area rather than a passive invoice store.

Progression includes:

- quote-to-invoice continuity
- invoice status normalization
- overdue and sent-state logic
- receipt tracking for paid invoices
- bank transaction import, reconciliation, and invoice matching
- invoice PDF attachment on matched payment transactions
- staged invoice chase handling
- payable and expense capture
- Outlook-assisted finance intake
- shared-mailbox receipt capture for finance evidence
- transaction-seeded expense review queue
- cloud-backed receipts that can be uploaded on mobile and reviewed on macOS
- FreeAgent transaction sync and category visibility in the main transaction workspace
- matched invoice export back into FreeAgent, including safer handling when the external transaction has already moved on
- accountant-pack export for year-end or bookkeeping handoff
- invoice-performance views that increasingly surface movement, exposure, and collection rhythm instead of only static totals

Why it matters:

This is moving the product toward a real finance-control layer rather than a document list with totals. The public shape now makes it easier to describe how DurantOS handles both internal finance evidence and external accounting-system follow-through.

## Product Confidence And Polish

Public product confidence is now becoming part of the progression story.

Progression includes:

- stronger branded presentation at launch
- cleaner visual framing around operational and finance-heavy areas
- more polished outward communication for customer-facing intake
- polish that supports clarity rather than competing with it
- calmer desktop startup behaviour for day-to-day operator use
- built-in RAMS preview access rather than treating core reference material as something outside the app
- lightweight cleanup guardrails around legacy-heavy screens so structure can improve without forcing a rewrite

Why it matters:

Operational software still needs to feel intentional. Confidence, readability, and seriousness affect trust in the same way as raw capability.

## Invoice Safety

Invoice safety has become a separate progression theme rather than an afterthought.

Recent hardening includes:

- local invoices moved off `SharedPreferences` and into transactional SQLite/Drift row storage
- legacy invoice cache migration into the database
- direct fast-path invoice mutation queueing
- cloud invoice writes guarded against stale overwrite using ETag or `If-Match` style conflict handling
- bounded mobile startup recovery when local cache or schema state is messy

Why it matters:

Billing records are high-trust operational data. Silent overwrites are unacceptable in that layer.

## LOLER And Review

LOLER work has progressed in two directions at once: stronger extraction and stronger review.

Progression includes:

- layered PDF text extraction with OCR fallback
- more grounded LOLER item extraction
- review-aware evidence display
- fewer silent drops at final save
- clearer unit-level visibility for outstanding LOLER actions

Why it matters:

The intelligence layer stays reviewable instead of becoming opaque.

## Sync And Recovery

Sync has been treated as a product capability, not just background plumbing.

Progression includes:

- mutation deduping
- queue reset tooling
- live progress counters
- bounded concurrency on push and pull
- safer id normalization across queued work
- better handling of larger queues and retry-heavy states
- fast-path propagation for higher-value operational records
- restore points and deleted-item recovery

Why it matters:

This work matters most on real devices, where degraded-network behavior, rapid edits, and machine changes define trust in the product.
