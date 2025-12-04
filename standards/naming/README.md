# Naming Conventions

## Overview

Naming conventions establish consistent identifier formats for files, documents, artifacts, and other PortusSophia™ project elements.

## Purpose

Standardized naming enables:

- Clear, unambiguous identification
- Predictable file and resource location
- Automated processing and tooling
- Consistent cross-reference patterns
- Professional, organized appearance

## File Naming

### Markdown Documents

Use `UPPERCASE.md` for major documents:
- `README.md`
- `CONTRIBUTING.md`
- `GOVERNANCE.md`
- `SPECIFICATION.md`
- `TEMPLATE.md`

Use `lowercase-kebab.md` for content documents:
- `metadata-schema.md`
- `path-conventions.md`
- `workflow-guide.md`

### YAML/JSON Files

Use `lowercase-kebab` format:
- `config.yaml`
- `metadata-schema.json`
- `validation-rules.yaml`

## Identifier Naming

### UICH IDs

Format: `lowercase-kebab-case`

Rules:
- Use descriptive names
- Separate words with hyphens
- No special characters except hyphens
- Keep reasonably concise
- Reflect content purpose

Examples:
- `uich-specification`
- `metadata-schema-v1`
- `governance-workflow`
- `compliance-checklist`

### Document Titles

Format: `Title Case with Spaces`

Rules:
- Capitalize major words
- Use natural language spacing
- Be descriptive and clear
- Match document purpose

Examples:
- "UICH Specification"
- "Metadata Schema"
- "Governance Workflow Guide"
- "Compliance Checklist"

## Directory Naming

Format: `lowercase` or `lowercase-with-hyphens`

Rules:
- Use single words when possible
- Use hyphens for multi-word names
- Be descriptive but concise
- Use standard terms

Examples:
- `standards`
- `workflows`
- `compliance`
- `uich` (abbreviation accepted as standard)

## Version Naming

Use semantic versioning where applicable:

Format: `vMAJOR.MINOR.PATCH`

Examples:
- `v1.0.0`
- `v2.1.0`
- `v1.0.0-beta`

For document versions in IDs:
- `schema-v1`
- `standard-v2`
- `template-v1`

## Tag Naming

For metadata tags, use:

Format: `lowercase-kebab-case`

Rules:
- Use common, searchable terms
- Avoid redundancy
- Be specific when needed
- Use plural for categories

Examples:
- `metadata`
- `compliance`
- `best-practices`
- `templates`

## Branch Naming (Git)

For governance work:

Format: `category/short-description`

Categories:
- `feature/` — New standards or workflows
- `fix/` — Corrections to existing content
- `docs/` — Documentation updates
- `refactor/` — Reorganization without content changes

Examples:
- `feature/metadata-schema`
- `fix/uich-template-typo`
- `docs/clarify-path-conventions`

## Trademark Naming

Always use: **PortusSophia™**

Never use:
- Portus Sophia
- PortusSophia (without ™)
- portussophia
- PORTUSSOPHIA
- PS or P.S.

## Prohibited Patterns

❌ Do not use:
- CamelCase for files (except established patterns)
- snake_case for files (use kebab-case)
- Spaces in file names
- Special characters in identifiers
- Non-descriptive names (e.g., `doc1.md`, `temp.yaml`)
- Version numbers in file names (use metadata instead)

## Naming Changes

Renaming established identifiers requires:

1. Governance discussion
2. Impact assessment
3. Redirect or alias plan
4. Documentation updates
5. Reference updates

Avoid renaming sealed artifacts.
