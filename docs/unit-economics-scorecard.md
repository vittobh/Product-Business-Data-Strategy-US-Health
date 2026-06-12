# Unit Economics Scorecard

Traditional storage reporting focuses on raw terabytes. For healthcare platforms, this is incomplete because terabytes do not show whether the same clinical evidence is being retained multiple times.

This scorecard reframes archival success around unit economics and duplication control.

## Primary Metrics

### Cost per Million HL7 Messages

Measures the total storage and retrieval cost associated with each million retained HL7 messages.

Why it matters:

- Normalizes cost against business volume.
- Helps separate organic clinical growth from structural storage waste.
- Supports FinOps comparison across storage classes and platforms.

### Duplicate-Copy Ratio

Measures how many retained representations exist for the same clinical evidence.

Target:

- Less than 1.2:1 for governed retained history

Why it matters:

- Exposes redundant raw, parsed, canonical, analytics, and partner copies.
- Creates executive visibility into the multiplication tax.
- Forces rationalization of stale or unmanaged assets.

### Premium Storage Share

Measures the percentage of data held in high-cost storage classes.

Why it matters:

- Prevents low-value history from remaining in hot storage.
- Aligns data tiering with actual business value.

### Canonical Retrieval Adoption

Measures the percentage of retrieval requests served through canonical service paths.

Why it matters:

- Reduces restore-heavy workflows.
- Improves retrieval reliability.
- Creates a standard operating model for support, product, and compliance needs.

### Redundant Asset Retirement Rate

Measures the retirement of stale marts, expired extracts, duplicate exports, and unnecessary historical datasets.

Why it matters:

- Converts strategy into measurable footprint reduction.
- Keeps momentum visible to leadership.

## Example Executive Scorecard

| Metric | Baseline Question | Target Direction |
| --- | --- | --- |
| Cost per million HL7 messages | What does each million messages cost to retain and retrieve? | Down |
| Duplicate-copy ratio | How many copies exist per evidence record? | Under 1.2:1 |
| Premium storage share | How much low-value history sits in high-cost storage? | Down |
| Canonical retrieval adoption | How much retrieval avoids raw replay? | Up |
| Redundant asset retirement | How much stale history was removed? | Up |
| Retrieval SLA adherence | Are retrieval commitments met by class? | Up |

## Executive Interpretation

If cost per million messages rises while patient or message volume is flat, the platform has a structural duplication problem. If duplicate-copy ratio falls while retrieval SLAs remain healthy, the strategy is working.
