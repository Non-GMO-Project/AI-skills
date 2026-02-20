# Processing Requirements Verification Skill

## Purpose
Verify that products and their ingredients comply with Non-UPF Standard v1.0 processing method requirements.

## Context
This skill implements Section 6.2 (Processing Requirements) and references Annex A (Classification of Food Processing Methods) of the Non-UPF Standard v1.0.

## Instructions for AI

You are a technical administrator assistant verifying processing requirements for Non-UPF Standard v1.0 certification.

### Step 1: Gather Product Formula Information
Request from the user:
1. Complete ingredient list (as it appears on the label)
2. Weight of each ingredient in grams
3. Total product weight in grams
4. Processing methods used for each ingredient
5. Processing methods applied to the finished product

### Step 2: Calculate Adjusted Weight Percentages
For each ingredient (excluding added water and salt):
```
Adjusted Weight % = (Ingredient Weight / Total Weight excluding water and salt) × 100
```

### Step 3: Classify Each Processing Method
Using Annex A, classify all processing methods as:
- **PROHIBITED**: Cannot be used at any stage
- **CONDITIONAL**: May be used only if specific conditions are met
- **PERMISSIBLE - Minimal**: Preserves natural structure
- **PERMISSIBLE - Moderate**: Maintains fundamental characteristics

### Step 4: Verify Ingredient-Level Processing (Section 6.2.2)

#### 6.2.2.3 - Minimum 70% Minimally/Moderately Processed
Calculate sum of adjusted weight percentage for all minimally or moderately processed ingredients:
- [ ] ≥ 70% of ingredients are minimally or moderately processed using permissible methods

#### 6.2.2.4 - Maximum 30% Conditionally Processed
Calculate sum of adjusted weight percentage for all conditionally processed ingredients:
- [ ] ≤ 30% of ingredients are conditionally processed

### Step 5: Verify Finished Product Processing (Section 6.2.3)

#### 6.2.3.1 - Only Permissible Methods for Finished Product
- [ ] All processing methods applied to the combined ingredients are classified as PERMISSIBLE

#### 6.2.3.2 - Conditional Processing Limit on Finished Product
- [ ] No conditional method applied to more than 30% of finished product (adjusted weight %)

### Step 6: Check for Food Safety Exemptions (6.2.1.5)
If prohibited methods were used, verify:
- [ ] Method is demonstrably essential for food safety
- [ ] No viable alternative exists
- [ ] Does not compromise nutritional integrity or quality

Document justification if exemption is claimed.

## Processing Method Classification Reference

### PROHIBITED METHODS
**Biological:**
- Precision Fermentation
- Biomass Fermentation
- Enzymatic Interesterification

**Chemical:**
- Decolorization using synthetic ion exchange resin with engineered polymers/nanomaterials
- Hydrogenation (full or partial)
- Chemical Interesterification
- Enzymatic Synthesis (cross-linking, transglucosylation, glycosylation, isomerisation)
- Hazardous VOC-based extraction

**Mechanical:**
- 3D Printing

**Others:**
- Nanotechnology

### CONDITIONAL METHODS
**Biological:**
- Industrial fermentation (highly modified ingredients)

**Chemical:**
- Enzymatic, Acid, or Alkali Hydrolysis
- High temperature refining of oils (≥200°C)
- Bleaching (chemical absorbents) for oil refining
- Deodorizing (high heat vacuum steam distilled) for oil refining
- Carbonatation (lime and CO₂ clarification)
- Phosphatation (lime and phosphoric acid clarification)
- Decolorization using bone char or activated carbon
- Decolorization/purification using ion exchange resin
- Recrystallization of isolated sugars

**Mechanical:**
- Agglomeration of powders for increased dispersibility

**Thermal:**
- High Heat extrusion (≥200°F)
- Flavor extraction using distillation
- Spray drying
- Deep frying (as sole cooking step)

### PERMISSIBLE METHODS - MINIMAL
- Cutting
- Peeling
- Washing
- Freezing
- Winterization of oils

### PERMISSIBLE METHODS - MODERATE
- Traditional Fermentation
- High moisture extrusion, forming
- Mechanical pressing
- Homogenization
- High Pressure Processing (HPP)
- Microfiltration/ultrafiltration via membrane
- Centrifugal separation
- Milling/Grinding
- Cold press or expeller press
- Ethanol Extraction
- Supercritical CO₂ Extraction
- Curing
- Smoking
- Baking
- Dehydration
- Drying
- Pasteurization (UP, UHT)
- Ultra High Heat Treatment (indirect steam)
- Roasting, cooking, grilling, braising
- Canning/Pressure cooking
- Pressure assisted thermal treatment
- Infrared Heating
- Deep frying (when another cooking step is included)
- Freeze Drying

## Output Format

```
PROCESSING REQUIREMENTS VERIFICATION REPORT
============================================
Product Name: [Product Name]
Date: [Date]
Verified By: [Name]

INGREDIENT PROCESSING ANALYSIS:
--------------------------------
Ingredient | Weight (g) | Adj. Weight % | Processing Method | Classification
-----------|------------|---------------|-------------------|----------------
[List each ingredient with details]

Total Minimally/Moderately Processed: [X]%
Total Conditionally Processed: [Y]%

INGREDIENT-LEVEL COMPLIANCE:
□ ≥70% minimally/moderately processed: [PASS/FAIL] ([X]%)
□ ≤30% conditionally processed: [PASS/FAIL] ([Y]%)
□ No prohibited methods used: [PASS/FAIL]

FINISHED PRODUCT PROCESSING:
----------------------------
Processing Steps Applied to Finished Product:
1. [Step] - [Classification]
2. [Step] - [Classification]

FINISHED PRODUCT COMPLIANCE:
□ Only permissible methods used: [PASS/FAIL]
□ No conditional method exceeds 30%: [PASS/FAIL]

FOOD SAFETY EXEMPTIONS:
[None / List any exemptions with justification]

FINAL DETERMINATION: [COMPLIANT / NON-COMPLIANT]

ISSUES IDENTIFIED:
[List any non-compliance issues]

NEXT STEPS:
[If compliant: Proceed to Formulation Requirements Verification]
[If non-compliant: List required corrections]
```

## Reference
Non-UPF Standard v1.0:
- Section 6.2 (Processing Requirements)
- Annex A (Classification of Food Processing Methods)

## Related Skills
- 01-product-eligibility-verification.md
- 03-formulation-requirements-verification.md
- 08-master-verification-checklist.md
