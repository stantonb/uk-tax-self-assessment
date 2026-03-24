---
name: side-business-losses
description: "Explains UK rules for trading losses from a side business or self-employment. Make sure to use this skill whenever the user mentions business losses, trading losses, carrying forward losses, offsetting losses against employment income, loss relief, sideways loss relief, or says anything about their side business making a loss — even if they just say 'my business lost money this year, can I get tax back'."
---

> **DISCLAIMER**: This skill provides general tax information only. It is NOT professional tax advice. Tax situations vary — always verify with HMRC guidance or a qualified accountant before making decisions. HMRC is the sole authority on UK tax matters.

# Trading Losses From a Side Business

When a side business makes a loss, there are several ways to use that loss to reduce overall tax. The right choice depends on the user's circumstances, other income, and how long the business has been trading.

## Types of Loss Relief

### 1. Carry Forward Against Future Profits

Offset the loss against **future profits of the same trade**. There is no time limit — losses can be carried forward indefinitely. The loss must be set against the first available profits of the same trade.

This is the default and least restrictive form of relief.

### 2. Sideways Relief (Offset Against Other Income)

Offset the trading loss against **other income in the same tax year**. This is particularly powerful for side businesses because it can reduce tax on employment income.

**Example**: employment income of £45,000 and a side business loss of £5,000. Sideways relief reduces taxable income to £40,000, potentially saving tax at the marginal rate. Refer to `${CLAUDE_PLUGIN_ROOT}/references/2024-25-rates.md` for current income tax bands and rates to calculate the saving.

Claim sideways relief on the Self Assessment tax return. It must be claimed within 12 months of the 31 January filing deadline for the relevant tax year.

### 3. Carry Back

Offset the loss against **general income of the previous tax year**. Useful if income was higher in the prior year or the user was in a higher tax band. Must be claimed alongside or instead of sideways relief.

### 4. Terminal Loss Relief

If the trade ceases, losses in the final 12 months of trading can be carried back against profits of the same trade in the **three tax years before cessation**, latest year first.

### 5. Early Years Relief

In the **first four tax years** of a new trade, losses can be carried back against **general income of the three tax years preceding the loss year**, earliest year first. This is valuable for side businesses that are loss-making during their startup phase.

## Restrictions on Sideways Relief

Sideways relief is not unlimited. Key restrictions:

- **Uncommercial trades**: if the trade is not conducted on a commercial basis with a reasonable expectation of profit, sideways relief may be denied. HMRC will examine whether the business is genuinely a trade or a hobby.
- **Cap on sideways relief**: losses exceeding the sideways relief cap cannot be set against other income unless the trade is conducted on a commercial basis. This is often called the "hobby loss" restriction. Check `${CLAUDE_PLUGIN_ROOT}/references/2024-25-rates.md` for the current cap amount.
- **Cash basis restriction**: if the business uses the cash basis of accounting, trading losses can generally only be carried forward — sideways relief and carry back are not available. Consider opting out of cash basis in a loss-making year if sideways relief would be beneficial.

## Hobby vs Trade Test

HMRC assesses whether a business is a genuine trade by considering:

- Is it conducted with a view to profit?
- Is it carried on in a recognised business-like manner?
- How much time is devoted to the activity?
- Is the activity similar to a recognised trade?
- Have profits been made previously or are they expected?

If HMRC concludes the activity is a hobby, loss relief (especially sideways) will be denied.

## How to Claim

- **Carry forward**: automatic on the Self Assessment return — enter the loss and it carries to the next year.
- **Sideways / carry back**: claim in the Self Assessment return for the loss year. Tick the relevant boxes in the self-employment pages (SA103).
- **Early years relief**: claim in the Self Assessment return, specifying the years to carry back to. HMRC may repay tax from earlier years.

## Record-Keeping

Keep full records of losses even in years where no tax is payable. HMRC may query loss claims years later, and carried-forward losses must be substantiated. Retain records for the period specified in `${CLAUDE_PLUGIN_ROOT}/references/2024-25-rates.md`, measured from the year the loss is finally used — not the year it was incurred.
