# Non-UPF Standard v1.0 - Quick Reference Guide

## 🎯 Which Skill Should I Use?

### I need to...

| Task | Use This Skill | Time |
|------|---------------|------|
| **Check if a product is eligible at all** | [01-product-eligibility-verification.md](01-product-eligibility-verification.md) | 5-10 min |
| **Verify processing methods are allowed** | [02-processing-requirements-verification.md](02-processing-requirements-verification.md) | 30-60 min |
| **Check the complete formulation** | [03-formulation-requirements-verification.md](03-formulation-requirements-verification.md) | 45-90 min |
| **Just check ingredients against banned list** | [04-prohibited-ingredients-checker.md](04-prohibited-ingredients-checker.md) | 10-15 min |
| **Calculate added sugar compliance** | [05-added-sugar-calculator.md](05-added-sugar-calculator.md) | 10-20 min |
| **Track documentation collection** | [06-documentation-collection.md](06-documentation-collection.md) | Ongoing |
| **Validate all collected evidence** | [07-evidence-validation.md](07-evidence-validation.md) | 2-4 hours |
| **Do a complete verification project** | [08-master-verification-checklist.md](08-master-verification-checklist.md) | 2-12 weeks |

---

## ⚡ Quick Decision Tree

```
START: Do I need to verify a product?
│
├─ YES, complete verification needed
│  └─ Use Skill 08 (Master Checklist)
│     └─ It will guide you through Skills 01-07
│
├─ NO, just checking eligibility
│  └─ Use Skill 01 (Product Eligibility)
│
├─ NO, just checking ingredients
│  └─ Use Skill 04 (Prohibited Ingredients)
│
├─ NO, just checking added sugar
│  └─ Use Skill 05 (Added Sugar Calculator)
│
└─ NO, just checking processing
   └─ Use Skill 02 (Processing Requirements)
```

---

## 📋 Common Scenarios

### Scenario 1: New Product Submission
**Path:** Skills 01 → 02 → 03 → 06 → 07 → 08
**Start with:** Master Checklist (Skill 08)
**Timeline:** 2-8 weeks depending on complexity

### Scenario 2: Quick Ingredient Review
**Path:** Skill 04 only
**Start with:** Prohibited Ingredients Checker
**Timeline:** 10-15 minutes

### Scenario 3: Reformulation Check
**Path:** Skills 04 → 05 → 03
**Start with:** Check what changed (ingredients? sugar? processing?)
**Timeline:** 30-60 minutes

### Scenario 4: Documentation Audit
**Path:** Skills 06 → 07
**Start with:** Documentation Collection to identify gaps
**Timeline:** 1-2 days

---

## 🚦 Standard Requirements At-A-Glance

### ✓ Product MUST Be:
- Food for human consumption
- NOT produce, vitamins/supplements, alcoholic beverages, controlled substances
- NO bioengineered disclosure

### ✓ Processing MUST Have:
- ≥70% ingredients minimally/moderately processed (permissible methods)
- ≤30% ingredients conditionally processed
- NO prohibited processing methods (unless food safety exception)
- Only permissible methods on finished product

### ✓ Formulation MUST Have:
- ZERO prohibited ingredients from Annex B
- Added sugars ≤ limit for product type (if conditionally processed sweeteners present)
- NO non-nutritive sweeteners (with narrow stevia exception)
- NO prohibited gums (with narrow functional exception)
- NO hydrogenated oils, solvent extracted oils, etc.
- NO prohibited sodium compounds

### ⚠️ Common Red Flags:
- Xanthan gum (PROHIBITED - industrial fermentation)
- Carrageenan (PROHIBITED)
- Artificial colors/flavors (PROHIBITED)
- High fructose corn syrup (PROHIBITED)
- MSG, disodium guanylate, disodium inosinate (PROHIBITED)
- Steviol glycosides (PROHIBITED - whole leaf stevia may be allowed)
- Sugar alcohols: erythritol, xylitol, sorbitol (PROHIBITED)
- Allulose (PROHIBITED)

---

## 🔢 Key Calculations

### Adjusted Weight Percentage
```
Adjusted % = (Ingredient Weight / Total Weight - Water - Salt) × 100
```
**Used for:** Processing requirements, oil limits

### Added Sugar Percentage
```
Added Sugar % = (Added Sugar per serving / Serving size) × 100
```
**Used for:** Added sugar limits
**Note:** Use UNROUNDED values if limit ≤5% or result is close to limit

### Processing Thresholds
```
Minimal + Moderate (Permissible) ≥ 70%
Conditional ≤ 30%
```

---

## 📊 Added Sugar Limits Table

| Product Type | Max % |
|--------------|-------|
| Confectionery | 40% |
| Creamers (≤2 tbsp) | 25% |
| Desserts | 20% |
| Breakfast Foods | 15% |
| Dairy/Alternatives | 7% |
| Breads/Tortillas/Bagels | 5% |
| Beverages | 5% |
| Nut Butters/Spreads | 5% |
| Protein Powders | 5% |
| Condiments | 3% |
| Prepared Meals | 3% |
| Soups/Savory Sauces | 2% |
| Snack Foods | 2% |
| Meat/Plant Protein | 2% |
| Baby/Toddler Foods | 2% |
| Dry Mixes | Variable (see 6.3.2.7) |

---

## 🔍 Processing Classification Quick Check

### PROHIBITED (Never allowed)
- Precision fermentation
- Hydrogenation (full or partial)
- Chemical interesterification
- 3D printing
- Nanotechnology
- Hazardous VOC-based extraction

### CONDITIONAL (≤30% of ingredients)
- Enzymatic/acid/alkali hydrolysis
- High temp oil refining (≥200°C)
- Spray drying
- High heat extrusion (≥200°F)
- Industrial fermentation
- Deep frying (as sole cooking step)

### PERMISSIBLE - MINIMAL
- Washing, cutting, peeling
- Freezing
- Winterization

### PERMISSIBLE - MODERATE
- Baking, roasting, cooking
- Pasteurization, UHT
- Fermentation (traditional)
- Cold press/expeller press
- Milling/grinding
- Homogenization
- Dehydration/drying

---

## 🎨 How to Use Skills with AI

### Template Prompt for Any Skill:

```
I'm a technical administrator verifying a product against the Non-UPF
Standard v1.0. I need to use the [SKILL NAME] skill.

Product Information:
- Product Name: [NAME]
- Company: [COMPANY]
- [OTHER RELEVANT INFO]

Please guide me through this verification following the skill instructions.
```

### Pro Tips:

1. **One skill per session** - Don't mix multiple skills in one conversation
2. **Complete information** - Provide all requested data upfront when possible
3. **Save outputs** - Copy AI-generated reports to your files
4. **Verify calculations** - Always double-check math
5. **Be specific** - More detail = better AI guidance

---

## 📁 Documentation Checklist

### Must Have:
- [ ] Product label (all panels)
- [ ] Ingredient statement
- [ ] Full formulation with weights
- [ ] Nutrition Facts panel
- [ ] Processing methods for each ingredient
- [ ] Supplier specifications
- [ ] Process flow diagram

### Should Have:
- [ ] Certificates of Analysis (COA)
- [ ] Processing temperature/time specifications
- [ ] Supplier audit reports
- [ ] Previous certifications

### May Need:
- [ ] Food safety exemption justification
- [ ] Functional necessity documentation (for gums)
- [ ] Product type classification rationale
- [ ] Natural flavor correspondence evidence

---

## ⏱️ Typical Timeline by Product Complexity

### Simple Product (e.g., plain nut butter, dried fruit)
- **Eligibility:** 5 minutes
- **Processing:** 30 minutes
- **Formulation:** 30 minutes
- **Documentation:** 1-2 weeks
- **Validation:** 2 hours
- **Total:** 2-3 weeks

### Moderate Product (e.g., granola, yogurt, bread)
- **Eligibility:** 10 minutes
- **Processing:** 1 hour
- **Formulation:** 1.5 hours
- **Documentation:** 2-4 weeks
- **Validation:** 4 hours
- **Total:** 4-6 weeks

### Complex Product (e.g., prepared meal, baked good with multiple components)
- **Eligibility:** 15 minutes
- **Processing:** 2-3 hours
- **Formulation:** 2-3 hours
- **Documentation:** 4-8 weeks
- **Validation:** 6-8 hours
- **Total:** 8-12 weeks

---

## 🚨 Red Flags to Watch For

### Immediate Disqualifiers:
- ❌ Bioengineered disclosure
- ❌ Any ingredient on Annex B prohibited list
- ❌ Prohibited processing method (without valid food safety exemption)
- ❌ Product not eligible category

### Common Issues:
- ⚠️ Xanthan gum (often assumed OK, but prohibited)
- ⚠️ "Natural flavors" without corresponding ingredients
- ⚠️ Refined oils exceeding 30%
- ⚠️ Added sugar calculation errors
- ⚠️ Processing classification mistakes

### Documentation Problems:
- ⚠️ Vague supplier specifications
- ⚠️ Missing sub-ingredient disclosure
- ⚠️ Outdated certifications
- ⚠️ Inconsistent formulation data

---

## 📞 When to Ask for Help

### Escalate When:
- Novel ingredient with no clear classification
- Ambiguous standard interpretation
- Conflicting evidence
- Complex conditional allowance claim
- Potential circumvention of standard intent

### Don't Guess:
- Processing method classifications
- Product type for added sugar limits
- Whether exemptions apply
- Evidence sufficiency

---

## 💡 Pro Tips for Efficient Verification

1. **Start with Skill 04** (ingredients check) before deep dive - saves time if product has prohibited ingredients

2. **Use Skills 04 & 05 first** on complex formulations to identify major issues early

3. **Keep supplier contact info handy** - you'll need clarifications

4. **Build a template library** from AI outputs for consistent formatting

5. **Track common issues** by product type to anticipate problems

6. **Batch similar products** to streamline supplier documentation requests

7. **Pre-screen reformulations** with quick ingredient/processing checks before full re-verification

8. **Document edge cases** for future reference and standard improvement

---

## 📖 Annex Quick Access

### Annex A - Processing Methods
Full table in Skill 02, quick reference:
- Biological, Chemical, Mechanical, Thermal classifications
- Prohibited vs. Conditional vs. Permissible
- Specific conditions for conditional methods

### Annex B - Prohibited Ingredients
Complete list in Skill 04, includes:
- 290+ prohibited ingredients alphabetically
- Sweeteners, colors, preservatives, emulsifiers, etc.
- Common names and E-numbers

---

## 🎓 Learning Curve

### First Time (Skill 08 - Master Checklist)
- Expect to reference standard frequently
- Budget extra time for learning
- Use skills sequentially to build understanding
- Don't skip steps

### Experienced (Skills 01-07 individually)
- Pick specific skills for targeted checks
- Use as reference while working
- Adapt templates to your workflow
- Focus on validation and edge cases

---

## ✅ Before You Start Any Verification

1. [ ] Have complete product information
2. [ ] Read the relevant skill(s) completely
3. [ ] Gather necessary documentation
4. [ ] Prepare to save outputs
5. [ ] Allocate sufficient time
6. [ ] Have Non-UPF Standard v1.0 accessible for reference

---

## 🔗 Essential Links

- **Non-UPF Standard v1.0:** Check official website for latest version
- **Skills Directory:** [README.md](README.md) for complete guide
- **Master Checklist:** [Skill 08](08-master-verification-checklist.md) for full workflow

---

**Version:** 1.0
**Date:** 2025-01-13
**Based on:** Non-UPF Standard v1.0 (November 2025)

---

## 🎯 Remember

> **These skills are tools to assist, not replace, professional judgment.**

> **When in doubt, refer to the official Non-UPF Standard v1.0.**

> **Verify AI calculations and classifications independently.**

> **Apply the standard in good faith and with integrity.**
