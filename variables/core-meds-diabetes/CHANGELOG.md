# Changelog

All notable changes to the `core-meds-diabetes` pack will be documented in this file.

## [1.0.0] - 2024-01-19

### Added
- Initial release

#### Oral Hypoglycemics
- `atc-A10BA` - Metformin (biguanide)
- `atc-A10BB` - Sulfonylurea (glipizide, gliclazide, glimepiride)
- `atc-A10BH` - DPP-4 Inhibitor (sitagliptin, linagliptin, saxagliptin)
- `atc-A10BK` - SGLT2 Inhibitor (empagliflozin, dapagliflozin, canagliflozin)
- `atc-A10BG` - Thiazolidinedione/TZD (pioglitazone)
- `atc-A10BF` - Alpha-Glucosidase Inhibitor (acarbose)
- `atc-A10BX` - Meglitinide (repaglinide, nateglinide)
- `atc-A10BD` - Oral Combination Products

#### Injectable Non-Insulin
- `atc-A10BJ` - GLP-1 Receptor Agonist (semaglutide, liraglutide, dulaglutide)

#### Insulins
- `atc-A10A` - Insulin (Any)
- `atc-A10AB` - Rapid-Acting Insulin (lispro, aspart, glulisine)
- `atc-A10AC` - Intermediate-Acting Insulin (NPH)
- `atc-A10AD` - Premixed Insulin (70/30, 75/25)
- `atc-A10AE` - Long-Acting/Basal Insulin (glargine, detemir, degludec)

### Notes
- All variables use WHO ATC classification codes
- Variables are boolean (yes/no) for documenting current medication use
- Clinical notes included for key prescribing considerations
- SGLT2 inhibitors and GLP-1 agonists have CV/renal benefits beyond glycemic control
- System URI: `http://www.whocc.no/atc`
