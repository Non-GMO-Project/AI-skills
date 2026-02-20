# Non-UPF Standard v1.0 Skills - Complete Index

## 📚 Complete Skill Library

### Getting Started
- **[README.md](README.md)** - Complete guide to using these skills
- **[QUICK-REFERENCE.md](QUICK-REFERENCE.md)** - Fast lookup and decision guide
- **[INDEX.md](INDEX.md)** ← You are here

---

## 🎯 Skills by Category

### Core Verification Workflow

| # | Skill Name | Purpose | Time Required | Difficulty |
|---|------------|---------|---------------|------------|
| 01 | [Product Eligibility Verification](01-product-eligibility-verification.md) | Determine if product qualifies for verification | 5-10 min | Easy |
| 02 | [Processing Requirements Verification](02-processing-requirements-verification.md) | Verify ingredient and product processing compliance | 30-60 min | Moderate |
| 03 | [Formulation Requirements Verification](03-formulation-requirements-verification.md) | Comprehensive formulation compliance check | 45-90 min | Advanced |
| 08 | [Master Verification Checklist](08-master-verification-checklist.md) | Complete end-to-end verification workflow | 2-12 weeks | Advanced |

### Quick Check Tools

| # | Skill Name | Purpose | Time Required | Difficulty |
|---|------------|---------|---------------|------------|
| 04 | [Prohibited Ingredients Checker](04-prohibited-ingredients-checker.md) | Fast ingredient screening against Annex B | 10-15 min | Easy |
| 05 | [Added Sugar Calculator](05-added-sugar-calculator.md) | Calculate and verify added sugar compliance | 10-20 min | Easy |

### Documentation & Validation

| # | Skill Name | Purpose | Time Required | Difficulty |
|---|------------|---------|---------------|------------|
| 06 | [Documentation Collection](06-documentation-collection.md) | Systematic documentation gathering and tracking | Ongoing | Moderate |
| 07 | [Evidence Validation](07-evidence-validation.md) | Validate documentation quality and consistency | 2-4 hours | Advanced |

---

## 🎬 Skills by Use Case

### "I'm starting a new verification"
→ Start with [Skill 08 - Master Verification Checklist](08-master-verification-checklist.md)
- It will guide you through Skills 01-07 in the proper sequence
- Use for complete, formal verification projects

### "I need to check if a product is eligible"
→ Use [Skill 01 - Product Eligibility Verification](01-product-eligibility-verification.md)
- Quick eligibility determination
- First gate check before proceeding

### "I need to verify processing methods"
→ Use [Skill 02 - Processing Requirements Verification](02-processing-requirements-verification.md)
- Classify all processing methods
- Calculate processing percentages
- Verify thresholds

### "I need to check the formulation"
→ Use [Skill 03 - Formulation Requirements Verification](03-formulation-requirements-verification.md)
- Comprehensive formulation review
- Covers all Section 6.3 requirements
- Integrates Skills 04 and 05

### "I just need to check ingredients quickly"
→ Use [Skill 04 - Prohibited Ingredients Checker](04-prohibited-ingredients-checker.md)
- Fast Annex B cross-reference
- Immediate flagging of prohibited items
- Standalone or integrated use

### "I need to verify added sugar compliance"
→ Use [Skill 05 - Added Sugar Calculator](05-added-sugar-calculator.md)
- Product type classification
- Added sugar calculation
- Limit verification

### "I need to collect documentation"
→ Use [Skill 06 - Documentation Collection](06-documentation-collection.md)
- Complete document checklist
- Status tracking
- Communication templates

### "I need to validate evidence"
→ Use [Skill 07 - Evidence Validation](07-evidence-validation.md)
- Document quality assessment
- Cross-reference verification
- Consistency checks

---

## 📊 Skills by Non-UPF Standard Section

### Section 6.1: Product Eligibility
- **Primary:** [Skill 01 - Product Eligibility Verification](01-product-eligibility-verification.md)
- **Reference in:** Skill 08 (Master Checklist)

### Section 6.2: Processing Requirements
- **Primary:** [Skill 02 - Processing Requirements Verification](02-processing-requirements-verification.md)
- **Reference in:** Skills 03, 07, 08
- **Uses:** Annex A - Classification of Food Processing Methods

### Section 6.3: Formulation Requirements
- **Primary:** [Skill 03 - Formulation Requirements Verification](03-formulation-requirements-verification.md)
- **Supporting:** Skills 04, 05
- **Reference in:** Skills 07, 08
- **Uses:** Annex B - Harmonized Prohibited Ingredients List

#### Section 6.3.1: Prohibited Ingredients
- **Primary:** [Skill 04 - Prohibited Ingredients Checker](04-prohibited-ingredients-checker.md)
- **Reference in:** Skills 03, 07, 08

#### Section 6.3.2: Added Sugar Limits
- **Primary:** [Skill 05 - Added Sugar Calculator](05-added-sugar-calculator.md)
- **Reference in:** Skills 03, 07, 08

#### Section 6.3.3: Non-Nutritive & Biotransformed Sweeteners
- **Primary:** [Skill 03 - Formulation Requirements Verification](03-formulation-requirements-verification.md)
- **Reference in:** Skills 07, 08

#### Section 6.3.4: Gums, Thickeners & Texturizers
- **Primary:** [Skill 03 - Formulation Requirements Verification](03-formulation-requirements-verification.md)
- **Reference in:** Skills 07, 08

#### Section 6.3.5: Natural Flavors
- **Primary:** [Skill 03 - Formulation Requirements Verification](03-formulation-requirements-verification.md)
- **Reference in:** Skills 07, 08
- **Note:** Optional for v1.0

#### Section 6.3.6: Refined Oils
- **Primary:** [Skill 03 - Formulation Requirements Verification](03-formulation-requirements-verification.md)
- **Reference in:** Skills 07, 08

#### Section 6.3.7: Sodium
- **Primary:** [Skill 03 - Formulation Requirements Verification](03-formulation-requirements-verification.md)
- **Reference in:** Skills 07, 08

### Documentation & Evidence
- **Collection:** [Skill 06 - Documentation Collection](06-documentation-collection.md)
- **Validation:** [Skill 07 - Evidence Validation](07-evidence-validation.md)
- **Reference in:** Skill 08 (Master Checklist)

---

## 🔄 Skill Relationships & Dependencies

```
┌─────────────────────────────────────────────────┐
│  SKILL 08: MASTER VERIFICATION CHECKLIST        │
│  (Coordinates all other skills)                 │
└─────────────────┬───────────────────────────────┘
                  │
        ┌─────────┴──────────┐
        │                    │
        ▼                    ▼
┌───────────────┐    ┌───────────────┐
│  SKILL 01     │    │  SKILL 06     │
│  Eligibility  │    │  Documentation│
└───────┬───────┘    └───────┬───────┘
        │                    │
        ▼                    ▼
┌───────────────┐    ┌───────────────┐
│  SKILL 02     │    │  SKILL 07     │
│  Processing   │    │  Evidence     │
└───────┬───────┘    │  Validation   │
        │            └───────────────┘
        ▼
┌───────────────┐
│  SKILL 03     │
│  Formulation  │◄───────────┐
└───────┬───────┘            │
        │                    │
   ┌────┴────┐              │
   ▼         ▼              │
┌──────┐  ┌──────┐          │
│SKILL │  │SKILL │          │
│  04  │  │  05  │──────────┘
│Ingred│  │Sugar │
└──────┘  └──────┘
```

### Standalone Skills (Can be used independently):
- Skill 01 (Product Eligibility)
- Skill 04 (Prohibited Ingredients)
- Skill 05 (Added Sugar Calculator)

### Integrated Skills (Best used as part of workflow):
- Skill 02 (Processing Requirements)
- Skill 03 (Formulation Requirements)
- Skill 06 (Documentation Collection)
- Skill 07 (Evidence Validation)

### Master Coordinator:
- Skill 08 (Master Verification Checklist) - Integrates all others

---

## 📈 Skill Complexity & Experience Level

### Beginner-Friendly
- ✅ [Skill 01 - Product Eligibility](01-product-eligibility-verification.md)
- ✅ [Skill 04 - Prohibited Ingredients](04-prohibited-ingredients-checker.md)
- ✅ [Skill 05 - Added Sugar Calculator](05-added-sugar-calculator.md)

**Start here if you're new to Non-UPF verification**

### Intermediate
- 📊 [Skill 02 - Processing Requirements](02-processing-requirements-verification.md)
- 📊 [Skill 06 - Documentation Collection](06-documentation-collection.md)

**Use after understanding basics**

### Advanced
- 🎓 [Skill 03 - Formulation Requirements](03-formulation-requirements-verification.md)
- 🎓 [Skill 07 - Evidence Validation](07-evidence-validation.md)
- 🎓 [Skill 08 - Master Checklist](08-master-verification-checklist.md)

**Requires comprehensive understanding of the standard**

---

## ⏱️ Typical Skill Usage Time

### Quick (< 30 minutes)
- Skill 01: Product Eligibility (5-10 min)
- Skill 04: Prohibited Ingredients (10-15 min)
- Skill 05: Added Sugar Calculator (10-20 min)

### Moderate (30 min - 2 hours)
- Skill 02: Processing Requirements (30-60 min)
- Skill 03: Formulation Requirements (45-90 min)

### Extended (Multiple hours/days)
- Skill 06: Documentation Collection (Ongoing, days-weeks)
- Skill 07: Evidence Validation (2-4 hours)

### Project-Level (Weeks)
- Skill 08: Master Verification Checklist (2-12 weeks full project)

---

## 🎯 Skills by Output Type

### Decision Outputs
- Skill 01: ELIGIBLE / INELIGIBLE
- Skill 08: APPROVED / CONDITIONAL / DENIED

### Compliance Outputs
- Skill 02: COMPLIANT / NON-COMPLIANT
- Skill 03: COMPLIANT / NON-COMPLIANT
- Skill 04: PASS / FAIL
- Skill 05: COMPLIANT / NON-COMPLIANT

### Status Outputs
- Skill 06: COMPLETE / PENDING
- Skill 07: VERIFIED / CONDITIONAL / INSUFFICIENT / NON-COMPLIANT

---

## 📋 Skills by Report Type

### Determination Reports
- [Skill 01](01-product-eligibility-verification.md) - Eligibility Report
- [Skill 08](08-master-verification-checklist.md) - Final Verification Report

### Compliance Reports
- [Skill 02](02-processing-requirements-verification.md) - Processing Compliance Report
- [Skill 03](03-formulation-requirements-verification.md) - Formulation Compliance Report

### Analysis Reports
- [Skill 04](04-prohibited-ingredients-checker.md) - Ingredient Check Report
- [Skill 05](05-added-sugar-calculator.md) - Added Sugar Calculation Report
- [Skill 07](07-evidence-validation.md) - Evidence Validation Report

### Tracking Reports
- [Skill 06](06-documentation-collection.md) - Documentation Status Tracker

---

## 🔍 Finding What You Need

### By Keyword

**Eligibility**
- → Skill 01

**Processing, Fermentation, Extrusion, Refining**
- → Skill 02
- → Also see: Annex A references in Skill 02

**Ingredients, Prohibited, Annex B, Banned**
- → Skill 04
- → Also see: Section 6.3.1 in Skill 03

**Sugar, Sweeteners, Stevia, Aspartame, Added Sugar**
- → Skill 05 (for added sugar calculation)
- → Skill 03 Section 6.3.3 (for non-nutritive sweeteners)

**Gums, Xanthan, Carrageenan, Thickeners**
- → Skill 03 Section 6.3.4

**Natural Flavors, Extracts**
- → Skill 03 Section 6.3.5

**Oils, Refined, Hydrogenated**
- → Skill 03 Section 6.3.6

**Sodium, MSG, Preservatives**
- → Skill 03 Section 6.3.7

**Documentation, Evidence, Validation**
- → Skill 06 (collection)
- → Skill 07 (validation)

**Complete Verification, Project, Workflow**
- → Skill 08

---

## 📱 Quick Access Codes

Bookmark these for fast navigation:

- **QR01**: Product Eligibility → [Skill 01](01-product-eligibility-verification.md)
- **QR02**: Processing → [Skill 02](02-processing-requirements-verification.md)
- **QR03**: Formulation → [Skill 03](03-formulation-requirements-verification.md)
- **QR04**: Ingredients → [Skill 04](04-prohibited-ingredients-checker.md)
- **QR05**: Sugar → [Skill 05](05-added-sugar-calculator.md)
- **QR06**: Docs → [Skill 06](06-documentation-collection.md)
- **QR07**: Validation → [Skill 07](07-evidence-validation.md)
- **QR08**: Master → [Skill 08](08-master-verification-checklist.md)

---

## 📚 Supporting Documents

- **[README.md](README.md)** - How to use these skills (start here!)
- **[QUICK-REFERENCE.md](QUICK-REFERENCE.md)** - Fast lookup guide
- **Non-UPF Standard v1.0.md** - The official standard document

---

## 🎓 Learning Path

### Week 1: Fundamentals
1. Read [README.md](README.md)
2. Practice with [Skill 04](04-prohibited-ingredients-checker.md) on sample products
3. Practice with [Skill 05](05-added-sugar-calculator.md) on labeled products

### Week 2: Core Skills
4. Work through [Skill 01](01-product-eligibility-verification.md)
5. Study processing classifications in [Skill 02](02-processing-requirements-verification.md)
6. Review Annex A thoroughly

### Week 3: Advanced Skills
7. Master [Skill 03](03-formulation-requirements-verification.md)
8. Practice with [Skill 06](06-documentation-collection.md)
9. Review Annex B thoroughly

### Week 4: Integration
10. Study [Skill 07](07-evidence-validation.md)
11. Review complete workflow in [Skill 08](08-master-verification-checklist.md)
12. Conduct practice verification using Skill 08

---

## 🔄 Update History

**Version 1.0** (2025-01-13)
- Initial creation of complete skill set
- Based on Non-UPF Standard v1.0 (November 2025)
- 8 core skills + supporting documents

---

## 📞 Need Help?

### Can't find what you need?
1. Check [QUICK-REFERENCE.md](QUICK-REFERENCE.md) for fast lookup
2. Review [README.md](README.md) for detailed guidance
3. Consult the official Non-UPF Standard v1.0

### Still stuck?
- Review the specific skill's "Common Issues" section
- Check cross-references to related skills
- Refer to Non-UPF Standard directly

---

## 🎯 Summary Table: All Skills at a Glance

| # | Skill | Section | Time | Difficulty | Standalone? | Output |
|---|-------|---------|------|------------|-------------|--------|
| 01 | Eligibility | 6.1 | 5-10m | Easy | ✓ | ELIGIBLE/INELIGIBLE |
| 02 | Processing | 6.2 | 30-60m | Moderate | ✓ | COMPLIANT/NON-COMPLIANT |
| 03 | Formulation | 6.3 | 45-90m | Advanced | ✓ | COMPLIANT/NON-COMPLIANT |
| 04 | Ingredients | 6.3.1 | 10-15m | Easy | ✓ | PASS/FAIL |
| 05 | Sugar | 6.3.2 | 10-20m | Easy | ✓ | COMPLIANT/NON-COMPLIANT |
| 06 | Documentation | All | Ongoing | Moderate | ✓ | COMPLETE/PENDING |
| 07 | Validation | All | 2-4h | Advanced | ✗ | VERIFIED/NOT VERIFIED |
| 08 | Master | All | 2-12w | Advanced | ✗ | APPROVED/CONDITIONAL/DENIED |

---

**Last Updated:** 2025-01-13
**Version:** 1.0
**Total Skills:** 8
**Total Pages:** 100+
