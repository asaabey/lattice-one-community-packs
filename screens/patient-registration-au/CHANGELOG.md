# Changelog

All notable changes to the `patient-registration-au` screen pack will be documented in this file.

## [1.0.0] - 2024-01-19

### Added
- Initial release

#### Screen: Patient Registration - Australia

**Personal Information Section**
- Given name(s) (required)
- Family name (required)
- Date of birth (required)
- Gender (required) - includes "Prefer not to say" option
- Indigenous status (required) - AIHW standard categories

**Healthcare Identifiers Section**
- Medicare Card Number (10 digits with Luhn validation)
- Individual Reference Number (IRN) - 1-9
- DVA File Number (for veterans/dependants)
- Individual Healthcare Identifier (IHI) - 16 digits starting with 800360

**Residential Address Section**
- Address Line 1 (required)
- Address Line 2
- Suburb/Town (required)
- State/Territory (required) - all 8 states and territories
- Postcode (required) - 4 digit Australian postcode

**Contact Information Section**
- Mobile phone (required) - Australian mobile format validation (04XX XXX XXX)
- Home phone
- Email address

**Emergency Contact Section**
- Emergency contact name
- Relationship
- Emergency contact phone

### Dependencies
- Requires `core-demographics-au` variable pack

### Notes
- Indigenous status uses AIHW (Australian Institute of Health and Welfare) standard codes
- Medicare number validation uses standard 10-digit format
- IHI format follows national e-health standards (800360 prefix)
- Mobile phone validation supports +61, 0, or no prefix formats
