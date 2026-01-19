# Changelog

All notable changes to the `core-demographics-au` pack will be documented in this file.

## [1.0.0] - 2024-01-19

### Added
- Initial release
- Australian healthcare identifiers:
  - Medicare Card Number (10 digits)
  - Medicare IRN (Individual Reference Number)
  - DVA File Number (Department of Veterans' Affairs)
  - IHI (Individual Healthcare Identifier - 16 digits)
- Basic patient demographics (name, DOB, gender)
- Australian address components:
  - State/Territory (8 states/territories)
  - Postcode (4 digits)
  - Suburb/Town
  - Street address
- Contact information (mobile, home phone, email)
- Indigenous status (AIHW standard classification)
- Validation patterns for Australian formats:
  - Medicare: 10 digits starting with 2-6
  - IHI: 16 digits starting with 800360
  - Mobile: 04XX XXX XXX
  - Postcode: 4 digits
