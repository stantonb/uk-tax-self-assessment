---
name: charitable-giving
description: "Explains UK charitable giving tax relief for Self Assessment. Use when the user asks about Gift Aid, charitable donations, payroll giving, donating to charity, charity tax relief, or tax-efficient giving."
---

> **DISCLAIMER**: This skill provides general tax information only. It is NOT professional tax advice. Tax situations vary — always verify with HMRC guidance or a qualified accountant before making decisions. HMRC is the sole authority on UK tax matters.

## Gift Aid

Gift Aid is the primary mechanism for tax-efficient charitable giving. When a donor makes a Gift Aid declaration, the charity reclaims basic rate tax from HMRC — effectively adding 25% to the donation at no extra cost to the donor.

Refer to `${CLAUDE_PLUGIN_ROOT}/references/2024-25-rates.md` for current tax rates and band thresholds relevant to relief calculations.

**How it works:**

- Donor gives £80 to charity with a Gift Aid declaration.
- Charity reclaims £20 from HMRC (basic rate grossing-up), receiving £100 total.
- The donor's basic rate band extends by the gross donation amount (£100).

**Higher and additional rate taxpayers** claim the difference between their marginal rate and the basic rate via Self Assessment. The relief is the gross donation multiplied by the difference in rates. Check the rates file for current marginal rates.

## Gift Aid and Adjusted Net Income

Gift Aid donations reduce **adjusted net income (ANI)**. This has knock-on benefits:

- **High Income Child Benefit Charge** — Reducing ANI below the HICBC threshold reduces or eliminates the charge.
- **Personal allowance tapering** — Donations can restore lost PA for those with ANI above the tapering threshold.

The gross donation amount (including the charity's basic rate reclaim) is deducted from ANI. This makes Gift Aid a useful planning tool beyond the direct tax relief.

## Payroll Giving

Payroll giving (Give As You Earn) deducts donations from **gross pay** before tax is calculated. Benefits:

- Relief is automatic at the donor's marginal rate — no SA claim needed.
- The charity receives the full amount without needing to reclaim from HMRC.
- Does **not** reduce ANI in the same way as Gift Aid (it reduces taxable pay instead).

The employer must operate an approved payroll giving scheme. Not all employers offer this.

## Carry-Back Election

A donor can elect to treat a Gift Aid donation made in the current tax year as if it were made in the **previous tax year**. This is useful when:

- The donor had higher marginal rate income last year.
- The donor wants to reduce last year's ANI (e.g., to mitigate HICBC or PA tapering).

The election must be made **before or at the same time as filing** the previous year's SA return. The donation must actually be paid before the filing date.

## Gifts of Shares and Property

Donors can give **listed shares, securities, or land/property** to charity and claim income tax relief on the market value plus any incidental costs of disposal, minus any consideration received. This also eliminates any capital gains tax that would otherwise arise on the disposal. The relief is claimed via Self Assessment.

## Gift Aid Small Donations Scheme (GASDS)

Charities can claim a Gift Aid-style top-up on small cash or contactless donations (up to the per-donation limit) without needing a Gift Aid declaration from the donor. This is a charity-side benefit — it does not affect the donor's tax position or SA return.

## Record-Keeping

Maintain records of all Gift Aid donations including:

- Date and amount of each donation
- Name of the charity
- Confirmation that a Gift Aid declaration was made

HMRC can enquire into claims. Keep records for at least 22 months after the end of the tax year (the standard SA enquiry window).

## Common Mistake: Insufficient Tax Paid

Gift Aid requires the donor to have paid enough UK income tax and/or capital gains tax in the tax year to cover the basic rate tax reclaimed by all charities on the donor's Gift Aid donations. If the donor has not paid enough tax:

- The donor is **liable to repay the shortfall** to HMRC.
- This commonly catches retirees, low earners, or those whose circumstances change mid-year.

Before making a Gift Aid declaration, verify that total tax paid for the year will at least equal the total basic rate amount charities will reclaim. Check the basic rate in the rates file and calculate accordingly.
