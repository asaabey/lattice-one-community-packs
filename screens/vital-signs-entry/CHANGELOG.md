# Changelog

All notable changes to the `vital-signs-entry` screen pack will be documented in this file.

## [1.0.0] - 2024-01-19

### Added
- Initial release

#### Screen: Vital Signs Entry

**Blood Pressure Section**
- Systolic BP (mmHg) - range 50-300
- Diastolic BP (mmHg) - range 20-200
- Position (sitting, standing, lying down)
- Arm (left, right)

**Heart Rate Section**
- Heart rate (bpm) - range 20-300
- Pulse regularity (regular, irregular)

**Respiratory**
- Respiratory rate (breaths/min) - range 4-60

**Oxygen Saturation**
- SpO2 (%) - range 50-100

**Temperature Section**
- Temperature in Celsius (°C) - range 30-45
- Temperature in Fahrenheit (°F) - range 86-113 (imperial variant)

**Anthropometrics Section**
- Weight in kg - range 0.5-500
- Weight in lbs - range 1-1100 (imperial variant)
- Height in cm - range 30-300
- Height in inches - range 12-120 (imperial variant)
- BMI (calculated, read-only) - auto-calculated from weight/height

**Notes**
- Clinical notes text field

### Dependencies
- Requires `core-vitals` variable pack

### Notes
- Both metric and imperial units provided for temperature, weight, and height
- BMI is auto-calculated when weight (kg) and height (cm) are entered
- All vital signs are optional to allow partial recording
- BP position and arm documented for proper clinical context
- Pulse regularity helps identify arrhythmias
