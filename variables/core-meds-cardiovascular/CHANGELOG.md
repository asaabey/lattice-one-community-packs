# Changelog

All notable changes to the `core-meds-cardiovascular` pack will be documented in this file.

## [1.0.0] - 2024-01-19

### Added
- Initial release

#### RAAS Inhibitors
- `atc-C09A` - ACE Inhibitor (enalapril, lisinopril, ramipril)
- `atc-C09C` - ARB (losartan, valsartan, irbesartan)
- `atc-C09D` - ARB Combinations

#### Other Antihypertensives
- `atc-C07` - Beta Blocker (metoprolol, bisoprolol, carvedilol)
- `atc-C08` - Calcium Channel Blocker (amlodipine, diltiazem, verapamil)
- `atc-C02` - Other Antihypertensives (clonidine, methyldopa, hydralazine)
- `atc-C02CA` - Alpha Blocker (prazosin, doxazosin)

#### Diuretics
- `atc-C03` - Any Diuretic
- `atc-C03C` - Loop Diuretic (furosemide, bumetanide)
- `atc-C03D` - Potassium-Sparing/MRA (spironolactone, eplerenone)
- `atc-C03E` - Thiazide (hydrochlorothiazide, chlorthalidone, indapamide)

#### Lipid-Lowering Agents
- `atc-C10AA` - Statin (atorvastatin, rosuvastatin, simvastatin)
- `atc-C10AB` - Fibrate (fenofibrate, gemfibrozil)
- `atc-C10AX09` - Ezetimibe
- `atc-C10BX` - PCSK9 Inhibitor (evolocumab, alirocumab)

#### Antithrombotic Agents
- `atc-B01AC` - Antiplatelet Agent (any)
- `atc-B01AC06` - Aspirin (low-dose)
- `atc-B01AA` - Warfarin/VKA
- `atc-B01AF` - DOAC Factor Xa Inhibitor (rivaroxaban, apixaban)
- `atc-B01AE` - DOAC Direct Thrombin Inhibitor (dabigatran)

#### Cardiac-Specific
- `atc-C01D` - Nitrate (any)
- `atc-C01DA` - GTN/Nitroglycerin
- `atc-C01A` - Digoxin
- `atc-C01BD` - Amiodarone

### Notes
- All variables use WHO ATC classification codes
- Variables are boolean (yes/no) for documenting current medication use
- Clinical notes included for key prescribing considerations
- Hierarchical: Can query at class level (e.g., C09A for any ACE-I) or specific drug
- System URI: `http://www.whocc.no/atc`
