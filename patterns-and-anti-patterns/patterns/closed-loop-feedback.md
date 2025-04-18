---
id: ci:pattern.closed-loop-feedback
category: pattern
version: 1.0
author: Rashid Azarang
canonicalDate: 2024-04-16
---

# Closed-Loop Feedback

**Intent** Design measurement systems that immediately inform adjustments through clear action pathways.

| Section | Notes |
|---------|-------|
| **Context** | Complex operational environments; continuous improvement programs; autonomous or semi-autonomous systems; dynamic market conditions. |
| **Problem** | Measurements exist but don't influence behavior; metrics are collected but not actioned; feedback cycles are too slow to prevent recurring issues. |
| **Forces** | Measurement vs. action orientation, lag time in traditional reporting, organizational silos, unclear ownership of response protocols, incentive misalignment. |
| **Solution** | For each critical metric, establish: 1) clear intervention thresholds, 2) predefined response protocols, 3) explicit ownership of action, and 4) verification mechanisms to confirm intervention effectiveness. Design feedback visualizations that incorporate both measure and response as a unified view. |
| **Resulting Context** | Self-regulating operational systems that respond to changes without manual coordination; continuous improvement driven by actual outcomes rather than planned initiatives; reduced firefighting as issues are addressed at earlier stages. |
| **Signals of Success** | Declining time-to-correction for detected issues; increasing percentage of corrections made without escalation; declining variance in key performance metrics; feedback mechanisms evolve based on effectiveness measurement. |
| **Anti-Patterns Prevented** | Metric Mirage, Cognitive Amnesia |
| **See Also** | [Friction Ontology](../../core-concepts/friction-ontology.md), [Modal Layer Architecture](../../core-concepts/modal-layer-architecture.md) |







## Related

- [Friction Ontology](../../core-concepts/friction-ontology.md) (Core Concept)
- [Modal Layer Architecture](../../core-concepts/modal-layer-architecture.md) (Core Concept)
- [Cognitive Amnesia](../anti-patterns/cognitive-amnesia.md) (Anti-Pattern)
- [Metric Mirage](../anti-patterns/metric-mirage.md) (Anti-Pattern)
