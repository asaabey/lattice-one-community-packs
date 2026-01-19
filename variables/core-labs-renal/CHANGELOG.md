# Changelog

All notable changes to the `core-labs-renal` pack will be documented in this file.

## [1.0.0] - 2024-01-19

### Added
- Initial release

#### Kidney Function Markers
- `loinc-2160-0` - Serum Creatinine (mg/dL)
- `loinc-48642-3` - eGFR Non-Black (CKD-EPI)
- `loinc-48643-1` - eGFR Black (deprecated, included for legacy data)
- `loinc-62238-1` - eGFR CKD-EPI 2021 (race-free, recommended)
- `loinc-3094-0` - BUN (mg/dL)
- `loinc-6299-2` - BUN/Creatinine Ratio
- `loinc-82810-3` - Cystatin C (mg/L)

#### Electrolytes
- `loinc-2951-2` - Sodium (mmol/L)
- `loinc-2823-3` - Potassium (mmol/L)
- `loinc-2075-0` - Chloride (mmol/L)
- `loinc-1963-8` - Bicarbonate/CO2 (mmol/L)

#### Minerals (CKD-MBD)
- `loinc-17861-6` - Calcium Total (mg/dL)
- `loinc-2777-1` - Phosphorus (mg/dL)
- `loinc-2601-3` - Magnesium (mg/dL)

#### Proteins
- `loinc-1751-7` - Albumin Serum (g/dL)
- `loinc-1920-8` - AST/SGOT (U/L)

#### Urinalysis
- `loinc-2965-2` - Urine Specific Gravity
- `loinc-14959-1` - Urine Albumin/Creatinine Ratio (UACR) - key CKD marker
- `loinc-13705-9` - Urine Albumin 24hr
- `loinc-9318-7` - Urine Albumin Random
- `loinc-32294-1` - Urine Protein/Creatinine Ratio (UPCR)
- `loinc-14958-3` - Urine Microalbumin Random
- `loinc-2889-4` - Urine Protein 24hr
- `loinc-3097-3` - Urine Creatinine Random

### Notes
- All variables use standard LOINC codes
- Normal ranges based on standard clinical references
- Critical values included for life-threatening abnormalities
- eGFR: CKD-EPI 2021 race-free equation (`loinc-62238-1`) is recommended
- UACR categories: Normal <30, Microalbuminuria 30-300, Macroalbuminuria >300 mg/g
- UCUM units used throughout for interoperability
