---
name: savings-interest
description: "Explains UK savings income tax rules for Self Assessment. Make sure to use this skill whenever the user mentions savings interest, personal savings allowance, bank interest, building society interest, NS&I, Premium Bonds tax, starting rate for savings, or asks whether they need to pay tax on interest from their savings accounts."
---

> **DISCLAIMER**: This skill provides general tax information only. It is NOT professional tax advice. Tax situations vary — always verify with HMRC guidance or a qualified accountant before making decisions. HMRC is the sole authority on UK tax matters.

## Purpose

This skill explains how savings income (bank and building society interest) is taxed for UK individuals. It covers the Personal Savings Allowance, the starting rate for savings, NS&I products, ISA interaction, and when savings interest triggers a Self Assessment filing requirement.

## Personal Savings Allowance (PSA)

Reference `${CLAUDE_PLUGIN_ROOT}/references/2024-25-rates.md` for the current PSA amounts. Explain the structure:

- **Basic rate taxpayers**: receive the full PSA — a set amount of savings interest tax-free each year.
- **Higher rate taxpayers**: receive a reduced PSA.
- **Additional rate taxpayers**: receive no PSA — all savings interest is taxable.

The PSA is determined by the user's overall tax band, not just their savings income. Ask the user for their total income to determine which PSA applies.

Key points:
- The PSA is a 0% rate band (like the dividend allowance), not a deduction — interest within the PSA still counts as income.
- Since April 2016, banks and building societies pay interest gross (no tax deducted at source). The user is responsible for reporting and paying any tax due.

## Starting Rate for Savings

Explain this often-overlooked allowance:

- There is a starting rate band for savings income at 0% — check the data file for the band width (up to £5,000).
- This band is reduced by £1 for every £1 of non-savings income above the personal allowance.
- If the user's non-savings income exceeds the personal allowance plus the starting rate band, the starting rate is unavailable.
- This primarily benefits individuals with very low earned income but significant savings interest (e.g. retirees with small pensions, part-time workers).

Calculate whether the user qualifies:
1. Determine non-savings income (employment, self-employment, pensions, rental).
2. Subtract the personal allowance.
3. If the result is less than the starting rate band width, the remaining amount is available at 0% for savings income.

## How Savings Interest Is Taxed

Walk through the calculation:

1. Add savings interest to total income.
2. Apply the personal allowance against non-savings income first.
3. Determine whether any starting rate band is available.
4. Apply the PSA at 0% on the next slice of savings income.
5. Tax remaining savings interest at the user's marginal rate (basic, higher, or additional — check data file for rates).

Savings income sits between non-savings income and dividend income in the stacking order. Refer to **income-tax-bands** for the full stacking explanation.

## NS&I Products

Explain the tax treatment of common National Savings & Investments products:

- **Premium Bond prizes**: Tax-free. Do not need to be reported on SA. This is one of the most common questions — confirm clearly that prizes are not taxable.
- **NS&I Direct Saver and Income Bonds**: Interest is taxable and paid gross. Must be included in savings interest on the SA return.
- **NS&I Fixed Rate Savings Bonds**: Taxable interest, reported in the year it is earned (or paid, depending on the product terms).
- **NS&I ISAs**: Tax-free as with all ISAs — not reportable.

Ask the user which NS&I products they hold to determine the correct treatment.

## ISA Interaction

Savings interest earned within any ISA wrapper (Cash ISA, Stocks and Shares ISA, Innovative Finance ISA, Lifetime ISA) is completely tax-free:

- ISA interest does not count towards the PSA.
- ISA interest does not need to be reported on the SA return.
- ISA interest does not count as income for any purpose (band calculation, HICBC, allowance taper).

Confirm with the user which savings accounts are within ISA wrappers and exclude them from the tax calculation.

## When Savings Interest Triggers Self Assessment

Advise the user on filing thresholds:

- If total untaxed savings interest exceeds the PSA, the user may need to file SA or HMRC may collect the tax by adjusting the PAYE tax code.
- HMRC receives interest data directly from banks and will often issue a Simple Assessment or adjust the tax code automatically for smaller amounts.
- SA filing is required if: the user has other SA obligations, savings interest is substantial and cannot be collected via PAYE, or HMRC issues a notice to file.
- Check `${CLAUDE_PLUGIN_ROOT}/references/2024-25-rates.md` for any specific thresholds that trigger SA filing for savings income.

## Practical Steps

1. Gather interest certificates or annual summaries from all banks and building societies.
2. Separate ISA interest (tax-free, not reported) from taxable interest.
3. Exclude Premium Bond prizes.
4. Determine the user's PSA based on their overall tax band.
5. Check eligibility for the starting rate for savings.
6. Calculate tax due on interest above the PSA and starting rate.
7. Enter taxable interest on the SA100 (or supplementary pages if applicable).

Chain to **income-tax-bands** for the full band and stacking calculation, or to **sa-overview** for filing requirements.
