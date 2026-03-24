---
name: income-tax-bands
description: "Explains UK income tax bands, rates, and the personal allowance for England taxpayers. Make sure to use this skill whenever the user mentions tax bands, tax rates, personal allowance, how much tax they'll pay, taxable income, additional rate tax, the £100k trap, marginal tax rate, or asks anything about how UK income tax is calculated — even if they just provide a salary and ask 'how much tax will I pay'."
---

> **DISCLAIMER**: This skill provides general tax information only. It is NOT professional tax advice. Tax situations vary — always verify with HMRC guidance or a qualified accountant before making decisions. HMRC is the sole authority on UK tax matters.

## Purpose

This skill explains UK income tax bands and rates for England, Wales, and Northern Ireland taxpayers. It covers the personal allowance, how income is taxed across bands, the personal allowance taper above £100k, and how different income types stack. Refer to `${CLAUDE_PLUGIN_ROOT}/references/2024-25-rates.md` for all current rates and thresholds.

## Personal Allowance

Check the data file for the current personal allowance amount. Key points to convey:

- Most individuals receive the full personal allowance — the first slice of income that is tax-free.
- The allowance is the same regardless of income type (employment, self-employment, pensions, etc.).
- Certain individuals may have a reduced allowance (e.g. pre-2016 married couple's allowance claimants, non-residents with no entitlement).
- Marriage Allowance allows transfer of a portion of unused personal allowance to a spouse/civil partner — check the data file for the transferable amount and eligibility conditions.

## Tax Bands and Rates

Reference `${CLAUDE_PLUGIN_ROOT}/references/2024-25-rates.md` for the exact band thresholds and rates. Explain the structure:

1. **Personal Allowance** — 0% on income up to the allowance threshold
2. **Basic Rate** — applies to the next band of taxable income
3. **Higher Rate** — applies to the next band above basic rate
4. **Additional Rate** — applies to income above the additional rate threshold

Walk the user through a calculation: total income minus the personal allowance equals taxable income, then apply each band sequentially. Offer to compute a worked example if the user provides their income figure.

## The £100k Personal Allowance Trap

This is a critical planning point. Explain the taper mechanism:

- For every £2 of adjusted net income above £100,000, the personal allowance is reduced by £1.
- This means the allowance is fully withdrawn at £125,140 (check data file for exact figure).
- The effective marginal tax rate in this band is approximately 60% — the user pays the higher rate on the income AND loses the tax-free allowance simultaneously.
- Advise the user to consider pension contributions or Gift Aid donations to bring adjusted net income below £100,000, as this can be highly tax-efficient.

Ask the user if their income is in or near this range and calculate the benefit of salary sacrifice or pension contributions if relevant.

## Income Stacking Order

Explain how different income types are taxed in a specific order:

1. **Non-savings income** (employment, self-employment, pensions, rental) — taxed first
2. **Savings income** (bank interest, building society interest) — taxed next, using any remaining basic/higher rate band
3. **Dividend income** — taxed last, sitting on top of all other income

This stacking order matters because it determines which tax band applies to each income type. A user with employment income that uses up the basic rate band will pay higher rate tax on their savings and dividends.

Refer the user to the **savings-interest** and **dividend-income** skills for the specific allowances and rates that apply to those income types.

## Scottish Taxpayers

Note that Scotland has its own income tax rates and bands for non-savings, non-dividend income. Scottish taxpayers are identified by their tax code (prefix "S"). The personal allowance remains the same across the UK, but the band thresholds and rates differ.

If the user is a Scottish taxpayer, advise them that the rates in the data file apply to England/Wales/NI only and direct them to check the Scottish rates on HMRC or Revenue Scotland guidance.

## Practical Steps

When helping a user estimate their tax liability:

1. Gather all income sources and amounts.
2. Determine adjusted net income (gross income minus pension contributions, Gift Aid gross-up, and other permitted deductions).
3. Apply the personal allowance (tapered if above £100k).
4. Stack income in the correct order and apply the relevant band rates.
5. Deduct tax already paid (PAYE, tax deducted at source) to find the balance due or refund owed.

Chain to **sa-overview** if the user needs to understand the filing process, or to specific income skills for detailed guidance.
