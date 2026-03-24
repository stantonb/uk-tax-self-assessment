---
name: hicbc
description: "Explains the UK High Income Child Benefit Charge for Self Assessment. Use when the user asks about HICBC, high income child benefit charge, child benefit tax, child benefit clawback, child benefit and high earners, or whether to opt out of child benefit."
---

> **DISCLAIMER**: This skill provides general tax information only. It is NOT professional tax advice. Tax situations vary — always verify with HMRC guidance or a qualified accountant before making decisions. HMRC is the sole authority on UK tax matters.

## What Is the High Income Child Benefit Charge?

The HICBC is an income tax charge that claws back some or all of the Child Benefit received by a household where one partner has adjusted net income (ANI) above the threshold. Refer to `${CLAUDE_PLUGIN_ROOT}/references/2024-25-rates.md` for the current threshold and upper limit.

The charge applies to the **higher earner** in the household, regardless of which partner claims Child Benefit.

## How the Charge Is Calculated

The charge equals **1% of the Child Benefit received for every £200** of ANI above the threshold. This means:

- At the threshold: no charge.
- At the upper limit (threshold plus the full range): the charge equals 100% of the Child Benefit — effectively repaying it all.
- Between the two: a proportional charge applies.

Check the rates file for the exact threshold and upper limit. The Child Benefit amounts per child are also in the rates file.

## Adjusted Net Income (ANI)

ANI is the figure that determines the HICBC charge. It is calculated as:

1. Total taxable income (employment, self-employment, rental, dividends, savings, etc.)
2. **Minus** gross Gift Aid donations
3. **Minus** gross personal pension contributions (relief at source)
4. **Minus** trading losses and certain other deductions

ANI is not the same as taxable income — it is broadly the net income figure before personal allowances but after specific deductions.

## Strategies to Reduce ANI

Reducing ANI below the threshold eliminates the HICBC charge. Common approaches:

- **Pension contributions** — Personal contributions (grossed up) and salary sacrifice both reduce ANI. This is the most effective tool. See the pension-tax-relief skill for details.
- **Gift Aid donations** — Gross Gift Aid reduces ANI. See the charitable-giving skill.
- **Salary sacrifice** — For benefits such as pensions, cycle-to-work, or workplace nursery. Reduces gross pay and therefore ANI.

Run the numbers: if the HICBC charge is, say, £1,000, an additional pension contribution may eliminate it entirely while also providing tax relief and NI savings.

## Opting Out vs Paying the Charge

Parents can **opt out** of receiving Child Benefit. However, consider carefully:

- **NI credits** — A parent who is not working and caring for a child under 12 receives Class 3 NI credits through Child Benefit claims. Opting out of receiving payment is fine, but **still register the claim** to preserve NI credits. Use the "do not pay" option rather than not claiming at all.
- **If ANI is only slightly above the threshold**, the charge may be small and the administrative burden of SA filing is the main cost.
- **If ANI is well above the upper limit**, the charge equals the full Child Benefit — opting out avoids the SA filing obligation (if SA is not otherwise required).

## How to Report on Self Assessment

The HICBC is reported on the SA return:

- Declare the total Child Benefit received by the household during the tax year.
- HMRC calculates the charge based on ANI.
- The charge is added to the SA tax bill.

Filing a Self Assessment return is **mandatory** if liable for HICBC, even if the individual would not otherwise need to file.

## Interaction with Partners

The charge falls on the partner with the **higher ANI**, even if:

- The other partner claims Child Benefit.
- The higher earner is not the biological parent.
- The couple is not married (cohabiting partners are included).

If both partners have ANI above the threshold, only the partner with the higher ANI is charged. If both earn exactly the same, either may be charged.

## Claiming for Multiple Children

The HICBC is based on the **total** Child Benefit received for all children. More children means a larger potential charge. The 1% per £200 formula applies to the total amount, not per child.

## Common Mistake: Not Filing SA When Required

Many people are unaware they must file a Self Assessment return solely because of HICBC. Failing to file can result in:

- **Penalties** for late filing and late payment.
- **Interest** on unpaid HICBC.
- **Discovery assessments** — HMRC can go back multiple years.

If the higher earner's ANI exceeds the HICBC threshold and the household receives Child Benefit, a Self Assessment return is required. Register for SA promptly — do not wait for HMRC to contact you.
