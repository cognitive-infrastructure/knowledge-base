# Source Library

This directory contains immutable source materials that form the foundation of the Cognitive Infrastructure knowledge base.

## Directory Structure

- `/manuscripts/` - Markdown versions of whitepapers, books, and articles for easy diffing and referencing
- `/raw-pdf/` - Original PDF versions of documents (tracked with Git LFS)
- `/excerpts/` - Chunked sections of manuscripts organized by logical ID for efficient LLM processing

## Citation System

All source materials are assigned a unique logical ID in `index.yaml`. These IDs should be used for citation throughout the repository using the following format:

```markdown
<!--cite:LOGICAL_ID p.15-->
```

## Guidelines

1. **Never modify** original source materials once committed
2. **Always register** new sources in `index.yaml` before citation
3. **Create excerpts** for frequently referenced sections
4. **Use Git LFS** for binary files like PDFs

## Contributing New Sources

1. Add your markdown version to `/manuscripts/`
2. Add the original file (if binary) to `/raw-pdf/`
3. Register a logical ID in `index.yaml`
4. Create excerpts as needed in `/excerpts/<LOGICAL_ID>/`
5. Reference in documentation using the citation format 