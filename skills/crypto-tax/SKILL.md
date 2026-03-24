---
name: crypto-tax
description: "Explains UK cryptocurrency and cryptoasset tax rules for Self Assessment. Make sure to use this skill whenever the user mentions crypto tax, bitcoin, ethereum, NFT tax, DeFi, staking rewards, crypto capital gains, token swaps, HMRC crypto rules, or anything about selling, swapping, or disposing of cryptocurrency — even if they just say 'I sold some crypto this year'."
---

> **DISCLAIMER**: This skill provides general tax information only. It is NOT professional tax advice. Tax situations vary — always verify with HMRC guidance or a qualified accountant before making decisions. HMRC is the sole authority on UK tax matters.

## How HMRC Classifies Cryptoassets

HMRC treats cryptocurrency as property, not currency. This means most crypto transactions fall under Capital Gains Tax (CGT) or Income Tax rules — not foreign currency rules. This applies to Bitcoin, Ethereum, NFTs, DeFi tokens, stablecoins, and all other cryptoassets.

## Capital Gains Tax on Crypto Disposals

A **disposal** occurs whenever you:

- **Sell** crypto for fiat currency (GBP, USD, etc.)
- **Swap** one token for another (including token-to-token trades)
- **Spend** crypto on goods or services
- **Gift** crypto to another person (not your spouse/civil partner)

Each disposal triggers a CGT calculation. Calculate the gain or loss as: **proceeds minus allowable costs** (acquisition cost plus transaction fees).

Refer to `${CLAUDE_PLUGIN_ROOT}/references/2024-25-rates.md` for the current annual exempt amount, CGT rates for basic-rate and higher-rate taxpayers, and the mid-year rate change effective **30 October 2024**. The October change means gains must be split into two periods with different rates applied to each.

## Income Tax on Crypto Receipts

Certain crypto activities generate **income**, not capital gains. Income Tax (and potentially National Insurance) applies to:

- **Mining** rewards (whether as a trade or hobby — the classification affects how it is reported)
- **Staking** rewards received for validating transactions
- **Airdrops** received in return for a service or as employment income
- **DeFi yields** — lending interest, liquidity pool rewards, and yield farming returns

Report crypto income in the relevant section of the Self Assessment return. The market value in GBP at the date of receipt determines the taxable amount.

## Share Pooling Rules

When calculating the cost basis of disposed tokens, apply HMRC's share pooling rules in this strict order:

1. **Same-day rule** — Match disposals first against any acquisitions of the same token on the same day.
2. **30-day bed and breakfast rule** — Then match against acquisitions of the same token within 30 days after the disposal.
3. **Section 104 pool** — Match remaining disposals against the average cost of all remaining tokens in the pooled holding.

These rules prevent artificial loss creation through selling and immediately rebuying.

## Record-Keeping Requirements

Maintain detailed records of every transaction, including:

- Date and time of each transaction
- Type of cryptoasset involved
- Amount in crypto units and GBP value at the time
- Cumulative total of tokens in the Section 104 pool
- Bank statements and wallet addresses linked to transactions
- Exchange records and transaction hashes

HMRC can request these records. Keep them for at least **5 years** after the 31 January filing deadline for the relevant tax year.

## Reporting on Self Assessment

Report crypto capital gains on the **Capital Gains Tax summary pages (SA108)**. If total disposal proceeds exceed four times the annual exempt amount, you must report even if there is no gain. Report crypto income in the appropriate section — self-employment, miscellaneous income, or employment depending on the nature of the activity.

## Common Mistakes

- **Forgetting token-to-token swaps are disposals.** Swapping ETH for a DeFi token is a taxable event, even though no fiat currency is involved.
- **Ignoring the 30-day rule.** Selling and rebuying the same token within 30 days changes the cost basis calculation.
- **Using incorrect GBP valuations.** Use a consistent, reputable source for exchange rates at the time of each transaction.
- **Missing the mid-year CGT rate change.** For 2024-25, apply the correct rate for disposals before and after 30 October 2024. Check the rates file for exact figures.
- **Failing to report small or frequent trades.** Every disposal counts, regardless of size.
