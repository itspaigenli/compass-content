# compass-content

Content repository for Cohort Compass documentation and participant resources.

## Purpose

This repo stores source content separately from the application repo so Techtonica-related participant resources can live in a structured, version-controlled content repository that Cohort Compass can consume.

## Repository Structure

- `docs/resources/` - general resources, guides, references, and support content
- `docs/faq/` - question-and-answer content
- `docs/program/` - program-specific documentation such as handbooks, policies, and onboarding materials
- `docs/workflows/` - participant-facing process and contribution instructions
- `docs/_templates/` - reusable authoring templates
- `assets/` - images and other supporting files
- `source/` - original source documents preserved during conversion

## Content Rules

- Preserve original source material faithfully.
- Do not rewrite, summarize, or change meaning unless explicitly asked.
- Convert formatting into Markdown conservatively.
- Use clean, descriptive, kebab-case filenames.
- Add frontmatter to each document using the shared template.
- If source formatting is unclear, preserve content rather than “improving” it.

## Frontmatter Fields

Each Markdown document should include:

- `title`
- `section`
- `category`
- `topic`
- `tags`
- `featured`
- `source`
- `audience`
- `content_type`
- `status`
- `original_format`
- `related_sections`
- `search_terms`
- `summary`

## Workflow

1. Identify the source document to convert.
2. Create a descriptive Markdown filename in the appropriate folder.
3. Copy content faithfully into Markdown.
4. Fill in frontmatter conservatively from known source information.
5. Leave unknown values blank or clearly neutral rather than inventing content.

See [docs/_templates/content-template.md](/Users/nessali/Desktop/GitHub/compass-content/docs/_templates/content-template.md) for the reusable template.

## Source Preservation

Original files can be stored alongside converted content in:

- `source/program/`
- `source/faq/`
- `source/resources/`
- `source/workflows/`
- `source/curriculum/`
- `source/media/`
- `source/admin/`

This supports a markdown-first consumption model while preserving the original `.docx`, `.pptx`, and `.xlsx` materials during migration.
