# Progression

## Overview

DurantOS started as a lightweight admin tool. It is now moving toward an internal operating system for lift-service delivery.

The main direction is not "more forms." The direction is tighter coordination between planning, field work, reporting, billing, document delivery, and follow-up.

## Jobs And Field Delivery

The jobs workflow has moved from a simpler assigned/completed model into a clearer office-to-field chain.

Recent progression includes:

- `Engineer Standby` as a first-class job type instead of ad hoc free text
- invoice creation support for standby work
- explicit dispatch state on jobs instead of treating engineer assignment as delivery
- field acknowledgement through `Accept` and `Decline`
- required decline reasons so refused jobs return to office review with context
- dedicated office workflow buckets for active, dispatched, declined, completed, and finished work

This matters because planning, dispatch, acknowledgement, and completion are now separate operational states instead of hidden assumptions.

## Engineer Mobile Flow

Engineer mobile work has also been tightened.

Progression includes:

- current-job state aligned with planner state
- accepted jobs moving into the engineer workflow cleanly
- active jobs no longer lingering in planned views
- clearer empty states around job receipt and acceptance

The effect is a more reliable handoff between office dispatch and field execution.

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

The platform is increasingly using customer data for real routing, billing, and document delivery, so a flat contact model is no longer enough.

## Finance

Finance is now a connected workflow area rather than a passive invoice store.

Progression includes:

- quote-to-invoice continuity
- invoice status normalization
- overdue and sent-state logic
- receipt tracking for paid invoices
- staged invoice chase handling
- purchase-order-aware invoice emailing
- payables workspace
- VAT-aware expense and payable handling
- finance attachment capture from connected mailboxes

This is moving the product toward a proper receivables and finance-control layer.

## LOLER And Review

LOLER work has progressed in two directions at once: stronger extraction and stronger review.

Progression includes:

- layered PDF text extraction with OCR fallback
- more grounded LOLER item extraction
- review-aware evidence display
- fewer silent drops at final save
- clearer unit-level visibility for outstanding LOLER actions

This keeps the intelligence layer reviewable instead of opaque.

## Sync And Runtime

Sync has been treated as a product capability, not just background plumbing.

Progression includes:

- mutation deduping
- queue reset tooling
- live progress counters
- bounded concurrency on push and pull
- safer id normalization across queued work
- better handling of larger queues and retry-heavy states

This work matters most on real devices, where offline and degraded-network behavior define trust in the product.
