# Changelog

All notable changes to the `lab-entry-liver` screen pack will be documented in this file.

## [1.0.0] - 2024-01-19

### Added
- Initial release

#### Screen: Liver Function Panel

**Specimen Information**
- Collection date (required)
- Lab reference number

**Hepatocellular Enzymes**
- AST/SGOT (U/L)
- ALT/SGPT (U/L)

**Cholestatic Markers**
- Alkaline Phosphatase (U/L)
- GGT/Gamma-GT (U/L)
- 5'-Nucleotidase (U/L)

**Bilirubin**
- Total Bilirubin (mg/dL)
- Direct/Conjugated Bilirubin (mg/dL)
- Indirect/Unconjugated Bilirubin (mg/dL)

**Synthetic Function**
- Albumin (g/dL)
- Total Protein (g/dL)
- Globulin (g/dL)
- PT (seconds)

**Metabolic Markers**
- Ammonia (umol/L)
- LDH (U/L)

**Viral Hepatitis Serology**
- Hepatitis B Surface Antigen (HBsAg) - Positive/Negative
- Hepatitis B Surface Antibody (Anti-HBs) - Positive/Negative
- Hepatitis C Antibody (Anti-HCV) - Positive/Negative
- Hepatitis A IgM Antibody - Positive/Negative

**Lab Notes**
- Free text notes field

### Dependencies
- Requires `core-labs-liver` variable pack

### Notes
- AST:ALT ratio helps differentiate alcoholic vs non-alcoholic liver disease
- 5'-Nucleotidase helps confirm hepatic origin of elevated ALP
- Viral serology included for hepatitis screening
- PT reflects synthetic function (coagulation factor production)
