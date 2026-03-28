# DurantOS Progress

![Status](https://img.shields.io/badge/status-public%20progress%20tracker-0f766e?style=for-the-badge)
![Release](https://img.shields.io/badge/current%20release-0.80.0%20(764)-111827?style=for-the-badge)
![Scope](https://img.shields.io/badge/repo-docs%20only-c2410c?style=for-the-badge)

This repository is a public progress tracker for DurantOS.

DurantOS is an internal operations platform for Durant Lifts. It connects office operations, engineering delivery, customer records, scheduling, finance, reporting, and customer-facing document flows into one system.

This public repository exists to show product direction and delivery progress without exposing private source code, infrastructure, customer data, or internal operating details.

## Current Status

- Current documented release: `0.80.0 (764)`
- Latest iOS build upload: March 28, 2026
- Delivery state reached: uploaded successfully to App Store Connect / TestFlight processing pipeline
- Source code repository: private

## What DurantOS Covers

DurantOS is being built to connect the real operating chain of the company:

`customer -> site -> unit -> job -> engineer -> report -> invoice -> portal -> payment -> follow-up`

Current platform areas include:

- customer, site, and unit records
- office job control and scheduling
- engineer dispatch and acknowledgement
- report review and LOLER follow-up
- quote and invoice handling
- payables and expense capture
- document storage and portal publishing
- operational sync, recovery, and audit flows

## Recent Progress

Recent product work has focused on six areas:

- clearer office-to-field job workflow, including dispatch, accept, and decline states
- stronger engineer mobile flow so current work and planned work do not drift apart
- richer customer and intake records, including payment terms and multi-recipient contact routing
- deeper finance workflows, including quote-to-invoice continuity, overdue chase stages, and receipt tracking
- stronger LOLER extraction and follow-up visibility
- faster and safer sync behavior on real devices under backlog and retry conditions

## In This Repository

- [Progression](docs/progression.md): product-shape and workflow progression summary
- [Releases](docs/releases.md): recent milestone and release log
- [Product Shape](docs/product-shape.md): what the platform is becoming
- [Notice](NOTICE.md): what is intentionally excluded from this public repo

## What Is Not Included

This repository does not include:

- application source code
- backend source code
- secrets, keys, or environment values
- deployment configuration
- customer data
- access instructions, login instructions, or internal operating procedures

This is intentional. The goal is public visibility into progress, not public distribution of the product itself.
