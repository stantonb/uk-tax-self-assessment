---
name: student-loan-repayments
description: "Explains UK student loan repayment rules for Self Assessment. Make sure to use this skill whenever the user mentions student loan repayments, Plan 1, Plan 2, Plan 4, Plan 5, postgraduate loan, SLC, student loan on tax return, student loan threshold, or asks anything about student loan deductions from their pay or tax return."
---

> **DISCLAIMER**: This skill provides general tax information only. It is NOT professional tax advice. Tax situations vary — always verify with HMRC guidance or a qualified accountant before making decisions. HMRC is the sole authority on UK tax matters.

## Which Plan Applies

Student loan repayment plans depend on when and where the loan was taken:

- **Plan 1** — Loans taken out before 1 September 2012 in England/Wales, or any Income Contingent Repayment loan from Northern Ireland.
- **Plan 2** — Loans taken out on or after 1 September 2012 in England/Wales.
- **Plan 4** — Loans taken out in Scotland (post-1998 Income Contingent Repayment loans).
- **Plan 5** — Loans taken out from 1 August 2023 onwards in England (new terms for academic year 2023/24 onward).
- **Postgraduate Loan** — Separate from undergraduate plans; applies to postgraduate Master's and Doctoral loans in England and Wales.

Refer to `${CLAUDE_PLUGIN_ROOT}/references/2024-25-rates.md` for the repayment threshold and rate for each plan type.

## Thresholds and Rates

Each plan has its own annual repayment threshold. Repayments are calculated as a percentage of income above that threshold. Check the rates file for exact thresholds and rates per plan. Postgraduate loans have a separate threshold and rate.

## Repayments via PAYE vs Self Assessment

**PAYE** — Employers deduct student loan repayments automatically when earnings exceed the threshold, based on a Student Loan Notice (SL1/SL2) from HMRC. Repayments are calculated on each pay period's earnings.

**Self Assessment** — The SA return includes a section for student loan repayments. SA-based repayments apply when the individual:

- Is self-employed with profits above the threshold.
- Has untaxed income (e.g., rental income, dividends) that pushes total income above the threshold.
- Has employment income where the employer did not deduct student loan repayments.

The SA calculation uses **total income** for the year, not just self-employment profits. This can trigger additional repayments beyond what PAYE has already collected.

## When SA Triggers Additional Payments

If PAYE has already collected repayments on employment income, SA calculates the total due on all income and deducts PAYE repayments already made. The difference is collected through SA. This commonly catches individuals who:

- Have a side self-employment alongside employment.
- Receive rental income or significant dividends.
- Change jobs mid-year and repayments are not deducted by the new employer immediately.

## Multiple Plans Simultaneously

A borrower can be on multiple plans at once (e.g., Plan 2 undergraduate and a Postgraduate Loan). Each plan's repayment is calculated independently against its own threshold and rate. Both repayments are collected — they stack, not replace each other.

On the SA return, indicate each plan type. HMRC calculates each separately.

## Voluntary Overpayments

Voluntary overpayments are made **directly to the Student Loans Company (SLC)**, not via HMRC or Self Assessment. Overpaying through SLC reduces the loan balance. Do not confuse mandatory repayments (via PAYE/SA) with voluntary overpayments — they are separate processes.

## Repayment While Self-Employed

Self-employed individuals repay entirely through Self Assessment. The repayment is calculated on total profits above the plan threshold. Unlike PAYE, there is no monthly spreading — the repayment is calculated annually and due with the SA tax bill (31 January for balancing payments).

Student loan repayments are **not** included in payments on account. The full annual repayment is due as a single balancing payment.

## Common Issue: Overpayment When Income Fluctuates

Overpayment is common when:

- Income drops mid-year but PAYE has already deducted based on a higher pay period.
- The borrower repays the loan in full partway through the year but PAYE deductions continue.
- SA and PAYE both collect repayments and the total exceeds what was due.

Contact the **SLC** (not HMRC) to request a refund of overpaid student loan repayments. HMRC passes collections to SLC — refunds come from SLC. Allow time for end-of-year reconciliation before claiming.
