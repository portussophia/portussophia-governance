# Metadata Schema

## Core Schema

The PortusSophia™ metadata schema is primarily defined through UICH (Universal Informational Content Header). See `/standards/uich/SPECIFICATION.md` for the complete schema definition.

## Extended Metadata

For specific artifact types, additional metadata fields may be defined:

### Document Metadata

Beyond UICH, documents may include:

```yaml
document:
  format: "markdown"
  encoding: "UTF-8"
  language: "en-US"
  wordCount: 1500
```

### Version Metadata

For versioned artifacts:

```yaml
version:
  major: 1
  minor: 0
  patch: 0
  prerelease: null
  build: null
```

### Relationship Metadata

For linked artifacts:

```yaml
relationships:
  requires: ["artifact-id-1", "artifact-id-2"]
  extends: "base-artifact-id"
  related: ["related-id-1", "related-id-2"]
```

## Schema Validation

All metadata must:

1. Conform to YAML syntax
2. Use defined field names
3. Provide required fields
4. Match allowed value sets
5. Maintain type consistency

## Schema Evolution

Metadata schema changes require:

1. Governance issue discussion
2. Impact assessment
3. Migration plan for existing artifacts
4. Version increment
5. Documentation update

## Sealed Status

Core UICH schema is **sealed**. Extended metadata schemas may be proposed through standard governance process.
