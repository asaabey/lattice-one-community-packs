# Lattice Community Packs

A repository of shareable variable definitions, screen templates, and clinical form bundles for [Lattice One](https://github.com/your-org/lattice-one).

## What are Packs?

Packs are portable collections of clinical data definitions that can be imported into any Lattice One installation:

| Pack Type | Description | Location |
|-----------|-------------|----------|
| **Variable Packs** | Reusable field definitions (labs, vitals, clinical data) | `/variables/` |
| **Screen Packs** | Form templates that reference variables | `/screens/` |
| **Bundles** | Complete packages with variables + screens | `/bundles/` |

## Quick Start

### Browse Available Packs

See the [catalog.json](./catalog.json) for a complete list of available packs.

### Install a Pack

In Lattice One Design Studio:

1. Go to **Design Studio** > **Variables** (or **Screens**)
2. Click **Import Pack**
3. Select from the catalog or upload a pack file
4. Review and confirm the import

### Using the CLI (Coming Soon)

```bash
# Install a variable pack
lattice pack install core-labs-renal

# Install a screen pack
lattice pack install ckd-assessment

# List installed packs
lattice pack list
```

## Available Packs

### Variable Packs

| Pack | Version | Variables | Description |
|------|---------|-----------|-------------|
| `core-demographics` | 1.0.0 | 15 | Patient demographic fields |
| `core-vitals` | 1.0.0 | 10 | Standard vital signs |
| `core-labs-renal` | 1.0.0 | 20 | Renal function laboratory tests |
| `core-labs-hematology` | 1.0.0 | 15 | CBC and related tests |
| `ckd-staging` | 1.0.0 | 8 | CKD stage and risk classification |
| `dialysis-hd` | 1.0.0 | 25 | Hemodialysis session variables |
| `dialysis-pd` | 1.0.0 | 20 | Peritoneal dialysis variables |

### Screen Packs

| Pack | Version | Screens | Description |
|------|---------|---------|-------------|
| `ckd-assessment` | 1.0.0 | 1 | Comprehensive CKD evaluation form |
| `dialysis-session` | 1.0.0 | 1 | Hemodialysis session documentation |
| `transplant-workup` | 1.0.0 | 3 | Transplant evaluation forms |

## Pack Structure

Each pack follows this structure:

```
pack-name/
├── pack.json           # Metadata (name, version, dependencies)
├── bundle.json         # FHIR Bundle containing the resources
└── CHANGELOG.md        # Version history
```

### pack.json

```json
{
  "id": "core-labs-renal",
  "name": "Renal Laboratory Variables",
  "version": "1.0.0",
  "description": "Standard laboratory variables for renal function monitoring",
  "author": "Lattice Health Foundation",
  "license": "CC-BY-4.0",
  "category": "labs",
  "tags": ["renal", "laboratory", "ckd", "nephrology"],
  "latticeMinVersion": "1.0.0",
  "fhirVersion": "R4",
  "variableCount": 20,
  "dependsOn": []
}
```

### bundle.json

A standard FHIR R4 Bundle containing the variable or screen definitions. See [schemas/](./schemas/) for the complete specification.

## Contributing

We welcome contributions! See [CONTRIBUTING.md](./CONTRIBUTING.md) for guidelines.

### Ways to Contribute

- **Submit a new pack** - Share your variable definitions or screens
- **Improve existing packs** - Fix issues, add variables, update documentation
- **Report issues** - Found a problem? Open an issue
- **Request packs** - Need a specific clinical domain? Request it

## Canonical Variable IDs

All variables use canonical IDs based on their code system:

| Code System | Prefix | Example |
|-------------|--------|---------|
| LOINC | `loinc-` | `loinc-2160-0` (Serum Creatinine) |
| SNOMED CT | `snomed-` | `snomed-44054006` (Type 2 Diabetes) |
| ICD-10 | `icd10-` | `icd10-n18-3` (CKD Stage 3) |
| Local | `local-` | `local-dialysis-access-type` |

This ensures the same variable has the same ID across all Lattice installations.

## License

Content in this repository is licensed under [CC-BY-4.0](./LICENSE) unless otherwise specified in individual pack metadata.

## Related Projects

- [Lattice One](https://github.com/your-org/lattice-one) - The main Lattice One application
- [Lattice Documentation](https://docs.lattice.one) - Full documentation

## Contact

- **Issues**: [GitHub Issues](https://github.com/your-org/lattice-community-packs/issues)
- **Discussions**: [GitHub Discussions](https://github.com/your-org/lattice-community-packs/discussions)
