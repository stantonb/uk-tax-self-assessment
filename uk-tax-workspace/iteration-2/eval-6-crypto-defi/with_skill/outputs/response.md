# UK Tax Treatment of Your Crypto and DeFi Activity — 2024/25

> **DISCLAIMER**: This response provides general tax information only. It is NOT professional tax advice. Your situation involves complex and evolving rules — always verify with HMRC's published guidance or consult a qualified accountant before filing. HMRC is the sole authority on UK tax matters.

---

## Overview: What You Are Dealing With

Your activity spans two distinct tax regimes:

1. **Capital Gains Tax (CGT)** — applies to disposals of cryptoassets (selling, swapping, or otherwise disposing of tokens).
2. **Income Tax** — applies to crypto received as rewards or as payment for services (staking rewards, DeFi fee income, liquidity pool rewards).

You almost certainly need to file a **Self Assessment return** for 2024/25. Given capital gains from selling Bitcoin and 40-50 token swaps, plus crypto income, you will have reportable events across both regimes. The online filing deadline is **31 January 2026**. If you have not already registered for Self Assessment, do so now via HMRC online — registration can take several weeks and missing the deadline triggers immediate penalties.

---

## 1. Your ETH-to-DeFi Token Swaps (40–50 Transactions)

### These are taxable disposals

This is the most commonly misunderstood rule in crypto taxation. **Every single token-to-token swap is a disposal for CGT purposes** — even though you never touched fiat currency. Each time you swapped ETH for a DeFi token, HMRC treats it as if you sold your ETH for its GBP market value at that moment, and separately acquired the new token at its GBP market value.

For each swap, the gain or loss is:

```
Gain / Loss = GBP value of token received (proceeds) − Cost basis of ETH disposed of
```

With 40–50 swaps, this means you could have 40–50 individual CGT calculations to perform.

### Calculating cost basis using the Section 104 pool

Your cost basis for the ETH you disposed of is not simply what you originally paid. HMRC requires you to apply share pooling rules in this strict order:

1. **Same-day rule** — if you acquired ETH on the same day you disposed of it, match those first.
2. **30-day bed and breakfast rule** — if you acquired ETH in the 30 days after a disposal, match those next (this prevents artificial loss creation).
3. **Section 104 pool** — all remaining ETH holdings are pooled together with a running average cost per token. Each disposal takes its cost from this average.

For example: if you held 5 ETH with a total pooled cost of £10,000 (average £2,000 per ETH), and you swapped 1 ETH when ETH was worth £2,800, your gain on that swap is £800.

### Gas fees

Transaction fees (gas) paid in ETH are an allowable incidental cost of disposal and can be added to your cost basis or deducted from proceeds. Keep records of all gas paid.

### Mid-year CGT rate change — important for 2024/25

For 2024/25 there was a CGT rate change mid-year. Rates applicable to crypto (a non-residential-property asset):

| Period | Basic rate taxpayer | Higher rate taxpayer |
|--------|--------------------|--------------------|
| 6 April 2024 – 29 October 2024 | 10% | 20% |
| 30 October 2024 – 5 April 2025 | 18% | 24% |

If your swaps occurred across both periods, you need to track which gains arose before and after 30 October 2024 and apply the correct rate to each.

---

## 2. Staking Rewards — £1,200 (Ethereum)

### This is Income Tax, not CGT

Staking rewards received for validating transactions are treated as **income** by HMRC, taxable at your marginal Income Tax rate in the year you receive them. The taxable amount is the **GBP market value of the tokens on the date you received them**.

Your £1,200 in staking rewards is added to your other income for the year and taxed at the relevant band rate:

| Band | Income | Rate |
|------|--------|------|
| Personal Allowance | Up to £12,570 | 0% |
| Basic rate | £12,571 – £50,270 | 20% |
| Higher rate | £50,271 – £125,140 | 40% |
| Additional rate | Over £125,140 | 45% |

The staking rewards are non-savings income and are stacked first in the income ordering. For most people, they will be taxed at 20% (basic rate) alongside employment income, or at 40% if you are a higher rate taxpayer.

### CGT applies when you later sell the staked tokens

The tokens received as staking rewards have a **cost basis equal to their GBP value on the day they were received** (because you already paid income tax on that amount). When you eventually sell or swap those tokens, any further gain above that cost basis will be subject to CGT.

Report staking rewards as **miscellaneous income** on the Self Assessment return (SA100, box for other income), unless HMRC considers the activity a trade.

---

## 3. Uniswap Liquidity Provision — £800 in Fees

This involves **two separate tax issues**:

### Issue A: Adding and removing liquidity is a disposal

When you deposited tokens into a Uniswap liquidity pool, HMRC treats that as a **disposal** of those tokens. You acquired LP tokens (pool shares) in return — those LP tokens have their own cost basis at the GBP value of tokens deposited. When you later withdrew from the pool, that is an **acquisition** of the underlying tokens (at their then-current GBP value) and a disposal of the LP tokens.

This means you may have CGT events simply from entering and exiting the liquidity pool, even before considering the fees earned. You need to calculate the gain or loss on the deposited tokens at the time of deposit.

### Issue B: LP fee rewards are Income Tax, not CGT

The **£800 in fees** you earned from providing liquidity is treated as income, not a capital gain. It is taxable at your marginal Income Tax rate, in the same way as staking rewards. The taxable amount is the GBP value of the fee income at the time it accrued or was received.

Report this as **miscellaneous income** on the Self Assessment return.

### Note on impermanent loss

Impermanent loss (the difference in value between holding tokens versus providing liquidity) is not itself a tax event. The CGT calculation is based on the actual proceeds when you dispose of your LP position, compared to the original cost basis of the tokens deposited.

---

## 4. NFT Sales at a Loss

### These are CGT events

NFTs are cryptoassets for UK tax purposes. Selling an NFT is a disposal. If you sold NFTs at a loss, you have **capital losses** — these are useful.

### Using your capital losses

Capital losses from NFT sales can be:

- **Offset against your capital gains in the same tax year** (e.g. against gains from the Bitcoin sale or ETH swaps). Losses must be used in the current year first, but only to reduce gains down to the annual exempt amount — not below it.
- **Carried forward indefinitely** to offset future gains, if not fully used this year.

To claim capital losses, you must **report them to HMRC within 4 years** of the end of the tax year in which they arose. If you do not report them, they are lost.

Make sure you have records of what you paid for each NFT and what you received on sale.

---

## 5. Bitcoin Sale — £12,000 Received

### This is a CGT disposal

Cashing out Bitcoin to GBP is a straightforward disposal. The gain is:

```
Gain = £12,000 proceeds − Cost basis of the Bitcoin sold
```

The cost basis is calculated using the same Section 104 pool rules described for ETH above — it is the average cost of your Bitcoin holdings in the pool at the time of disposal.

You also need to determine whether this sale happened before or after 30 October 2024 to apply the correct CGT rate (see the table above).

### Annual Exempt Amount

The CGT annual exempt amount for 2024/25 is **£3,000**. This is the total across all your assets — it covers your net gains from the Bitcoin sale, ETH swaps, LP token disposals, and NFTs combined (after offsetting losses). Net gains above £3,000 are chargeable to CGT.

---

## Summary of What You Owe — Broad Picture

| Activity | Tax Regime | Treatment |
|----------|-----------|-----------|
| ETH-to-DeFi swaps (40–50) | CGT | Each swap is a disposal; gain/loss per swap |
| Bitcoin sale (£12,000 proceeds) | CGT | Gain = proceeds minus pooled cost basis |
| NFT sales at a loss | CGT | Capital losses — offset or carry forward |
| Staking rewards (£1,200) | Income Tax | Taxable as income at marginal rate |
| Uniswap LP fee income (£800) | Income Tax | Taxable as miscellaneous income |
| Adding/removing Uniswap liquidity | CGT | Disposals and acquisitions of underlying tokens |

Total income to report: at minimum £2,000 (staking + LP fees) on top of your other income.

Total CGT events: potentially 40–55+ disposals (all swaps + Bitcoin sale + NFT sales + LP entries/exits).

---

## The Record-Keeping Problem — What To Do Now

You mention you have not kept great records. This is the most urgent issue. HMRC can request records for up to 5 years after the filing deadline. Here is how to approach reconstruction:

### Step 1: Pull your transaction history from exchanges and wallets

- Download CSV exports from every exchange you used (Coinbase, Binance, Kraken, etc.).
- Export transaction history from your Ethereum wallets using a blockchain explorer such as Etherscan (etherscan.io) — every on-chain transaction is permanently recorded.
- Export Uniswap LP history using a DeFi portfolio tracker.

### Step 2: Use crypto tax software

Given 40–50+ transactions, manual calculation is error-prone and time-consuming. Dedicated crypto tax tools can import your transaction history, apply the Section 104 pool rules automatically, handle the 30-day rule, and generate HMRC-compliant CGT reports. Examples include Koinly, CoinTracker, and Recap. These tools are not free but the cost is almost certainly less than an accountant doing it manually.

### Step 3: Establish GBP values for every transaction

For each transaction, you need the GBP sterling value of the tokens at the date and time of the transaction. Use a consistent, reputable source (e.g. CoinGecko historical data, CoinMarketCap, or your exchange's own trade records). HMRC requires a consistent methodology.

### Step 4: Separate income events from disposal events

For each transaction, classify it:
- Received tokens as staking rewards → income event (GBP value on receipt)
- Received LP fees → income event (GBP value on receipt)
- Swapped or sold tokens → disposal event (CGT)

---

## Reporting on Self Assessment

You will need to complete:

- **SA100** (main return) — include staking rewards and LP fee income as miscellaneous income
- **SA108** (Capital Gains Tax summary pages) — report all crypto disposals

Note: if your **total disposal proceeds** across all cryptoassets exceed four times the annual exempt amount (i.e. exceed £12,000 in 2024/25), you must complete the SA108 pages even if your net gain is zero or below the exempt amount.

Given you received £12,000 from Bitcoin alone, plus proceeds from ETH swaps and NFT sales, you will almost certainly exceed this reporting threshold.

---

## Key Deadlines

| Date | Deadline |
|------|---------|
| 5 October 2025 | Register for Self Assessment (if first return) |
| 31 October 2025 | Paper return deadline |
| **31 January 2026** | **Online return deadline + balancing payment due** |
| 31 July 2026 | Second payment on account (if applicable) |

The online return deadline is **31 January 2026**. As of today (March 2026), this deadline has already passed. If you have not yet filed your 2024/25 return, you are already late and a £100 fixed penalty will have been applied automatically. File as soon as possible — penalties escalate to daily charges (£10/day) after 3 months, and further percentage-based penalties at 6 and 12 months. If you have a reasonable excuse for late filing, you can appeal via HMRC's process.

---

## Practical Recommendations

1. **File as soon as possible** — the 31 January 2026 deadline has passed; every day you delay increases penalties.
2. **Use crypto tax software** to reconstruct and calculate your transaction history — do not attempt 40–50+ manual calculations.
3. **Separate your income events and disposal events** clearly before importing to software or passing to an accountant.
4. **Do not forget the LP deposit/withdrawal disposals** — these are frequently missed and can create unexpected gains.
5. **Report your NFT losses** even if you owe nothing on them — they can be carried forward to offset future gains.
6. **Apply the correct CGT rates** for the pre/post 30 October 2024 periods if any of your disposals straddle that date.
7. **Consider engaging a specialist crypto accountant** given the volume and complexity of your activity. The cost is typically deductible as a cost of managing your tax affairs.

---

*This response is based on HMRC's published guidance on cryptoassets and the 2024/25 tax rates. For HMRC's official guidance see: HMRC Cryptoassets Manual (CRYPTO) and the Self Assessment helpsheets HS284 (Shares and Capital Gains Tax). Always verify current rules directly with HMRC or a qualified tax professional before filing.*
