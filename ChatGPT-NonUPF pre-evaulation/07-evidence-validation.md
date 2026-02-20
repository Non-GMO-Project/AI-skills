# Evidence Validation Skill

## Purpose
Validate collected documentation and evidence to ensure it meets Non-UPF Standard v1.0 verification requirements and supports compliance claims.

## Context
This skill implements the critical review phase where collected documents are analyzed for completeness, accuracy, consistency, and compliance. Evidence validation ensures the integrity of the verification process.

## Instructions for AI

You are a technical administrator assistant validating evidence for Non-UPF Standard v1.0 verification.

### Step 1: Organize Evidence by Requirement

Map collected documents to specific standard requirements:
- Section 6.1: Product Eligibility
- Section 6.2: Processing Requirements
- Section 6.3: Formulation Requirements

### Step 2: Apply Validation Criteria

For each piece of evidence, evaluate:
1. **Completeness** - All required information present
2. **Accuracy** - Information is correct and precise
3. **Consistency** - Documents align with each other
4. **Currency** - Documents are current and up-to-date
5. **Authority** - Source is credible and authoritative
6. **Traceability** - Can trace claims back to evidence

### Step 3: Cross-Reference Documents

Verify consistency across multiple documents:
- Label matches formulation
- Formulation matches supplier specs
- Processing claims match supplier documentation
- Calculations are reproducible from provided data

### Step 4: Flag Discrepancies

Document any:
- Inconsistencies between documents
- Missing information
- Unclear or ambiguous statements
- Unverifiable claims
- Outdated information

### Step 5: Request Clarifications or Additional Evidence

For any deficiencies, prepare specific requests for:
- Additional documentation
- Clarifying statements
- Updated versions
- Supporting evidence

### Step 6: Make Determination

For each requirement, determine:
- **VERIFIED**: Evidence fully supports compliance
- **CONDITIONAL**: Compliance subject to confirmation of specific items
- **INSUFFICIENT**: Evidence does not support compliance claim
- **NON-COMPLIANT**: Evidence shows non-compliance

## Validation Checklist by Standard Section

### SECTION 6.1: PRODUCT ELIGIBILITY

**Evidence Required:**
- Product description and intended use
- Product category documentation
- Bioengineered disclosure statement (if applicable)

**Validation Criteria:**
□ Product clearly defined as food for human consumption
□ Product category documented and not in ineligible list
□ If bioengineered disclosure exists, verification halted (product ineligible)
□ Evidence is current and accurate

**Common Issues:**
- Vague product descriptions
- Unclear whether product is supplement or food
- Missing bioengineered status declaration

---

### SECTION 6.2: PROCESSING REQUIREMENTS

#### 6.2.1: Processing Classification

**Evidence Required:**
- Process flow diagrams for finished product
- Processing method descriptions for each ingredient
- Supplier specifications confirming processing methods
- Temperature, time, equipment specifications (where relevant)

**Validation Criteria:**
□ All processing methods clearly identified
□ Each method classified using Annex A
□ No prohibited methods used (or food safety exemption documented)
□ Conditional methods meet specified conditions
□ Documentation from authoritative sources (suppliers, manufacturers)

**Cross-Reference Checks:**
- Ingredient supplier specs match formulation processing claims
- Process flow diagram consistent with finished product processing description
- Equipment specifications support claimed processing methods

**Common Issues:**
- Generic processing terms without specific method identification
- Missing temperature specifications for thermal processes
- Vague supplier statements about processing
- Processing aids not disclosed or considered
- Inconsistent processing descriptions across documents

---

#### 6.2.2: Ingredient-Level Processing

**Evidence Required:**
- Complete formulation with weights
- Ingredient processing classifications
- Adjusted weight percentage calculations

**Validation Criteria:**
□ All ingredients listed with accurate weights
□ Water and salt clearly identified for adjusted weight calculation
□ Adjusted weight percentage calculation is correct
□ ≥70% ingredients are minimally/moderately processed (permissible methods)
□ ≤30% ingredients are conditionally processed
□ Calculations reproducible from provided data

**Calculation Verification:**
```
Step 1: Verify total product weight
Step 2: Subtract added water and salt
Step 3: Recalculate each ingredient's adjusted weight %
Step 4: Sum minimal/moderate processed ingredients
Step 5: Sum conditionally processed ingredients
Step 6: Verify thresholds met
```

**Common Issues:**
- Incorrect adjusted weight percentage calculations
- Water not properly excluded from calculations
- Salt not properly excluded from calculations
- Processing classification errors
- Ingredients near threshold not properly documented
- Sub-ingredients not properly accounted for

---

#### 6.2.3: Finished Product Processing

**Evidence Required:**
- Final processing steps applied to combined ingredients
- Process flow diagram
- Processing method classifications for final steps

**Validation Criteria:**
□ All final processing steps identified
□ Only permissible methods used on finished product
□ No conditional method applied to >30% of finished product
□ Process flow matches product description

**Common Issues:**
- Undisclosed processing steps
- Assumption that conditional methods used on ingredients can be reapplied
- Missing documentation of final product processing

---

### SECTION 6.3: FORMULATION REQUIREMENTS

#### 6.3.1: Prohibited Ingredients

**Evidence Required:**
- Ingredient statement (as labeled)
- Full ingredient disclosure including sub-ingredients
- Annex B cross-reference check completed

**Validation Criteria:**
□ Complete ingredient list obtained
□ All sub-ingredients disclosed
□ Each ingredient checked against Annex B
□ No prohibited ingredients present
□ Ambiguous ingredient names clarified

**Cross-Reference Checks:**
- Label ingredient statement matches formulation
- Supplier specs confirm ingredients not on prohibited list
- Processing aids disclosed and verified not prohibited

**Common Issues:**
- Incomplete sub-ingredient disclosure
- Generic ingredient names (e.g., "natural colors" without specifying which)
- Missing supplier confirmations
- Processing aids assumed to be exempt but actually prohibited
- Regional naming variations causing confusion

---

#### 6.3.2: Added Sugar Limits

**Evidence Required:**
- Nutrition Facts panel
- Product type classification rationale
- Added sugar calculation
- Unrounded values (if limit ≤5% or result close to limit)

**Validation Criteria:**
□ Product contains conditionally processed sweeteners (if not, exempt)
□ Product type classification reasonable and documented
□ Added sugar calculation correct
□ Appropriate data used (rounded vs. unrounded per 6.3.2.5)
□ Result complies with limit for product type
□ For dry mixes: as-prepared calculation provided

**Calculation Verification:**
```
Verify: (Added Sugar per serving ÷ Serving size) × 100 = Claimed %
Compare to: Maximum allowed % for product type
Check: Result ≤ Maximum
```

**Cross-Reference Checks:**
- Nutrition Facts matches formulation
- Added sugar values consistent across documents
- Product classification aligns with product description and marketing

**Common Issues:**
- Incorrect product type classification
- Calculation errors
- Using rounded values when unrounded required
- Dry mix calculations based on dry weight instead of prepared weight
- Ambiguous sweetener processing status

---

#### 6.3.3: Non-Nutritive & Biotransformed Sweeteners

**Evidence Required:**
- Complete sweetener ingredient list
- Sweetener specifications
- For any Stevia: documentation of whole-leaf or crude extract status

**Validation Criteria:**
□ No sweeteners with <2% caloric value of sucrose per unit sweetening
□ No biotransformed sweeteners present
□ If Stevia present: confirmed as whole-leaf or crude aqueous extract only
□ If Stevia present: confirmed flavor-level use (not replacing caloric sweeteners)

**Common Issues:**
- Steviol glycosides (prohibited) confused with whole-leaf stevia (conditionally allowed)
- Monk fruit extract (prohibited) not identified as non-nutritive
- Sugar alcohols (prohibited) present
- Allulose (prohibited) present
- Vague sweetener specifications

---

#### 6.3.4: Gums, Thickeners & Texturizers

**Evidence Required:**
- List of all gums/thickeners/texturizers
- Processing method for each
- If conditional allowance claimed: functional necessity documentation

**Validation Criteria:**
□ No prohibited gums per Annex B (carrageenan, microcrystalline cellulose, etc.)
□ No gums from industrial fermentation (xanthan, gellan)
□ No gums from enzymatic hydrolysis (maltodextrin, modified celluloses)
□ If gum used: functional necessity documented
□ If gum used: mechanical or aqueous extraction confirmed
□ If gum used: specific purpose documented (vitamin suspension OR gluten-free binding)
□ If gum used: documentation of no viable alternative

**Conditional Allowance Validation:**
Must have ALL of:
- Technical justification for functional necessity
- Confirmation of extraction method (mechanical or aqueous)
- Statement of specific purpose
- Evidence no minimally processed alternative available

**Common Issues:**
- Xanthan gum (prohibited) assumed to be allowed
- Pectin extraction method not specified
- Functional necessity claimed without supporting evidence
- Generic "texture" justification (insufficient)
- No documentation of alternative investigation

---

#### 6.3.5: Natural Flavors (Optional for v1.0)

**Evidence Required:**
- Natural flavor specifications
- Corresponding ingredient identification
- Weight data for flavors and corresponding ingredients
- Extract specifications (if applicable)

**Validation Criteria (if evaluated):**
□ Natural flavor doesn't imply absent ingredients
□ Corresponding ingredient present (from permissible processing)
□ Corresponding ingredient weight > flavor weight
□ Each natural flavor ≤0.5% (recommended)
□ Extracts meet exemption criteria (traditional methods, no additives)

**Note:** Compliance optional for v1.0, but collect data for future versions.

**Common Issues:**
- "Strawberry flavor" with no actual strawberries
- Flavor weight exceeds ingredient weight
- Extract contains carriers or preservatives
- Flavor used for masking rather than flavor enhancement

---

#### 6.3.6: Refined Oils

**Evidence Required:**
- Oil ingredient list
- Processing method for each oil
- Adjusted weight percentage for conditionally processed oils
- Supplier confirmations of processing methods

**Validation Criteria:**
□ No hydrogenated oils (partial or full)
□ No interesterified oils
□ No solvent extracted oils
□ No brominated vegetable oil
□ No cottonseed oil
□ RBD oils properly classified as conditional
□ Total conditionally processed oils ≤30% (adjusted weight %)

**Common Issues:**
- "Refined" oils assumed to be allowed without checking specific process
- Solvent extraction not disclosed by supplier
- Oil processing methods vaguely described
- Cottonseed oil overlooked as prohibited
- Incorrect calculation of oil percentage

---

#### 6.3.7: Sodium

**Evidence Required:**
- List of all sodium-containing ingredients
- Annex B cross-reference for sodium compounds
- Clarification of naturally occurring vs. added sodium ingredients

**Validation Criteria:**
□ No prohibited sodium-based preservatives
□ No prohibited sodium-based flavor enhancers (MSG, disodium guanylate, etc.)
□ No prohibited sodium-based leavening agents
□ No prohibited sodium-based chelators (EDTA variants)
□ No prohibited sodium-based emulsifiers
□ Naturally occurring sodium sources documented
□ Salt (sodium chloride) use documented

**Common Issues:**
- Sodium benzoate or sodium sorbate (preservatives) present
- MSG or related compounds not identified
- Sodium aluminum phosphate in baking powder
- Sodium-based emulsifiers in "clean label" formulations
- Confusion between sodium chloride (salt) and other sodium compounds

---

## Cross-Document Consistency Validation

### Label vs. Formulation
□ All label ingredients present in formulation
□ All formulation ingredients present on label (or exempt per labeling rules)
□ Order of ingredients matches weight order
□ Sub-ingredients disclosed consistently

### Formulation vs. Nutrition Facts
□ Serving size matches
□ Added sugars align with sweetener ingredients
□ Nutrient values reasonable for declared formulation

### Supplier Specs vs. Formulation Claims
□ Processing methods match supplier documentation
□ Ingredient names match
□ Specifications current (typically <1 year old)

### Processing Claims vs. Annex A Classifications
□ All claimed processing methods are classifiable under Annex A
□ Classifications accurate
□ Conditions met for conditional methods

---

## Evidence Quality Assessment

### Document Currency
- **Current**: <6 months old for specifications, <1 year for certifications
- **Acceptable**: <1 year for specs, <2 years for certifications (with confirmation no changes)
- **Outdated**: >1 year for specs, >2 years for certifications

### Source Authority
- **Primary**: Manufacturer, direct supplier, lab analysis
- **Secondary**: Distributor, broker with manufacturer documentation
- **Insufficient**: Generic claims, undocumented statements, third-party hearsay

### Specificity
- **Specific**: Exact values, named methods, identified sources
- **General**: Ranges, category descriptions, typical values
- **Vague**: "Natural", "minimal", "standard" without definition

---

## Output Format

```
EVIDENCE VALIDATION REPORT
===========================
Product: [Product Name]
Verification ID: [ID]
Date: [Date]
Validated By: [Name]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
VALIDATION SUMMARY
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Total Requirements Evaluated: [X]
Verified: [Y]
Conditional: [Z]
Insufficient Evidence: [W]
Non-Compliant: [V]

Overall Status: [VERIFIED / CONDITIONAL / INSUFFICIENT / NON-COMPLIANT]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
SECTION 6.1: PRODUCT ELIGIBILITY
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Status: [VERIFIED / CONDITIONAL / INSUFFICIENT / NON-COMPLIANT]

Evidence Reviewed:
- [Document 1]: [Quality assessment]
- [Document 2]: [Quality assessment]

Findings:
□ [Criterion]: [VERIFIED / ISSUE]
  Evidence: [Specific document reference]
  [If issue: Description and required action]

Cross-Reference Validation:
[Any consistency checks performed]

Discrepancies: [None / List]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
SECTION 6.2: PROCESSING REQUIREMENTS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Status: [VERIFIED / CONDITIONAL / INSUFFICIENT / NON-COMPLIANT]

6.2.1 Processing Classification
Evidence Reviewed:
- [Documents]

Validation Results:
Ingredient | Claimed Processing | Evidence | Classification | Status
-----------|-------------------|----------|----------------|--------
[Name]     | [Method]          | [Doc]    | [Class]        | ✓/✗/?

Issues Identified:
[None / List with specific concerns and required actions]

6.2.2 Ingredient-Level Processing
Calculation Verification:
Total product weight: [X]g
Less water: [Y]g
Less salt: [Z]g
Adjusted basis: [W]g

Ingredient | Weight | Adj. % | Processing | Classification
-----------|--------|--------|------------|----------------
[List all ingredients with verified data]

Verified Calculations:
✓ Minimal/Moderate processed: [X]% (require ≥70%)
✓ Conditionally processed: [Y]% (require ≤30%)

Calculation Review: [VERIFIED / ERRORS FOUND]
[If errors: Detail discrepancies and corrections]

6.2.3 Finished Product Processing
Processing Steps Validated:
1. [Step] - [Classification] - [Evidence] - [Status]
2. [Step] - [Classification] - [Evidence] - [Status]

Cross-Reference Results:
[Process flow vs. product description vs. manufacturing specs]

Issues: [None / List]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
SECTION 6.3: FORMULATION REQUIREMENTS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Status: [VERIFIED / CONDITIONAL / INSUFFICIENT / NON-COMPLIANT]

6.3.1 Prohibited Ingredients
Cross-Reference Completed: [YES / NO]
Total Ingredients Checked: [X]
Prohibited Ingredients Found: [Y]

[If Y > 0:]
PROHIBITED INGREDIENTS IDENTIFIED:
- [Ingredient] (matches Annex B: [prohibited ingredient name])
  Evidence: [Document]
  Action Required: [Reformulation required]

Label-Formulation Consistency: [VERIFIED / DISCREPANCIES]
[If discrepancies: Detail]

6.3.2 Added Sugar Limits
Applicability: [APPLIES / EXEMPT]
[If exempt: Reasoning]

[If applies:]
Product Type Validation:
Claimed: [Type]
Evidence: [Product description, marketing, format]
Assessment: [APPROPRIATE / QUESTIONABLE]
[If questionable: Reasoning and recommended classification]

Calculation Verification:
Serving size: [X]g (verified from: [source])
Added sugars: [Y]g (verified from: [source])
Calculated %: [Z]%
Maximum allowed: [W]%
Data type: [Rounded / Unrounded] (appropriate per 6.3.2.5: [YES/NO])

Result: [Z]% [≤ or >] [W]% → [COMPLIANT / NON-COMPLIANT]

Cross-Reference:
- Nutrition Facts vs. Formulation: [CONSISTENT / DISCREPANCY]
  [If discrepancy: Detail]

6.3.3 Non-Nutritive & Biotransformed Sweeteners
Sweeteners Identified: [List]

Validation Results:
Sweetener | Type | Caloric Value | Classification | Status
----------|------|---------------|----------------|--------
[Name]    | [Type]| [%]          | [Prohibited/Allowed] | ✓/✗

[If any Stevia:]
Stevia Specification Review:
- Product: [Whole-leaf / Crude extract / Isolated steviol glycosides]
- Processing: [Method]
- Use level: [Flavor-level / Replacing caloric sweeteners]
- Status: [ALLOWED / PROHIBITED]
- Evidence: [Document reference]

Issues: [None / List]

6.3.4 Gums, Thickeners & Texturizers
Gums/Thickeners Present: [List]

Validation Results:
Ingredient | Processing | Annex B Status | Conditional Allowance | Status
-----------|------------|----------------|----------------------|--------
[Name]     | [Method]   | [Prohibited/Not] | [Claimed/No]      | ✓/✗

[If conditional allowance claimed:]
Functional Necessity Validation:
- Purpose: [Vitamin suspension / Gluten-free binding / Other]
- Evidence provided: [Document references]
- Quality of evidence: [Sufficient / Insufficient]
- Alternative investigation: [Documented / Not documented]
- Extraction method confirmed: [Mechanical/Aqueous / Other]

Determination: [VALIDATED / REJECTED]
[If rejected: Reasoning]

6.3.5 Natural Flavors (Optional)
[If evaluated:]
Natural Flavors Present: [List]

Validation Results:
[Assessment of each criterion]

[If not evaluated:]
Natural flavors present but not evaluated (optional for v1.0).
Data collected for future reference.

6.3.6 Refined Oils
Oils Present: [List]

Validation Results:
Oil | Processing | Classification | Adj. % | Status
----|------------|----------------|--------|--------
[Name] | [Method] | [Conditional/Prohibited] | [X]% | ✓/✗

Total conditionally processed oils: [Y]%
Threshold: ≤30%
Result: [COMPLIANT / NON-COMPLIANT]

Issues: [None / List]

6.3.7 Sodium
Sodium Compounds Identified: [List]

Validation Results:
Compound | Category | Annex B Status | Evidence | Status
---------|----------|----------------|----------|--------
[Name]   | [Preservative/etc] | [Prohibited/Allowed] | [Doc] | ✓/✗

Issues: [None / List]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
CRITICAL ISSUES SUMMARY
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
[List all non-compliant findings]

1. [Issue]
   Section: [X.X.X]
   Evidence: [Document]
   Impact: [Verification blocking / Requires reformulation / etc.]
   Action Required: [Specific corrective action]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
CONDITIONAL ITEMS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
[List items requiring clarification or additional evidence]

1. [Item]
   Section: [X.X.X]
   Current Evidence: [What's available]
   Deficiency: [What's missing or unclear]
   Required Action: [Specific request]
   Impact if Unresolved: [Consequence]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
MINOR ISSUES / RECOMMENDATIONS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
[Non-blocking items that should be addressed]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
FINAL DETERMINATION
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
VERIFICATION STATUS: [APPROVED / CONDITIONAL / REJECTED]

[If APPROVED:]
All requirements verified. Product complies with Non-UPF Standard v1.0.
Proceed to final verification report.

[If CONDITIONAL:]
Product may comply subject to resolution of [X] conditional items listed above.
Cannot issue verification until all conditions satisfied.

[If REJECTED:]
Product does not comply with Non-UPF Standard v1.0 due to [X] critical issues.
Reformulation required. Re-verification needed after corrections.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
NEXT STEPS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
1. [Action with responsible party and deadline]
2. [Action with responsible party and deadline]
3. [Action with responsible party and deadline]

Follow-up Validation Date: [Date]

Validator Signature: _______________________ Date: _______
```

## Tips for Effective Validation

### Be Systematic
Work through requirements in order. Don't skip sections even if they seem simple.

### Document Everything
Note which specific documents were reviewed for each finding. Create audit trail.

### Question Inconsistencies
Don't accept contradictions between documents. Demand clarification.

### Verify Calculations
Always recalculate percentages and thresholds. Don't trust provided calculations without verification.

### Use Professional Skepticism
Approach validation with appropriate skepticism. Verify rather than accept claims.

### Distinguish Between Non-Compliance and Insufficient Evidence
- Non-compliance: Evidence shows product doesn't meet requirements
- Insufficient evidence: Can't determine compliance from available evidence

### Request Specific Evidence
When evidence is insufficient, don't accept vague assurances. Request specific documentation.

## Reference
Non-UPF Standard v1.0: All sections

## Related Skills
- 01-product-eligibility-verification.md
- 02-processing-requirements-verification.md
- 03-formulation-requirements-verification.md
- 04-prohibited-ingredients-checker.md
- 05-added-sugar-calculator.md
- 06-documentation-collection.md
- 08-master-verification-checklist.md
