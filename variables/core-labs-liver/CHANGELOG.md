# Changelog

All notable changes to the `core-labs-liver` pack will be documented in this file.

## [1.0.0] - 2024-01-19

### Added
- Initial release

#### Hepatocellular Enzymes
- `loinc-1920-8` - AST/SGOT (U/L)
- `loinc-1742-6` - ALT/SGPT (U/L)

#### Cholestatic Markers
- `loinc-6768-6` - Alkaline Phosphatase (U/L)
- `loinc-2324-2` - GGT/Gamma-GT (U/L)
- `loinc-1825-2` - 5'-Nucleotidase (U/L)

#### Bilirubin Fractions
- `loinc-1975-2` - Total Bilirubin (mg/dL)
- `loinc-1968-7` - Direct/Conjugated Bilirubin (mg/dL)
- `loinc-1971-1` - Indirect/Unconjugated Bilirubin (mg/dL)

#### Synthetic Function
- `loinc-1751-7` - Albumin Serum (g/dL)
- `loinc-2885-2` - Total Protein Serum (g/dL)
- `loinc-10834-0` - Globulin Serum (g/dL)
- `loinc-5905-5` - PT (seconds)

#### Metabolic Markers
- `loinc-1841-9` - Ammonia Plasma (umol/L)
- `loinc-2532-0` - LDH (U/L)

#### Viral Hepatitis Serology
- `loinc-16935-9` - Hepatitis B Surface Antigen (HBsAg)
- `loinc-5196-1` - Hepatitis B Surface Antibody (Anti-HBs)
- `loinc-5195-3` - Hepatitis C Antibody (Anti-HCV)
- `loinc-22664-7` - Hepatitis A IgM Antibody

### Notes
- All variables use standard LOINC codes
- Normal ranges based on standard clinical references
- Critical values included for life-threatening abnormalities
- AST:ALT ratio can help differentiate alcoholic vs non-alcoholic liver disease
- Viral serology tests included for hepatitis screening
- UCUM units used throughout for interoperability
