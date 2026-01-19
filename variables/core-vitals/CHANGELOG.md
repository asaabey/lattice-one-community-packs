# Changelog

All notable changes to the `core-vitals` pack will be documented in this file.

## [1.0.0] - 2024-01-19

### Added
- Initial release

#### Blood Pressure
- `loinc-8480-6` - Systolic Blood Pressure (mmHg)
- `loinc-8462-4` - Diastolic Blood Pressure (mmHg)
- `local-bp-position` - Measurement position (sitting, standing, supine, reclining)
- `local-bp-arm` - Measurement arm (left, right)

#### Heart Rate & Rhythm
- `loinc-8867-4` - Heart Rate (/min)
- `local-pulse-regularity` - Pulse regularity (regular, irregular, etc.)

#### Respiratory
- `loinc-9279-1` - Respiratory Rate (/min)
- `loinc-2708-6` - Oxygen Saturation SpO2 (%)
- `loinc-59408-5` - Oxygen Saturation by Pulse Oximetry (%)

#### Temperature (Metric & Imperial)
- `loinc-8310-5` - Body Temperature (Celsius)
- `loinc-8331-1` - Body Temperature (Fahrenheit)

#### Weight (Metric & Imperial)
- `loinc-29463-7` - Body Weight (kg)
- `loinc-3141-9` - Body Weight (lbs)
- `local-weight-method` - Measurement method (measured, stated, estimated)

#### Height (Metric & Imperial)
- `loinc-8302-2` - Body Height (cm)
- `loinc-8306-3` - Body Height (inches)

#### Calculated
- `loinc-39156-5` - BMI (kg/m²) - calculated from weight and height

#### Other
- `local-vitals-notes` - Free text notes

### Notes
- All LOINC-coded variables use standard LOINC codes
- Metric and imperial variants provided for temperature, weight, and height
- Normal ranges and critical values included where clinically appropriate
- UCUM units used throughout for interoperability
