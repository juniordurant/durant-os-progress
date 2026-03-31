# DurantOS Progress

<p align="center">
  <img src="docs/progress-console.svg" alt="DurantOS progress console" width="100%" />
</p>

<p align="center">
  <img alt="Status" src="https://img.shields.io/badge/status-public%20progress%20tracker-0f766e?style=for-the-badge" />
  <img alt="Release" src="https://img.shields.io/badge/current%20release-0.80.0%20(766)-111827?style=for-the-badge" />
  <img alt="Shape" src="https://img.shields.io/badge/shape-operations%20command%20system-1d4ed8?style=for-the-badge" />
  <img alt="Source" src="https://img.shields.io/badge/source-private%20implementation-f97316?style=for-the-badge" />
</p>

<p align="center">
  <a href="#snapshot"><strong>Snapshot</strong></a>
  ·
  <a href="#finance-flight-deck"><strong>Finance Flight Deck</strong></a>
  ·
  <a href="#workflow-spine"><strong>Workflow Spine</strong></a>
  ·
  <a href="#milestone-timeline"><strong>Milestone Timeline</strong></a>
  ·
  <a href="#explore-the-docs"><strong>Explore The Docs</strong></a>
</p>

DurantOS is an internal operating platform for Durant Lifts.

This public repository is the clean window into that work. It tracks direction, maturity, and release momentum without exposing source code, infrastructure secrets, customer data, or private operating logic.

> Updated March 31, 2026. The current visible push is finance command: transaction reconciliation, cloud receipts, mobile receipt scanning, and a cleaner accountant handoff.

## Snapshot

| Signal | Current state |
| --- | --- |
| Public repository | docs-only progress tracker |
| Current documented release | `0.80.0 (766)` |
| Workflow tone | internal command system, not just admin software |
| Finance momentum | transactions, expenses, receipts, invoice matching, accountant-pack export |
| Field momentum | clearer engineer mobile flow with native receipt scanning |
| Runtime direction | local-first client behavior with wider cloud-backed evidence and handoff |

## Finance Flight Deck

The finance layer has moved from “invoice list plus totals” toward a real operating loop:

- bank transactions can be imported, filtered, exported, and matched to invoices
- invoice PDFs can now travel with matched payment transactions
- outgoing transactions can seed the expense queue
- receipts can be uploaded from engineer mobile and stored in the cloud
- finance review can be staged for an accountant instead of staying as loose notes and files
- the platform can now export an accountant pack with linked supporting documents

That matters because year-end handoff, audit follow-up, and day-to-day bookkeeping all depend on evidence staying attached to the transaction chain.

## Workflow Spine

DurantOS is being shaped around the real chain of lift-service work:

```mermaid
flowchart LR
    A["Customer"] --> B["Site"]
    B --> C["Unit"]
    C --> D["Job"]
    D --> E["Engineer"]
    E --> F["Report"]
    F --> G["Invoice"]
    G --> H["Payment"]
    H --> I["Expense / Receipt Evidence"]
    I --> J["Accountant Review"]
```

The goal is not just digitising paperwork. The goal is tightening the chain between planning, field delivery, review, billing, evidence capture, and follow-through.

## Current Momentum

- office, field, finance, and portal workflows are increasingly sharing one data spine instead of passing loose files around
- mobile engineers are no longer just completing jobs; they are contributing evidence into the same bookkeeping flow
- billing workflows are now closer to an auditable record than a generated PDF archive
- sync and recovery work continues to matter because this product is expected to survive real devices, real backlogs, and real interruptions

## Platform Areas

The public view of the platform now spans:

- customer, site, and unit records
- office planning, dispatch, and job control
- engineer mobile delivery
- review and LOLER follow-up
- quotes, invoices, and payment tracking
- expenses, receipts, payables, and accountant handoff
- document storage and portal publishing
- sync, rollback, and audit-oriented platform work

## Milestone Timeline

| Date | Milestone | Directional impact |
| --- | --- | --- |
| March 31, 2026 | Finance command and accountant handoff | Transactions, expenses, receipts, invoice-PDF linking, accountant-pack export, and native receipt scanning pushed DurantOS further into a true finance operations surface |
| March 29, 2026 | Notifications, realtime sync expansion, and invoice safety hardening | Engineer push notifications, faster live propagation, safer invoice persistence, and guarded cloud invoice writes moved the platform closer to trusted operational execution |
| March 28, 2026 | Dispatch workflow and broader platform progression | Jobs gained explicit dispatch and engineer response flow, while customer, finance, and extraction work expanded further |
| March 27, 2026 | Sync runtime improvement | Queue flushing and sync throughput improved under backlog conditions |
| March 25, 2026 | Finance and assisted workflow expansion | Finance capture, Outlook intake, payables, VAT automation, and LOLER intelligence moved forward together |

## Product Direction

DurantOS is increasingly acting like an internal command system rather than a single admin tool.

The platform now links:

- customers
- sites
- units
- engineers
- jobs
- quotes
- invoices
- transactions
- expenses
- payables
- contracts
- documents
- portal accounts

That shared graph matters because real business work rarely starts and ends inside one screen or one team.

## Explore The Docs

- [Progression](docs/progression.md): workflow-by-workflow progression summary
- [Releases](docs/releases.md): release and milestone log
- [Product Shape](docs/product-shape.md): public summary of what DurantOS is becoming
- [Notice](NOTICE.md): what is intentionally excluded

## What Stays Private

This repository does not include:

- application source code
- backend source code
- secrets, keys, or environment values
- deployment configuration
- customer data
- app access instructions
- internal operating procedures

That boundary is deliberate. The purpose of this repository is progress visibility, not product exposure.
