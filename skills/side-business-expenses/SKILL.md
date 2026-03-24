---
name: side-business-expenses
description: "Explains allowable business expenses for UK self-employed and side business owners. Use when the user asks about business expenses, tax deductions, what expenses can I claim, allowable expenses, business costs, equipment for business, or deductible expenses."
---

> **DISCLAIMER**: This skill provides general tax information only. It is NOT professional tax advice. Tax situations vary — always verify with HMRC guidance or a qualified accountant before making decisions. HMRC is the sole authority on UK tax matters.

# Allowable Business Expenses for Side Businesses

## The Core Rule: "Wholly and Exclusively"

An expense is allowable only if it is incurred **wholly and exclusively** for the purposes of the trade. This does not mean the item can only be used for business, but the reason for the expenditure must be entirely business-driven.

Refer to `${CLAUDE_PLUGIN_ROOT}/references/2024-25-rates.md` under "Allowable Business Expenses" for the foundational rules on deductibility, cash basis turnover limits, and record retention periods.

## Common Allowable Expenses

- **Office supplies** — stationery, printer ink, postage
- **Software and subscriptions** — tools used for the business (accounting software, design tools, hosting)
- **Phone and internet** — business proportion of bills if used for both personal and business
- **Travel** — business travel costs (not ordinary commuting). Includes fuel, public transport, parking, hotels for business trips
- **Professional services** — accountant fees, legal fees related to the business
- **Insurance** — professional indemnity, public liability, business contents insurance
- **Marketing and advertising** — website costs, online ads, business cards, flyers
- **Training** — courses and materials directly related to maintaining or updating existing business skills (not training for a new trade)
- **Bank charges** — fees on business accounts, payment processing fees

## Mixed-Use Items

Where an item is used for both business and personal purposes, claim only the **business proportion**. Calculate a reasonable percentage and apply it consistently. Document the basis for the apportionment.

Examples: a laptop used 70% for business — claim 70% of the cost. A phone bill where 40% of calls are business — claim 40%.

## Capital Allowances

Items with lasting value (equipment, computers, machinery) are capital expenditure. Claim them through capital allowances rather than as a revenue expense.

- **Annual Investment Allowance (AIA)** — provides 100% relief in the year of purchase for qualifying plant and machinery. The current AIA limit is generous and unlikely to be exceeded by a side business.
- Under **cash basis**, capital expenditure on most plant and machinery is deductible when paid, simplifying the process. Cars are excluded and must use capital allowances.

## Simplified Expenses

HMRC offers flat-rate simplified expenses for certain categories, removing the need to calculate actual costs:

- **Vehicles** — flat rate per business mile instead of tracking actual fuel, insurance, and maintenance
- **Working from home** — flat rate based on hours (see **side-business-wfh** skill)
- **Living at business premises** — flat monthly rate

Simplified expenses are only available on the cash basis or for sole traders/partnerships.

## Cash Basis vs Accruals

- **Cash basis** — record income when received and expenses when paid. Available if turnover is below the threshold in the rates file. Simpler for most side businesses.
- **Accruals basis** — record income when earned and expenses when incurred, regardless of when money changes hands. Required above the cash basis threshold.

The choice affects when expenses are recognised for tax purposes.

## Non-Allowable Expenses

These cannot be claimed:

- **Commuting** — travel between home and a regular workplace
- **Clothing** — unless it is a uniform, costume, or protective equipment specific to the trade
- **Entertaining clients** — business entertainment is not deductible (though staff entertaining may be in limited circumstances)
- **Fines and penalties** — parking tickets, late-payment penalties, HMRC penalties
- **Personal drawings** — money taken out of the business for personal use
- **Depreciation** — use capital allowances instead

## Record-Keeping

Retain all receipts, invoices, bank statements, and mileage logs for the period specified in `${CLAUDE_PLUGIN_ROOT}/references/2024-25-rates.md`. Digital records are acceptable and recommended, especially as Making Tax Digital requirements expand. Keep a consistent, organised system from day one.
