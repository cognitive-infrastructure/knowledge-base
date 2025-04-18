---
title: "Citation Examples"
author: "Rashid Azarang"
date: 2025-04-18
draft: false
---

<!-- Migration Status: Complete -->

# Citation Examples

This document provides examples of how to cite source documents in your Markdown files.

## Basic Citation Format

Citations are created using HTML comments with a specific format:

```markdown
The concept of Modal Layer Architecture is fundamental to Cognitive Infrastructure <!--cite:FIELD_GUIDE_2024 p.12-->
```

When rendered, this appears as normal text without the comment visible:

The concept of Modal Layer Architecture is fundamental to Cognitive Infrastructure 

## Extended Citation Format

For more specific references, you can include additional metadata:

```markdown
<!--cite:INT_STACK_2024 section="Structural Debt" pages="42-45" context="Definition and impact"-->
```

## Citation with CI-Writer

When working with CI-Writer, you can direct it to specific sources:

```
@ci-writer Please explain the Structure-Memory-Interaction triad based on <!--cite:FIELD_GUIDE_2024 p.15-->
```

## Multiple Citations

You can include multiple citations in a document:

```markdown
Modal Layer Architecture <!--cite:FIELD_GUIDE_2024 p.22--> relates closely to the concept of Layered Modularity <!--cite:INT_STACK_2024 p.56-->
```

## Citation in Various Document Types

Citations work in all Markdown files:

### Core Concepts

```markdown
# Structure-Memory-Interaction Triad

## Definition

The Structure-Memory-Interaction (SMI) Triad is the foundational model of Cognitive Infrastructure <!--cite:FIELD_GUIDE_2024 p.8--> that describes how usable intelligence requires...
```

### Patterns

```markdown
# Layered Modularity

## Intent

To align system boundaries with Modal Layers, creating independent evolution paths <!--cite:INT_STACK_2024 p.103-->
```

### Anti-Patterns

```markdown
# Semantic Drift

## Symptoms

Teams gradually develop divergent interpretations of key terminology <!--cite:STRUCT_DIAG_2025 p.67--> resulting in coordination failures...
```

## Using with the Validation Tool

You can validate that all your citations reference valid source documents:

```bash
python tools/validate_citations.py sources/index.yaml $(git ls-files '*.md')
``` 