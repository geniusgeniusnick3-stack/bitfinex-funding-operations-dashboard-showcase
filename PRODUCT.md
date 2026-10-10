# Product Truth

## Product
Bitfinex Funding Operations Dashboard — a read-only, portfolio-safe showcase of automated margin-funding operations.

## Audience
Hiring managers, engineers, quantitative researchers, and product reviewers evaluating a trading-operations system.

## Purpose
Make funding operations legible: wallet allocation, active funding, offers, net APR, earnings, event history, and the distinction between an exchange API's current funding segment and the original persisted funding lifecycle.

## Primary job
A reviewer should understand the system's current state and the lifecycle reconciliation problem within one minute.

## Evidence
Synthetic but realistic demo data derived from the project's documented USD funding lifecycle. Every displayed portfolio value is demo data and must not imply a live public account.

## Safety constraints
- Read-only demo mode.
- No exchange credentials, API calls, order actions, or account identifiers.
- Clearly label demo data as simulated.
- Do not claim audited or live performance.

## Required content
Overview, funding positions, lifecycle timeline, earnings, event log, and system health.

## Mode
Operate: the interface must prioritize scanability, state clarity, and operational trust over decorative finance UI conventions.
