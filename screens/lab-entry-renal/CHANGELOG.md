# Changelog

All notable changes to the `lab-entry-renal` screen pack will be documented in this file.

## [1.0.0] - 2024-01-19

### Added
- Initial release

#### Screen: Renal Function Panel

**Specimen Information**
- Collection date (required)
- Lab reference number

**Kidney Function Markers**
- Serum Creatinine (mg/dL)
- eGFR CKD-EPI 2021 (mL/min/1.73m²) - race-free equation
- BUN (mg/dL)
- BUN/Creatinine Ratio
- Cystatin C (mg/L)

**Electrolytes**
- Sodium (mmol/L)
- Potassium (mmol/L)
- Chloride (mmol/L)
- Bicarbonate/CO2 (mmol/L)

**Minerals (CKD-MBD)**
- Calcium Total (mg/dL)
- Phosphorus (mg/dL)
- Magnesium (mg/dL)

**Proteins**
- Albumin Serum (g/dL)

**Urinalysis**
- Urine Specific Gravity
- UACR - Urine Albumin/Creatinine Ratio (mg/g)
- UPCR - Urine Protein/Creatinine Ratio (mg/g)
- Urine Albumin Random (mg/L)
- Urine Microalbumin Random (mg/L)
- Urine Creatinine Random (mg/dL)

**Lab Notes**
- Free text notes field

### Dependencies
- Requires `core-labs-renal` variable pack

### Notes
- Uses CKD-EPI 2021 race-free eGFR equation (recommended)
- UACR is the key marker for CKD staging and progression monitoring
- All fields optional to allow partial panel entry
