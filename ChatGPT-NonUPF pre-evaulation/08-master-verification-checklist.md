# Master Verification Checklist Skill

## Purpose
Comprehensive end-to-end checklist for complete Non-UPF Standard v1.0 product verification, integrating all verification steps and skills.

## Context
This skill serves as the master workflow coordinator, guiding technical administrators through the complete verification process from initial eligibility check through final determination.

## Instructions for AI

You are a technical administrator assistant conducting comprehensive Non-UPF Standard v1.0 verification.

### Verification Workflow

This master checklist integrates all specialized skills in proper sequence:

1. **Product Eligibility** (Skill 01)
2. **Processing Requirements** (Skill 02)
3. **Formulation Requirements** (Skill 03)
   - Including Prohibited Ingredients (Skill 04)
   - Including Added Sugar Calculation (Skill 05)
4. **Documentation Collection** (Skill 06)
5. **Evidence Validation** (Skill 07)
6. **Final Verification Report** (This skill)

### How to Use This Checklist

- Work through sections sequentially
- Complete all items in each section before proceeding
- Mark items as: ✓ Complete | ✗ Non-Compliant | ○ Pending | N/A Not Applicable
- Document all findings and evidence references
- Stop at any critical failure and document corrective actions needed
- Track status and progress throughout verification process

---

## MASTER VERIFICATION CHECKLIST

```
NON-UPF STANDARD v1.0 VERIFICATION
====================================
Product Name: _________________________________
Company: ______________________________________
Verification ID: ______________________________
Start Date: ___________________________________
Target Completion: ____________________________
Technical Administrator: ______________________

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
PHASE 1: PRODUCT ELIGIBILITY (Section 6.1)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Reference: Skill 01-product-eligibility-verification.md

□ Product information received
  Date: _______ Evidence: _________________

6.1.1 Eligible Goods
□ Product meets definition of "food"
  Finding: ________________________________
  Evidence: _______________________________

□ Product intended for human consumption
  Finding: ________________________________
  Evidence: _______________________________

6.1.2 Ineligible Goods - Verify product is NOT:
□ Household/industrial product
□ Body care/cosmetic product
□ Pharmaceutical/non-food supplement
□ Animal feed/supplement
□ Produce (fresh fruits/vegetables)
□ Vitamin/dietary supplement
□ Controlled substance
□ Alcoholic beverage
□ Subject to bioengineered food disclosure (7 CFR § 66)

  Bioengineered Status Verified: __________
  Evidence: _______________________________

PHASE 1 RESULT: [ELIGIBLE / INELIGIBLE]

If INELIGIBLE:
  Reason: _________________________________
  STOP - Product cannot be verified

If ELIGIBLE: Proceed to Phase 2

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
PHASE 2: PROCESSING REQUIREMENTS (Section 6.2)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Reference: Skill 02-processing-requirements-verification.md

Documentation Received:
□ Complete ingredient list with weights
  Date: _______ Document: ________________
□ Processing methods for all ingredients
  Date: _______ Document: ________________
□ Supplier specifications confirming processing
  Date: _______ Document: ________________
□ Finished product process flow diagram
  Date: _______ Document: ________________

6.2.1 Processing Classification

INGREDIENT PROCESSING REVIEW:
Total Ingredients: _____

For each ingredient, classify processing:
[Use table format or list]

Ingredient | Weight | Processing Method | Classification | Evidence | Status
-----------|--------|-------------------|----------------|----------|--------
1. _______ | ____g  | _______________ | P/C/Pe-Min/Pe-Mod | ______ | ✓/✗/○
2. _______ | ____g  | _______________ | P/C/Pe-Min/Pe-Mod | ______ | ✓/✗/○
[Continue for all ingredients]

Legend: P=Prohibited, C=Conditional, Pe-Min=Permissible-Minimal, Pe-Mod=Permissible-Moderate

□ All ingredient processing methods classified
□ No prohibited methods identified (OR)
□ Food safety exemption documented for prohibited method (6.2.1.5)
  Exemption Details: ______________________
  Justification: __________________________
  Evidence: _______________________________

6.2.2 Ingredient-Level Processing Calculations

Total Product Weight: _________ g
Added Water: _________ g
Added Salt: _________ g
Adjusted Basis: _________ g (Total - Water - Salt)

ADJUSTED WEIGHT PERCENTAGE CALCULATIONS:
[Recalculate and verify]

Ingredient | Weight (g) | Adjusted % | Classification
-----------|------------|------------|----------------
[List all except water and salt]

THRESHOLD VERIFICATION:
□ Sum of minimally/moderately processed (permissible): _____%
  Requirement: ≥70%
  Status: [PASS / FAIL]

□ Sum of conditionally processed: _____%
  Requirement: ≤30%
  Status: [PASS / FAIL]

Calculations verified by: _______________
Verification method: ____________________

6.2.3 Finished Product Processing

Finished Product Processing Steps:
1. _________________ Classification: _______ Evidence: ________
2. _________________ Classification: _______ Evidence: ________
3. _________________ Classification: _______ Evidence: ________

□ All steps classified as permissible
  Status: [PASS / FAIL]

□ No conditional method applied to >30% of finished product
  If conditional methods used: ____________
  Applied to: _____% of product
  Status: [PASS / FAIL]

PHASE 2 RESULT: [COMPLIANT / NON-COMPLIANT]

If NON-COMPLIANT:
  Issues: _________________________________
  Corrective Action Required: ______________

If COMPLIANT: Proceed to Phase 3

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
PHASE 3: FORMULATION REQUIREMENTS (Section 6.3)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Reference: Skill 03-formulation-requirements-verification.md

Documentation Received:
□ Ingredient statement (as labeled)
  Date: _______ Document: ________________
□ Full formulation with sub-ingredients
  Date: _______ Document: ________________
□ Nutrition Facts panel
  Date: _______ Document: ________________
□ Supplier specifications for all ingredients
  Date: _______ Document: ________________

────────────────────────────────────────────────
6.3.1 PROHIBITED INGREDIENTS
────────────────────────────────────────────────
Reference: Skill 04-prohibited-ingredients-checker.md

□ Annex B cross-reference completed
  Date: _______ Completed by: _____________

Total Ingredients Checked: _____
Prohibited Ingredients Found: _____

[If any found:]
PROHIBITED INGREDIENTS:
1. _____________ (Matches Annex B: ____________)
   Evidence: _____________________________
   Action Required: Reformulation

[If none found:]
□ No prohibited ingredients identified
□ All ingredients verified against Annex B
□ Ambiguous ingredients clarified

RESULT: [COMPLIANT / NON-COMPLIANT]

────────────────────────────────────────────────
6.3.2 ADDED SUGAR LIMITS
────────────────────────────────────────────────
Reference: Skill 05-added-sugar-calculator.md

□ Applicability determined
  Contains conditionally processed sweeteners: [YES / NO]

[If NO: Mark N/A and skip to 6.3.3]
[If YES: Complete below]

Product Type Classification:
  Classified as: ___________________________
  Rationale: _______________________________
  Maximum Allowed: _____%

Nutrition Facts Data:
  Serving Size: _____ g
  Added Sugars: _____ g (per serving)
  Unrounded values used: [YES / NO]
  Reason for unrounded: ____________________

Calculation:
  (_____ g ÷ _____ g) × 100 = _____%

  Calculated: _____%
  Maximum: _____%

□ Added sugar calculation verified
  Verified by: _____________________________

□ Product complies with added sugar limit
  Status: [COMPLIANT / NON-COMPLIANT]
  Margin: ± _____%

Special Cases:
□ Dry Mix: As-prepared calculation performed
  [If applicable, document]

RESULT: [COMPLIANT / NON-COMPLIANT / N/A]

────────────────────────────────────────────────
6.3.3 NON-NUTRITIVE & BIOTRANSFORMED SWEETENERS
────────────────────────────────────────────────

Sweeteners Present:
1. _______________ Type: ________ Status: _____
2. _______________ Type: ________ Status: _____

□ No non-nutritive sweeteners present
  (<2% caloric value of sucrose)

□ No biotransformed sweeteners present

□ Stevia exception (if applicable)
  Type: [Whole-leaf / Crude extract / Steviol glycosides]
  Use level: [Flavor-level / Caloric replacement]
  Processing: ______________________________
  Evidence: ________________________________
  Status: [ALLOWED / PROHIBITED]

RESULT: [COMPLIANT / NON-COMPLIANT]

────────────────────────────────────────────────
6.3.4 GUMS, THICKENERS & TEXTURIZERS
────────────────────────────────────────────────

Gums/Thickeners Present:
1. _______________ Processing: ________ Status: _____
2. _______________ Processing: ________ Status: _____

□ No prohibited gums per Annex B
  (carrageenan, microcrystalline cellulose, polysorbates, etc.)

□ No gums from industrial fermentation
  (xanthan, gellan, etc.)

□ No gums from enzymatic hydrolysis
  (maltodextrin, modified celluloses)

Conditional Allowance Claimed: [YES / NO]

[If YES:]
Ingredient: _________________________________
Purpose: [Vitamin suspension / Gluten-free binding]
Functional Necessity Evidence: ______________
  Document: _________________________________
Extraction Method: [Mechanical / Aqueous]
  Confirmed by: _____________________________
No Alternative Available: ___________________
  Evidence: _________________________________

□ Conditional allowance validated
  Status: [VALIDATED / REJECTED]

RESULT: [COMPLIANT / NON-COMPLIANT]

────────────────────────────────────────────────
6.3.5 NATURAL FLAVORS (OPTIONAL for v1.0)
────────────────────────────────────────────────

Evaluation Performed: [YES / NO]

[If YES:]
Natural Flavors Present: ____________________

□ No misleading flavor implications
□ Corresponding ingredients present
□ Ingredient weight > flavor weight
□ Each flavor ≤0.5% formulation (recommended)

Extract Exemptions:
[List any traditional extracts exempt]

RESULT: [COMPLIANT / INFO ONLY / NOT EVALUATED]

────────────────────────────────────────────────
6.3.6 REFINED OILS
────────────────────────────────────────────────

Oils Present:
1. _____________ Processing: _______ Adj. %: ____%
2. _____________ Processing: _______ Adj. %: ____%

□ No hydrogenated oils (partial or full)
□ No interesterified oils
□ No solvent extracted oils
□ No brominated vegetable oil
□ No cottonseed oil

Conditionally Processed Oils:
  Total: _____%
  Threshold: ≤30%
  Status: [COMPLIANT / NON-COMPLIANT]

RESULT: [COMPLIANT / NON-COMPLIANT]

────────────────────────────────────────────────
6.3.7 SODIUM
────────────────────────────────────────────────

Sodium-Containing Ingredients:
1. _______________ Category: _______ Status: _____
2. _______________ Category: _______ Status: _____

□ No sodium-based preservatives
  (sodium benzoate, sodium sorbate, etc.)

□ No sodium-based flavor enhancers
  (MSG, disodium guanylate, disodium inosinate)

□ No sodium-based leavening agents
  (sodium aluminum phosphate, sodium aluminum sulfate)

□ No sodium-based chelators
  (EDTA variants)

□ No sodium-based emulsifiers
  (sodium stearoyl lactylate, etc.)

□ Naturally occurring sodium documented
□ Salt (NaCl) use documented

RESULT: [COMPLIANT / NON-COMPLIANT]

────────────────────────────────────────────────

PHASE 3 OVERALL RESULT: [COMPLIANT / NON-COMPLIANT]

If NON-COMPLIANT:
  Issues: _________________________________
  Sections Failed: _________________________
  Corrective Action Required: ______________

If COMPLIANT: Proceed to Phase 4

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
PHASE 4: DOCUMENTATION COLLECTION
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Reference: Skill 06-documentation-collection.md

Documentation Tracking:
  Total Documents Required: _____
  Documents Received: _____
  Documents Verified: _____
  Documents Deficient: _____

□ All required documentation collected
  Collection complete date: _______________

□ Document repository organized
  Location: _______________________________

□ Document naming conventions followed

□ Version control maintained

Outstanding Documents:
[List any pending documents with due dates]

Deficiencies Identified:
[List any document quality issues requiring correction]

PHASE 4 RESULT: [COMPLETE / PENDING]

If PENDING:
  Outstanding Items: _______________________
  Expected Completion: _____________________
  Cannot proceed to evidence validation

If COMPLETE: Proceed to Phase 5

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
PHASE 5: EVIDENCE VALIDATION
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Reference: Skill 07-evidence-validation.md

Validation Performed By: ____________________
Validation Date: ____________________________

CROSS-DOCUMENT CONSISTENCY CHECKS:

□ Label vs. Formulation consistency
  Status: [CONSISTENT / DISCREPANCIES]
  [If discrepancies: Detail]

□ Formulation vs. Nutrition Facts consistency
  Status: [CONSISTENT / DISCREPANCIES]
  [If discrepancies: Detail]

□ Supplier specs vs. Formulation claims consistency
  Status: [CONSISTENT / DISCREPANCIES]
  [If discrepancies: Detail]

□ Processing claims vs. Annex A classifications
  Status: [VERIFIED / ERRORS]
  [If errors: Detail]

EVIDENCE QUALITY ASSESSMENT:

□ Document currency verified
  All documents current: [YES / NO]
  Outdated documents: _____________________

□ Source authority verified
  All sources authoritative: [YES / NO]
  Weak sources: ___________________________

□ Evidence specificity adequate
  All evidence specific: [YES / NO]
  Vague evidence: _________________________

CALCULATION VERIFICATION:

□ Adjusted weight percentages recalculated
  Result: [MATCHES / ERRORS]
  [If errors: Detail]

□ Added sugar calculation recalculated
  Result: [MATCHES / ERRORS / N/A]
  [If errors: Detail]

□ All claimed thresholds verified
  Result: [VERIFIED / DISCREPANCIES]
  [If discrepancies: Detail]

VALIDATION SUMMARY:

Total Requirements: _____
  Verified: _____
  Conditional: _____
  Insufficient Evidence: _____
  Non-Compliant: _____

PHASE 5 RESULT: [VERIFIED / CONDITIONAL / INSUFFICIENT / NON-COMPLIANT]

Critical Issues:
[List all blocking issues]

Conditional Items:
[List items requiring clarification]

If NOT VERIFIED:
  Required Actions: ________________________
  Re-validation Date: ______________________
  Cannot proceed to final determination

If VERIFIED: Proceed to Phase 6

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
PHASE 6: FINAL DETERMINATION
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

VERIFICATION SUMMARY:

Phase 1 - Product Eligibility: [PASS / FAIL]
Phase 2 - Processing Requirements: [PASS / FAIL]
Phase 3 - Formulation Requirements: [PASS / FAIL]
Phase 4 - Documentation Collection: [COMPLETE / INCOMPLETE]
Phase 5 - Evidence Validation: [VERIFIED / NOT VERIFIED]

COMPLIANCE DETERMINATION:

All normative requirements met: [YES / NO]

Good faith compliance verified: [YES / NO]
  (No circumvention of standard intent per Section 3)

Partial compliance rejected: [CONFIRMED]
  (All requirements must be met per Section 3)

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
FINAL VERIFICATION DECISION
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

[   ] VERIFIED - APPROVED FOR NON-UPF CERTIFICATION
      Product complies with all requirements of Non-UPF Standard v1.0

      Verification Date: ______________________
      Valid Until: __________________________
      Certificate Number: ____________________

[   ] CONDITIONAL VERIFICATION
      Product may comply subject to resolution of:
      [List conditions]

      Re-verification required upon resolution
      Conditional status expires: _____________

[   ] VERIFICATION DENIED
      Product does not comply with Non-UPF Standard v1.0

      Reason(s) for Denial:
      [List all non-compliances]

      Required Actions:
      [List corrective actions]

      Re-application permitted after: _________

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
VERIFICATION RECORD
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Product: ___________________________________
Company: ___________________________________
Verification ID: ___________________________

Verification Team:
  Lead Technical Administrator: ___________
  Supporting Staff: _______________________

Verification Period:
  Start Date: _____________________________
  Completion Date: ________________________

Total Hours: _______________________________

Documents Reviewed: ________________________
Suppliers Contacted: _______________________
Issues Resolved: ___________________________

Special Notes:
[Any noteworthy aspects of verification]

Signatures:

Technical Administrator: ___________________ Date: ________

Quality Reviewer: __________________________ Date: ________

Program Manager: ___________________________ Date: ________

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
VERIFICATION COMPLETE
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

## Workflow Management Tips

### Sequential Completion
Complete phases in order. Don't skip ahead even if later information is available.

### Gate Checks
Each phase serves as a gate. Don't proceed to next phase if current phase fails or is incomplete.

### Document Everything
Every checkbox should have supporting evidence documented.

### Use Specialized Skills
Reference and use the specialized skills (01-07) for detailed work within each phase.

### Track Time
Monitor time spent in each phase to identify bottlenecks and improve efficiency.

### Communication
Maintain regular communication with product manufacturer throughout process, especially when requesting corrections or clarifications.

### Maintain Objectivity
Apply standard uniformly without bias toward approval or denial. Let evidence determine outcome.

## Common Verification Pathways

### Fast-Track (Simple Products)
- Clear eligibility
- Simple processing (mainly permissible methods)
- No prohibited ingredients
- No sweeteners or exempt from added sugar limits
- Minimal gums/thickeners if any
- Complete documentation

Typical timeline: 2-4 weeks

### Standard Verification (Moderate Complexity)
- Clear eligibility
- Mix of permissible and conditional processing
- Some complex ingredients requiring supplier documentation
- Added sugar calculation required
- Some conditional allowances claimed
- Documentation requires follow-up

Typical timeline: 4-8 weeks

### Complex Verification (High Complexity)
- Formulation near threshold limits
- Multiple conditional processing methods
- Conditional allowances requiring extensive justification
- Ambiguous product classification
- Extensive supplier documentation required
- Multiple rounds of clarification needed

Typical timeline: 8-12+ weeks

## Escalation Procedures

### When to Escalate
- Ambiguous standard interpretation
- Novel ingredients or processing methods not clearly covered
- Conflicts between requirements
- Evidence of potential circumvention attempts
- Significant non-compliance requiring policy decision

### How to Escalate
Document issue clearly with:
- Specific standard section reference
- Evidence of the issue
- Your preliminary assessment
- Question or decision needed
- Impact on verification timeline

## Continuous Improvement

### Track Metrics
- Average verification time by phase
- Common documentation deficiencies
- Frequent non-compliances
- Supplier response times
- Re-verification rates

### Identify Patterns
- Which product types have most issues?
- Which requirements cause most confusion?
- Which suppliers provide best documentation?
- Which verification steps take longest?

### Update Procedures
- Refine checklists based on experience
- Develop templates for common issues
- Create guidance for ambiguous situations
- Share learnings across technical administrators

## Reference
Non-UPF Standard v1.0: All sections (comprehensive)

## Related Skills
- 01-product-eligibility-verification.md
- 02-processing-requirements-verification.md
- 03-formulation-requirements-verification.md
- 04-prohibited-ingredients-checker.md
- 05-added-sugar-calculator.md
- 06-documentation-collection.md
- 07-evidence-validation.md

---

## Quick Reference: Phase Dependencies

```
Phase 1: Product Eligibility
   ↓ [If ELIGIBLE]
Phase 2: Processing Requirements
   ↓ [If COMPLIANT]
Phase 3: Formulation Requirements
   ↓ [If COMPLIANT]
Phase 4: Documentation Collection
   ↓ [If COMPLETE]
Phase 5: Evidence Validation
   ↓ [If VERIFIED]
Phase 6: Final Determination
   → APPROVED / CONDITIONAL / DENIED
```

Each phase is dependent on successful completion of the previous phase.

## Archive and Retention

Maintain complete verification file including:
- All checklists (completed)
- All documentation received
- All correspondence
- All calculations and verification work
- Final determination letter
- Any appeals or amendments

Retention period: Minimum 5 years or per regulatory requirements
