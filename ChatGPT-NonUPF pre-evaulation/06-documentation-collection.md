# Documentation Collection Skill

## Purpose
Systematically collect all required documentation and evidence needed for Non-UPF Standard v1.0 verification.

## Context
This skill helps technical administrators gather complete documentation packages for product verification. Proper documentation is essential for audit trails and compliance validation.

## Instructions for AI

You are a technical administrator assistant collecting documentation for Non-UPF Standard v1.0 verification.

### Step 1: Create Documentation Checklist

For each product verification, create a comprehensive documentation request list covering all standard requirements.

### Step 2: Organize Documentation by Category

Structure requests into logical groups:
1. Product Identity Documents
2. Formulation Documents
3. Processing Documents
4. Label and Marketing Materials
5. Supplier Documentation
6. Supporting Evidence

### Step 3: Request Specific Documents

Guide the user through collecting each required document with clear explanations of what's needed and why.

### Step 4: Track Document Status

Maintain a tracking system showing:
- Document requested
- Document received
- Document verified
- Document deficiencies

### Step 5: Create Document Repository

Organize collected documents in a structured format with:
- Clear naming conventions
- Version control
- Date stamps
- Responsible parties

## Required Documentation Checklist

### CATEGORY 1: PRODUCT IDENTITY
```
□ Product name (official/legal name)
□ Brand name
□ Product description
□ UPC/barcode
□ Product photos (front, back, sides showing all label panels)
□ Current product label (high resolution)
□ Product category/classification
□ Intended market (US, Canada, Mexico, etc.)
□ Target consumer demographic
□ Shelf life and storage requirements
```

### CATEGORY 2: FORMULATION DOCUMENTS
```
□ Complete ingredient statement (as appears on label)
□ Full formulation with sub-ingredients disclosed
□ Ingredient weights (in grams or by percentage)
□ Total product weight
□ Serving size
□ Nutrition Facts panel (current)
□ Added sugars calculation (if applicable)
  └─ Unrounded values
  └─ Calculation methodology
□ Product type classification rationale (for added sugar limits)
□ Adjusted weight percentage calculations
□ Total weight percentage calculations
```

### CATEGORY 3: PROCESSING INFORMATION
```
For EACH ingredient:
□ Ingredient name
□ Supplier name and contact
□ Processing method(s) used
□ Processing classification (Prohibited/Conditional/Permissible)
□ If conditional: justification and conditions met
□ Source material (raw material before processing)
□ Country of origin

For FINISHED PRODUCT:
□ Manufacturing process flow diagram
□ Processing steps applied to combined ingredients
□ Processing method classification for each step
□ Processing temperatures (if applicable)
□ Processing times (if applicable)
□ Equipment used
□ Co-manufacturing facility information (if applicable)
```

### CATEGORY 4: INGREDIENT-SPECIFIC DOCUMENTATION

#### For Natural Flavors (if present):
```
□ Natural flavor specification sheets
□ Corresponding ingredient identification
□ Weight comparison (ingredient vs. flavor)
□ Flavor source materials
□ Processing methods used for flavor extraction
□ Certification that flavor doesn't imply absent ingredients
```

#### For Gums/Thickeners (if conditional allowance claimed):
```
□ Functional necessity justification
□ Specific purpose (vitamin suspension / gluten-free binding)
□ Documentation of no viable alternative
□ Technical specification showing mechanical or aqueous extraction
□ Supplier confirmation of processing method
```

#### For Refined Oils (if present):
```
□ Oil type and source
□ Refining process description
□ Processing classification
□ Adjusted weight percentage calculation
□ Confirmation total refined oils ≤30%
```

#### For Extracts:
```
□ Extract specification
□ Source material identification
□ Extraction method (maceration/percolation/distillation/pressing)
□ Confirmation: no carriers, preservatives, or stabilizers
□ Certificate of analysis
```

### CATEGORY 5: COMPLIANCE DECLARATIONS
```
□ Prohibited ingredients checklist (Annex B) - completed
□ Declaration: No bioengineered ingredients (7 CFR § 66)
□ Declaration: No precision fermentation ingredients
□ Declaration: No synthetic biology ingredients
□ Declaration: No 3D printed components
□ Declaration: No nanotechnology
□ Declaration: Product reformulated in good faith (if applicable)
□ Food safety exemption justification (if any prohibited methods used)
```

### CATEGORY 6: SUPPLIER DOCUMENTATION
```
For EACH supplier (especially for complex/processed ingredients):
□ Supplier name and contact information
□ Ingredient specification sheet
□ Processing method description
□ Certificate of Analysis (COA)
□ Allergen statement
□ GMO status declaration
□ Processing aid disclosure
□ Country of origin certificate
□ Supplier audit report (if available)
□ Third-party certifications (if applicable)
```

### CATEGORY 7: LABEL AND MARKETING MATERIALS
```
□ All product labels (current version)
□ Previous labels (if recently changed)
□ Marketing claims review
□ Website product descriptions
□ Packaging specifications
□ Label approval documentation
□ Compliance with regional labeling laws
```

### CATEGORY 8: QUALITY AND SAFETY
```
□ Allergen control documentation
□ HACCP plan (if applicable)
□ Food safety plan
□ Quality control procedures
□ Testing protocols
□ Batch records (sample)
□ Recall procedures
□ Traceability system documentation
```

### CATEGORY 9: VERIFICATION HISTORY
```
□ Previous Non-UPF verification status (if applicable)
□ Other certifications held (organic, Non-GMO Project, etc.)
□ Audit history
□ Non-conformance reports and corrective actions
□ Formula change history
□ Supplier change documentation
```

### CATEGORY 10: SPECIAL CIRCUMSTANCES
```
□ Food safety exemption documentation (Section 6.2.1.5)
  └─ Demonstration of essentiality
  └─ Proof no viable alternative exists
  └─ Evidence of maintained nutritional integrity

□ Dry mix preparation instructions
  └─ Standard preparation method
  └─ As-prepared serving size
  └─ As-prepared nutrition facts

□ Conditional processing justification
  └─ Specific conditions met
  └─ Supporting evidence

□ Product type classification rationale (for ambiguous products)
  └─ Decision-making process
  └─ Factors considered
  └─ Good faith determination basis
```

## Document Naming Convention

Establish consistent naming for all collected documents:

```
[Company]_[Product Name]_[Document Type]_[Version]_[Date]

Examples:
- AcmeFoods_OatmealRaisin_Formulation_v2_2025-01-13.pdf
- AcmeFoods_OatmealRaisin_Label_v1_2025-01-13.pdf
- AcmeFoods_OatmealRaisin_ProcessFlowDiagram_v1_2025-01-13.pdf
- AcmeFoods_OatmealRaisin_SupplierCOA_Oats_2025-01-13.pdf
```

## Output Format

```
DOCUMENTATION COLLECTION TRACKER
==================================
Product: [Product Name]
Company: [Company Name]
Verification ID: [ID Number]
Date Started: [Date]
Collected By: [Name]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
DOCUMENTATION STATUS OVERVIEW
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Total Documents Required: [X]
Received: [Y]
Verified: [Z]
Pending: [X-Y]
Deficient: [W]

Completion: [Z/X] ([percentage]%)

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
CATEGORY 1: PRODUCT IDENTITY
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Document                    | Status    | Date Received | Notes
----------------------------|-----------|---------------|-------
Product Label               | ✓ Verified| 2025-01-13   | Current
Product Photos              | ○ Pending |              | Requested 1/13
UPC/Barcode                 | ✓ Received| 2025-01-13   | Need verification
...

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
CATEGORY 2: FORMULATION DOCUMENTS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Document                    | Status    | Date Received | Notes
----------------------------|-----------|---------------|-------
Ingredient Statement        | ✓ Verified| 2025-01-13   | Matches label
Full Formulation            | ✓ Received| 2025-01-13   | Need to verify weights
Nutrition Facts             | ✓ Verified| 2025-01-13   | Current
...

[Repeat for each category]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
OUTSTANDING REQUESTS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Priority | Document               | Requested | Due Date  | Assigned To
---------|------------------------|-----------|-----------|-------------
HIGH     | Processing flow diagram| 2025-01-10| 2025-01-17| J. Smith
MEDIUM   | Supplier COA - Oats    | 2025-01-13| 2025-01-20| M. Jones
...

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
DEFICIENCIES IDENTIFIED
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Document               | Issue                          | Action Required
-----------------------|--------------------------------|------------------
Natural Flavor Spec    | Missing processing method      | Request updated spec
Oil Supplier COA       | Doesn't specify refining temp  | Request clarification
...

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
DOCUMENT REPOSITORY STRUCTURE
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
/Product_Verification/
  /[Product_Name]/
    /01_Product_Identity/
      - [files listed]
    /02_Formulation/
      - [files listed]
    /03_Processing/
      - [files listed]
    /04_Supplier_Documents/
      /[Supplier_Name]/
        - [files listed]
    /05_Labels_Marketing/
      - [files listed]
    /06_Quality_Safety/
      - [files listed]
    /07_Verification_Reports/
      - [files listed]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
NEXT STEPS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
1. [Action item with responsible party and due date]
2. [Action item with responsible party and due date]
3. [Action item with responsible party and due date]

Follow-up scheduled for: [Date]

DOCUMENTATION COMPLETE: [YES / NO]

[If NO: "Cannot proceed to evidence validation until all required documents received and verified"]
[If YES: "Ready to proceed to evidence validation (Skill 07)"]
```

## Communication Templates

### Initial Documentation Request Email

```
Subject: Non-UPF Verification - Documentation Request for [Product Name]

Dear [Contact Name],

We are initiating Non-UPF Standard v1.0 verification for [Product Name].
To proceed with the verification process, we require the following documentation:

IMMEDIATE PRIORITY (needed within 5 business days):
- [List high-priority items]

STANDARD DOCUMENTATION (needed within 10 business days):
- [List standard items]

Please submit all documents using the following naming convention:
[Company]_[Product]_[DocumentType]_[Version]_[Date]

Upload documents to: [portal/email/location]

Please let me know if you have any questions about these requirements.

Best regards,
[Your Name]
Technical Administrator
```

### Follow-Up Request

```
Subject: FOLLOW-UP: Outstanding Documentation for [Product Name]

Dear [Contact Name],

The following documents remain outstanding for Non-UPF verification of [Product Name]:

OVERDUE:
- [List overdue items with original request date]

DUE SOON:
- [List items due within next few days]

Please prioritize these submissions to avoid delays in the verification process.

Best regards,
[Your Name]
```

### Deficiency Notice

```
Subject: Document Deficiency - Action Required for [Product Name]

Dear [Contact Name],

We have reviewed the submitted documentation for [Product Name] and identified
the following deficiencies that require correction:

DEFICIENCY 1: [Document Name]
Issue: [Specific problem]
Required Action: [What needs to be provided or corrected]

DEFICIENCY 2: [Document Name]
Issue: [Specific problem]
Required Action: [What needs to be provided or corrected]

Please resubmit corrected documentation by [Date] to maintain the verification timeline.

Best regards,
[Your Name]
```

## Tips for Efficient Collection

### Batch Requests
Group related documents in requests to suppliers rather than requesting one at a time.

### Use Templates
Provide suppliers with document templates or specification sheet templates to standardize submissions.

### Clear Deadlines
Set specific deadlines and communicate consequences of missed deadlines.

### Regular Check-ins
Schedule regular status meetings to review outstanding documentation.

### Digital Repository
Maintain organized digital repository with version control and access logs.

### Verification Alongside Collection
Begin preliminary verification of documents as they're received rather than waiting for complete submission.

## Reference
Non-UPF Standard v1.0: All sections (comprehensive documentation needed)

## Related Skills
- 01-product-eligibility-verification.md
- 02-processing-requirements-verification.md
- 03-formulation-requirements-verification.md
- 07-evidence-validation.md
- 08-master-verification-checklist.md
