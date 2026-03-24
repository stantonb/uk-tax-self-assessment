---
name: dividend-income
description: "Explains UK dividend tax rules for Self Assessment. Make sure to use this skill whenever the user mentions dividend tax, dividend allowance, dividend vouchers, company dividends, how dividends are taxed, shareholder income, or anything about receiving dividends from investments or their own company."
---

> **DISCLAIMER**: This skill provides general tax information only. It is NOT professional tax advice. Tax situations vary — always verify with HMRC guidance or a qualified accountant before making decisions. HMRC is the sole authority on UK tax matters.

## Purpose

This skill explains how dividend income is taxed for UK individuals filing Self Assessment. It covers the dividend allowance, tax rates by band, how dividends interact with other income, record-keeping requirements, and the distinction between dividends from the user's own company versus investment holdings.

## Dividend Allowance

Reference `${CLAUDE_PLUGIN_ROOT}/references/2024-25-rates.md` for the current dividend allowance amount. Key points:

- The dividend allowance is a 0% rate band, not a deduction — dividends within the allowance still count towards total income and use up the basic/higher rate band.
- This is a critical distinction: a user whose other income already fills the basic rate band will pay higher rate tax on dividends above the allowance, even though the allowance itself is at 0%.
- The allowance applies per individual, not per source of dividends.

Ask the user for their total dividend income and their other income to determine how the allowance interacts with their tax position.

## Dividend Tax Rates

Reference the data file for the exact rates. Explain the structure:

- Dividends within the allowance: 0%
- Dividends in the basic rate band: the basic dividend rate
- Dividends in the higher rate band: the higher dividend rate
- Dividends in the additional rate band: the additional dividend rate

These rates are lower than the equivalent rates for non-savings income, reflecting that dividends are paid from post-corporation-tax profits.

## How Dividends Stack on Top of Other Income

Explain the stacking order clearly:

1. Non-savings income (employment, self-employment, pensions, rental) is taxed first.
2. Savings income is taxed next.
3. Dividend income sits on top — it is the last income to be taxed.

This means the tax band that applies to dividends depends on how much of the basic and higher rate bands have already been consumed by other income. Calculate where the user's dividends fall:

- Determine total non-savings and savings income.
- Subtract the personal allowance from non-savings income.
- Identify how much of the basic rate band remains.
- Dividends fill the remaining basic rate band first, then spill into higher and additional rates.

Offer to walk through a worked example if the user provides their income figures.

## Dividends From Own Company vs Investments

Distinguish between the two common scenarios:

**Director/shareholder of own company:**
- Dividends are a common method of extracting profits alongside a salary.
- The combined salary/dividend strategy is a planning decision — chain to **income-tax-bands** for help optimising the split.
- Dividends are not subject to National Insurance, which is why they are often preferred over additional salary.
- The company must have sufficient distributable reserves (retained profits) to pay dividends legally.
- Interim dividends can be declared by board resolution; final dividends require shareholder approval.

**Investment dividends:**
- Dividends from shares held in a general investment account (GIA) are taxable.
- Dividend vouchers or statements from the registrar/broker are the evidence for the return.
- Foreign dividends may have withholding tax deducted at source — a tax credit may be available. Ask the user if any dividends are from overseas holdings.

## ISA and Tax-Free Dividends

Dividends received within an ISA (Stocks and Shares ISA) are completely tax-free and do not need to be reported on the SA return. Confirm with the user whether any of their dividend-paying holdings are within an ISA wrapper and exclude those from the calculation.

## Record-Keeping

Advise the user to retain:

- Dividend vouchers from their own company (showing date, amount per share, total amount)
- Broker statements or tax certificates for investment dividends
- Records of any foreign dividends and withholding tax deducted
- ISA statements to evidence tax-free holdings

Records must be kept for at least 5 years after the 31 January filing deadline.

## Practical Steps

1. Gather all dividend vouchers and broker statements.
2. Separate ISA dividends (tax-free, not reported) from taxable dividends.
3. Add taxable dividends to total income and determine the band they fall into.
4. Apply the dividend allowance at 0%.
5. Tax remaining dividends at the appropriate rate from the data file.
6. Enter figures on the SA100 dividends section (or SA104 for trust distributions).

Chain to **income-tax-bands** for the full band calculation, or to **sa-overview** for filing deadlines.
