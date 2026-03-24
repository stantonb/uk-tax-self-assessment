---
name: share-schemes-sip
description: "Explains UK Share Incentive Plan (SIP) and employee share scheme tax rules. Use when the user asks about SIP, share incentive plan, free shares, partnership shares, matching shares, SAYE, sharesave, company share options, or employee share schemes."
---

> **DISCLAIMER**: This skill provides general tax information only. It is NOT professional tax advice. Tax situations vary — always verify with HMRC guidance or a qualified accountant before making decisions. HMRC is the sole authority on UK tax matters.

## Share Incentive Plan (SIP) Overview

A SIP is an HMRC-approved employee share scheme that allows employers to offer shares with significant tax advantages. There are three types of SIP shares:

- **Free shares** — Given to employees by the employer at no cost, up to the annual limit.
- **Partnership shares** — Purchased by employees from pre-tax salary, up to the annual or percentage-of-salary limit.
- **Matching shares** — Given by the employer to match partnership share purchases, up to the permitted ratio.

Refer to `${CLAUDE_PLUGIN_ROOT}/references/2024-25-rates.md` for all current annual limits, salary percentage caps, and matching ratios for 2024-25.

## Tax Treatment at Each Stage

### On Acquisition

- **Free shares** and **matching shares**: No Income Tax or National Insurance at the point of award, provided shares are held in the SIP trust.
- **Partnership shares**: Purchased from **gross salary** — Income Tax and NI are not deducted on the salary used to buy them.

### During the Holding Period

Shares must be held in the SIP trust. Dividends received on SIP shares can be reinvested as **dividend shares** (tax-free if held for the required period) or taken as cash (taxed as dividend income).

### On Disposal — The 5-Year Rule

The tax treatment on withdrawal depends on how long the shares have been held:

| Holding period | Income Tax and NI liability |
|---|---|
| **0 to 3 years** | Full market value at withdrawal is taxed as employment income, subject to Income Tax and NI |
| **3 to 5 years** | The lower of market value at award or market value at withdrawal is taxed |
| **5 years or more** | **No Income Tax or NI** — full tax relief achieved |

After withdrawal, shares enter your personal ownership. Any subsequent gain from that point is subject to **Capital Gains Tax** on disposal. The CGT base cost is the market value on the date of withdrawal from the SIP trust. Refer to the rates file for CGT rates and the annual exempt amount.

## Leaving Your Employer

When you leave, SIP shares are normally withdrawn from the trust. The tax treatment follows the same holding period rules above. If you leave within 5 years, expect an Income Tax and NI charge. There is an exception: if you leave due to **injury, disability, redundancy, retirement, or TUPE transfer**, the shares may be treated as if held for the full 5 years.

## SAYE / Sharesave Basics

The **Save As You Earn (SAYE)** scheme is a separate HMRC-approved scheme:

- Save a fixed monthly amount (within HMRC limits — see the rates file) for 3 or 5 years.
- At the end, choose to buy shares at the **option price** set at the start (may include a discount of up to 20%).
- **No Income Tax or NI** on the discount at exercise, provided the option is exercised at the correct time.
- CGT applies on any gain when you later sell the shares. The base cost is the option price paid.

## Reporting on Self Assessment

- SIP shares held for 5 years or more and sold with no gain beyond the withdrawal value: typically nothing to report.
- SIP shares withdrawn before 5 years: your employer should handle the Income Tax and NI through PAYE. Verify this appears on your P11D or payslip.
- Gains on subsequent disposal of withdrawn shares: report on the **SA108 Capital Gains Tax summary pages**.
- SAYE option exercises and subsequent disposals: report any CGT liability on SA108.

## Common Pitfall

**Selling SIP shares within 5 years triggers both Income Tax and NI on the value of the shares, plus potential CGT on any further gain.** Many employees withdraw shares early without realising the combined tax cost. Always check the holding period before requesting a withdrawal. Where possible, wait for the 5-year anniversary to achieve full relief.
