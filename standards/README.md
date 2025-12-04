# PortusSophia™ Standards

## Overview

This directory contains all governance standards for the PortusSophia™ project. Standards define required practices, formats, and conventions.

## Standard Categories

### UICH (Universal Informational Content Header)
Location: `/standards/uich/`

The UICH standard defines metadata headers for all governance documents. This is the foundational standard that ensures consistent identification and classification.

**Key Documents:**
- `SPECIFICATION.md` — Complete UICH format specification
- `TEMPLATE.md` — Ready-to-use UICH templates
- `README.md` — UICH overview and purpose

**Status:** Sealed (requires governance approval to modify)

### Metadata
Location: `/standards/metadata/`

Metadata standards define schema, validation rules, and extended metadata beyond UICH.

**Key Documents:**
- `SCHEMA.md` — Metadata schema definition
- `README.md` — Metadata overview

**Status:** Approved

### Paths
Location: `/standards/paths/`

Path conventions establish directory structures and file locations across repositories.

**Key Documents:**
- `README.md` — Path conventions and rules

**Status:** Approved

### Naming
Location: `/standards/naming/`

Naming conventions define formats for files, identifiers, directories, and other project elements.

**Key Documents:**
- `README.md` — Comprehensive naming standards

**Status:** Approved

## Standard Hierarchy

1. **UICH** — Foundation for all documents
2. **Metadata** — Extends UICH with additional schema
3. **Paths** — Governs location and structure
4. **Naming** — Governs identifiers and names

Standards should be applied in this order when creating new governance content.

## Using Standards

### For New Documents

1. Review applicable standards
2. Use UICH template from `/standards/uich/TEMPLATE.md`
3. Follow naming conventions for file and ID
4. Place in correct location per path conventions
5. Validate with compliance checklists

### For Existing Documents

1. Audit against current standards
2. Identify non-conformance
3. Plan remediation
4. Update incrementally
5. Document changes

## Standard Evolution

Standards evolve through governance process:

1. **Identify Need** — Gap, issue, or improvement opportunity
2. **Propose Change** — Open issue with detailed proposal
3. **Discuss** — Governance team and community review
4. **Approve** — Consensus reached
5. **Implement** — Update standards and migrate existing content
6. **Communicate** — Announce changes

See `/workflows/document-review.md` for detailed process.

## Sealed Standards

Some standards are marked as "sealed" indicating they are authoritative and stable. Changes to sealed standards require:

- Governance issue discussion before PR
- Impact assessment
- Migration plan for affected documents
- Governance team approval
- Extended review period

Current sealed standards:
- UICH Specification

## Compliance

All governance documents must comply with applicable standards. Use checklists in `/compliance/` to verify conformance.

## Questions

For questions about standards:
1. Check standard documentation
2. Review examples and templates
3. Search existing issues
4. Open new issue with tag `standard-question`
