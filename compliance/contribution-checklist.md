# Contribution Checklist

## Purpose

Pre-submission checklist to ensure contributions meet governance standards before creating a pull request.

## Before You Start

- [ ] ✅ Contribution is governance-related (not canon, narrative, or implementation)
- [ ] ✅ Reviewed [GOVERNANCE.md](/GOVERNANCE.md) for repository scope
- [ ] ✅ Reviewed [CONTRIBUTING.md](/CONTRIBUTING.md) for guidelines
- [ ] ✅ Checked existing standards to avoid duplication
- [ ] ✅ Searched existing issues for related discussions

## Document Preparation

### UICH Header

- [ ] ✅ UICH header included at document start
- [ ] ✅ All required UICH fields present
- [ ] ✅ UICH values valid per specification
- [ ] ✅ Document ID unique within repository
- [ ] ✅ Dates in ISO 8601 format (YYYY-MM-DD)
- [ ] ✅ Status set to "draft" for new documents

**Tip:** Use templates from `/standards/uich/TEMPLATE.md`

### Naming and Paths

- [ ] ✅ File name follows conventions (UPPERCASE.md or lowercase-kebab.md)
- [ ] ✅ File placed in correct directory
- [ ] ✅ ID uses lowercase-kebab-case
- [ ] ✅ Title uses Title Case

**Reference:** 
- `/standards/naming/README.md`
- `/standards/paths/README.md`

### Trademark Usage

- [ ] ✅ All references use "PortusSophia™" (with ™ symbol)
- [ ] ✅ No trademark variations (Portus Sophia, portussophia, etc.)
- [ ] ✅ Trademark in UICH header

### Content Quality

- [ ] ✅ Content is governance-related only
- [ ] ✅ Neutral, technical tone (no promotional language)
- [ ] ✅ Clear and precise language
- [ ] ✅ Factual and objective
- [ ] ✅ Free of typos and grammar errors
- [ ] ✅ No canon, narrative, or WebKernel content

### Formatting

- [ ] ✅ Valid Markdown syntax
- [ ] ✅ Proper heading hierarchy
- [ ] ✅ Code blocks properly formatted
- [ ] ✅ Lists properly structured
- [ ] 💡 Links work correctly
- [ ] 💡 Examples clear and helpful

### Completeness

- [ ] ✅ Document is complete (no "TODO" sections)
- [ ] ✅ All necessary information included
- [ ] ✅ Cross-references added where needed
- [ ] 💡 Examples provided where helpful

## Validation

### Self-Review

- [ ] ✅ Read document start to finish
- [ ] ✅ Verified accuracy
- [ ] ✅ Checked for clarity
- [ ] ✅ Previewed rendered Markdown

### Compliance Verification

- [ ] ✅ Completed UICH checklist (`/compliance/uich-checklist.md`)
- [ ] ✅ Completed document checklist (`/compliance/document-checklist.md`)
- [ ] ✅ All required items satisfied
- [ ] 💡 Most recommended items addressed

### Testing

- [ ] ✅ YAML parses without errors
- [ ] ✅ Links navigate correctly
- [ ] ✅ Code examples valid (if applicable)
- [ ] 💡 Tested in Markdown preview

## Pull Request Preparation

### Branch and Commits

- [ ] ✅ Created feature branch (e.g., `feature/metadata-schema`)
- [ ] ✅ Commit messages clear and descriptive
- [ ] ✅ Changes focused on single purpose
- [ ] ✅ No unrelated changes included

### PR Description

- [ ] ✅ Clear title describing change
- [ ] ✅ Description explains purpose
- [ ] ✅ References related issues (if any)
- [ ] ✅ Notes any special considerations
- [ ] 💡 Includes testing or validation notes

## Special Cases

### Sealed Artifacts

If modifying document with `status: sealed`:

- [ ] ✅ Opened issue for discussion first
- [ ] ✅ Obtained preliminary feedback
- [ ] ✅ Prepared impact assessment
- [ ] ✅ Created migration plan (if breaking changes)
- [ ] ✅ Awaiting governance team approval

### Major Changes

For significant standard changes:

- [ ] ✅ Discussed in issue first
- [ ] ✅ Community feedback received
- [ ] ✅ Impact on existing documents assessed
- [ ] ✅ Migration strategy defined
- [ ] 💡 Example updates prepared

### Breaking Changes

If change breaks existing documents:

- [ ] ✅ Clearly marked as breaking
- [ ] ✅ Deprecation period defined
- [ ] ✅ Migration guide created
- [ ] ✅ Affected documents identified
- [ ] ✅ Communication plan prepared

## Final Check

Before submitting PR:

- [ ] ✅ All checklist items addressed
- [ ] ✅ Branch up to date with main
- [ ] ✅ No merge conflicts
- [ ] ✅ Ready for review
- [ ] ✅ Prepared to respond to feedback

## After Submission

- [ ] Monitor PR for review comments
- [ ] Respond to feedback promptly
- [ ] Make requested changes
- [ ] Update PR description if scope changes
- [ ] Thank reviewers for their time

## Non-Compliance

If unable to meet checklist requirements:

1. Document specific issues
2. Explain constraints or justification
3. Propose alternatives
4. Include in PR description
5. Request guidance from stewards

## Questions

If uncertain about any checklist item:

1. Review relevant standard documentation
2. Check examples in existing documents
3. Search for related issues
4. Ask in issue before submitting PR
5. Tag question with appropriate label

## Resources

- [GOVERNANCE.md](/GOVERNANCE.md) — Repository scope
- [CONTRIBUTING.md](/CONTRIBUTING.md) — Contribution guidelines
- [Standards](/standards/) — All standards documentation
- [UICH Templates](/standards/uich/TEMPLATE.md) — Document templates
- [UICH Checklist](/compliance/uich-checklist.md) — UICH validation
- [Document Checklist](/compliance/document-checklist.md) — Full document validation
- [Document Review Workflow](/workflows/document-review.md) — Review process

---

**Good luck with your contribution to PortusSophia™ Governance!**
