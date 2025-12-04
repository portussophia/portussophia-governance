# Path Conventions

## Overview

Path conventions establish consistent directory structures and file locations across PortusSophia™ repositories.

## Purpose

Standardized paths provide:

- Predictable file organization
- Easier navigation and discovery
- Automated tooling support
- Clear separation of concerns
- Consistent repository structure

## Governance Repository Structure

```
portussophia-governance/
├── standards/          # Standard definitions
│   ├── uich/          # UICH specifications
│   ├── metadata/      # Metadata schemas
│   ├── paths/         # Path conventions
│   └── naming/        # Naming standards
├── workflows/         # Stewardship workflows
├── compliance/        # Compliance artifacts
├── GOVERNANCE.md      # Repository scope
├── CONTRIBUTING.md    # Contribution guidelines
└── README.md         # Repository overview
```

## Standard Directory Names

Use these names consistently:

- `standards/` — Standards and specifications
- `workflows/` — Process definitions
- `compliance/` — Compliance checklists and audits
- `templates/` — Reusable templates (if needed)
- `docs/` — Additional documentation (if needed)

## File Location Rules

### Specifications
Place in appropriate `standards/` subdirectory based on topic

### Workflows
Place in `workflows/` directory

### Compliance Artifacts
Place in `compliance/` directory

### Templates
Place in relevant `standards/` subdirectory or `templates/` if cross-cutting

## Path Naming

- Use lowercase for directories
- Use kebab-case for multi-word names
- Use descriptive, clear names
- Avoid abbreviations unless standard
- Keep paths reasonably short

## Examples

✅ Good:
- `/standards/uich/SPECIFICATION.md`
- `/workflows/governance-review.md`
- `/compliance/uich-checklist.md`

❌ Avoid:
- `/specs/UICH_SPEC.md` (non-standard location/name)
- `/WorkFlows/Gov-Review.md` (inconsistent case)
- `/c/uc.md` (unclear abbreviations)

## Reserved Paths

These paths have specific purposes:

- `/standards/` — Standards only, no implementation
- `/workflows/` — Process documents only
- `/compliance/` — Compliance artifacts only
- Root level — High-level governance documents only

Do not place other content types in these locations.

## Path Stability

Once established, paths should remain stable. Path changes require:

1. Governance discussion
2. Redirect or migration plan
3. Documentation updates
4. Link updates across repository
