# Changelog

All notable changes to the `patient-registration-lk` screen pack will be documented in this file.

## [1.0.0] - 2024-01-19

### Added
- Initial release

#### Screen: Patient Registration - Sri Lanka

**Personal Information Section**
- Given name (required)
- Family name (required)
- Date of birth (required)
- Gender (required)

**National Identifiers Section**
- NIC - National Identity Card with validation for both old (9+V/X) and new (12 digit) formats
- Passport number (optional)

**Address Section**
- Street address
- City/Town
- Grama Niladhari Division
- Divisional Secretariat
- District (dropdown with all 25 districts)
- Province (dropdown with all 9 provinces)
- Postal code (5 digits)

**Contact Information Section**
- Mobile phone (with Sri Lankan format validation)
- Landline phone
- Email address

**Emergency Contact Section**
- Emergency contact name
- Emergency contact phone

### Dependencies
- Requires `core-demographics-lk` variable pack

### Notes
- NIC validation supports both old format (123456789V) and new format (200012345678)
- District and province selections are linked to variables with full choice lists
- Phone validation supports +94, 0, or no prefix formats
