---
name: side-business-overview
description: "Provides an overview of running a side business alongside employment in the UK for tax purposes. Make sure to use this skill whenever the user mentions having a side business, side hustle, second job, freelancing alongside employment, running a business while employed, selling things online, Etsy shop, tutoring income, or any form of extra income from self-directed work — even if they just say 'I make some money on the side'. This skill orchestrates the other side-business sub-skills."
---

> **DISCLAIMER**: This skill provides general tax information only. It is NOT professional tax advice. Tax situations vary — always verify with HMRC guidance or a qualified accountant before making decisions. HMRC is the sole authority on UK tax matters.

# Side Business Overview — Running a Business Alongside Employment

## Gather Key Information First

Before advising on tax obligations, ask the user:

1. **What does the business do?** (services, goods, digital products, etc.)
2. **Business structure** — sole trader or partnership?
3. **When did trading start?** (determines registration deadline and available reliefs)
4. **Approximate annual turnover and profit** (triggers different obligations at different levels)
5. **Do you work from home for the business?** (unlocks WFH deductions)

These answers determine which sub-skills to chain into.

## Trading Allowance

If gross income from the side business is under the trading allowance threshold, there is no obligation to register or report. Refer to `${CLAUDE_PLUGIN_ROOT}/references/2024-25-rates.md` under "Allowable Business Expenses" and "Self Assessment Key Dates" for the current trading allowance amount and registration deadlines.

If income exceeds the trading allowance, registration and Self Assessment filing are required.

## Registration with HMRC

Register as self-employed by the deadline shown in the rates file under "Self Assessment Key Dates." Failing to register on time can result in penalties. See the **side-business-registration** skill for full registration guidance including UTR numbers, Making Tax Digital, and VAT thresholds.

## How Employment + Self-Employment Income Stacks

Employment income is taxed first through PAYE. Self-employment profit is then added on top. The combined total determines the applicable tax band. Refer to `${CLAUDE_PLUGIN_ROOT}/references/2024-25-rates.md` for current income tax bands and rates.

Example: if PAYE earnings already use up the Personal Allowance and basic rate band, side business profits may fall partly or entirely into the higher rate band.

## National Insurance

Self-employment profits attract different NI classes on top of Class 1 NI already paid through employment:

- **Class 2 NI** — refer to the rates file for the current Small Profits Threshold and voluntary rate.
- **Class 4 NI** — charged on profits above the lower threshold. Refer to the rates file for Class 4 bands and rates.

Class 1 NI from employment and Class 4 NI from self-employment are calculated independently. There is no offset between them.

## Self Assessment Filing

Once registered, file a Self Assessment tax return each year. The return includes both employment income (from P60) and self-employment income. Key deadlines are in `${CLAUDE_PLUGIN_ROOT}/references/2024-25-rates.md` under "Self Assessment Key Dates."

Payments on account may be required if the tax bill exceeds £1,000 and less than 80% was collected at source through PAYE.

## Chain to Sub-Skills

Based on the user's situation, direct them to:

- **side-business-expenses** — what costs can be deducted from profits
- **side-business-wfh** — flat rate vs actual cost home office deductions
- **side-business-rent-costs** — claiming rent, mortgage interest, and housing costs
- **side-business-losses** — offsetting losses against employment income or carrying forward
- **side-business-registration** — step-by-step HMRC registration, UTR, MTD obligations

## Key Reminders

- Keep business and personal finances separate where possible.
- Retain all records for the period specified in the rates file.
- Consider setting aside 25-30% of profit for tax and NI.
- Payment on account means the first year's tax bill may effectively cover 18 months.
