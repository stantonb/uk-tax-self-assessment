# UK Tax Treatment of Crypto and DeFi Activity: Self Assessment Guide

## Overview

Your situation is fairly typical of an active DeFi user, but it does span several different tax categories under UK rules. HMRC has published detailed cryptoasset guidance (most recently updated in 2024) and treats crypto firmly within the existing tax framework — there is no special "crypto tax." Here is a breakdown of each activity you described, followed by practical advice on how to calculate everything.

---

## 1. ETH-to-Token Swaps (40-50 Trades)

**Tax treatment: Capital Gains Tax (CGT)**

Under HMRC's rules, swapping one cryptoasset for another is a **disposal**. It does not matter that you never converted to GBP — exchanging ETH for a DeFi token is treated as if you sold the ETH at its GBP market value at the moment of the swap, and simultaneously acquired the new token at that same value.

Each of your 40-50 swaps is therefore a separate CGT event. For each one you need:
- The GBP value of the ETH you disposed of at the time of the swap (this is your disposal proceeds)
- The allowable cost of that ETH (calculated using HMRC's pooling rules — see below)
- The resulting gain or loss

The difference between proceeds and allowable cost is your gain or loss for that disposal.

---

## 2. Bitcoin Cash-Out (£12,000 to GBP)

**Tax treatment: Capital Gains Tax (CGT)**

This is a straightforward disposal. You need:
- Proceeds: £12,000 (the GBP you received)
- Allowable cost: the pooled average cost of the bitcoin you sold (see pooling rules below)
- Gain = £12,000 minus your allowable cost

If you originally bought bitcoin for, say, £4,000 and sold for £12,000, your gain is £8,000.

---

## 3. Staking Rewards (£1,200 from Ethereum staking)

**Tax treatment: Income Tax + National Insurance (likely)**

HMRC's position (confirmed in the 2024 guidance) is that staking rewards are **miscellaneous income** (or potentially trading income if done at sufficient scale, but for most individuals it is miscellaneous income under Section 687 ITTOIA 2005). The value at the point you **receive** each reward is the taxable income figure.

- £1,200 is added to your total income for the tax year
- You pay Income Tax on it at your marginal rate (20%, 40%, or 45% depending on your total income)
- Class 2/4 NIC is generally not applicable to miscellaneous income (unlike trading income)
- The GBP value at receipt also becomes your **cost basis** for those tokens if you later dispose of them

Important: if you have not been recording the GBP value of each staking reward at the time you received it, you will need to reconstruct this from blockchain data and historical price feeds.

---

## 4. Uniswap Liquidity Provision (£800 in fees)

**Tax treatment: Likely Income Tax, but with complexity**

This is one of the less settled areas. HMRC guidance does not address liquidity mining in great detail, but the general view among tax practitioners is:

- **Fees earned from liquidity provision** are likely to be **miscellaneous income** (similar to staking), taxable at the point of receipt at their GBP market value. Your £800 in fees would therefore be added to your income.
- **Adding and removing liquidity** itself involves CGT disposals. When you deposit tokens into a Uniswap pool, HMRC may treat this as a disposal of those tokens (you are exchanging them for LP tokens). When you withdraw, you are disposing of LP tokens and reacquiring the underlying. The gain or loss on those disposals needs to be calculated separately.
- **Impermanent loss** is not separately recognised by HMRC — it is simply reflected in the proceeds and costs of the disposals described above.

The LP token mechanics mean you potentially have additional CGT events beyond just the fee income.

---

## 5. NFT Sales at a Loss

**Tax treatment: Capital Gains Tax (CGT) — losses are allowable**

NFTs are cryptoassets for HMRC purposes. Selling at a loss gives you an **allowable capital loss**, which can be:
- Set against other capital gains in the same tax year (reducing your CGT bill)
- Carried forward to future years if not fully used (you must claim them on your Self Assessment)

You must still report the disposals even if they are losses, and you should document the cost and proceeds for each NFT sold.

---

## How CGT Is Calculated: The Share Pooling Rules

HMRC requires you to use the **Section 104 pool** (share pooling) method for cryptoassets, with two priority rules applied first:

**Same-day rule:** If you buy and sell the same asset on the same day, match those transactions first.

**Bed-and-breakfasting rule (30-day rule):** If you dispose of an asset and reacquire the same asset within 30 days, match the disposal against that later acquisition (at the later acquisition's cost), not the pool. This prevents "washing" gains.

**Section 104 pool:** All remaining acquisitions of the same asset are pooled together. The pool holds a running total of the number of tokens and total allowable cost. Each disposal takes a proportionate slice of the pool cost.

Example for your ETH swaps:
- Suppose you have a pool of 5 ETH with a total cost of £6,000 (average cost £1,200 per ETH)
- You swap 1 ETH for a DeFi token when ETH is worth £2,000
- Disposal proceeds = £2,000; Allowable cost = £1,200; Gain = £800
- The pool now holds 4 ETH with total cost £4,800

Each of your 40-50 swaps must be processed in chronological order, updating the pool after each one.

---

## CGT Annual Exempt Amount

For the 2024-25 tax year, the CGT annual exempt amount is **£3,000**. Net gains below this are not taxable. However, you must still report gains on Self Assessment if your total proceeds from disposals exceed **£50,000** in the year, even if the net gain is below £3,000.

Given you cashed out £12,000 of bitcoin alone, and had 40-50 additional swap events, you likely exceed the £50,000 reporting threshold depending on the values involved — you should check this.

CGT rates for 2024-25 on cryptoassets (which are not residential property):
- Basic rate taxpayer: **18%**
- Higher/additional rate taxpayer: **24%**

Note: the rates changed from April 2024 (previously 10%/20%). Confirm the applicable rates for the specific tax year you are reporting.

---

## Income Tax Summary

Your combined income items from crypto:
- Staking rewards: £1,200
- Uniswap fees: £800 (approximately)
- **Total crypto income: ~£2,000**

This is added to your other income (salary, etc.) and taxed at your marginal rate. If you are a basic rate taxpayer, that is £400 in Income Tax on this amount (at 20%). If higher rate, £800 (at 40%).

You may have allowable expenses against this income (e.g., gas fees paid to claim staking rewards), though HMRC's position on deductibility of gas fees is not always straightforward.

---

## What to Do About Poor Records

This is a real problem but it is solvable. Here is the practical approach:

**Step 1: Export your on-chain transaction history**
Your Ethereum address is public. Use a blockchain explorer (Etherscan) to export every transaction. This will show all swaps, staking reward claims, liquidity events, and NFT sales with timestamps.

**Step 2: Use a crypto tax software tool**
Tools such as Koinly, CoinTracker, TaxBit, or Accointing can import your wallet addresses and exchange CSVs, apply HMRC's pooling rules automatically, and generate a CGT report in a format suitable for Self Assessment. These tools handle the Section 104 pool calculations and the same-day/30-day rules. Most support Uniswap LP tokens and staking rewards, though DeFi classification sometimes requires manual review.

**Step 3: Reconstruct GBP values**
For each transaction, you need the GBP price of the relevant asset at that moment. The tax tools pull historical price data automatically. For more obscure DeFi tokens, you may need to use CoinGecko's historical data or similar.

**Step 4: Obtain exchange records**
For the bitcoin cash-out, get a full transaction history from the exchange you used (Coinbase, Kraken, etc.). They are required to provide this.

**Step 5: Consider a crypto-specialist accountant**
Given 40-50 DeFi swap events, LP positions, staking, and NFT disposals, your tax position is genuinely complex. A specialist accountant familiar with HMRC's crypto guidance will pay for themselves by ensuring you do not over-report (missing allowable costs) or under-report (missing disposal events). Fees are typically £300-£800 for a situation like yours.

---

## How to Report on Self Assessment

All of this goes on your **SA100** (main tax return) and supplementary pages:

- **Capital gains:** Use the **SA108** (Capital Gains Summary) supplementary page. List each disposal (or use the "other property, assets and gains" box with a summary if there are too many to list individually). You can attach a supporting schedule with the full list of disposals.
- **Income from staking/fees:** Report on the **SA100** under "other income" (box 17 or the relevant miscellaneous income box), or on **SA101** (Additional Information) if relevant.
- You do not need to complete a separate schedule for every one of your 50 swaps — you can group them and provide a summary, attaching a spreadsheet or report as supporting documentation.

**Deadline:** 31 January following the end of the tax year (so 31 January 2026 for the 2024-25 tax year, which ended 5 April 2025).

---

## Key Risks to Be Aware Of

- **HMRC data powers:** HMRC has issued information notices to major UK exchanges (Coinbase, eToro, etc.) and receives data on UK customers. Non-disclosure is therefore increasingly detectable.
- **Discovery assessments:** HMRC can go back 4 years for innocent errors, 6 years for careless errors, and 20 years for deliberate non-disclosure.
- **Voluntary disclosure:** If you have under-reported crypto gains in prior years, HMRC's Cryptoassets Disclosure Facility (or a standard voluntary disclosure) can reduce penalties significantly compared to being investigated.

---

## Summary Table

| Activity | Tax Category | Approximate Taxable Amount |
|---|---|---|
| ETH-to-token swaps (40-50 events) | CGT | Depends on gains/losses per swap |
| Bitcoin cash-out (£12,000) | CGT | £12,000 proceeds minus pooled cost |
| NFT sales at a loss | CGT (allowable loss) | Reduces overall CGT liability |
| Staking rewards | Income Tax (miscellaneous income) | £1,200 |
| Uniswap fees | Income Tax (miscellaneous income) | ~£800 |
| LP token deposits/withdrawals | CGT | Depends on token values at each event |

---

## Recommended Next Steps

1. Export your full wallet transaction history from Etherscan and any centralised exchanges used.
2. Sign up for a crypto tax tool (Koinly is widely used in the UK and has HMRC-specific reporting).
3. Review the categorisation of DeFi income events carefully — some tools misclassify LP fees.
4. Check whether your total disposal proceeds exceed £50,000 to confirm you have a reporting obligation regardless of net gains.
5. Consider engaging a crypto-specialist accountant or tax adviser given the complexity.
6. File your Self Assessment by 31 January 2026 if reporting for 2024-25.

---

*This response is for general information only and does not constitute tax advice. Tax rules can change and individual circumstances vary. You should seek professional advice tailored to your specific situation.*
