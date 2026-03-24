---
name: self-employment-income
description: "Covers UK self-employment income reporting for Self Assessment. Make sure to use this skill whenever the user mentions being self-employed, sole trader, freelancer, contractor, SA103, trading income, business profits, or anything about reporting self-employment on their tax return — even if they just say 'I do some freelancing on the side'."
---

> **DISCLAIMER**: This skill provides general tax information only. It is NOT professional tax advice. Tax situations vary — always verify with HMRC guidance or a qualified accountant before making decisions. HMRC is the sole authority on UK tax matters.

## Purpose

This skill covers reporting self-employment income on the SA103 supplementary pages. It addresses registration, distinguishing trading from non-trading income, accounting methods, allowable expenses, National Insurance contributions, and key considerations for sole traders and freelancers.

## Registration as Self-Employed

Guide the user through the requirements:

- Register with HMRC as self-employed by 5 October following the tax year in which trading began.
- Registration is done online via HMRC or by calling the newly self-employed helpline.
- HMRC will issue a UTR (if the user does not already have one) and set up Class 2 NIC liability.
- If the user is already registered for SA (e.g. for rental income), they still need to notify HMRC of self-employment separately.

Ask the user when they started trading to confirm they have registered in time.

## Trading Income vs Hobby Income

Help the user determine whether their activity constitutes a trade. Apply the "badges of trade":

- Is there a profit-seeking motive?
- Is the activity repeated and systematic (not a one-off sale)?
- Is there commercial organisation (invoicing, bookkeeping, marketing)?
- Is stock acquired for resale?

If the activity is a genuine trade, report on SA103. If it is a hobby or one-off transaction, it may fall outside trading income (though capital gains may still apply). The £1,000 trading allowance covers small amounts — check `${CLAUDE_PLUGIN_ROOT}/references/2024-25-rates.md` for the threshold.

## SA103: Short vs Full

Determine which version the user needs:

- **SA103S (Short)**: Turnover below the threshold in the data file, no losses to carry forward, and using simple accounting.
- **SA103F (Full)**: Turnover above the threshold, capital allowances claimed, losses brought forward or carried, or more complex situations.

Ask the user for their turnover to direct them to the correct form.

## Cash Basis vs Accruals

Explain the two accounting methods:

- **Cash basis**: Record income when received and expenses when paid. Simpler, suitable for most small businesses. Available if turnover is below the cash basis threshold — check data file.
- **Accruals basis**: Record income when earned and expenses when incurred, regardless of cash movement. Required above the threshold or if the user opts in for more accurate matching.

Advise the user that once they choose a method, consistency is expected. Cash basis has restrictions on some deductions (e.g. interest costs are capped — check data file).

## Allowable Expenses

Ask the user about common deductible expenses:

- Office costs (stationery, phone, internet — business proportion)
- Travel (business mileage at HMRC approved rates, public transport, parking)
- Premises costs (rent, utilities, insurance — business proportion if home-based)
- Stock and materials
- Professional fees (accountant, solicitor, professional body subscriptions)
- Marketing and advertising
- Insurance (professional indemnity, public liability)
- Simplified expenses: HMRC flat rates for vehicles, home-as-office, and living on business premises — reference data file for current rates.

Remind the user: expenses must be "wholly and exclusively" for business purposes. Mixed-use items need apportioning.

## National Insurance Contributions

Reference `${CLAUDE_PLUGIN_ROOT}/references/2024-25-rates.md` for NIC rates and thresholds:

- **Class 2 NIC**: Flat weekly rate payable if profits exceed the Small Profits Threshold. Voluntary payment below this threshold to protect state pension entitlement.
- **Class 4 NIC**: Percentage-based, calculated on profits between the Lower Profits Limit and Upper Profits Limit, with a reduced rate above the UPL.

Both are calculated and collected through the SA return. Walk the user through the thresholds using the data file.

## Overlap Relief and Basis Period Reform

Note the transition to the tax year basis (from 2024-25 onwards):

- Previously, businesses with non-31 March/5 April year-ends had overlap profits taxed twice. Overlap relief was given on cessation or change of accounting date.
- Under the new rules, all businesses report profits arising in the tax year. Transitional provisions spread excess overlap profits over multiple years — check data file for the spreading period.

Ask the user their accounting year-end to determine if transitional rules apply.

## Construction Industry Scheme (CIS)

If the user works in construction, ask whether they are registered under CIS. Subcontractors have tax deducted at source by contractors (at the standard or higher CIS rate — check data file). These deductions are credited against the user's SA liability. Ensure the user reports gross income and claims the CIS deductions on the return.

## Practical Steps

1. Confirm registration and trading status.
2. Choose cash basis or accruals.
3. Calculate turnover and determine SA103S or SA103F.
4. Deduct allowable expenses to arrive at taxable profit.
5. Calculate Class 2 and Class 4 NIC using the data file.
6. Enter figures on SA103 and carry totals to the SA100.

Chain to **income-tax-bands** for how profits are taxed, or to **sa-overview** for deadlines and filing.
