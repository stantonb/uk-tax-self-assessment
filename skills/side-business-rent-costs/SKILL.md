---
name: side-business-rent-costs
description: "Explains claiming rent and housing costs as business expenses for UK side businesses. Make sure to use this skill whenever the user mentions claiming rent as a business expense, mortgage interest for home office, council tax deduction, business proportion of rent, housing costs for side business, or asks anything about deducting housing costs when working from home for their business."
---

> **DISCLAIMER**: This skill provides general tax information only. It is NOT professional tax advice. Tax situations vary — always verify with HMRC guidance or a qualified accountant before making decisions. HMRC is the sole authority on UK tax matters.

# Claiming Rent and Housing Costs for a Side Business

If the side business is run from home, a proportion of housing costs may be claimed as a business expense. The rules differ depending on whether the property is rented or owned.

## If Renting

Claim the **business proportion of rent** as an allowable expense. Calculate the proportion using one of two methods:

### Room Method
Number of rooms used for business / total number of rooms (excluding bathrooms, kitchens, hallways). Adjust for time proportion if the room is not used exclusively for business.

**Example**: 1 room out of 4 usable rooms = 25%. If the room is used for business 40 hours out of 168 hours in a week, the combined proportion is 25% x 24% = 6% of rent.

### Area Method
Floor area of business space / total habitable floor area. Apply the same time adjustment.

Choose whichever method is more appropriate for the property and apply it consistently.

### Landlord Permission

Check the tenancy agreement before claiming. Many residential leases prohibit or restrict business use. Running a business from a rented property without permission could breach the lease. Obtaining written consent from the landlord is recommended.

## If the Property Is Owned

Claim the business proportion of **mortgage interest only** — not capital repayments. The interest portion is shown on annual mortgage statements.

Other claimable costs for homeowners:
- Council tax (business proportion)
- Utilities — gas, electricity, water (business proportion)
- Building and contents insurance (business proportion)
- General repairs and maintenance (business proportion of whole-property costs)

### Capital Gains Tax Warning

If a room is declared as used **exclusively** for business, it may lose private residence relief. On sale of the property, HMRC could charge CGT on the proportion attributable to the exclusive business-use room. Refer to `${CLAUDE_PLUGIN_ROOT}/references/2024-25-rates.md` for CGT rates.

**Recommended approach**: describe the room as used "mainly but not exclusively" for business. Retain some personal use (e.g., guest room, hobby space). This preserves full private residence relief while still allowing a reasonable expense claim.

## Other Housing Costs to Claim

Regardless of renting or owning, apply the calculated business proportion to:

| Cost | Notes |
|------|-------|
| Council tax | Annual bill, apply proportion |
| Water rates | Annual or metered, apply proportion |
| Gas and electricity | Use actual bills, apply proportion |
| Broadband | Business proportion — often higher than room proportion if business relies heavily on internet |
| Building insurance | Apply room/time proportion |
| General repairs | Only whole-property maintenance, not room improvements |

Do **not** claim: capital improvements (new kitchen, extension), furniture for personal rooms, redecoration of non-business areas.

## Documentation Requirements

Keep all supporting records for the retention period specified in `${CLAUDE_PLUGIN_ROOT}/references/2024-25-rates.md`:

- Rent receipts or tenancy agreement showing monthly rent
- Mortgage statements showing interest vs capital split
- Utility bills (annual summaries are sufficient)
- Council tax bills
- A written record of the calculation method used, including room dimensions or counts and hours of business use
- Floor plans or room measurements if using the area method

## Common Mistakes

- **Overclaiming** — using an unrealistically high proportion. HMRC may challenge claims that seem disproportionate.
- **Not adjusting for seasonal use** — if the business is seasonal, adjust the time proportion accordingly rather than claiming for the full year.
- **Claiming capital repayments** — only mortgage interest qualifies, never the capital portion.
- **Mixing methods** — if using the simplified flat rate for WFH expenses (see **side-business-wfh** skill), actual housing costs cannot also be claimed. Choose one approach.
- **Ignoring lease restrictions** — business use without landlord consent can create legal issues beyond tax.
