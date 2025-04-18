---
id: ci:pattern.progressive-typing
category: pattern
version: 1.0
author: Rashid Azarang
canonicalDate: 2024-04-16
---

# Progressive Typing

**Intent** Begin with flexible data structures that tighten as understanding grows, balancing exploration with eventual consistency.

| Section | Notes |
|---------|-------|
| **Context** | Emerging domains with evolving understanding; initial implementations of data models; knowledge work systems; exploration-oriented tools. |
| **Problem** | Premature type rigidity prevents discovery and adaptation, while permanent looseness creates inconsistency and unreliability. |
| **Forces** | Exploration needs vs. consistency requirements, unknown future use cases, varying skill levels among contributors, knowledge emergence patterns. |
| **Solution** | Design data structures with explicit evolutionary stages: 1) start with schema-flexible formats that capture raw information, 2) identify recurring patterns through regular analysis, 3) formalize schema elements as patterns stabilize, 4) gradually increase validation requirements as understanding solidifies. |
| **Resulting Context** | Balance between exploration freedom and structural reliability; data models that evolve with understanding rather than constraining it; reduced need for disruptive migrations; natural knowledge formalization paths. |
| **Signals of Success** | Decreasing schema change frequency over time; data validation exceptions cluster around emerging concepts rather than established ones; reduced friction in both early exploration and mature usage; clear evolutionary history visible in data structures. |
| **Anti-Patterns Prevented** | Ballup, Over-Layering |
| **See Also** | [Universal Evolutionary Stages](../../core-concepts/universal-evolutionary-stages.md), [Continuity-Disruption Balance](../../core-concepts/continuity-disruption-balance.md) |







## Related

- [Continuity-Disruption Balance](../../core-concepts/continuity-disruption-balance.md) (Core Concept)
- [Universal Evolutionary Stages](../../core-concepts/universal-evolutionary-stages.md) (Core Concept)
- [Ballup](../anti-patterns/ballup.md) (Anti-Pattern)
