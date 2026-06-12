# CALCULATION_ASSUMPTIONS.md

## GharUrja Calculation Assumptions

This file defines the assumptions used by the calculators.

The purpose of this file is to keep calculations:
- transparent,
- conservative,
- editable,
- and easy to maintain.

Do not hardcode these assumptions inside scattered UI code.

---

## General Rules

1. Keep calculations conservative.
2. Show assumptions to the user.
3. Allow state-specific overrides where needed.
4. Allow subsidy values to be updated without changing application logic.
5. Do not present estimates as guarantees.

---

## Solar Sizing Assumption

### Objective
Estimate a likely rooftop solar system size from the user’s monthly electricity usage or electricity bill.

### Method
If the user provides monthly units consumed, estimate system size directly from units.

If the user provides electricity bill amount only, estimate units using a configurable local tariff assumption, then calculate system size from the estimated units.

### Formula Logic
- Input units per month → estimated system size
- Bill amount → estimated units → estimated system size

### Notes
- This should be a conservative estimate.
- The output should always say “estimated” or “recommended.”
- State-specific corrections may be applied later.

---

## Savings Assumption

### Objective
Estimate how much the user might save after installing solar.

### Method
Savings are estimated using:
- monthly electricity cost offset,
- expected solar generation,
- and a conservative self-consumption model.

### General Rules
- Use conservative savings.
- Do not assume perfect offset unless the product explicitly supports that model.
- Explain that actual savings vary by usage pattern, tariff, roof orientation, shading, and installation quality.

---

## Payback Assumption

### Objective
Estimate how long it may take for the solar system to recover its cost.

### Method
Payback period = effective system cost after subsidy / estimated annual savings

### Notes
- This is an estimate, not a guarantee.
- Payback should be presented as approximate.
- The calculator should avoid overly optimistic assumptions.

---

## Subsidy Assumption

### Objective
Estimate likely subsidy benefits by system size and location.

### Rule
Subsidy values must be stored in editable configuration, not hardcoded into the calculator formula.

### Data Handling
Use a structured configuration source such as:
- a JSON config file,
- a CMS field,
- or an admin-editable settings panel.

### Notes
- Subsidy rules can change.
- Always display a verification notice.
- Always encourage users to verify through official government sources.

---

## Installer Verification Assumption

### Objective
Show trusted and verified installers only.

### Rule
An installer is not trusted by default.

They must be:
- manually reviewed,
- admin approved,
- or otherwise verified before appearing publicly.

### Trust Indicators
Possible indicators include:
- verified badge,
- service area,
- years in business,
- support responsiveness,
- completed projects,
- or internal review status.

---

## Lead Qualification Assumption

A lead is considered qualified if the user has:
- shown purchase intent,
- completed the quote form,
- and provided enough information for an installer to respond meaningfully.

Minimum fields:
- name
- phone number
- city
- bill estimate or units
- rooftop type
- timeline

Optional fields can improve quality:
- rooftop area
- roof ownership
- electricity provider
- address area

---

## Data Freshness Assumption

Any subsidy-related content must be periodically reviewed.

Rules:
- If subsidy information is old, mark it for review.
- If official rules change, update the config first and then the content.
- Do not leave outdated numbers on public pages.

---

## Display Rules for Estimates

Every estimate should show:
- the result,
- the basis of the estimate,
- a short disclaimer,
- and a note that actual results may differ.

Do not make the result look exact if it is only an estimate.

---

## Calculation Transparency Rule

Where possible, show a simple “How we calculated this” section.

Keep it short and non-technical.

Users should understand:
- what input they gave,
- how the estimate was produced,
- and why the result is approximate.

---

## Future Update Rule

If later versions add:
- bill OCR,
- state-specific solar assumptions,
- or financing/EMI logic,

then update this file before changing production calculations.
