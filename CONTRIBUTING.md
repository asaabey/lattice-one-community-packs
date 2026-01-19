# Contributing to Lattice Community Packs

Thank you for your interest in contributing! This document provides guidelines for submitting variable packs, screen packs, and bundles.

## Types of Contributions

### 1. New Variable Pack

A collection of related variable definitions (e.g., "Cardiac Labs", "Diabetes Management").

### 2. New Screen Pack

Form templates that use existing or new variables.

### 3. New Bundle

A complete package containing both variables and screens for a clinical workflow.

### 4. Improvements

Updates to existing packs: bug fixes, new variables, documentation improvements.

## Contribution Workflow

### Step 1: Check Existing Packs

Before creating a new pack, check if similar content already exists:

- Review the [catalog.json](./catalog.json)
- Search existing packs for overlapping variables
- Consider extending an existing pack instead of creating a new one

### Step 2: Create Your Pack

#### Directory Structure

```
your-pack-name/
├── pack.json           # Required: Pack metadata
├── bundle.json         # Required: FHIR Bundle
├── CHANGELOG.md        # Required: Version history
└── README.md           # Optional: Additional documentation
```

#### pack.json Requirements

```json
{
  "id": "your-pack-id",
  "name": "Human Readable Name",
  "version": "1.0.0",
  "description": "Clear description of what this pack contains",
  "author": "Your Name or Organization",
  "license": "CC-BY-4.0",
  "category": "labs|vitals|clinical|dialysis|transplant|demographics|admin",
  "tags": ["relevant", "searchable", "tags"],
  "latticeMinVersion": "1.0.0",
  "fhirVersion": "R4",
  "variableCount": 0,
  "screenCount": 0,
  "dependsOn": []
}
```

#### Variable ID Requirements

All variables MUST use canonical IDs:

| Code System | Format | Example |
|-------------|--------|---------|
| LOINC | `loinc-{code}` | `loinc-2160-0` |
| SNOMED CT | `snomed-{code}` | `snomed-44054006` |
| ICD-10 | `icd10-{code}` | `icd10-n18-3` |
| Local/Custom | `local-{descriptive-id}` | `local-dialysis-access-type` |

**Important**:
- Use lowercase for all IDs
- Replace special characters with hyphens
- Use established code systems (LOINC, SNOMED) when available
- Only use `local-` prefix for organization-specific variables

### Step 3: Validate Your Pack

Before submitting, validate your pack:

```bash
# Validate pack structure
npm run validate -- path/to/your-pack

# Or manually check:
# 1. pack.json matches schema
# 2. bundle.json is valid FHIR R4
# 3. All variable IDs follow canonical format
# 4. All referenced variables exist (for screens)
# 5. No duplicate IDs within the pack
```

### Step 4: Submit a Pull Request

1. Fork this repository
2. Create a branch: `git checkout -b add-your-pack-name`
3. Add your pack to the appropriate directory:
   - `/variables/your-pack-name/` for variable packs
   - `/screens/your-pack-name/` for screen packs
   - `/bundles/your-pack-name/` for combined bundles
4. Update `catalog.json` with your pack entry
5. Submit a pull request with:
   - Clear description of the pack contents
   - Clinical use case explanation
   - Any dependencies or prerequisites

## Quality Guidelines

### Variable Definitions

- **Use standard codes**: Prefer LOINC for labs, SNOMED for clinical concepts
- **Include validation**: Set appropriate min/max, normal ranges, critical values
- **Document units**: Always specify units using UCUM when applicable
- **Add help text**: Include user-friendly descriptions
- **Set categories**: Use consistent categorization

### Screen Definitions

- **Logical grouping**: Organize fields into meaningful sections
- **Appropriate layout**: Choose layout based on content (tabs for many sections, wizard for workflows)
- **Conditional logic**: Use showWhen/requiredWhen for dynamic behavior
- **Mobile-friendly**: Consider field widths for responsive display

### Documentation

- **CHANGELOG.md**: Document all changes with dates
- **Clear descriptions**: Explain clinical context and use cases
- **Dependencies**: List all required packs

## Code Review Criteria

Pull requests will be reviewed for:

1. **Correctness**: Valid FHIR resources, proper canonical IDs
2. **Completeness**: All required fields, proper documentation
3. **Consistency**: Follows existing patterns and naming conventions
4. **Clinical validity**: Appropriate codes, units, validation rules
5. **No duplicates**: Doesn't duplicate existing pack content

## Versioning

We use [Semantic Versioning](https://semver.org/):

- **MAJOR**: Breaking changes (removed variables, type changes)
- **MINOR**: New variables, non-breaking enhancements
- **PATCH**: Documentation, display text, bug fixes

When updating an existing pack:

1. Increment the version appropriately
2. Update CHANGELOG.md
3. Update catalog.json with new version

## Getting Help

- **Questions**: Open a [Discussion](https://github.com/your-org/lattice-community-packs/discussions)
- **Issues**: Report bugs via [Issues](https://github.com/your-org/lattice-community-packs/issues)
- **Slack**: Join #lattice-community on our Slack workspace

## License

By contributing, you agree that your contributions will be licensed under CC-BY-4.0 (or the license specified in your pack.json).
