---
title: "Source Excerpts"
author: "Rashid Azarang"
date: 2025-04-18
draft: false
---

# Source Excerpts

<!-- migrated from knowledge-base repo on 2025-04 -->

This directory contains excerpts from various source materials that are relevant to the Cognitive Infrastructure knowledge base.

Excerpts are typically:
- Smaller, focused selections from larger works
- Formatted with proper citations
- Tagged with relevant concepts
- Organized by source and date

Excerpts serve as reference material for concept development and can be transformed into source documents or directly into canonical entries when appropriate.

## Organization

Excerpts are organized by logical ID, with each source having its own directory:

```
excerpts/
├── FIELD_GUIDE_2024/
│   ├── 001-introduction.md
│   ├── 002-key-concepts.md
│   └── ...
├── INT_STACK_2024/
│   ├── 001-executive-summary.md
│   └── ...
└── ...
```

## Excerpt Format

Each excerpt file should include metadata:

```markdown
---
source: LOGICAL_ID
title: "Section Title"
pages: "12-15"
context: "Brief description of what this excerpt covers"
---

# Section Title

[Excerpt content...]
```

## Purpose

These excerpts serve several key functions:

1. **LLM Context Management**: Allows CI-Writer to access only relevant portions of documents, preventing token bloat and reducing the risk of hallucinations
2. **Quick Reference**: Provides easy access to frequently cited sections
3. **Granular Citation**: Enables precise citation of specific ideas and concepts

## When to Create Excerpts

Create excerpts when:
- A section is frequently cited in documentation
- A concept spans multiple source documents and needs consolidation
- A document is too large for efficient processing

## Usage with CI-Writer

When using CI-Writer, you can reference specific excerpts:

```
@ci-writer Please explain Modal Layer Architecture based on excerpt INT_STACK_2024/003-modal-layers.md
``` 