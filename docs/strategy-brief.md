# Strategy Brief

## Problem

Healthcare data platforms retain large volumes of HL7 messages, logs, patient records, raw payloads, parsed records, canonical records, analytics extracts, partner exports, and support copies. The growth problem is not only data volume. It is the number of representations retained for the same clinical evidence.

This creates a multiplication tax:

- Raw messages are retained indefinitely.
- Parsed and canonical records are stored as separate long-lived assets.
- Analytics marts duplicate history for convenience.
- Partner extracts remain active beyond their useful life.
- Troubleshooting logs and support datasets lack expiry discipline.

The result is storage cost growth that outpaces patient volume growth.

## Strategic Thesis

The path to durable storage economics is not just cheaper archive media. It is less duplicated history.

The strategy is to retain one governed evidence layer, protect it strongly, and make canonical-first retrieval the default operating path.

## Product Strategy

Pillar 06: Data Archival, Retention, and Retrieval Economics introduces a formal product and platform discipline for historical footprint reduction.

It converts archive management from a backend storage concern into a product strategy:

- Classify retained assets by business value.
- Assign lifecycle policy at creation time.
- Price storage and retrieval using unit economics.
- Route standard retrieval through canonical service paths.
- Treat raw replay as an exception, not a default.

## Key Moves

### Move 1: Collapse the Redundant Base

Identify and retire duplicate marts, long-lived extracts, redundant exports, stale snapshots, and support datasets that do not provide distinct regulatory or operational value.

### Move 2: Govern New Copies at Source

Require every new retained asset to have:

- Business-value class
- Retrieval class
- Lifecycle policy
- Data owner
- Expiry or review date

### Move 3: Route Retrieval Through Canonical Path

Make canonical-first retrieval the standard pattern for product, audit, support, and interoperability workflows. Raw replay remains available only through governed exception paths.

## Product Outcome

The platform scales economically as well as technically:

- Lower redundant storage footprint
- Better auditability
- Faster standard retrieval
- Stronger compliance evidence
- Reduced operational ambiguity
- Improved cost-to-serve visibility
