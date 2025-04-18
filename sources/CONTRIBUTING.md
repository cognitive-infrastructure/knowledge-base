# Contributing to the Source Library

This guide explains how to add and reference source materials in the Cognitive Infrastructure repository.

## Adding New Source Materials

### Step 1: Prepare Your Files

1. Convert your document to Markdown if possible
   - For books/papers, maintain the original structure with headers
   - Include proper attribution at the top of the file

2. Keep the original file (PDF, DOCX, etc.) for reference

### Step 2: Add Files to the Repository

1. Add Markdown version:
   ```bash
   # Use a descriptive filename with publication year
   cp your-document.md sources/manuscripts/cognitive-infrastructure-field-guide.md
   ```

2. Add original file using Git LFS:
   ```bash
   # Ensure Git LFS is installed and tracking PDFs
   git lfs install
   git lfs track "*.pdf"
   git add .gitattributes
   
   # Copy your PDF to the raw-pdf directory
   cp YourDocument.pdf sources/raw-pdf/FieldGuide.pdf
   git add sources/raw-pdf/FieldGuide.pdf
   ```

### Step 3: Register in Index

Add your document to `sources/index.yaml` with a logical ID:

```yaml
# Naming convention: SHORT_DESCRIPTIVE_NAME_YEAR
FIELD_GUIDE_2024: manuscripts/cognitive-infrastructure-field-guide.md
```

Guidelines for logical IDs:
- Use ALL_CAPS with underscores
- Include publication year
- Keep it concise but descriptive
- Once published, never change the ID

### Step 4: Create Excerpts (Optional but Recommended)

For documents you'll reference frequently:

1. Create a directory for your document:
   ```bash
   mkdir -p sources/excerpts/FIELD_GUIDE_2024
   ```

2. Split into topic-sized chunks (1-3 pages) with sequential numbers:
   ```
   sources/excerpts/FIELD_GUIDE_2024/001-introduction.md
   sources/excerpts/FIELD_GUIDE_2024/002-key-concepts.md
   ```

3. Add metadata to each excerpt:
   ```markdown
   ---
   source: FIELD_GUIDE_2024
   title: "Introduction to Cognitive Infrastructure"
   pages: "1-3"
   context: "Defines the field and its scope"
   ---

   # Introduction to Cognitive Infrastructure

   [excerpt content here]
   ```

## Citing Source Materials

### Basic Citation

In any Markdown file, cite sources using HTML comments:

```markdown
The Structure-Memory-Interaction triad forms the foundation of Cognitive Infrastructure <!--cite:FIELD_GUIDE_2024 p.15-->
```

### Extended Citation Format

For more specific references:

```markdown
<!--cite:FIELD_GUIDE_2024 section="Modal Layers" pages="42-45"-->
```

### Using with CI-Writer

When using CI-Writer, you can instruct it to incorporate specific excerpts:

```
@ci-writer Please explain Modal Layer Architecture based on <!--cite:FIELD_GUIDE_2024 section="Modal Layers"-->
```

## Citation Validation

Our CI pipeline automatically validates that:
1. All cited IDs exist in `index.yaml`
2. The referenced files exist in the repository
3. Citations follow the correct format

If you encounter validation errors, ensure your logical IDs match exactly what's in `index.yaml`. 