# Three-Plane Governance Model

The strategy separates retained data into three planes. Each plane has a distinct purpose, latency expectation, ownership model, and cost posture.

## 1. Evidence Plane

Purpose:

- Preserve immutable clinical evidence.
- Support audit, legal, regulatory, and clinical traceability needs.
- Maintain source-level integrity.

Data examples:

- Raw HL7 messages
- Original inbound payloads
- Audit-required logs
- Immutable source events

Characteristics:

- Cold or archive-optimized
- Immutable
- Strongly governed
- Retrieval by exception
- High audit value

## 2. Service Plane

Purpose:

- Power operational product workflows and standard retrieval journeys.
- Provide canonical data access for applications, support, and interoperability.

Data examples:

- Canonical patient records
- Normalized HL7/FHIR resources
- Retrieval service indexes
- Operational metadata

Characteristics:

- Hot or warm
- Canonical-first
- API-accessible
- SLA-managed
- Product-owned

## 3. Insight Plane

Purpose:

- Support analytics, reporting, forecasting, and business intelligence.
- Enable derived insight without creating unmanaged historical sprawl.

Data examples:

- Aggregated reporting tables
- De-identified analytics datasets
- Executive dashboards
- Trend and cost models

Characteristics:

- Warm
- Derived
- Expiry-managed
- Data product oriented
- Rebuildable from governed sources

## Governance Principle

The same clinical evidence should not be retained indefinitely in every plane. The evidence plane protects proof, the service plane serves users, and the insight plane supports decisions.
