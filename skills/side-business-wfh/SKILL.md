---
name: side-business-wfh
description: "Explains working from home tax deductions for UK side businesses and self-employed. Make sure to use this skill whenever the user mentions working from home expenses, home office deduction, claiming rent for business, utility bills for business, WFH allowance self-employed, home office proportion, or asks anything about claiming household costs against their business — even if they just say 'I work from home for my side business, can I claim anything'."
---

> **DISCLAIMER**: This skill provides general tax information only. It is NOT professional tax advice. Tax situations vary — always verify with HMRC guidance or a qualified accountant before making decisions. HMRC is the sole authority on UK tax matters.

# Working From Home Deductions for Side Businesses

There are two methods for claiming home office costs as a self-employed person or side business owner. Choose one method and apply it consistently for the tax year.

## Method 1: Flat Rate (Simplified Expenses)

HMRC provides fixed monthly amounts based on hours worked from home per month:

| Hours worked from home per month | Flat rate per month |
|----------------------------------|---------------------|
| 25 to 50 hours                   | £10                 |
| 51 to 100 hours                  | £18                 |
| 101 hours or more                | £26                 |

**Advantages**: no receipts needed for household bills, simple to calculate, no risk of CGT complications.

**Disadvantages**: the flat rate may be significantly less than the actual proportion of costs, especially if housing costs are high.

Track hours worked from home in a log or diary to support the claim.

## Method 2: Actual Costs

Calculate the business proportion of actual household running costs. This requires a two-step apportionment:

### Step 1 — Room Proportion

Determine what fraction of the home is used for business:

- **By room count**: number of rooms used for business / total rooms in the property (exclude bathrooms, kitchens, hallways)
- **By floor area**: square footage of business area / total habitable floor area

### Step 2 — Time Proportion

If the room is not used exclusively for business, reduce the proportion by the fraction of time it is used for business purposes. For example, a spare bedroom used as an office 8 hours a day, 5 days a week, is used for business approximately 24% of the time (40/168 hours).

### Claimable Household Costs

Apply the combined proportion (room x time) to:

- Rent (if renting) or mortgage interest only (if owned — not capital repayments)
- Council tax
- Gas and electricity
- Water rates
- Home insurance (buildings and contents)
- Broadband and phone line
- Repairs and maintenance to the property (general, not room-specific improvements)

See the **side-business-rent-costs** skill for detailed guidance on rent and mortgage interest claims specifically.

## Capital Gains Tax Warning

If you **own** your home and claim a room is used **exclusively** for business, that room may lose its private residence relief exemption. When you sell the property, HMRC could assess CGT on the proportion attributable to the business-use room.

**Mitigation**: ensure the room retains some personal use (e.g., it doubles as a guest bedroom). Describe it as "mainly but not exclusively" used for business. This preserves private residence relief while still allowing a reasonable proportion claim on expenses.

Refer to `${CLAUDE_PLUGIN_ROOT}/references/2024-25-rates.md` for current CGT rates and the annual exempt amount.

## Interaction with Employment WFH Allowance

If the user also works from home for an employer, they may receive or claim the flat rate employment WFH allowance. Refer to `${CLAUDE_PLUGIN_ROOT}/references/2024-25-rates.md` under "Working From Home" for the current weekly allowance rate.

**You cannot claim both** the employment WFH allowance and self-employment home office costs for the same space and the same time period. If the same room is used for both employed and self-employed work, apportion accordingly or choose which claim to make for which periods.

## Practical Tips

- Keep a consistent calculation method year to year.
- Photograph or scan utility bills and keep digital records.
- If costs fluctuate seasonally (e.g., higher heating in winter), use annual totals rather than monthly estimates.
- The flat rate method cannot be combined with actual cost claims — choose one for the entire tax year.
- Refer to the **side-business-expenses** skill for broader guidance on allowable deductions.
