# UK Tax on Your Crypto & DeFi Activity — 2024/25 Self Assessment

> **DISCLAIMER**: This is general tax information only. It is NOT professional tax advice. Your situation involves complexity (high transaction volume, DeFi, NFTs, poor records) where professional advice from a qualified accountant or tax specialist is strongly recommended. HMRC is the sole authority on UK tax matters.

---

## Overview: What You Are Dealing With

Your activity spans two distinct tax categories: **Capital Gains Tax (CGT)** and **Income Tax**. You need to treat them separately. Here is how your activity breaks down:

| Activity | Tax Category |
|---|---|
| ETH swapped for DeFi tokens (40-50 times) | CGT — each swap is a disposal |
| Bitcoin cashed out to GBP (~£12,000 proceeds) | CGT — straightforward disposal |
| NFTs sold at a loss | CGT — reportable loss |
| Staking rewards (~£1,200) | Income Tax |
| Uniswap liquidity pool fees (~£800) | Income Tax (DeFi yield) |

---

## Section 1: Capital Gains Tax (CGT)

### What Counts as a Disposal

HMRC treats every one of the following as a taxable disposal — even where no GBP ever changes hands:

- Swapping ETH for a DeFi token (each of your 40-50 swaps is a separate CGT event)
- Cashing out Bitcoin to GBP
- Selling an NFT (even at a loss)

**The core calculation for each disposal is:**

> **Gain (or loss) = Proceeds minus Allowable Cost**

"Proceeds" means the GBP market value of what you received at the time of the transaction. "Allowable cost" is what you originally paid for the tokens you disposed of (in GBP at acquisition), plus any transaction fees directly attributable to that trade.

---

### The Annual Exempt Amount

For 2024/25, the CGT Annual Exempt Amount is **£3,000**. Gains up to this threshold incur no CGT. Losses reduce your gains before the exemption is applied — you only use the exemption to reduce gains down to zero, not to create a negative figure.

Your NFT losses should be netted against your gains. If your total net gains across all disposals are £3,000 or less, no CGT is due (though you may still need to report — see below).

---

### CGT Rates for 2024/25 — Mid-Year Rate Change

There was a rate change on **30 October 2024**, which is significant if you were trading across both periods:

| Period | Basic Rate Taxpayer | Higher Rate Taxpayer |
|---|---|---|
| 6 April 2024 – 29 October 2024 | 10% | 20% |
| 30 October 2024 – 5 April 2025 | 18% | 24% |

Crypto assets are not residential property, so the above rates apply to all your crypto gains. The rate that applies to you depends on your total taxable income for the year — add your net crypto gain to your other income and check which band it pushes you into. The basic rate band runs up to £50,270 (after your £12,570 Personal Allowance).

If you had disposals on both sides of 30 October 2024, you must calculate gains in each period separately and apply the correct rate to each.

---

### Share Pooling Rules (Section 104 Pool)

You cannot simply average all your purchase prices across the year. HMRC requires you to apply share pooling rules **in strict order** for each token type:

1. **Same-day rule**: If you bought and sold the same token on the same day, match those first.
2. **30-day bed and breakfast rule**: If you disposed of a token and then bought the same token again within 30 days, the disposal is matched to that later acquisition — not to your historical pool. This prevents artificial loss creation.
3. **Section 104 pool**: All remaining tokens of the same type are pooled together. The cost basis is the average cost of all tokens in the pool. Each acquisition adds to the pool; each disposal removes a proportionate share.

**Practical implication for your 40-50 ETH swaps**: Each time you swapped ETH for a DeFi token, you disposed of a portion of your ETH Section 104 pool. You need the GBP value of the ETH at the time of each swap to calculate the proceeds, and the average pool cost at that moment to calculate the allowable cost.

---

### Reporting Threshold

You must complete the SA108 Capital Gains pages if:

- Your total net gains exceed the £3,000 annual exempt amount, **or**
- Your total disposal **proceeds** across all crypto (and other CGT assets) exceed **£12,000** (four times the annual exempt amount of £3,000)

Given your Bitcoin cash-out alone is ~£12,000, and you have 40-50+ additional disposal events from ETH swaps and NFT sales, you almost certainly exceed the proceeds threshold regardless of whether you made a net gain. **You will need to complete the SA108.**

---

## Section 2: Income Tax on Crypto Receipts

### Staking Rewards (~£1,200)

Staking rewards from Ethereum are treated as **income** by HMRC at the market value in GBP on the date you received each reward. Your total of approximately £1,200 is reportable as miscellaneous income on your Self Assessment return.

Note: once you have received staking rewards and they enter your wallet, the tokens acquire a new cost basis (the GBP value at receipt) for future CGT purposes — if you later sell those staked tokens, you calculate any further gain or loss from that point.

### Uniswap Liquidity Pool Fees (~£800)

Fees earned from providing liquidity in a DeFi protocol are treated as **DeFi yield / income**, not capital gains. The approximately £800 you received is taxable income at the GBP value when received. Report this as miscellaneous income on your SA return.

**Important**: The underlying liquidity position itself (your deposited tokens) may also give rise to CGT events when you add or withdraw liquidity, as this can constitute a disposal of the original tokens. This is a complex and evolving area of HMRC guidance — you should check the latest HMRC cryptoasset manual (CRYPTO62000 onwards) or take specialist advice.

### Combined Income Tax Picture

Your staking rewards (~£1,200) and liquidity fees (~£800) total approximately **£2,000** in additional taxable income. This sits on top of your other income for the year and is taxed at your marginal rate (20%, 40%, or 45% depending on your total income). There are no special allowances for crypto income specifically.

---

## Section 3: The Records Problem — What to Do Now

You mentioned your records are not great. This is the most urgent issue to address, because HMRC can open enquiries up to 4 years after filing (and 6 years for careless errors). Here is a practical reconstruction approach:

### Step 1: Gather Exchange and Wallet Data

- Download full transaction history CSVs from every exchange you used (Coinbase, Binance, Kraken, etc.). Most exchanges retain this for at least several years.
- Export transaction history from your Ethereum wallets using blockchain explorers (Etherscan.io) — every wallet address has a public transaction history.
- For Uniswap activity, your wallet's on-chain history will show all LP deposits, withdrawals, and swap events.

### Step 2: Use Crypto Tax Software

With 40-50+ transactions, manual calculation is impractical. UK-compatible crypto tax tools can import exchange and on-chain data and automatically apply HMRC's share pooling rules:

- **Koinly** (widely used, UK HMRC-compliant output)
- **CoinTracker**
- **Accointing / Blockpit**
- **TaxBit**

These tools generate an SA-compatible CGT report. You will need to review the output carefully, as DeFi transactions (particularly LP positions) often require manual categorisation.

### Step 3: Establish GBP Values at Transaction Dates

For each disposal and each income receipt, you need the GBP sterling market value at the time. Use a consistent and reputable source (CoinGecko, CoinMarketCap historical data, or the rates your exchange recorded at execution). HMRC expects consistency — do not mix sources arbitrarily.

### Step 4: Consider a Specialist Crypto Accountant

Given the volume and complexity (DeFi, LP positions, NFTs, staking, and poor initial records), the cost of a specialist crypto accountant may be well worth it. They can review the reconstructed records, apply the correct rules, and ensure the return is defensible if HMRC enquires.

---

## Section 4: Filing Your Self Assessment

### Triggers — You Definitely Need to File

You are required to file a Self Assessment return for 2024/25 if you have:

- Capital gains above the £3,000 annual exempt amount, **or**
- Total disposal proceeds exceeding £12,000 (which you likely do), **or**
- Taxable income not covered by PAYE (your staking rewards and LP fees of ~£2,000 are untaxed income)

All three likely apply to you.

### Key Deadlines (2024/25 Tax Year)

| Deadline | Date |
|---|---|
| Register for Self Assessment (if new) | 5 October 2025 |
| Paper return deadline | 31 October 2025 |
| Online return deadline + payment | **31 January 2026** |
| Second payment on account | 31 July 2026 |

The online deadline is 31 January 2026. As today is 24 March 2026, this deadline has now **passed**. If you have not yet filed, you will already have incurred a £100 late filing penalty. You should file as soon as possible — penalties escalate with further delay (daily penalties of £10/day apply after 3 months late, i.e., from 1 May 2026). File immediately to stop the penalties increasing.

### Where on the Return

- **SA100** (main return): Tick the Capital Gains and/or additional income boxes
- **SA108** (CGT summary pages): Report all crypto disposals — total proceeds, total allowable costs, total gains/losses, and the net gain after the annual exempt amount
- **Income Tax sections**: Report staking rewards and LP fees as "miscellaneous income" (other income)

---

## Summary: Your Action Plan

1. **File your Self Assessment return immediately** — the 31 January 2026 deadline has passed and penalties are already accruing.

2. **Reconstruct your transaction history** — download CSVs from all exchanges, use Etherscan for on-chain history.

3. **Use crypto tax software** to apply HMRC share pooling rules across your 40-50+ disposal events.

4. **Identify the split** of disposals before and after 30 October 2024 to apply the correct CGT rate to each period.

5. **Categorise income separately** — your ~£1,200 staking rewards and ~£800 LP fees are income, not capital gains. Record the GBP value at the date of each receipt.

6. **Record your NFT losses** — these offset your gains for CGT purposes. Ensure each NFT sale is documented with proceeds and original cost.

7. **Consider specialist advice** — DeFi LP positions involve HMRC guidance that is still evolving. A crypto-specialist accountant can ensure your return is accurate and defensible.

---

*This response is based on HMRC's published guidance and 2024/25 rates as of the date of this advice. Tax law can change and individual circumstances vary. Always verify with HMRC directly or consult a qualified tax professional before filing.*
