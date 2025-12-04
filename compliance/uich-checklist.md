# UICH Compliance Checklist

## Purpose

Verify that documents include valid UICH (Universal Informational Content Header) conforming to specification.

## Checklist

### Structure

- [ ] ✅ UICH header is at the beginning of the document
- [ ] ✅ UICH header uses YAML frontmatter (between `---` delimiters)
- [ ] ✅ UICH content is under `uich:` key
- [ ] ✅ YAML syntax is valid (no parsing errors)

### Required Fields - Presence

- [ ] ✅ `version` field present
- [ ] ✅ `id` field present
- [ ] ✅ `title` field present
- [ ] ✅ `type` field present
- [ ] ✅ `status` field present
- [ ] ✅ `created` field present
- [ ] ✅ `updated` field present
- [ ] ✅ `steward` field present
- [ ] ✅ `classification` field present
- [ ] ✅ `trademark` field present

### Required Fields - Format

- [ ] ✅ `version` is a string (e.g., "1.0")
- [ ] ✅ `id` uses lowercase-kebab-case format
- [ ] ✅ `id` contains only lowercase letters, numbers, and hyphens
- [ ] ✅ `title` is a human-readable string
- [ ] ✅ `type` is one of: specification, standard, template, workflow, compliance, guideline
- [ ] ✅ `status` is one of: draft, review, approved, sealed, deprecated, archived
- [ ] ✅ `created` follows ISO 8601 date format (YYYY-MM-DD)
- [ ] ✅ `updated` follows ISO 8601 date format (YYYY-MM-DD)
- [ ] ✅ `steward` identifies responsible party
- [ ] ✅ `classification` is one of: public, internal, restricted
- [ ] ✅ `trademark` is exactly "PortusSophia™" (with trademark symbol)

### Required Fields - Validity

- [ ] ✅ `id` is unique within repository
- [ ] ✅ `created` date is valid (not future date)
- [ ] ✅ `updated` date is valid (not future date)
- [ ] ✅ `updated` date is same or after `created` date
- [ ] ✅ `status` reflects actual document state

### Optional Fields (if present)

- [ ] 💡 `tags` is an array of strings
- [ ] 💡 `dependencies` is an array of valid document IDs
- [ ] 💡 `supersedes` is a valid document ID
- [ ] 💡 `notes` provides useful context

### Content Alignment

- [ ] ✅ Document content matches declared `type`
- [ ] ✅ Document adheres to declared `status`
- [ ] ✅ Document location matches `classification` (if restricted)
- [ ] 💡 Tags accurately describe content

## Verification Process

1. **Visual Inspection**
   - Check that UICH header exists at document start
   - Verify YAML structure is correct

2. **Field Validation**
   - Confirm all required fields present
   - Verify field values match allowed formats
   - Check dates are logical and valid

3. **Content Check**
   - Ensure UICH metadata aligns with document content
   - Verify trademark usage is correct
   - Confirm ID is unique

4. **Status Review**
   - Verify status matches document maturity
   - Check if sealed status requires special handling

## Common Issues

### Missing Fields
**Problem**: Required field not present
**Solution**: Add missing field using UICH template

### Invalid Format
**Problem**: Field value doesn't match specification
**Solution**: Correct to allowed format (see SPECIFICATION.md)

### Trademark Error
**Problem**: Trademark not "PortusSophia™"
**Solution**: Use exact format with ™ symbol

### Date Issues
**Problem**: Invalid or illogical dates
**Solution**: Use ISO 8601 format, ensure updated ≥ created

### Non-Unique ID
**Problem**: ID conflicts with existing document
**Solution**: Choose unique, descriptive ID

## Automated Validation

Consider using YAML validators and custom scripts to automate portions of this checklist. Manual review still recommended for semantic checks.

## Reference

See `/standards/uich/SPECIFICATION.md` for complete UICH specification.
