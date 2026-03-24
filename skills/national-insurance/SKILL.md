---
name: national-insurance
description: "Explains UK National Insurance contributions for Self Assessment. Make sure to use this skill whenever the user mentions National Insurance, NI contributions, Class 1, Class 2, Class 4, NI rates, voluntary NI, state pension qualifying years, NI number, or asks anything about how much NI they owe — even if they just say 'what NI do I pay on my side business'."
---

> **DISCLAIMER**: This skill provides general tax information only. It is NOT professional tax advice. Tax situations vary — always verify with HMRC guidance or a qualified accountant before making decisions. HMRC is the sole authority on UK tax matters.

## Overview

National Insurance contributions (NICs) fund state benefits including the State Pension. Different classes apply depending on employment status. Refer to `${CLAUDE_PLUGIN_ROOT}/references/2024-25-rates.md` for all current rates, thresholds, and limits.

## Class 1 — Employees

Class 1 NICs are deducted by the employer through PAYE. Two components:

- **Employee (primary)** — Paid on earnings between the Primary Threshold and Upper Earnings Limit at the main rate, then at the reduced rate above the UEL. See the rates file for exact thresholds and percentages.
- **Employer (secondary)** — Paid on earnings above the Secondary Threshold at the employer rate. No upper limit applies.

Class 1 is not calculated via Self Assessment. It is handled entirely through payroll. However, Class 1 contributions appear on the SA return as part of the employment information and may be relevant when checking total NI paid.

## Class 2 — Self-Employed

Class 2 NICs are a flat weekly amount paid by self-employed individuals. See the rates file for the current weekly rate and Small Profits Threshold.

- If profits are **above** the Small Profits Threshold, Class 2 is due and collected through Self Assessment.
- If profits are **below** the threshold, Class 2 is not compulsory but can be paid voluntarily to protect State Pension entitlement.

Class 2 contributions count toward qualifying years for the State Pension.

## Class 4 — Self-Employed

Class 4 NICs are profit-based and calculated through Self Assessment. They are charged on profits between the Lower Profits Limit and the Upper Profits Limit at the main rate, then at the reduced rate above the UPL. Check the rates file for current thresholds and rates.

Class 4 does **not** count toward State Pension qualifying years — only Class 2 does.

## When NI Is Calculated via Self Assessment

Self Assessment calculates and collects:

- **Class 2** — Added to the SA tax bill if self-employment profits exceed the Small Profits Threshold.
- **Class 4** — Calculated automatically on self-employment profits and added to the SA bill, including payments on account.

Employed individuals do not pay Class 1 through SA — it remains a PAYE obligation.

## Employment and Self-Employment Simultaneously

When a person is both employed and self-employed:

- **Class 1** is paid through PAYE on employment earnings.
- **Class 2 and 4** are paid through SA on self-employment profits.
- There is a **maximum contributions limit** — if combined Class 1 and Class 4 exceed the annual maximum, HMRC may defer or refund Class 2/4. Apply for deferment if this is expected, or HMRC will reconcile after the year ends.

## Voluntary Contributions — Class 2 and Class 3

Voluntary NICs fill gaps in the NI record to protect State Pension entitlement:

- **Class 2 (voluntary)** — Available to self-employed individuals with profits below the Small Profits Threshold. This is the cheapest way to build qualifying years.
- **Class 3** — Available to anyone not otherwise paying NICs (e.g., not working, living abroad). The weekly rate is higher than Class 2. See the rates file.

Gaps can usually be filled for the **previous 6 tax years**. Check the NI record online via the HMRC Personal Tax Account before paying — some years may already qualify through credits (e.g., child benefit, carer's allowance).

## Salary Sacrifice and NI Savings

Salary sacrifice reduces gross pay, which reduces both employee and employer Class 1 NICs. This is a genuine NI saving — unlike income tax relief on pensions, which can be achieved without salary sacrifice, the NI saving is **only** available through sacrifice. See the rates file for Class 1 rates to quantify the benefit.

## State Pension Qualifying Years

A full new State Pension requires **35 qualifying years**. A minimum of **10 qualifying years** is needed to receive any State Pension at all. A qualifying year is built through:

- Paying sufficient Class 1 or Class 2 NICs
- Receiving NI credits (e.g., claiming Child Benefit for a child under 12, receiving certain benefits)

Check the NI record at gov.uk/check-national-insurance-record to identify gaps and decide whether voluntary contributions are worthwhile.
