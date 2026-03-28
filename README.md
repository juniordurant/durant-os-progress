# DurantOS Progress

![Status](https://img.shields.io/badge/status-public%20progress%20tracker-0f766e?style=for-the-badge)
![Release](https://img.shields.io/badge/current%20release-0.80.0%20(764)-111827?style=for-the-badge)
![Scope](https://img.shields.io/badge/repo-docs%20only-c2410c?style=for-the-badge)
![Visibility](https://img.shields.io/badge/source%20repo-private-7c3aed?style=for-the-badge)

## 🚀 Public Window Into DurantOS

DurantOS is an internal operating platform for Durant Lifts.

It is being shaped to connect office control, engineer delivery, reporting, finance, compliance follow-up, document publishing, and customer-facing workflows into one coordinated operating system.

This public repository is intentionally docs-only. It exists to show momentum, product direction, and workflow maturity without exposing source code, infrastructure, customer data, or internal operating details.

> 🔒 Public progress only. Private implementation remains private.

## ✨ Snapshot

| Signal | Current state |
| --- | --- |
| 🗂️ Public repository | Docs-only progress tracker |
| 📦 Current documented release | `0.80.0 (764)` |
| 📱 Latest iOS milestone | Build uploaded to App Store Connect on March 28, 2026 |
| 🔐 Source visibility | Private |
| 🧭 Product direction | From isolated records to connected operational workflows |

## 🧭 Workflow Spine

DurantOS is being designed around the real chain of lift-service work:

```mermaid
flowchart LR
    A["Customer"] --> B["Site"]
    B --> C["Unit"]
    C --> D["Job"]
    D --> E["Engineer"]
    E --> F["Report"]
    F --> G["Invoice"]
    G --> H["Portal"]
    H --> I["Payment"]
    I --> J["Follow-up"]
```

The goal is not just digitising paperwork. The goal is reducing friction between planning, field delivery, review, billing, document handling, and follow-through.

## 🔥 Current Momentum

Recent work has pushed the platform in a more system-level direction:

- 🚚 jobs now move through explicit dispatch instead of hiding delivery assumptions inside assignment
- 📲 engineers can receive, accept, or decline work with context captured for office review
- 🛠️ engineer mobile state is tighter, so active work no longer lingers in planned views
- 🧾 finance is moving beyond invoice storage into chase, receipt, payable, and continuity workflows
- 🧠 LOLER extraction and review paths are becoming more visible, safer, and easier to validate
- 🔄 sync and runtime behavior keep getting hardened for real-world device usage

## 🧱 Platform Areas

The public view of the platform now spans:

- 👥 customer, site, and unit records
- 🗓️ office job control and scheduling
- 📡 engineer dispatch and acknowledgement
- 📋 report review and LOLER follow-up
- 💷 quote and invoice handling
- 🧾 payables and expense capture
- 📄 document storage and portal publishing
- 🛡️ sync, recovery, and audit-oriented operational flows

## 🌊 Progress Themes

### 🚚 Office To Field Workflow

Recent work has moved jobs from a simpler assigned/completed model into a clearer delivery chain:

- explicit dispatch state
- field accept / decline response
- decline reasons returning work to office review
- clearer separation between planning, dispatch, acknowledgement, and completion

### 📲 Engineer Mobile Reliability

Engineer mobile flow has been tightened so:

- accepted work moves cleanly into planning and current-job views
- active jobs do not linger in planned lists
- current-job state stays aligned with live workflow state

### 🏢 Customer And Commercial Records

Customer data has expanded beyond a basic contact record:

- payment terms
- company registration data
- multiple billing recipients
- multiple job-report recipients
- separate accounts and communication contacts
- website-originated intake with approval flow

### 💷 Finance Control

Finance is progressing from simple invoice storage into a workflow area with:

- quote-to-invoice continuity
- overdue and sent-state logic
- receipt tracking
- staged chase handling
- purchase-order-aware delivery
- payables and richer expense capture

### 🧠 LOLER And Review

LOLER work is progressing on both extraction quality and operational follow-up:

- stronger extraction and evidence handling
- better review support
- safer save behavior
- clearer unit-level visibility for outstanding actions

### 🔄 Sync And Runtime

Runtime work continues to focus on trust under real device conditions:

- deduped queue handling
- clearer progress counters
- bounded push and pull concurrency
- better behavior under backlog, retries, and degraded network conditions

## 🗓️ Milestone Timeline

| Date | Milestone | Directional impact |
| --- | --- | --- |
| March 28, 2026 | Dispatch workflow, engineer response flow, customer and finance expansion, extraction modularisation | Linked office planning more tightly to field acknowledgement while extending commercial, intake, and finance workflows |
| March 27, 2026 | Sync queue flushing improvements | Improved reliability and speed under real backlog conditions |
| March 25, 2026 | Finance capture, Outlook finance intake, payables, VAT automation, LOLER intelligence expansion | Deepened the finance layer and document-assisted workflows |
| March 8, 2026 | Portal PDF publishing, company documents, recovery and rollback improvements | Strengthened customer-facing delivery and operational recovery |

## 🧩 Product Shape

DurantOS is increasingly acting like an internal command system rather than a single admin tool.

The platform now links:

- customers
- sites
- units
- engineers
- jobs
- quotes
- invoices
- payables
- expenses
- contracts
- documents
- portal accounts

That shared graph matters because real business work rarely starts and ends inside one screen or one department.

## 📚 Explore The Docs

- [Progression](docs/progression.md): workflow-by-workflow progression summary
- [Releases](docs/releases.md): milestone and release log
- [Product Shape](docs/product-shape.md): public summary of what DurantOS is becoming
- [Notice](NOTICE.md): what is intentionally excluded

## 🔒 What Stays Private

This repository does not include:

- application source code
- backend source code
- secrets, keys, or environment values
- deployment configuration
- customer data
- login instructions
- internal operating procedures

That boundary is deliberate. The purpose of this repository is progress visibility, not product exposure.
