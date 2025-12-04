# Document Compliance Checklist

## Purpose

Comprehensive checklist for verifying governance document compliance with all applicable standards.

## Checklist

### UICH Compliance

- [ ] ✅ Valid UICH header present (use `uich-checklist.md` for detailed verification)
- [ ] ✅ All required UICH fields complete
- [ ] ✅ UICH values match specification

### Trademark Usage

- [ ] ✅ All references use "PortusSophia™" (with trademark symbol)
- [ ] ✅ No variations like "Portus Sophia", "portussophia", etc.
- [ ] ✅ Trademark appears at least once in document (preferably UICH)

### Naming Conventions

- [ ] ✅ File name follows conventions (UPPERCASE.md or lowercase-kebab.md)
- [ ] ✅ UICH `id` uses lowercase-kebab-case
- [ ] ✅ UICH `title` uses Title Case
- [ ] ✅ No spaces or special characters in file name (except hyphens, underscores)

### Path Conventions

- [ ] ✅ File located in appropriate directory
- [ ] ✅ Path follows standard structure
- [ ] ✅ No files in reserved locations without justification

### Content Scope

- [ ] ✅ Content is governance-related
- [ ] ✅ No canon or narrative material
- [ ] ✅ No WebKernel implementation code
- [ ] ✅ No public-facing promotional content
- [ ] ✅ Focus on standards, metadata, workflows, or compliance

### Tone and Style

- [ ] ✅ Neutral, technical tone
- [ ] ✅ Objective and factual content
- [ ] ✅ Clear and precise language
- [ ] ✅ No promotional or creative language
- [ ] ✅ Professional presentation

### Structure and Formatting

- [ ] ✅ Proper Markdown syntax
- [ ] ✅ Clear headings hierarchy
- [ ] ✅ Consistent formatting
- [ ] 💡 Code blocks properly formatted
- [ ] 💡 Lists properly structured
- [ ] 💡 Links properly formatted

### Content Quality

- [ ] ✅ Accurate information
- [ ] ✅ Clear and understandable
- [ ] ✅ Complete (no missing sections)
- [ ] ✅ Free of obvious errors
- [ ] 💡 Examples provided where helpful
- [ ] 💡 Cross-references to related documents

### Dependencies

- [ ] 💡 Referenced documents exist
- [ ] 💡 Dependencies are current and valid
- [ ] 💡 Links work correctly

### Version Control

- [ ] ✅ `created` date accurate
- [ ] ✅ `updated` date reflects last change
- [ ] ✅ `status` appropriate for document maturity
- [ ] 💡 Change history documented (if applicable)

## Document Type Specific

### For Specifications

- [ ] ✅ Complete technical details
- [ ] ✅ Clear format definitions
- [ ] ✅ Examples provided
- [ ] ✅ Validation rules defined

### For Standards

- [ ] ✅ Clear requirements
- [ ] ✅ Rationale provided
- [ ] ✅ Compliance criteria defined
- [ ] 💡 Best practices included

### For Workflows

- [ ] ✅ Process steps clearly defined
- [ ] ✅ Roles and responsibilities clear
- [ ] ✅ Prerequisites stated
- [ ] ✅ Outcomes defined

### For Templates

- [ ] ✅ Easy to copy and use
- [ ] ✅ Clear instructions
- [ ] ✅ Placeholders marked
- [ ] ✅ Examples provided

### For Guidelines

- [ ] ✅ Clear recommendations
- [ ] ✅ Rationale explained
- [ ] ✅ Examples provided
- [ ] 💡 Common pitfalls addressed

### For Compliance Documents

- [ ] ✅ Comprehensive coverage
- [ ] ✅ Clear criteria
- [ ] ✅ Easy to apply
- [ ] ✅ Actionable items

## Sealed Documents

If document has `status: sealed`:

- [ ] ✅ Changes discussed in issue first
- [ ] ✅ Impact assessment completed
- [ ] ✅ Migration plan (if needed)
- [ ] ✅ Governance team approval obtained

## Pre-Submission Verification

Before submitting pull request:

1. ✅ Complete this checklist
2. ✅ Complete UICH checklist
3. ✅ Self-review content
4. ✅ Test any code examples
5. ✅ Preview rendered Markdown
6. ✅ Check for typos and errors

## Post-Submission

After PR submission:

- [ ] Monitor for review feedback
- [ ] Address comments promptly
- [ ] Update checklist if needed
- [ ] Confirm final approval

## Non-Compliance

If unable to meet requirements:

1. Document specific issue
2. Explain why compliance not possible
3. Propose alternative or exception
4. Seek governance team input

## Reference Documents

- UICH Specification: `/standards/uich/SPECIFICATION.md`
- Naming Conventions: `/standards/naming/README.md`
- Path Conventions: `/standards/paths/README.md`
- Metadata Schema: `/standards/metadata/SCHEMA.md`
- Contributing Guidelines: `/CONTRIBUTING.md`
- Governance Scope: `/GOVERNANCE.md`
