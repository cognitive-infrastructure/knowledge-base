# Pending Documents Directory

This directory serves as the staging area for new documents awaiting processing through the Pending Ingestion Protocol.

## Purpose

The `/docs/pending/` directory is designed as a single entry point for adding new content to the Cognitive Infrastructure knowledge base. Documents placed here will be automatically:

1. Classified by type (concept, pattern, anti-pattern, etc.)
2. Routed to the appropriate destination
3. Transformed to follow canonical structure
4. Published to the main repository structure

## How to Use

### 1. Add Draft Documents

Place your Markdown (`.md`) files in this directory. Each draft should include:

**Required:**
- A descriptive filename
- A clear title (H1)
- Basic content outlining the concept/pattern

**Optional:**
- Frontmatter with preliminary metadata
- TODO markers for sections requiring AI-assisted completion
- References to related concepts

### 2. Process Pending Documents

To process the documents in this directory, run:

```bash
node tools/ci-coder.js process-pending
```

This will:
- Analyze and classify each document
- Apply canonical structure and formatting
- Generate corresponding JSON files
- Move documents to their appropriate locations
- Remove the original files from the pending directory
- Update the knowledge base summary

### 3. Review Results

After processing, review the transformed documents in their new locations and make any necessary adjustments.

## Additional Notes

- Documents will be auto-classified based on content keywords, but you can include explicit type markers (e.g., "Pattern:", "Anti-Pattern:", "Concept:") in the title or content to ensure correct classification.
- Use the `--keep-original` flag with the `process-pending` command to keep copies of the original files in this directory.
- TODOs in your documents will not be processed automatically during routing - use `node tools/ci-writer.js --path docs/pending` first if you want to generate content from TODOs. 