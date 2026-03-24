---
name: sa-overview
description: "Provides an overview of the UK Self Assessment tax return process, key deadlines, who needs to file, and how to register with HMRC. Use when the user asks about Self Assessment, SA100, tax returns, filing deadlines, registering for self assessment, UTR numbers, or HMRC online services."
---

> **DISCLAIMER**: This skill provides general tax information only. It is NOT professional tax advice. Tax situations vary — always verify with HMRC guidance or a qualified accountant before making decisions. HMRC is the sole authority on UK tax matters.

## Purpose

This skill walks users through the UK Self Assessment (SA) tax return process end-to-end: who must file, how to register, key deadlines, record-keeping requirements, and penalties. It serves as the entry point and chains with topic-specific skills for detailed guidance on particular income types.

## Who Needs to File

Determine whether the user is required to file a Self Assessment return. The following triggers SA filing — ask the user which apply:

- Self-employed sole traders or partners with trading income above £1,000
- Total taxable income exceeding £150,000 (even if fully taxed via PAYE)
- Untaxed income of any kind (e.g. rental income, foreign income, tips)
- Capital gains requiring reporting (above the annual exempt amount)
- High Income Child Benefit Charge (HICBC) liability
- Income from dividends or savings interest above the relevant allowances
- Directors of companies (unless non-profit with no pay/benefits)
- Rental income from UK or overseas property
- Income from trusts, estates, or settlements
- HMRC has issued a notice to file (SA316) — filing is mandatory regardless

If none of these apply, advise the user they likely do not need SA but should check HMRC's online tool to confirm.

## Registration and UTR

Guide the user through registration:

1. Register for Self Assessment via HMRC online or by post (form SA1 for individuals, CWF1 for self-employed).
2. HMRC issues a 10-digit Unique Taxpayer Reference (UTR) by post — this takes up to 10 working days (longer if overseas).
3. Set up a Government Gateway account to file online.
4. An Activation Code is posted separately — allow additional days.

Warn the user: registering close to the deadline risks missing it. Advise registering as early as possible, especially for first-time filers.

## Key Deadlines

Refer to `${CLAUDE_PLUGIN_ROOT}/references/2024-25-rates.md` for the exact dates and penalty amounts for the 2024-25 tax year. Summarise the key milestones:

- **Registration deadline** for new self-employed filers
- **Paper return deadline** (typically 31 October following the end of the tax year)
- **Online return deadline** (typically 31 January following the end of the tax year)
- **Payment deadline** for balancing payment and first payment on account
- **Second payment on account** deadline (typically 31 July)

Ask the user whether this is their first return or a continuing obligation, then tailor the timeline accordingly.

## Record-Keeping

Advise the user on what records to keep:

- All income sources: payslips, P60s, bank statements, dividend vouchers, rental accounts
- All allowable expenses with receipts or digital records
- Capital gains records: acquisition costs, disposal proceeds, improvement costs
- Records must be kept for at least 5 years after the 31 January submission deadline (longer for some business records)

Recommend digital record-keeping and note that Making Tax Digital (MTD) for Income Tax is being phased in — check the data file for current thresholds.

## Penalties for Late Filing and Payment

Reference `${CLAUDE_PLUGIN_ROOT}/references/2024-25-rates.md` for the exact penalty structure. Outline the escalating penalty regime:

- Immediate fixed penalty for missing the filing deadline
- Daily penalties after 3 months
- Additional penalties at 6 and 12 months (percentage-based or minimum, whichever is greater)
- Late payment interest accrues from the due date
- Surcharges for late payments at 30 days, 6 months, and 12 months

If the user has already missed a deadline, advise filing as soon as possible to minimise penalties and direct them to HMRC's appeal process if they have a reasonable excuse.

## Chaining With Other Skills

This skill provides the framework. For specific income types or calculations, chain to:

- **income-tax-bands** — for band calculations and the personal allowance
- **employment-paye** — for P60/P45 and employment-related questions
- **self-employment-income** — for sole trader and freelancer reporting
- **dividend-income** — for dividend tax and allowances
- **rental-income** — for property income and landlord expenses
- **savings-interest** — for bank interest and the personal savings allowance

Ask the user which income sources they have and direct them to the relevant skill.
