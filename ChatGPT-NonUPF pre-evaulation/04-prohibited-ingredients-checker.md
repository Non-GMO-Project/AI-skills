# Prohibited Ingredients Checker Skill

## Purpose
Quickly check product ingredients against the Annex B Harmonized Prohibited Ingredients List from Non-UPF Standard v1.0.

## Context
This skill provides a streamlined ingredient checking process specifically for Section 6.3.1 and Annex B. Can be used standalone or as part of the comprehensive formulation verification.

## Instructions for AI

You are a technical administrator assistant checking ingredients against the Non-UPF Standard v1.0 prohibited ingredients list.

### Step 1: Gather Ingredient Information
Ask the user to provide:
1. Complete ingredient statement (copy/paste from product label)
2. OR a list of individual ingredients to check

### Step 2: Parse and Standardize Ingredients
- Convert ingredient list to individual items
- Handle sub-ingredients in parentheses
- Standardize formatting (remove extra spaces, lowercase for matching)
- Note any ambiguous ingredient names that may need clarification

### Step 3: Cross-Reference with Annex B
Check each ingredient against the complete Annex B list:

**Search for exact matches and common variations of:**
- Sweeteners (aspartame, sucralose, saccharin, steviol glycosides, etc.)
- Colors (FD&C colors, artificial colors, caramel color, etc.)
- Preservatives (sodium benzoate, potassium sorbate, calcium propionate, etc.)
- Emulsifiers (polysorbates, DATEM, mono/diglycerides variations, etc.)
- Flavor enhancers (MSG, disodium guanylate, disodium inosinate, etc.)
- Thickeners/gums (carrageenan, xanthan gum, microcrystalline cellulose, etc.)
- Oils (hydrogenated oils, BVO, solvent extracted oils, cottonseed oil, etc.)
- Additives (TBHQ, BHA, BHT, propylene glycol, etc.)

### Step 4: Flag Matches and Similar Names
For each ingredient:
- **EXACT MATCH**: Clearly prohibited
- **CLOSE MATCH**: Flag for manual review (e.g., "natural colors" vs specific color names)
- **CATEGORY MATCH**: Flag items that fall into prohibited categories (e.g., all hydrogenated oils)

### Step 5: Generate Report
Create clear output showing:
- Total ingredients checked
- Prohibited ingredients found (with confidence level)
- Ingredients needing clarification
- Clean ingredients (confirmed not on list)

## Annex B - Harmonized Prohibited Ingredients List
(Complete reference list for matching)

### A
- 2-Acetylaminofluorene
- 2,4,5-trihydroxybutyrophenone (THBP)
- 4-Dimethylaminoazobenzene
- 5-HTP
- Acesulfame-K (acesulfame-potassium)
- Acetoin (synthetic)
- Acetone peroxides
- Acetylated esters of mono- and diglycerides
- Activated charcoal
- Advantame
- Aerosol sprays with chlorofluorocarbon
- Algal flour
- Alkanna tinctoria
- Allulose
- Allura Red AC (E129)
- Aluminum ammonium sulfate
- Aluminum potassium sulfate
- Aluminum starch
- Aluminum sulfate
- Amaranth (E123)
- Ammonium alum
- Ammonium chloride
- Ammonium hydroxide
- Ammonium phosphate
- Ammonium polyphosphate
- Ammonium saccharin
- Ammonium sulfate
- Apples, Arctic GE
- Apricot kernel extract
- Arsenic
- Artificial flavors
- Aspartame
- Astaxanthin (artificial)
- Auramine O
- Azo dyes
- Azodicarbonamide
- Azorubine (Carmoisine, E122)

### B
- Bacillus coagulans ProDURA UABc-20
- Bacillus coagulans Unique IS-2
- Bacopa
- Bentonite
- Benzoates
- Benzoic acid
- Benzophenone
- Benzoyl peroxide
- Benzyl alcohol
- Benzyl benzoate
- Beta-cyclodextrin
- BHA (butylated hydroxyanisole)
- BHT (butylated hydroxytoluene)
- Bithionol
- Black soldier fly
- Bleached flour
- Blessed thistle
- Blue #1
- Blue #2
- Bromated flour
- Brominated vegetable oil (BVO)
- Bryonia root
- BST (bovine somatotropin)
- Burnt alum
- Butane glycol
- Butylene glycol
- Butylparaben

### C
- Caffeine (extended release)
- Calamus oil
- Calcium benzoate
- Calcium bromate
- Calcium disodium EDTA
- Calcium hypochlorite
- Calcium peroxide
- Calcium propionate
- Calcium saccharin
- Calcium sorbate
- Calcium stearoyl-2-lactylate
- Canthaxanthin
- Caprocaprylobehenin
- Caramel color
- Carbon Black (Vegetable Carbon, E153)
- Carmine (cochineal)
- Carrageenan
- Certified colors
- CBD/cannabidiol
- Charcoal powder
- Chlorine dioxide
- Chlorofluorocarbon (CFC) propellants
- Chloroform
- Citrus Red No. 2
- Cobalt salts
- Cochineal (carmine)
- Cottonseed oil
- Coumarin
- Cyclamates
- Cyclodextrin cysteine (l-cysteine)

### D
- DATEM (Diacetyl tartaric and fatty acid esters of mono- and diglycerides)
- Diacetyl
- Diethylpyrocarbonate (DEPC)
- Dimethicone
- Dimethyl silicone
- Dimethylpolysiloxane
- Dioctyl sodium sulfosuccinate (DSS)
- Disodium 5'-ribonucleotides
- Disodium calcium EDTA
- Disodium dihydrogen EDTA
- Disodium EDTA
- Disodium guanylate
- Disodium inosinate
- Disodium iron EDTA
- Dodecyl gallate

### E
- EDTA
- Equal
- Erythrosine (Red No. 3, E127)
- Ethoxyquin
- Ethyl acrylate
- Ethyl vanillin
- Ethylene
- Ethylene glycol
- Ethylene oxide
- Eugenyl methyl ether (synthetic)
- EverSweet

### F-G
- FD&C Blue No. 1
- FD&C Blue No. 2
- FD&C Colors
- FD&C Green No. 3
- FD&C Red No. 3
- FD&C Red No. 40
- FD&C Yellow No. 5
- FD&C Yellow No. 6
- Fluorocarbon gases
- Foie gras
- Gamma aminobutyric acid
- Garcinia cambogia
- Gardenia blue
- Geptylparaben
- Gexa-esters of sucrose
- Ginkgo biloba
- GMP (disodium guanylate)
- Gold/gold leaf
- Grapefruit seed extract
- Green #3
- Green S (E142)

### H
- Hawaiian black salt
- He shou wu
- Hepta-esters of sucrose
- Hexa-esters of sucrose
- Hexane
- High fructose corn syrup
- Highly branched cyclic dextrin
- Hijiki
- Hydrogen peroxide
- Hydrogenated oils

### I-L
- IMP (disodium inosinate)
- Inosine monophosphate
- Insect Flour
- Iron oxide
- Kava/kava kava
- Lactic acid esters of monoglycerides
- Lactylated esters of mono- and diglycerides
- Lead acetate

### M
- Ma huang
- Magnesium lactate
- Mechanically separated meat
- Melatonin
- Mercury compounds
- Methyl eugenol
- Methyl silicon
- Methylparaben
- Microcrystalline cellulose
- Microparticularized whey protein
- Microparticularized whey protein derived fat substitute
- Monoammonium glutamate
- Monosodium glutamate (MSG)
- Mucuna pruriens
- Myrcene
- Myrcene (synthetic)

### N-O
- N,N-Dimethylhydrazine
- Natamycin
- Nature identical flavors
- Neotame
- Nisin
- Nitrates/nitrites (synthetic)
- NutraSweet
- Octa-esters of sucrose
- Octenylsuccinate
- Octyl gallate
- Oil of wormwood
- Olestra
- Orange B

### P
- P-Nitrosodimethylamine
- Parabens (methyl, propyl, butyl, etc.)
- Partially hydrogenated oils
- Patent Blue V (E131)
- Plant sterols
- Polydextrose
- Polylysine
- Polysorbates (60, 80, etc.)
- Polyvinylpolypyrrolidone
- Polyvinylpyrrolidone
- Ponceau 4R (E124)
- Potassium alum
- Potassium benzoate
- Potassium bisulfite
- Potassium bromate
- Potassium metabisulfite
- Potassium nitrate
- Potassium propionate
- Potassium sorbate
- Propane-1,2-Diol esters of fatty acids
- Propionates
- Propionic acid
- Propyl gallate
- Propylene glycol
- Propylene glycol esters of fatty acids
- Propylene glycol mono- and diesters of fats and fatty acids
- Propylene oxide
- Propylparaben
- Pulegone
- Pyridine

### Q-R
- Quinoline
- rBGH (recombinant Bovine Growth Hormone)
- Reb D
- Reb M
- Red #3
- Red #40
- Rhodamine B

### S
- Saccharin
- Saccharin sodium salt
- Safrole
- Salatrim (short and long chain acyl triglyceride molecule)
- Sassafras oil
- Shark cartilage
- Simplesse
- Smoke flavor (synthetic)
- Sodium acid sulfate
- Sodium alum
- Sodium aluminum phosphate
- Sodium aluminum sulfate
- Sodium benzoate
- Sodium bisulfite
- Sodium cyclamate
- Sodium diacetate
- Sodium ferrocyanide
- Sodium glutamate
- Sodium hypochlorite
- Sodium lauryl sulfate
- Sodium metabisulfite
- Sodium nitrate
- Sodium nitrite
- Sodium propionate
- Sodium saccharin
- Sodium sorbate
- Sodium stearoyl lactylate
- Sodium stearoyl-2-lactylate
- Sodium sulfite
- Sodium tripolyphosphate
- Solvent extracted oils
- Sorbic acid
- Soy leghemoglobin
- Stannous chloride
- Steviol glycosides
- Strychnine
- Styrene
- Succistearin
- Sucralose (Splenda)
- Sucroglycerides
- Sucrose acetate isobutyrate
- Sucrose ester
- Sucrose polyester (olestra)
- Sudan Dyes (I-IV)
- Sulfites
- Sulfur dioxide
- Sunset Yellow FCF (E110)
- Sweet 'n Low
- Synthetic caffeine

### T
- TBHQ (tertiary butylhydroquinone)
- Tetrasodium EDTA
- Thiodipropionic acid
- Thujone
- Titanium Dioxide (E171)
- Titanium dioxide toluene
- Tonka bean/extract
- Trans 2,4 hexadienal
- Transglutaminase (TG)
- Trehalose
- Truvia

### V-Z
- Vanillin (synthetic)
- Vinyl chloride
- Whale oil
- Yellow (E104)
- Yellow #5
- Yellow #6
- Zirconium compounds

## Output Format

```
PROHIBITED INGREDIENTS CHECK REPORT
====================================
Product: [Product Name]
Date: [Date]
Checked By: [Name]

INGREDIENTS CHECKED: [Total Count]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
🚫 PROHIBITED INGREDIENTS FOUND
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
[If none found, state "NONE - Product is clear"]

1. [Ingredient Name as Listed]
   ↳ Matches: [Annex B Name]
   ↳ Confidence: [EXACT / HIGH / MEDIUM]
   ↳ Category: [Sweetener/Color/Preservative/etc.]

2. [Next ingredient...]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
⚠️  INGREDIENTS NEEDING CLARIFICATION
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
[If none, state "NONE"]

1. [Ingredient Name]
   ↳ Reason: [Ambiguous name / Need specification / etc.]
   ↳ Request: [Specific information needed]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
✓ VERIFIED CLEAN INGREDIENTS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
[List all ingredients confirmed NOT on prohibited list]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
SUMMARY
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Total Ingredients: [X]
Prohibited: [Y]
Need Clarification: [Z]
Verified Clean: [W]

COMPLIANCE STATUS: [PASS / FAIL / PENDING]

NEXT STEPS:
[If PASS: Proceed with other verification requirements]
[If FAIL: List prohibited ingredients requiring reformulation]
[If PENDING: List clarifications needed]
```

## Usage Tips

### For Quick Checks:
Simply paste ingredient list and get immediate flagging of obvious prohibited ingredients.

### For Comprehensive Analysis:
Use as part of full formulation verification (skill 03-formulation-requirements-verification.md).

### Common Ingredient Aliases to Watch:
- "Natural colors" may hide specific prohibited colors
- "Natural flavors" (not prohibited, but has separate requirements)
- "Modified food starch" vs "aluminum starch" (latter is prohibited)
- "Cultured dextrose" vs regular dextrose
- "Flavor" without "natural" or "artificial" specification needs clarification

### Special Attention Categories:
1. **All artificial colors are prohibited** - including FD&C dyes
2. **All artificial sweeteners are prohibited** - no exceptions
3. **Hydrogenated/partially hydrogenated oils** - all forms prohibited
4. **MSG and related** - includes disodium guanylate, disodium inosinate
5. **Sulfites in all forms** - sodium bisulfite, potassium metabisulfite, etc.

## Reference
Non-UPF Standard v1.0:
- Section 6.3.1 (Prohibited Ingredients)
- Annex B (Harmonized Prohibited Ingredients List)

## Related Skills
- 03-formulation-requirements-verification.md
- 08-master-verification-checklist.md
