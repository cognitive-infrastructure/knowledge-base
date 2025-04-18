---
id: ci:pattern.single-source-of-truth
category: pattern
version: 1.0
author: Rashid Azarang
canonicalDate: 2024-04-16
---

# Single Source of Truth

**Intent** Establish authoritative entity records from which all other representations derive.

| Section | Notes |
|---------|-------|
| **Context** | Multiple systems tracking the same entities; distributed teams; reporting inconsistencies; high data reconciliation costs. |
| **Problem** | Same entity exists in multiple systems with conflicting attributes, creating reconciliation burdens and eroding trust in operational data. |
| **Forces** | System specialization needs vs. data integrity, distributed ownership models, history of siloed development, performance requirements for local data. |
| **Solution** | Designate one system as the authoritative record for each entity type. Create clear data ownership model with published SLAs. Implement synchronization mechanisms where other systems need local copies, with explicit freshness metadata and lineage tracking. |
| **Resulting Context** | Clear resolution path for data conflicts; reduced reconciliation effort; foundation for reliable analytics; trust in system data improves operational decision quality. |
| **Signals of Success** | Entity lookups converge to same result regardless of starting system; reduced time spent reconciling conflicting records; declining duplicate entity counts; increased reference to canonical sources in reporting. |
| **Anti-Patterns Prevented** | Semantic Drift, Cognitive Amnesia |
| **See Also** | [Canonical IDs](canonical-ids.md), [Semantic Foundation](semantic-foundation.md) |







## Related

- [Canonical IDs](canonical-ids.md) (Pattern)
- [Semantic Foundation](semantic-foundation.md) (Pattern)
- [Cognitive Amnesia](../anti-patterns/cognitive-amnesia.md) (Anti-Pattern)
- [Semantic Drift](../anti-patterns/semantic-drift.md) (Anti-Pattern)
