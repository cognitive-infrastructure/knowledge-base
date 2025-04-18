---
id: ci:meta.library-patterns-antipatterns
status: canonical
version: 1.0
summary: Collection of implementation patterns that preserve clarity and anti-patterns that erode it in cognitive systems
---

# Patterns & Anti‑Patterns

Architecture lives in recurring shapes.  
*Patterns* capture designs that preserve clarity. *Anti‑patterns* (frictions) describe structures that erode it.

## Using This Library
1. Diagnose your system → identify a pattern or anti‑pattern.  
2. Follow the "Forces → Remedies" table to decide interventions.  
3. Contribute improvements via pull‑request (see `CONTRIBUTING.md`).

### Implementation Patterns

| Pattern | Intent |
|---------|--------|
| **[Semantic Foundation](patterns/semantic-foundation.md)** | Establish shared definitions before automation. |
| **[Layered Modularity](patterns/layered-modularity.md)** | Separate concerns along Modal Layers. |
| **[Single Source of Truth (SSoT)](patterns/single-source-of-truth.md)** | Authoritative entity records; everything else derives. |
| **[Closed‑Loop Feedback](patterns/closed-loop-feedback.md)** | Measurements that immediately inform adjustments. |
| **[Canonical IDs](patterns/canonical-ids.md)** | Stable, global identifiers for entities and concepts. |
| **[Progressive Typing](patterns/progressive-typing.md)** | Start loose, tighten types as understanding grows. |
| **[Return Path Engineering](patterns/return-path-engineering.md)** | Design explicit routes back to prior knowledge. |
| **[Hero-Structure Inverse Correlation Law](patterns/hero-structure-inverse-correlation.md)** | Balance between individual heroism and structural maturity. |

### Anti‑Patterns

| Anti‑Pattern | Symptom |
|--------------|---------|
| **[Ballup](anti-patterns/ballup.md)** | Same friction resurfaces despite fixes. |
| **[Semantic Drift](anti-patterns/semantic-drift.md)** | Words mean different things in different teams. |
| **[Dashboard Theater](anti-patterns/dashboard-theater.md)** | Beautiful visuals, zero trusted decisions. |
| **[Hero Syndrome](anti-patterns/hero-syndrome.md)** | Operations rely on irreplaceable individuals. |
| **[Cognitive Amnesia](anti-patterns/cognitive-amnesia.md)** | Org solves a problem, forgets, repeats. |
| **[Trigger Chaos](anti-patterns/trigger-chaos.md)** | Automations behave unpredictably under change. |
| **[Metric Mirage](anti-patterns/metric-mirage.md)** | Metrics exist, but behaviour doesn't change. |
| **[Over‑Layering](anti-patterns/over-layering.md)** | Layers piled on without refactoring; brittle complexity. |
| **[Toolification](anti-patterns/toolification.md)** | Adopting new tools instead of addressing architectural issues. |
| **[Metastable Intelligence](anti-patterns/metastable-intelligence.md)** | Systems appear functional until stress reveals fragilities. |

> 🔗 Every pattern file ends with "See also" links to clarify relationships and avoid semantic drift inside the library itself.

## Pattern Structure

Each pattern and anti-pattern document follows a consistent structure:

### Pattern Files Format

```
START_DEFINITION
<50-100 words canonical definition>
END_DEFINITION

## Intent
<The primary purpose this pattern serves>

## Context
<When and where this pattern is applicable>

## Forces
<The competing concerns that make this pattern necessary>

## Solution
<The specific architectural approach>

## Implementation
<Practical steps for applying the pattern>

## Consequences
<Benefits and tradeoffs>

## Examples
<Real-world examples>

## Related Patterns
<Links to related patterns>
```

### Anti-Pattern Files Format

```
START_DEFINITION
<50-100 words canonical definition>
END_DEFINITION

## Symptoms
<Observable signs this anti-pattern is present>

## Causes
<Common reasons this anti-pattern emerges>

## Forces
<The competing concerns that create this anti-pattern>

## Consequences
<Negative impacts on systems and organizations>

## Remedies
<Specific interventions to address the anti-pattern>

## Examples
<Real-world examples>

## Related Anti-Patterns
<Links to related anti-patterns>
```

## Diagnostic Frameworks

The patterns and anti-patterns in this library can be used with the following diagnostic frameworks:

1. **Structural Debt Assessment**: Identify accumulated architectural misalignments using anti-patterns as indicators.
2. **Modal Layer Analysis**: Evaluate pattern implementation across the five layers (Data, Logic, Interface, Orchestration, Feedback).
3. **Semantic Coherence Check**: Measure the consistency of terminology and definitions across teams.
4. **Return Path Audit**: Assess how effectively systems can revisit and refine previous understanding.

## Evolutionary Context

Patterns and anti-patterns exist within the context of [Universal Evolutionary Stages](../core-concepts/universal-evolutionary-stages.md):

- **Stages 0-2**: Focus on implementing foundational patterns like Semantic Foundation and Canonical IDs
- **Stages 3-4**: Address anti-patterns like Hero Syndrome and Cognitive Amnesia
- **Stages 5-7**: Apply advanced patterns like Layered Modularity and Return Path Engineering

## Revision Log

- v1.0 (Apr 2025): Canonicalization pass to standardize frontmatter and formatting 