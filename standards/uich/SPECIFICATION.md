# UICH Specification

## Format

UICH headers are encoded in YAML frontmatter at the beginning of content files.

```yaml
---
uich:
  version: "1.0"
  id: "unique-identifier"
  title: "Document Title"
  type: "document-type"
  status: "status-value"
  created: "YYYY-MM-DD"
  updated: "YYYY-MM-DD"
  steward: "steward-identifier"
  classification: "classification-level"
  trademark: "PortusSophia™"
---
```

## Required Fields

### version
- **Type**: String
- **Format**: Semantic version (e.g., "1.0", "1.1")
- **Description**: UICH specification version
- **Required**: Yes

### id
- **Type**: String
- **Format**: Lowercase with hyphens (kebab-case)
- **Description**: Unique identifier for the document
- **Required**: Yes
- **Example**: `"uich-specification"`, `"metadata-schema-v1"`

### title
- **Type**: String
- **Description**: Human-readable document title
- **Required**: Yes

### type
- **Type**: String
- **Allowed Values**: 
  - `"specification"`
  - `"standard"`
  - `"template"`
  - `"workflow"`
  - `"compliance"`
  - `"guideline"`
- **Description**: Document classification
- **Required**: Yes

### status
- **Type**: String
- **Allowed Values**:
  - `"draft"` — Work in progress
  - `"review"` — Under review
  - `"approved"` — Approved for use
  - `"sealed"` — Authoritative, requires special approval to modify
  - `"deprecated"` — No longer recommended
  - `"archived"` — Historical reference only
- **Description**: Document lifecycle status
- **Required**: Yes

### created
- **Type**: String
- **Format**: ISO 8601 date (YYYY-MM-DD)
- **Description**: Initial creation date
- **Required**: Yes

### updated
- **Type**: String
- **Format**: ISO 8601 date (YYYY-MM-DD)
- **Description**: Last modification date
- **Required**: Yes

### steward
- **Type**: String
- **Description**: Individual or team responsible for maintenance
- **Required**: Yes
- **Example**: `"governance-team"`, `"@username"`

### classification
- **Type**: String
- **Allowed Values**:
  - `"public"` — Publicly available
  - `"internal"` — Internal use only
  - `"restricted"` — Limited access
- **Description**: Access control classification
- **Required**: Yes

### trademark
- **Type**: String
- **Fixed Value**: `"PortusSophia™"`
- **Description**: Project trademark assertion
- **Required**: Yes

## Optional Fields

### tags
- **Type**: Array of strings
- **Description**: Categorization keywords
- **Example**: `["metadata", "versioning", "compliance"]`

### dependencies
- **Type**: Array of strings
- **Description**: Related document IDs
- **Example**: `["uich-specification", "path-conventions"]`

### supersedes
- **Type**: String
- **Description**: ID of document this replaces
- **Example**: `"metadata-schema-v0"`

### notes
- **Type**: String
- **Description**: Additional context or remarks
- **Example**: `"Aligned with 2025 standards review"`

## Validation Rules

1. All required fields must be present
2. Field values must match allowed values (where specified)
3. Dates must be valid ISO 8601 format
4. IDs must be unique within the repository
5. Trademark field must exactly match `"PortusSophia™"`
6. Status must reflect current document state

## Examples

### Minimal UICH

```yaml
---
uich:
  version: "1.0"
  id: "example-document"
  title: "Example Document"
  type: "guideline"
  status: "draft"
  created: "2025-01-15"
  updated: "2025-01-15"
  steward: "governance-team"
  classification: "public"
  trademark: "PortusSophia™"
---
```

### Complete UICH

```yaml
---
uich:
  version: "1.0"
  id: "advanced-metadata-guide"
  title: "Advanced Metadata Guidelines"
  type: "guideline"
  status: "approved"
  created: "2025-01-10"
  updated: "2025-01-20"
  steward: "@metadata-lead"
  classification: "internal"
  trademark: "PortusSophia™"
  tags: ["metadata", "advanced", "best-practices"]
  dependencies: ["uich-specification", "metadata-schema"]
  notes: "Incorporates feedback from Q1 2025 review"
---
```

## Sealed Status

This specification has status: **sealed**

Modifications require approval through governance issue discussion before PR submission.
