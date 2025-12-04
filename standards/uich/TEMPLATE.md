# UICH Templates

## Basic Template

Copy and paste this template at the beginning of new governance documents:

```yaml
---
uich:
  version: "1.0"
  id: "unique-document-id"
  title: "Document Title"
  type: "document-type"
  status: "draft"
  created: "YYYY-MM-DD"
  updated: "YYYY-MM-DD"
  steward: "your-name-or-team"
  classification: "public"
  trademark: "PortusSophia™"
---
```

## Template by Document Type

### Specification Document

```yaml
---
uich:
  version: "1.0"
  id: "spec-name"
  title: "Specification Name"
  type: "specification"
  status: "draft"
  created: "YYYY-MM-DD"
  updated: "YYYY-MM-DD"
  steward: "governance-team"
  classification: "public"
  trademark: "PortusSophia™"
  tags: ["specification", "technical"]
---
```

### Standard Document

```yaml
---
uich:
  version: "1.0"
  id: "standard-name"
  title: "Standard Name"
  type: "standard"
  status: "draft"
  created: "YYYY-MM-DD"
  updated: "YYYY-MM-DD"
  steward: "governance-team"
  classification: "public"
  trademark: "PortusSophia™"
  tags: ["standard"]
---
```

### Workflow Document

```yaml
---
uich:
  version: "1.0"
  id: "workflow-name"
  title: "Workflow Name"
  type: "workflow"
  status: "draft"
  created: "YYYY-MM-DD"
  updated: "YYYY-MM-DD"
  steward: "governance-team"
  classification: "internal"
  trademark: "PortusSophia™"
  tags: ["workflow", "process"]
---
```

### Compliance Document

```yaml
---
uich:
  version: "1.0"
  id: "compliance-item"
  title: "Compliance Item"
  type: "compliance"
  status: "approved"
  created: "YYYY-MM-DD"
  updated: "YYYY-MM-DD"
  steward: "governance-team"
  classification: "internal"
  trademark: "PortusSophia™"
  tags: ["compliance", "checklist"]
---
```

### Guideline Document

```yaml
---
uich:
  version: "1.0"
  id: "guideline-name"
  title: "Guideline Name"
  type: "guideline"
  status: "draft"
  created: "YYYY-MM-DD"
  updated: "YYYY-MM-DD"
  steward: "governance-team"
  classification: "public"
  trademark: "PortusSophia™"
  tags: ["guideline", "best-practices"]
---
```

### Template Document

```yaml
---
uich:
  version: "1.0"
  id: "template-name"
  title: "Template Name"
  type: "template"
  status: "approved"
  created: "YYYY-MM-DD"
  updated: "YYYY-MM-DD"
  steward: "governance-team"
  classification: "public"
  trademark: "PortusSophia™"
  tags: ["template"]
---
```

## Usage Instructions

1. **Copy** the appropriate template
2. **Replace** placeholder values:
   - `unique-document-id`: Descriptive kebab-case identifier
   - `Document Title`: Human-readable title
   - `YYYY-MM-DD`: Current date in ISO 8601 format
   - `your-name-or-team`: Your identifier or team name
3. **Adjust** optional fields (tags, classification) as needed
4. **Paste** at the very beginning of your document
5. **Validate** using compliance checklist

## Field Selection Guide

### type
Choose based on document purpose:
- `specification` — Technical format or protocol definition
- `standard` — Required practice or convention
- `template` — Reusable document structure
- `workflow` — Process or procedure
- `compliance` — Verification or audit document
- `guideline` — Recommended practice or advice

### status
Start with `draft`, progress through lifecycle:
- `draft` → `review` → `approved`
- `sealed` for authoritative documents
- `deprecated` for phased-out content
- `archived` for historical reference

### classification
- `public` — Can be shared externally
- `internal` — PortusSophia™ team only
- `restricted` — Limited access required

## Validation

After adding UICH, verify:
- All required fields present
- Values match allowed options
- Dates are valid ISO 8601
- Trademark is exactly `PortusSophia™`
- ID is unique and kebab-case

Use `/compliance/uich-checklist.md` for detailed validation.
