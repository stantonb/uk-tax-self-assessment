---
name: rental-income
description: "Covers UK rental income tax rules for Self Assessment. Use when the user asks about rental income, buy to let tax, property income, SA105, letting relief, rent-a-room scheme, or landlord tax."
---

> **DISCLAIMER**: This skill provides general tax information only. It is NOT professional tax advice. Tax situations vary — always verify with HMRC guidance or a qualified accountant before making decisions. HMRC is the sole authority on UK tax matters.

## Purpose

This skill covers reporting UK property income on the SA105 supplementary pages. It addresses allowable expenses, the mortgage interest restriction, Rent-a-Room scheme, record-keeping, and specific rules for jointly owned property and furnished holiday lets.

## SA105 Property Income Pages

Determine the user's property situation:

- UK property income is reported on SA105. Foreign property income uses SA106.
- The £1,000 property income allowance covers small amounts of income — if total property income is below this threshold (check `${CLAUDE_PLUGIN_ROOT}/references/2024-25-rates.md`), the user may not need to report it.
- If claiming expenses, the user cannot also use the property income allowance — it is one or the other.

Ask the user for their gross rental income to determine which approach is more beneficial.

## Allowable Expenses for Landlords

Ask the user about each category of deductible expenses:

- **Letting agent fees and management costs**
- **Buildings and contents insurance**
- **Maintenance and repairs** (like-for-like replacement only — improvements are capital expenditure, not deductible against income)
- **Council tax, water rates, and utility bills** (if paid by the landlord)
- **Ground rent and service charges**
- **Accountancy and legal fees** (for rental accounts and tenant matters, not purchase/sale costs)
- **Advertising for tenants**
- **Travel to the property** for management purposes (at HMRC approved mileage rates)
- **Stationery, phone calls, and other incidental costs**

Remind the user: expenses must relate to the rental business and be incurred in the period they are claimed.

## Mortgage Interest Restriction

This is a critical area for buy-to-let landlords. Explain the restriction:

- Finance costs (mortgage interest, arrangement fees, overdraft interest) are NOT deductible from rental profits.
- Instead, a tax credit is given at the basic rate (check data file for the percentage) on the finance costs incurred.
- This means higher and additional rate taxpayers pay more tax on rental income than before the restriction was introduced.
- The restriction can also push the user's total income into a higher band (because the full rental profit, before finance costs, counts as income), potentially triggering the personal allowance taper or HICBC.

Calculate the net effect for the user: compare the tax on gross rental profits with the basic rate credit to show the actual tax cost.

## Rent-a-Room Scheme

Explain the scheme for users letting furnished rooms in their main home:

- Gross rental income up to the Rent-a-Room threshold (check data file — currently £7,500 per year) is tax-free.
- If the property is jointly let, the threshold is halved per person.
- The user can choose to use the scheme (reporting nothing if under the limit) or opt out and claim actual expenses instead — whichever is more beneficial.
- The scheme applies only to furnished accommodation in the user's main residence (not separate properties).

Ask whether the user lets a room in their own home or a separate property to determine eligibility.

## Replacement of Domestic Items (Wear and Tear)

Explain the current rules:

- The old 10% wear and tear allowance for furnished lets has been replaced by the Replacement of Domestic Items relief.
- Landlords can deduct the cost of replacing furnishings, appliances, and kitchenware in residential lets — but only when an old item is actually replaced, not on the initial purchase.
- The deduction is for a like-for-like replacement. If the replacement is an improvement, only the cost of an equivalent item is deductible.

## Furnished Holiday Lets (FHL)

Note the changes to the FHL regime:

- The special tax treatment for qualifying furnished holiday lets (capital allowances, CGT reliefs, pension-relevant earnings) has been reformed. Check `${CLAUDE_PLUGIN_ROOT}/references/2024-25-rates.md` for the current status and transitional rules.
- If the user has an FHL, ask about occupancy conditions (available for letting for a minimum number of days, actually let for a minimum number of days) and confirm whether the property still qualifies under current rules.

## Jointly Owned Property

Clarify the rules for shared ownership:

- Married couples and civil partners: income is split 50:50 by default, regardless of actual ownership shares, unless a Form 17 declaration is made to HMRC with evidence of unequal beneficial ownership.
- Other joint owners: income is split according to actual ownership shares.

Ask whether the property is jointly owned and whether the user's share is correctly reflected.

## Practical Steps

1. Calculate gross rental income for the tax year.
2. Determine whether to use the property income allowance or claim actual expenses.
3. List all allowable expenses with supporting records.
4. Calculate the mortgage interest tax credit separately.
5. Consider Rent-a-Room if the let is in the user's main home.
6. Enter figures on SA105 and carry the profit to the SA100.

Chain to **income-tax-bands** for understanding how rental profit is taxed, or to **sa-overview** for filing requirements.
