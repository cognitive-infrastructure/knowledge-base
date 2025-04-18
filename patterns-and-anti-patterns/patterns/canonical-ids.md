---
id: ci:pattern.canonical-ids
status: canonical
version: 1.0
summary: Create stable, globally unique identifiers for entities and concepts that transcend specific systems
category: pattern
author: Rashid Azarang
canonicalDate: 2024-04-16
relatedConcepts: ["Dashboard Theater", "Semantic Drift", "Semantic Foundation", "Semantic Friction", "Single Source of Truth"]
---

<!-- Migration Status: Complete -->

# Canonical IDs

**Intent** Create stable, globally unique identifiers for entities and concepts that transcend specific systems.

| Section | Notes |
|---------|-------|
| **Context** | Multi-system environments, data integration requirements, entity disambiguation needs, long-lived digital records. |
| **Problem** | Entities are identified differently across systems, creating reconciliation challenges, potential duplicates, and an inability to track items across their lifecycle. |
| **Forces** | System-specific ID requirements, legacy identification schemes, performance considerations for lookups, governance complexity. |
| **Solution** | Implement a stable ID architecture with: 1) system-agnostic IDs managed in a central registry, 2) structured format with namespaces and entity types, 3) immutable assignment policy, and 4) bidirectional mappings to local system identifiers. Publish ID resolution services accessible across organizational boundaries. |
| **Resulting Context** | Reliable entity tracking across system boundaries; foundation for comprehensive entity timelines; reduced integration complexity; elimination of identity resolution as a recurring challenge. |
| **Signals of Success** | Decreasing entity resolution exceptions; stable references in long-running processes; elimination of "which customer is this?" type questions; ability to track entity state changes across system boundaries. |
| **Anti-Patterns Prevented** | Semantic Drift, Dashboard Theater |
| **See Also** | [Single Source of Truth](single-source-of-truth.md), [Semantic Foundation](semantic-foundation.md) |

## Related

- [Semantic Foundation](semantic-foundation.md) (Pattern)
- [Single Source of Truth](single-source-of-truth.md) (Pattern)
- [Dashboard Theater](../anti-patterns/dashboard-theater.md) (Anti-Pattern)
- [Semantic Drift](../anti-patterns/semantic-drift.md) (Anti-Pattern)

## Revision Log

- v1.0 (Apr 2025): Canonicalization pass to standardize frontmatter and formatting
