# Changelog

All notable changes to the `lab-entry-lipid` screen pack will be documented in this file.

## [1.0.0] - 2024-01-19

### Added
- Initial release

#### Screen: Lipid Panel

**Specimen Information**
- Collection date (required)
- Fasting status (required) - Fasting/Non-fasting/Unknown
- Lab reference number

**Standard Lipid Panel**
- Total Cholesterol (mg/dL)
- HDL Cholesterol (mg/dL)
- LDL Cholesterol - Calculated (mg/dL) - Friedewald equation
- LDL Cholesterol - Direct (mg/dL) - for elevated TG
- Triglycerides (mg/dL)
- VLDL Cholesterol (mg/dL)

**Calculated Values & Ratios**
- Non-HDL Cholesterol (mg/dL) - auto-calculated
- Total/HDL Ratio - auto-calculated
- LDL/HDL Ratio - auto-calculated
- TG/HDL Ratio - auto-calculated, marker of insulin resistance

**Apolipoproteins**
- Apolipoprotein A-I (mg/dL)
- Apolipoprotein B (mg/dL) - reflects atherogenic particle count

**Advanced Lipid Markers**
- Lipoprotein(a) (nmol/L) - genetically determined CV risk factor
- LDL Particle Number (nmol/L)
- Small Dense LDL Cholesterol (mg/dL)
- Remnant Cholesterol (mg/dL)

**Lab Notes**
- Free text notes field

### Dependencies
- Requires `core-labs-lipid` variable pack

### Notes
- Fasting status required for accurate triglyceride interpretation
- Calculated LDL inaccurate when TG >400 mg/dL - use direct LDL
- TG/HDL ratio >4 suggests insulin resistance and atherogenic phenotype
- Lp(a) is genetically determined and should be measured once in lifetime
- Non-HDL = Total - HDL, secondary treatment target per guidelines
