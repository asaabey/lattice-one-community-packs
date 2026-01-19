# Changelog

All notable changes to the `core-labs-lipid` pack will be documented in this file.

## [1.0.0] - 2024-01-19

### Added
- Initial release

#### Standard Lipid Panel
- `loinc-2093-3` - Total Cholesterol (mg/dL)
- `loinc-2085-9` - HDL Cholesterol (mg/dL)
- `loinc-2089-1` - LDL Cholesterol Calculated (mg/dL) - Friedewald equation
- `loinc-18262-6` - LDL Cholesterol Direct (mg/dL)
- `loinc-2571-8` - Triglycerides (mg/dL)
- `loinc-2091-7` - VLDL Cholesterol (mg/dL)

#### Calculated Ratios
- `loinc-43396-1` - Non-HDL Cholesterol (mg/dL)
- `loinc-9830-1` - Total/HDL Cholesterol Ratio
- `loinc-11054-4` - LDL/HDL Cholesterol Ratio
- `loinc-13457-7` - Triglyceride/HDL Ratio

#### Apolipoproteins
- `loinc-1869-0` - Apolipoprotein A-I (mg/dL)
- `loinc-1884-9` - Apolipoprotein B (mg/dL)

#### Advanced Lipid Markers
- `loinc-10835-7` - Lipoprotein(a) (nmol/L)
- `loinc-49132-4` - LDL Particle Number (nmol/L)
- `loinc-96259-7` - Small Dense LDL Cholesterol (mg/dL)
- `loinc-35198-1` - Remnant Cholesterol (mg/dL)

### Notes
- All variables use standard LOINC codes
- LDL-C targets based on ATP III and ACC/AHA guidelines
- Calculated LDL (Friedewald) inaccurate when TG >400 mg/dL - use direct LDL
- TG/HDL ratio >4 suggests insulin resistance and small dense LDL pattern
- Lp(a) is genetically determined and an independent CV risk factor
- Non-HDL = Total - HDL, represents all atherogenic cholesterol
- UCUM units used throughout for interoperability
