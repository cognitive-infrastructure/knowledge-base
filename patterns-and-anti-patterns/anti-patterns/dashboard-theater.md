---
id: ci:antipattern.dashboard-theater
category: antipattern
version: 1.0
author: Rashid Azarang
canonicalDate: 2024-04-16
---

# Dashboard Theater

"It looks impressive until someone asks what the numbers actually mean."

| Section | Notes |
|---------|-------|
| **Symptoms** | Beautiful visualizations that don't drive decisions; extensive manual preparation before using reports; increasing dashboard count without corresponding insight growth; persistent questions about metric definitions. |
| **Root Cause** | Interface layer sophistication has advanced beyond Logic and Data layer foundations; visualization tools used to create meaning rather than reflect it; aesthetic considerations prioritized over structural accuracy. |
| **Impact** | Declining trust in operational metrics; increasing time spent debating numbers rather than implications; decisions driven by offline analysis rather than systems; shadow reporting structures emerging to compensate. |
| **Structural Cure** | Pause dashboard development to strengthen Logic and Data layers. Implement Semantic Foundation pattern for key metrics. Create clear data lineage from source to visualization. Rebuild interfaces to accurately reflect underlying data quality and certainty. |
| **Quick Fixes (Stop-Gaps)** | Add data quality indicators to existing visualizations. Document known limitations in prominent locations. Create simplified "most trusted" views with fewer but more reliable metrics. Clearly separate facts from interpretations. |
| **Related Frictions** | Semantic Drift, Metric Mirage |







## Related

- [Semantic Foundation](../patterns/semantic-foundation.md) (Pattern)
- [Metric Mirage](metric-mirage.md) (Anti-Pattern)
- [Semantic Drift](semantic-drift.md) (Anti-Pattern)
