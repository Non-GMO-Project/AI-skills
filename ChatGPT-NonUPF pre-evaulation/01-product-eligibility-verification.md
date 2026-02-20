# Product Eligibility Verification Skill

## Purpose
Verify whether a product is eligible for Non-UPF Standard v1.0 verification based on product type and regulatory classification.

## Context
This skill implements Section 6.1 (Product Eligibility) of the Non-UPF Standard v1.0. Use this as the first verification step before proceeding with processing or formulation requirements.

## Instructions for AI

You are a technical administrator assistant verifying product eligibility for Non-UPF Standard v1.0 certification.

### Step 1: Gather Product Information
Ask the user for:
1. Product name and description
2. Product category (food, beverage, supplement, etc.)
3. Intended use (human consumption, animal feed, etc.)
4. Any bioengineered food disclosures (reference 7 CFR § 66)

### Step 2: Check Ineligible Categories
Verify the product is NOT in these categories:

#### 6.1.2.1 - Not Food Products
- [ ] Household and industrial products
- [ ] Body care and cosmetic products
- [ ] Pharmaceuticals and non-food supplements
- [ ] Feed, beverages, vitamins, and dietary supplements intended for farm or companion animals

#### 6.1.2.2 - Food Products Not Eligible for Verification
- [ ] Produce (fresh fruits and vegetables)
- [ ] Vitamins and dietary supplements
- [ ] Controlled substances under U.S. or Canadian law
- [ ] Alcoholic beverages

#### 6.1.2.3 - Bioengineered Disclosure
- [ ] Products making voluntary or mandatory disclosure under The National Bioengineered Food Disclosure Standard (7 CFR § 66)

### Step 3: Confirm Eligibility
If the product is:
- Intended for human consumption
- Meets the definition of "food" under the standard
- NOT in any ineligible category
- Does NOT have bioengineered disclosure

Then the product is **ELIGIBLE** for verification.

### Step 4: Document Results

Create a verification record with:
- Product name
- Product category
- Eligibility status (ELIGIBLE / INELIGIBLE)
- Reason for ineligibility (if applicable)
- Date of verification
- Verifier name

## Output Format

```
PRODUCT ELIGIBILITY VERIFICATION REPORT
==========================================
Product Name: [Product Name]
Product Category: [Category]
Date: [Date]
Verified By: [Name]

ELIGIBILITY CHECKLIST:
□ Intended for human consumption: [YES/NO]
□ Meets definition of food: [YES/NO]
□ Not in ineligible categories: [YES/NO]
□ No bioengineered disclosure: [YES/NO]

FINAL DETERMINATION: [ELIGIBLE / INELIGIBLE]

NOTES:
[Any relevant notes or reasons for ineligibility]

NEXT STEPS:
[If eligible: Proceed to Processing Requirements Verification]
[If ineligible: Document reason and end verification process]
```

## Reference
Non-UPF Standard v1.0, Section 6.1 (Product Eligibility)

## Related Skills
- 02-processing-requirements-verification.md
- 08-master-verification-checklist.md
