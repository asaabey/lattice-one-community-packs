# Changelog

All notable changes to the `lab-entry-hematology` screen pack will be documented in this file.

## [1.0.0] - 2024-01-19

### Added
- Initial release

#### Screen: Hematology Panel

**Specimen Information**
- Collection date (required)
- Lab reference number

**Complete Blood Count (CBC)**
- Hemoglobin (g/dL)
- Hematocrit (%)
- RBC Count (10^6/uL)
- WBC Count (10^3/uL)
- Platelet Count (10^3/uL)

**Red Cell Indices**
- MCV (fL)
- MCH (pg)
- MCHC (g/dL)
- RDW (%)
- Reticulocyte Count (%)

**WBC Differential**
- Neutrophils (%)
- Lymphocytes (%)
- Monocytes (%)
- Eosinophils (%)
- Basophils (%)
- Absolute Neutrophil Count (10^3/uL)

**Iron Studies**
- Serum Iron (ug/dL)
- TIBC (ug/dL)
- Transferrin Saturation (%)
- Ferritin (ng/mL)

**Vitamins**
- Vitamin B12 (pg/mL)
- Folate (ng/mL)

**Coagulation**
- PT (seconds)
- INR
- PTT (seconds)
- Fibrinogen (mg/dL)

**Inflammatory Markers**
- ESR (mm/h)
- CRP (mg/L)

**Lab Notes**
- Free text notes field

### Dependencies
- Requires `core-labs-hematology` variable pack

### Notes
- Comprehensive panel covering anemia workup, infection markers, and coagulation
- ANC critical for neutropenic patients
- Iron studies help differentiate iron deficiency vs anemia of chronic disease
