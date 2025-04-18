---
id: ci:antipattern.ballup
status: canonical
version: 1.0
summary: Chronic recurring issues that repeatedly resurface despite attempted fixes due to inadequate structural solutions
category: antipattern
author: Rashid Azarang
canonicalDate: 2024-04-16
---

# Ballup

"No matter how many times we fix it, this problem keeps coming back."

| Section | Notes |
|---------|-------|
| **Symptoms** | Teams repeatedly solve the same issue every few months; fixes don't stick; chronic "priority interruptions" for predictable failures; escalating workaround complexity. |
| **Root Cause** | Current architectural structure cannot adequately hold the complexity pushing on it; attempted fixes address symptoms while ignoring structural pressures. |
| **Impact** | Chronic firefighting culture; morale erosion as problems recur; escalating maintenance costs; increasing technical and structural debt; opportunity cost as innovation capacity diverts to recurring issues. |
| **Structural Cure** | Conduct Modal Layer diagnosis to identify which layer is under pressure. Re-evaluate architectural balance and implement appropriate patterns (e.g., Layered Modularity, Semantic Foundation). Refactor rather than patch the affected subsystem. |
| **Quick Fixes (Stop-Gaps)** | Document workarounds as explicit playbooks to reduce handling time. Add monitoring specifically for early detection of recurring pattern. Create designated handling team to protect wider organization while restructuring occurs. |
| **Related Frictions** | Over-Layering, Trigger Chaos |

## Related

- [Structural Debt](../../core-concepts/structural-debt.md) (Core Concept)
- [Layered Modularity](../patterns/layered-modularity.md) (Pattern)
- [Semantic Foundation](../patterns/semantic-foundation.md) (Pattern)
- [Trigger Chaos](trigger-chaos.md) (Anti-Pattern)

## Revision Log

- v1.0 (Apr 2025): Canonicalization pass to standardize frontmatter and formatting
