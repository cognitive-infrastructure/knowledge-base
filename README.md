---
id: ci:kb.readme
author: "Rashid Azarang"
status: canonical
version: 1.0
summary: Introduction to the Cognitive Infrastructure Knowledge Base
---

# Cognitive Infrastructure Knowledge Base

<!-- migrated from knowledge-base repo on 2025-04 -->

This repository contains the core concepts, patterns, anti-patterns, essays, frameworks, diagnostics, and lexicon of the Cognitive Infrastructure project.

## Repository Structure

- `/core-concepts/` - Foundational ideas and concepts
- `/patterns-and-anti-patterns/` - Effective and ineffective patterns
- `/essays/` - Long-form explorations of ideas
- `/frameworks/` - Structured approaches to cognitive challenges
- `/diagnostics/` - Tools for diagnosing cognitive issues
- `/lexicon/` - Terminology and definitions
- `/meta/` - Meta-information about the knowledge base
- `/docs/` - Documentation, canonical sources, and source documents
  - `/docs/canonical-source-documents/` - Structured canonical source documents
  - `/docs/source-documents/` - Original source documents before canonicalization
  - `/docs/pending/` - Draft documents awaiting processing and integration
  - `/docs/scripts-guide.md` - Guide to using scripts and tools
  - `/docs/json-guide.md` - Guide to JSON file usage
  - `/docs/PRD-ci-coder.md` - Product Requirements Document for CI-Coder
- `/sources/` - Original source materials and contribution guidelines
  - `/sources/excerpts/` - Excerpts from source materials
  - `/sources/manuscripts/` - Original manuscripts
- `canonical-index.md` - Index of all canonical documents

## Related Repositories

- [meta-stack](../meta-stack) - Tools, schemas, and infrastructure for managing the knowledge base
- [agentic-systems](../agentic-systems) - Implementation blueprints, agent orchestration strategies, and modular software system patterns

## Core Concepts

Cognitive Infrastructure rests on a small set of first‑principles. Each concept below is a **source‑of‑truth definition**: short enough to read in one sitting, stable enough to cite, and versioned for evolution.

| Concept | One‑Line Essence |
|---------|------------------|
| Structure–Memory–Interaction (SMI) Triad | Usable intelligence = organisation + return + recursive refinement. |
| Modal Layer Architecture | Data → Logic → Interface → Orchestration → Feedback. Five separable, integ­ratable layers. |
| Clarity Laws | Empirical rules on how structure constrains capability. |
| Structural Debt | Hidden cost of mis‑aligned architecture; grows like interest. |
| Friction Ontology | Taxonomy of recurring clarity frictions. |
| Multi‑Axis Integration | Vertical, horizontal, end‑to‑end coherence across organisations. |
| Continuity–Disruption Balance | Safely evolving systems without breaking trust. |
| Universal Evolutionary Stages | 0–7 maturity ladder from fragmentation to integrated intelligence. |
| Role–Structure Coherence | Responsibility must match the scaffold that supports it. |
| Return‑as‑Intelligence | Revisiting understanding is itself a generative act. |
| Epistemophany | The moment when a system perceives the architecture shaping its understanding. |
| Coherence Debt | Cumulative deficit in shared meaning and interpretive trust. |
| Structural Receptivity | System's capacity to incorporate new knowledge without fragmentation. |
| Epistemic Substrate Theory | Foundational architecture determining possible forms of knowledge. |
| Semantic Friction | Resistance encountered when translating meaning across boundaries. |

## Patterns & Anti‑Patterns

Architecture lives in recurring shapes. *Patterns* capture designs that preserve clarity. *Anti‑patterns* (frictions) describe structures that erode it.

### Implementation Patterns

| Pattern | Purpose |
|---------|---------|
| Canonical IDs | Create stable, globally unique identifiers that transcend specific systems. |
| Closed-Loop Feedback | Design measurement systems that immediately inform adjustments. |
| Layered Modularity | Align system boundaries with Modal Layers for independent evolution. |
| Progressive Typing | Begin with flexible data structures that tighten as understanding grows. |
| Return Path Engineering | Design explicit routes back to previous knowledge and contexts. |
| Semantic Foundation | Establish unified definitions for consistent meaning across systems. |
| Single Source of Truth | Establish authoritative entity records from which all others derive. |
| Hero-Structure Inverse Correlation Law | Balance between individual heroism and structural maturity. |

### Anti-Patterns

| Anti‑Pattern | Symptom |
|--------------|---------|
| Ballup | Same friction resurfaces despite fixes. |
| Semantic Drift | Words mean different things in different teams. |
| Dashboard Theater | Beautiful visuals, zero trusted decisions. |
| Hero Syndrome | Operations rely on irreplaceable individuals. |
| Cognitive Amnesia | Org solves a problem, forgets, repeats. |
| Trigger Chaos | Automations behave unpredictably under change. |
| Metric Mirage | Metrics exist, but behaviour doesn't change. |
| Over‑Layering | Layers piled on without refactoring; brittle complexity. |
| Toolification | Adopting new tools instead of addressing architectural issues. |
| Metastable Intelligence | Systems appear functional until stress reveals fragilities. |

## Documentation

This repository contains comprehensive documentation on Cognitive Infrastructure concepts, patterns, and anti-patterns.

### Document Types

#### Canonical Library

The `/library/` folder contains the structured canon of the Cognitive Infrastructure knowledge base, including:

- `/library/core-concepts/`: foundational ideas and principles
- `/library/frameworks/`: structured models and systems
- `/library/patterns-and-anti-patterns/`: recurring structures of success or failure
- `/library/diagnostics/`: tools for system assessment and friction tracing
- `/library/essays/`: narrative and philosophical reflections on intelligence architecture
- `/library/lexicon/`: original terms and metaphors with epistemic significance

All contents in this folder follow canonical formatting, versioning, and bidirectional referencing standards.

#### Epistemological Source Documents

Epistemological source documents, located in `sources/`, provide research and external references rather than definitive concept descriptions. They explore the broader implications and connections of concepts within the field.

## The Publishing Workflow: From Draft to Truth

Cognitive Infrastructure follows a specific recursive publishing workflow that ensures content is structured, verified, and interconnected. This is not a "write once, forget" approach, but rather a continuous process of write, structure, validate, reuse, and evolve.

### How It Works

1. **You drop a new manuscript into `/sources`**
   - Place raw manuscripts in `/sources/manuscripts/`
   - Place PDF files in `/sources/raw-pdf/`
   - Create excerpts in `/sources/excerpts/`

2. **Run CI-Writer to auto-generate documentation**
   - CI-Writer scans for TODO markers in Markdown files
   - It finds relevant content from your manuscripts
   - It fills in TODOs with structured, consistent content
   ```bash
   node tools/ci-writer.js [--path specific-file-or-dir]
   ```

3. **Run CI-Coder to validate and maintain the repository**
   - Validates JSON files against schemas
   - Updates related sections across files
   - Fixes broken links and ensures consistency
   ```bash
   node tools/ci-coder.js validate
   node tools/ci-coder.js fix-links
   node scripts/update-related-sections.js
   ```

4. **Review and commit the changes**
   - Check the generated content for quality
   - Make any necessary manual adjustments
   - Commit the changes to the repository

5. **GitBook updates automatically with the new content**
   - CI/CD processes deploy the updated documentation
   - Users see the latest version with proper linking and structure

6. **Both AI models and humans benefit from the structure**
   - Machine-readable JSON enables AI integration
   - Human-readable Markdown provides clear documentation
   - The structural connections allow for deeper exploration

For detailed information about the tools and scripts available, see the [Scripts Guide](docs/scripts-guide.md).

## Getting Started

To explore the Cognitive Infrastructure framework:

1. Browse the [Core Concepts](canonical-index.md#diagnostic-concepts) to understand the foundational ideas
2. Examine the [Patterns](canonical-index.md#implementation-patterns) for practical implementation approaches
3. Learn to recognize [Anti-Patterns](canonical-index.md#anti-patterns) to avoid common pitfalls
4. Dive deep into the [Canonical Library](/library/README.md) for comprehensive understanding

### Contributing to Cognitive Infrastructure

Contributions to Cognitive Infrastructure are welcome. Please follow these steps:

1. **Set up your environment**
   ```bash
   # Install dependencies
   npm install
   
   # Set up OpenAI API key (required for CI-Writer and CI-Coder)
   export OPENAI_API_KEY=your_api_key_here
   ```

2. **Follow the publishing workflow**
   - Start by adding your content to the `/sources` directory
   - Use the tools to generate and validate documentation
   - Maintain consistent formatting and structure

3. **Validate before submitting**
   ```bash
   # Validate JSON files against schema
   npm run validate
   
   # Run linting checks
   npm run lint
   ```

4. **Submit your contribution**
   - Create a pull request with your changes
   - Ensure all validation checks pass
   - Provide context for your contribution

## License

MIT © Rashid Azarang 

## Meta Structure

This repository is self-documenting. For a recursive summary of its structure and evolution rules, see [`knowledge-base-summary.md`](./meta/knowledge-base-summary.md).

## Revision Log

- v1.0 (Apr 2025): Canonicalization pass to standardize frontmatter and formatting 