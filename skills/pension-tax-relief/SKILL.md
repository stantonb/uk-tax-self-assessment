---
name: pension-tax-relief
description: "Explains UK pension tax relief rules for Self Assessment and tax planning. Make sure to use this skill whenever the user mentions pension contributions, pension tax relief, annual allowance, carry forward, salary sacrifice pension, SIPP, tapered annual allowance, pension tax benefits, or asks anything about reducing tax through pensions — even if they just say 'should I put more into my pension'."
---

> **DISCLAIMER**: This skill provides general tax information only. It is NOT professional tax advice. Tax situations vary — always verify with HMRC guidance or a qualified accountant before making decisions. HMRC is the sole authority on UK tax matters.

## How Pension Tax Relief Works

Pension contributions receive tax relief through two mechanisms:

- **Relief at source** — The pension provider claims basic rate tax back from HMRC automatically. A £100 contribution costs the member £80; the provider reclaims £20. Higher and additional rate taxpayers must claim the extra relief via Self Assessment.
- **Net pay** — The employer deducts the contribution from gross pay before calculating tax. Relief is automatic at the member's marginal rate. No SA claim is needed, but non-taxpayers miss out on the basic rate top-up.

Refer to `${CLAUDE_PLUGIN_ROOT}/references/2024-25-rates.md` for current annual allowance figures, tax band thresholds, and NI rates relevant to salary sacrifice.

## Annual Allowance and Carry Forward

The annual allowance caps the total pension contributions eligible for tax relief in a tax year. Check the rates file for the current limit. Both employer and employee contributions count toward this cap.

**Carry forward** allows use of unused annual allowance from the three previous tax years, provided the member was in a registered pension scheme during those years. Apply the earliest year's unused allowance first. This is powerful for making large one-off contributions.

## Tapered Annual Allowance

High earners face a reduced annual allowance. The taper applies when both:

- **Threshold income** exceeds the limit in the rates file, AND
- **Adjusted income** exceeds the higher threshold in the rates file.

The allowance reduces by £1 for every £2 of adjusted income above the threshold, down to the minimum stated in the rates file. Check the rates file for exact figures.

## Money Purchase Annual Allowance (MPAA)

Once a member flexibly accesses defined contribution pension benefits (e.g., drawdown income, uncrystallised funds pension lump sum), the MPAA applies. See the rates file for the current MPAA limit. Carry forward cannot be used against the MPAA.

## Salary Sacrifice

Salary sacrifice for pension contributions saves both income tax and National Insurance for the employee. The employer also saves employer NI. This makes it more efficient than personal contributions with relief at source. Confirm NI savings rates in the rates file.

Be aware that salary sacrifice reduces pensionable pay, which may affect:

- Mortgage applications (lower stated salary)
- Death-in-service benefits
- Other salary-linked benefits

## Employer Contributions and SIPPs

Employer contributions do not attract employee tax or NI but count toward the annual allowance. There is no separate cap — the overall annual allowance applies.

SIPP contributions use relief at source. The provider reclaims basic rate relief; claim higher or additional rate relief on the Self Assessment return in boxes under "Tax reliefs" on the SA100 (or equivalent online fields).

## Claiming Higher/Additional Rate Relief via SA

Enter total personal pension contributions (gross amount including basic rate relief) on the Self Assessment return. HMRC calculates the additional relief due as:

- Higher rate taxpayers: extra 20% relief
- Additional rate taxpayers: extra 25% relief

This typically extends the basic rate band by the gross contribution amount.

## Lifetime Allowance Abolition and New Lump Sum Limits

The lifetime allowance was abolished from 6 April 2024. In its place, new lump sum limits apply. See the rates file for the lump sum allowance and lump sum and death benefit allowance figures. These cap the tax-free amounts that can be taken, not the total fund size.

## Pension Contributions as a Tax Planning Tool

Pension contributions reduce **adjusted net income (ANI)**, which is the key figure for:

- **High Income Child Benefit Charge** — Reducing ANI below the HICBC threshold eliminates or reduces the charge.
- **Personal allowance tapering (the 60% trap)** — ANI above £100,000 triggers loss of £1 of personal allowance for every £2 over, creating an effective 60% marginal tax rate in the £100,000–£125,140 band. Pension contributions can restore the full personal allowance. For someone earning £112,000, an additional £12,000 in pension contributions brings ANI to £100,000, restoring £6,000 of personal allowance — the effective relief on that £12,000 contribution is dramatically higher than the headline rate.
- **Tax band management** — Contributions can bring income below the higher or additional rate threshold.

This makes pension contributions one of the most effective tax planning tools available through Self Assessment.
