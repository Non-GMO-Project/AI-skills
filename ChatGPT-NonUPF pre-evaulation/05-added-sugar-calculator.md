# Added Sugar Calculator Skill

## Purpose
Calculate and verify compliance with Non-UPF Standard v1.0 added sugar limits based on product type.

## Context
This skill implements Section 6.3.2 (Added Sugar Limits) of the Non-UPF Standard v1.0. Only applies to products containing sweeteners that are the result of conditional processing.

## Instructions for AI

You are a technical administrator assistant calculating added sugar compliance for Non-UPF Standard v1.0 certification.

### Step 1: Determine If Added Sugar Limits Apply

Ask the user about sweetener processing:
- Does the product contain any sweeteners?
- Are any sweeteners the result of conditional processing per Annex A?

**If NO conditionally processed sweeteners:** Product is EXEMPT from added sugar limits (Section 6.3.2.6)

**If YES:** Proceed with calculation and verification.

### Step 2: Classify Product Type

Review the product and determine which category from Table 6-1 best fits:

| Product Type | Maximum Added Sugar % |
|--------------|----------------------|
| Confectionery (candy, chocolate) | 40% |
| Creamers (dairy and non-dairy, serving ≤2 tbsp) | 25% |
| Desserts (cookies, ice cream, bars, cakes, pastries, popsicles) | 20% |
| Breakfast Foods (cereal, granola, instant oatmeal, french toast, crêpes) | 15% |
| Dairy & Dairy Alternatives (yogurt, milk, cream cheese) | 7% |
| Breads, Tortillas, Buns, Bagels | 5% |
| Beverages (juice, coffee, tea, soda, kombucha) | 5% |
| Nut Butters & Spreads | 5% |
| Protein Powders (whey, pea protein, collagen) | 5% |
| Condiments (ketchup, dressing, mayonnaise) | 3% |
| Prepared Meals (frozen or shelf-stable) | 3% |
| Soups & Savory Sauces (tomato sauce, broth) | 2% |
| Snack Foods (chips, crackers, popcorn) | 2% |
| Meat & Plant-Based Protein (jerky, sausage, deli meat) | 2% |
| Baby & Toddler Foods (marketed to children <4 years) | 2% |
| Dry Mixes (baking mixes, dried soups, ready-to-mix beverages) | Variable* |

*For Dry Mixes: Calculate based on prepared product following manufacturer's directions

**Note per 6.3.2.4:** When product doesn't clearly fit a single type, use good faith judgment to determine most suitable type and document rationale.

### Step 3: Gather Nutrition Facts Data

Request from the user:
1. Nutrition Facts panel (photo or text)
2. Serving size in grams
3. Added sugars in grams per serving
4. (Optional) Unrounded values if available

### Step 4: Calculate Added Sugar Percentage

**Standard Calculation (per 6.3.2.2):**
```
Added Sugar % = (Added Sugars in grams per serving / Serving Size in grams) × 100
```

**Alternative if per 100g is available:**
```
Added Sugar % = (Added Sugars per 100g / 100g) × 100
```

**Important Notes (per 6.3.2.5):**
- Use unrounded values before applying nutrition labeling rounding rules
- Exception: When compliance is clearly evident using rounded Nutrition Facts values
- MUST use unrounded data when:
  - Limits are ≤5%, OR
  - Results based on rounded values are close to the limit

### Step 5: Special Case - Dry Mixes (6.3.2.7)

For dry mix products:
1. Identify the prepared serving size per manufacturer's directions
2. Calculate added sugar in the prepared product
3. Apply the limit for the corresponding prepared product type

Example:
- Pancake mix → Apply "Breakfast Foods" limit (15%)
- Dried soup mix → Apply "Soups & Savory Sauces" limit (2%)
- Drink mix → Apply "Beverages" limit (5%)

### Step 6: Verify Compliance

Compare calculated percentage to the maximum allowed for the product type:
- **PASS**: Calculated % ≤ Maximum %
- **FAIL**: Calculated % > Maximum %

### Step 7: Document Findings

Include:
- Product classification rationale
- Calculation showing work
- Compliance determination
- Any special considerations or notes

## Calculation Examples

### Example 1: Yogurt (Simple Case)
```
Product: Strawberry Yogurt
Product Type: Dairy & Dairy Alternatives (7% limit)
Serving Size: 150g
Added Sugars: 9g

Calculation:
9g ÷ 150g × 100 = 6.0%

Result: 6.0% ≤ 7% → PASS
```

### Example 2: Granola (Using Unrounded Values)
```
Product: Honey Almond Granola
Product Type: Breakfast Foods (15% limit)
Serving Size: 50g
Added Sugars (rounded on label): 7g
Added Sugars (unrounded): 7.4g

Note: Calculation is close to limit, must use unrounded values

Calculation:
7.4g ÷ 50g × 100 = 14.8%

Result: 14.8% ≤ 15% → PASS (but very close!)
```

### Example 3: Dry Mix - Muffin Mix
```
Product: Blueberry Muffin Mix
Product Type: Breakfast Foods (15% limit)

Dry Mix Data:
- Dry serving: 45g
- Added sugars in dry mix: 10g

Prepared Product (per directions: add 1 egg, 1/4 cup milk):
- Prepared serving: 75g (45g mix + 30g wet ingredients)
- Added sugars: 10g (from mix only)

Calculation (use prepared weight):
10g ÷ 75g × 100 = 13.3%

Result: 13.3% ≤ 15% → PASS
```

### Example 4: Ambiguous Classification
```
Product: Protein Bar with Chocolate Coating
Could fit: "Desserts" (20%) OR "Protein Powders" (5%)

Rationale: Despite chocolate coating, primary function is protein
supplementation. However, texture and consumption occasion are
dessert-like.

Good faith determination: Classify as "Desserts" (20%) due to:
- Candy bar format
- Chocolate coating
- Consumer treats as dessert/snack
- More restrictive than treating as protein supplement

Serving Size: 60g
Added Sugars: 11g

Calculation:
11g ÷ 60g × 100 = 18.3%

Result: 18.3% ≤ 20% → PASS
Documentation: Classification rationale recorded for transparency
```

## Output Format

```
ADDED SUGAR CALCULATION REPORT
================================
Product: [Product Name]
Date: [Date]
Calculated By: [Name]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
APPLICABILITY CHECK
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Contains sweeteners: [YES/NO]
Contains conditionally processed sweeteners: [YES/NO]

Added sugar limits apply: [YES/NO]

[If NO: "Product is EXEMPT from added sugar limits per Section 6.3.2.6"]
[If YES: Continue below]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
PRODUCT CLASSIFICATION
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Product Type: [Type from Table 6-1]
Maximum Allowed: [X]%

Classification Rationale:
[Explanation for product type selection, especially if ambiguous]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
NUTRITION FACTS DATA
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Serving Size: [X]g
Added Sugars (per serving): [Y]g
  └─ Rounded (label): [Y]g
  └─ Unrounded (if available): [Y.Y]g

Data Source: [Nutrition Facts label / Manufacturer specification]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
CALCULATION
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Added Sugar % = (Added Sugars ÷ Serving Size) × 100

[If using unrounded:]
= ([Y.Y]g ÷ [X]g) × 100
= [Z.Z]%

[If using rounded:]
= ([Y]g ÷ [X]g) × 100
= [Z]%

Note: [Using unrounded values because: limit ≤5% / result close to limit / other reason]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
COMPLIANCE VERIFICATION
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Calculated Added Sugar: [Z.Z]%
Maximum Allowed: [X]%

[Z.Z]% [≤ or >] [X]%

RESULT: [PASS / FAIL]

Margin: [+/- X.X]% [above/below limit]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
NOTES & RECOMMENDATIONS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
[Any relevant notes about:]
- Calculation methodology
- Data sources
- Special considerations
- Proximity to limit
- Reformulation recommendations if failed

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
NEXT STEPS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
[If PASS: Continue with other formulation requirements]
[If FAIL: Reformulation required to reduce added sugar to ≤[X]%]
[If close to limit: Consider buffer for batch variation]
```

## Important Reminders

### When to Use Unrounded Values (6.3.2.5):
1. Product limit is 5% or less
2. Calculated result is within 0.5% of the limit (either direction)
3. When precision matters for compliance determination

### Good Faith Classification (6.3.2.4):
- Document reasoning when product type is ambiguous
- Consider primary product function
- Consider consumer perception and use case
- Lean toward more restrictive category when uncertain
- Maintain transparency in classification decisions

### Exempt Products:
Products containing ONLY permissible-processing sweeteners (e.g., honey, maple syrup, date syrup obtained through permissible methods) are not subject to these limits.

## Reference
Non-UPF Standard v1.0:
- Section 6.3.2 (Added Sugar Limits)
- Table 6-1 (Product Type and Added Sugar Limits)
- 21 CFR §101.9 (FDA Nutrition Labeling)

## Related Skills
- 02-processing-requirements-verification.md
- 03-formulation-requirements-verification.md
- 08-master-verification-checklist.md
