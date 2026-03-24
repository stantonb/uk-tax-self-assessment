---
name: side-business-registration
description: "Explains how to register a side business with HMRC and related obligations. Make sure to use this skill whenever the user mentions registering as self-employed, getting a UTR number, HMRC registration, CIS registration, Making Tax Digital, business registration requirements, or asks anything about how to set up their business with HMRC — even if they just say 'how do I register my side business'."
---

> **DISCLAIMER**: This skill provides general tax information only. It is NOT professional tax advice. Tax situations vary — always verify with HMRC guidance or a qualified accountant before making decisions. HMRC is the sole authority on UK tax matters.

# Registering a Side Business With HMRC

## When to Register

Register as self-employed with HMRC by the deadline specified in `${CLAUDE_PLUGIN_ROOT}/references/2024-25-rates.md` under "Self Assessment Key Dates" — this is 5 October following the end of the tax year in which trading started.

**Example**: if trading started in January 2025 (within the 2024/25 tax year), register by 5 October 2025.

Late registration can lead to penalties, even if no tax is owed.

## Trading Allowance Exception

If gross trading income is below the trading allowance threshold, there is **no obligation to register or report**. The trading allowance provides a tax-free amount for casual or small-scale trading. However, if expenses exceed income (creating a loss), it may be beneficial to register and file in order to claim loss relief — see the **side-business-losses** skill.

## How to Register

1. **Register online** at gov.uk — search "register for Self Assessment" and follow the self-employed registration path.
2. If already registered for Self Assessment (e.g., for rental income), add self-employment as a new income source rather than creating a duplicate registration.
3. HMRC will issue a **Unique Taxpayer Reference (UTR)** — a 10-digit number sent by post, typically within 10 working days (longer if overseas).
4. An **Activation Code** for the online account follows separately, also by post.

Keep the UTR safe — it is needed for every Self Assessment return and is not easily replaced quickly.

## National Insurance Registration

Registering for Self Assessment also registers for Class 2 and Class 4 National Insurance. Refer to `${CLAUDE_PLUGIN_ROOT}/references/2024-25-rates.md` for current Class 2 and Class 4 rates and thresholds.

Class 2 NI is no longer mandatory if profits are above the Small Profits Threshold (from April 2024), but voluntary contributions can protect state pension entitlement.

## Choosing an Accounting Date

Select an accounting year-end for the business. The simplest options:

- **31 March** or **5 April** — aligns with the tax year, avoiding complex basis period adjustments.
- Any other date is permitted but creates additional complexity when reporting on the Self Assessment return.

For a side business, 31 March or 5 April is strongly recommended.

## Record-Keeping Obligations

From the moment trading begins, keep records of:

- All income received (invoices, bank receipts)
- All business expenses (receipts, bank statements)
- Mileage logs if claiming vehicle costs
- Home office calculations if claiming WFH costs

Retain records for the period specified in the rates file. Digital records are acceptable and recommended.

## Making Tax Digital (MTD) for Income Tax

MTD for Income Tax Self Assessment requires digital record-keeping and quarterly reporting to HMRC via compatible software.

- **From April 2026**: mandatory for self-employed individuals and landlords with gross income over £50,000.
- Below this threshold: MTD is not yet mandatory but is expected to be extended in future years.

If the side business combined with any other self-employment or rental income exceeds £50,000 gross, prepare for MTD compliance.

## VAT Registration

The VAT registration threshold is £90,000 in taxable turnover. Most side businesses will not approach this, but flag it if the user's turnover is growing. Voluntary VAT registration is possible below the threshold and may be advantageous if customers are VAT-registered businesses (they can reclaim the VAT charged).

## Business Bank Account

A separate business bank account is **recommended but not legally required** for sole traders. Benefits:

- Cleaner record-keeping
- Easier to identify business transactions
- Simpler to demonstrate business vs personal spending if HMRC enquires

## After Registration — What Happens Next

- HMRC will send a Self Assessment tax return to complete after the end of the tax year.
- File by the deadlines in `${CLAUDE_PLUGIN_ROOT}/references/2024-25-rates.md` under "Self Assessment Key Dates."
- Pay any tax and NI owed by the payment deadline.
- If the tax bill exceeds £1,000, HMRC may require payments on account (advance payments towards the next year's bill).

See the **side-business-overview** skill for how employment and self-employment income interact for tax purposes.
