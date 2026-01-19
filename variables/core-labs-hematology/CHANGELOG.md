# Changelog

All notable changes to the `core-labs-hematology` pack will be documented in this file.

## [1.0.0] - 2024-01-19

### Added
- Initial release

#### Complete Blood Count (CBC)
- `loinc-718-7` - Hemoglobin (g/dL)
- `loinc-4544-3` - Hematocrit (%)
- `loinc-789-8` - RBC Count (10^6/uL)
- `loinc-6690-2` - WBC Count (10^3/uL)
- `loinc-777-3` - Platelet Count (10^3/uL)

#### Red Cell Indices
- `loinc-787-2` - MCV (fL)
- `loinc-785-6` - MCH (pg)
- `loinc-786-4` - MCHC (g/dL)
- `loinc-788-0` - RDW (%)
- `loinc-30384-2` - Reticulocyte Count (%)

#### WBC Differential
- `loinc-751-8` - Neutrophils %
- `loinc-731-0` - Lymphocytes %
- `loinc-742-7` - Monocytes %
- `loinc-711-2` - Eosinophils %
- `loinc-704-7` - Basophils %
- `loinc-17849-1` - Absolute Neutrophil Count (ANC)

#### Iron Studies
- `loinc-2500-7` - Serum Iron (ug/dL)
- `loinc-14800-7` - TIBC (ug/dL)
- `loinc-2502-3` - Transferrin Saturation (%)
- `loinc-3173-2` - Ferritin (ng/mL)

#### Vitamins
- `loinc-35572-7` - Vitamin B12 (pg/mL)
- `loinc-4537-7` - Folate (ng/mL)

#### Coagulation
- `loinc-5902-2` - PT (seconds)
- `loinc-5964-2` - INR
- `loinc-6301-6` - PTT (seconds)
- `loinc-71695-1` - Fibrinogen (mg/dL)

#### Inflammatory Markers
- `loinc-30341-2` - ESR (mm/h)
- `loinc-1988-5` - CRP (mg/L)

### Notes
- All variables use standard LOINC codes
- Normal ranges provided (may vary by lab and patient demographics)
- Critical values included for life-threatening abnormalities
- Hemoglobin normal ranges are broad to cover male/female differences
- UCUM units used throughout for interoperability
