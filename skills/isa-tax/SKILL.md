---
name: isa-tax
description: "Explains UK ISA tax rules and how ISAs interact with Self Assessment. Make sure to use this skill whenever the user mentions ISA, stocks and shares ISA, cash ISA, lifetime ISA, LISA, ISA allowance, ISA transfers, tax-free savings, bed and ISA, or asks anything about sheltering investments from tax — even if they just say 'should I use my ISA allowance'."
---

> **DISCLAIMER**: This skill provides general tax information only. It is NOT professional tax advice. Tax situations vary — always verify with HMRC guidance or a qualified accountant before making decisions. HMRC is the sole authority on UK tax matters.

## ISA Types

There are four types of Individual Savings Account:

- **Cash ISA** — Holds cash deposits. Interest earned is tax-free.
- **Stocks and Shares ISA** — Holds investments (shares, funds, bonds). All growth, dividends, and interest are tax-free.
- **Lifetime ISA (LISA)** — For those aged 18-39. Used for a first home purchase or retirement at 60. Receives a 25% government bonus.
- **Innovative Finance ISA** — Holds peer-to-peer lending investments. Interest earned is tax-free.

## Annual Allowance

You can contribute up to the ISA annual allowance across all ISA types combined in each tax year. Refer to `${CLAUDE_PLUGIN_ROOT}/references/2024-25-rates.md` for the current allowance and the separate LISA contribution limit for 2024-25. The LISA limit counts within the overall ISA allowance, not in addition to it.

## Tax-Free Status

All income and gains within an ISA are **completely tax-free**:

- No Income Tax on interest or dividends
- No Capital Gains Tax on investment growth
- No tax on withdrawals

There is **no need to report ISA income or gains on your Self Assessment return**. ISA holdings do not count towards any income or gains thresholds.

## Lifetime ISA Specifics

The LISA has unique rules:

- **25% government bonus** on contributions up to the annual LISA limit — see the rates file for the current figure.
- Qualifying withdrawals: purchasing a **first home** (property up to the price cap) or reaching **age 60**.
- **Non-qualifying withdrawals** incur a **25% withdrawal charge** on the full amount withdrawn (bonus plus growth). This effectively means you lose the bonus and pay a penalty on your own contributions.
- You can contribute to a LISA until age 50 but must open one before age 40.

## ISA Transfer Rules

- Transfer between ISA providers **without losing the tax-free wrapper** by using the formal ISA transfer process.
- **Never withdraw and redeposit** to move ISAs — the withdrawal uses up allowance, and redepositing counts as a new subscription.
- Current-year contributions can be transferred in whole or in part. Previous years' contributions can be transferred in whole or in part.
- Transfers between ISA types are permitted (e.g., Cash ISA to Stocks and Shares ISA).

## Flexible ISA Rules

Some providers offer **flexible ISAs**. With a flexible ISA:

- If you withdraw money and replace it in the **same tax year**, the replacement does not count against your annual allowance.
- Only applies if the provider has opted into flexible ISA rules — confirm with your provider.
- This is useful for short-term cash needs without permanently losing allowance space.

## Bed and ISA Strategy

A **bed and ISA** is a tax-planning technique:

1. **Sell** investments held in a taxable general investment account.
2. **Rebuy** the same (or similar) investments inside your Stocks and Shares ISA.

This crystallises a disposal for CGT purposes. If the gain is within your annual exempt amount (see `${CLAUDE_PLUGIN_ROOT}/references/2024-25-rates.md`), no CGT is due. Future growth then occurs tax-free within the ISA.

Key considerations:

- The disposal is a chargeable event — calculate the gain and check it falls within the exempt amount before proceeding.
- The 30-day bed and breakfast rule does **not** apply when you rebuy inside an ISA — you can sell shares in a taxable account and immediately rebuy the same shares in your ISA without the disposal being matched to the ISA purchase. Always confirm current HMRC guidance.
- You are limited by the annual ISA allowance for how much you can shelter each year.

## Interaction with CGT Planning

Use ISAs strategically alongside CGT planning:

- Prioritise holding high-growth or high-income assets inside the ISA wrapper.
- Use the annual ISA allowance each year to gradually move taxable holdings into the ISA via bed and ISA.
- Combine with the annual CGT exempt amount to move assets tax-efficiently over multiple tax years.
- ISA assets are not subject to CGT on death — they form part of the estate for Inheritance Tax purposes but with no CGT charge.
