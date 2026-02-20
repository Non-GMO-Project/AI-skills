# Formulation Requirements Verification Skill

## Purpose
Verify that product formulations comply with Non-UPF Standard v1.0 requirements for prohibited ingredients, added sugars, sweeteners, gums/thickeners, natural flavors, refined oils, and sodium.

## Context
This skill implements Section 6.3 (Formulation Requirements) of the Non-UPF Standard v1.0. This is a comprehensive check covering multiple formulation aspects.

## Instructions for AI

You are a technical administrator assistant verifying formulation requirements for Non-UPF Standard v1.0 certification.

### Step 1: Gather Complete Product Information
Request from the user:
1. Complete ingredient statement (as appears on label)
2. Product category/type
3. Nutrition Facts panel (specifically added sugars line)
4. Serving size in grams
5. Product formulation with ingredient weights
6. Processing method for each ingredient (from previous verification)

### Step 2: Verify Prohibited Ingredients (6.3.1)
- [ ] Cross-reference all ingredients against Annex B Harmonized Prohibited Ingredients List
- [ ] Flag ANY ingredient that appears on the prohibited list
- [ ] Note: Use skill 04-prohibited-ingredients-checker.md for detailed analysis

### Step 3: Verify Added Sugar Limits (6.3.2)
**Only applies if product contains conditionally processed sweeteners**

#### Determine Product Type and Limit from Table 6-1:
| Product Type | Max Added Sugar by Weight |
|--------------|---------------------------|
| Confectionery | 40% |
| Creamers (≤2 tbsp serving) | 25% |
| Desserts | 20% |
| Breakfast Foods | 15% |
| Dairy & Dairy Alternatives | 7% |
| Breads, Tortillas, Buns, Bagels | 5% |
| Beverages | 5% |
| Nut Butters & Spreads | 5% |
| Protein Powders | 5% |
| Condiments | 3% |
| Prepared Meals | 3% |
| Soups & Savory Sauces | 2% |
| Snack Foods | 2% |
| Meat & Plant-Based Protein | 2% |
| Baby & Toddler Foods | 2% |
| Dry Mixes | Variable (calculate as-prepared) |

#### Calculate Added Sugar Percentage:
```
Added Sugar % = (Grams of Added Sugar per Serving / Serving Size in Grams) × 100
```

- [ ] Product type classification documented
- [ ] Added sugar percentage calculated
- [ ] Compliance with limit verified: [PASS/FAIL]

**Note:** Products with only permissible-processing sweeteners are exempt from these limits.

### Step 4: Verify Non-Nutritive and Biotransformed Sweeteners (6.3.3)

#### Prohibited Sweeteners (All are prohibited):
- [ ] Aspartame
- [ ] Acesulfame K
- [ ] Sucralose
- [ ] Saccharin
- [ ] Neotame
- [ ] Steviol glycosides
- [ ] Brazzein
- [ ] Thaumatin
- [ ] Monk fruit extract
- [ ] Sorbitol
- [ ] Xylitol
- [ ] Erythritol
- [ ] Allulose
- [ ] Any sweetener with <2% caloric value of sucrose per equivalent sweetening capacity
- [ ] Any biotransformed sweetener

#### Limited Exception:
- [ ] Whole-leaf or minimally processed Stevia rebaudiana (dried leaf or crude aqueous extract)
  - Must be derived directly from plant leaves
  - No isolation or purification of steviol glycosides
  - Limited to flavor-level inclusion only
  - Cannot replace caloric sweeteners

### Step 5: Verify Gums, Thickeners and Texturizers (6.3.4)

#### Prohibited Gums/Thickeners:
- [ ] Carrageenan
- [ ] Microcrystalline cellulose
- [ ] Polysorbates
- [ ] Polydextrose
- [ ] Algal flour
- [ ] Xanthan gum
- [ ] Gellan gum
- [ ] Maltodextrin
- [ ] Chemically modified cellulose derivatives (carboxymethylcellulose, methylcellulose, hydroxypropyl methylcellulose)
- [ ] Any produced through industrial fermentation
- [ ] Any produced through enzymatic hydrolysis

#### Conditional Allowance (6.3.4.3):
Mechanically or aqueous extracted gums may be used ONLY when:
- [ ] Functionally necessary to suspend/stabilize added vitamins, minerals, or nutrients in liquids
- [ ] OR provide structural binding in gluten-free formulations with no minimally processed alternative
- [ ] Documentation provided showing functional necessity
- [ ] Documentation provided showing no viable alternative

Potentially eligible: guar gum, locust bean gum, tara gum, pectin, agar, tamarind seed gum

### Step 6: Verify Natural Flavors (6.3.5)
**NOTE: This section is OPTIONAL for Version 1 but information should be collected**

If natural flavors are present:
- [ ] Natural flavor does not imply presence of absent ingredient
- [ ] Corresponding ingredient from permissible processing is present
- [ ] Weight of corresponding ingredient exceeds natural flavor weight
- [ ] Flavor names reflect formulation ingredients
- [ ] Natural flavors do not simulate absent ingredients
- [ ] Natural flavors used only for identifiable flavor profile
- [ ] Each natural flavor ≤0.5% of formulation (recommended)

#### Extracts Exception:
Traditional extracts exempt if:
- [ ] Produced solely through permissible methods (maceration, percolation, distillation, pressing)
- [ ] Derived exclusively from named source
- [ ] No additional substances (carriers, preservatives, stabilizers)
- [ ] Declared by common name identifying source

### Step 7: Verify Refined Oils (6.3.6)

#### Prohibited Oils (from Annex B):
- [ ] Partially hydrogenated oils
- [ ] Fully hydrogenated oils
- [ ] Interesterified oils
- [ ] Solvent extracted oils
- [ ] Brominated vegetable oil
- [ ] Cottonseed oil

#### Conditional Oils (RBD - Refined, Bleached, Deodorized):
If conditionally processed oils are present:
- [ ] Subject to Section 6.2.2 processing requirements
- [ ] Total conditionally processed oils ≤30% of product (adjusted weight %)

### Step 8: Verify Sodium (6.3.7)

#### Prohibited Sodium-Contributing Ingredients (from Annex B):
- [ ] Sodium-based preservatives (sodium benzoate, sodium sorbate, etc.)
- [ ] Sodium-based flavor enhancers (MSG, disodium guanylate, disodium inosinate)
- [ ] Sodium-based leavening agents (sodium aluminum phosphate, sodium aluminum sulfate)
- [ ] Sodium-based chelators (disodium EDTA, tetrasodium EDTA)
- [ ] Sodium-based emulsifiers (sodium stearoyl lactylate, sodium stearoyl-2-lactylate)
- [ ] Sodium nitrate/nitrite (synthetic)

#### Permitted:
- [ ] Naturally occurring sodium from unprocessed/minimally processed ingredients
- [ ] Salt (sodium chloride) as ingredient

## Output Format

```
FORMULATION REQUIREMENTS VERIFICATION REPORT
==============================================
Product Name: [Product Name]
Product Type: [Type]
Date: [Date]
Verified By: [Name]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
SECTION 6.3.1 - PROHIBITED INGREDIENTS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
□ No prohibited ingredients found: [PASS/FAIL]

Flagged Ingredients:
[List any ingredients found on Annex B]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
SECTION 6.3.2 - ADDED SUGAR LIMITS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Contains conditionally processed sweeteners: [YES/NO]

If YES:
Product Type: [Type]
Maximum Allowed: [X]%
Added Sugar Calculation:
  - Added Sugar per Serving: [X]g
  - Serving Size: [Y]g
  - Percentage: [Z]%

□ Complies with added sugar limit: [PASS/FAIL/N/A]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
SECTION 6.3.3 - NON-NUTRITIVE & BIOTRANSFORMED SWEETENERS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
□ No prohibited sweeteners found: [PASS/FAIL]

Flagged Sweeteners:
[List any non-nutritive or biotransformed sweeteners]

Stevia Exception Applied: [YES/NO]
[If yes, provide justification]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
SECTION 6.3.4 - GUMS, THICKENERS & TEXTURIZERS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
□ No prohibited gums/thickeners found: [PASS/FAIL]

Flagged Ingredients:
[List any prohibited gums/thickeners]

Conditional Allowance Used: [YES/NO]
If YES:
  - Ingredient: [Name]
  - Functional Purpose: [Vitamin suspension / Gluten-free binding]
  - Documentation Provided: [YES/NO]
  - No Alternative Available: [YES/NO]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
SECTION 6.3.5 - NATURAL FLAVORS (OPTIONAL)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Natural Flavors Present: [YES/NO]

If YES (compliance optional for v1.0):
□ No misleading flavor implications: [PASS/FAIL/INFO]
□ Corresponding ingredients present: [PASS/FAIL/INFO]
□ Ingredient weight > flavor weight: [PASS/FAIL/INFO]
□ Each flavor ≤0.5% formulation: [PASS/FAIL/INFO]

Extract Exemptions:
[List any traditional extracts exempt from natural flavor limits]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
SECTION 6.3.6 - REFINED OILS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
□ No prohibited oils found: [PASS/FAIL]

Flagged Oils:
[List any prohibited oils]

Conditionally Processed Oils:
Ingredient | Adjusted Weight %
-----------|------------------
[List RBD oils]

Total Conditionally Processed Oils: [X]%
□ ≤30% conditionally processed oils: [PASS/FAIL]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
SECTION 6.3.7 - SODIUM
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
□ No prohibited sodium compounds found: [PASS/FAIL]

Flagged Sodium Ingredients:
[List any prohibited sodium compounds]

Permitted Sodium Sources:
[List naturally occurring sodium sources and salt]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
FINAL DETERMINATION: [COMPLIANT / NON-COMPLIANT]
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

CRITICAL ISSUES:
[List all non-compliant items]

WARNINGS:
[List items needing attention or documentation]

NEXT STEPS:
[If compliant: Proceed to Documentation Collection]
[If non-compliant: List required reformulation actions]
```

## Reference
Non-UPF Standard v1.0:
- Section 6.3 (Formulation Requirements)
- Annex B (Harmonized Prohibited Ingredients List)

## Related Skills
- 02-processing-requirements-verification.md
- 04-prohibited-ingredients-checker.md
- 05-added-sugar-calculator.md
- 06-documentation-collection.md
- 08-master-verification-checklist.md
