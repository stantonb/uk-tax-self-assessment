# UK Tax Self Assessment Plugin

A Claude Code plugin that helps England-based taxpayers navigate Self Assessment. It covers PAYE employees with side income, capital gains, dividends, crypto, pensions, and tax planning — all grounded in 2024/25 HMRC rates and thresholds.

> **This plugin provides general tax information only. It is NOT professional tax advice.** Tax situations vary — always verify with HMRC guidance or a qualified accountant before making decisions.

## Installation

### Claude Cowork (claude.ai)

If your organisation admin has added this plugin to a Cowork marketplace, it will appear in your available plugins automatically.

**For organisation admins (Team/Enterprise plans):**

1. Go to **Organization Settings > Plugins** in Claude Desktop
2. Upload the plugin as a ZIP, or sync from a private GitHub repo via the Claude GitHub App
3. Once added, all organisation members can activate it in Cowork

> **Note:** GitHub sync requires the repository to be **private or internal**. If using a public fork, ZIP the plugin directory and upload manually instead.

### Claude Code (CLI)

Add the repository as a marketplace, then install the plugin:

```bash
claude plugin marketplace add stantonb/uk-tax-self-assessment
claude plugin install uk-tax-self-assessment
```

### From local directory

If you've cloned the repo locally:

```bash
# Claude Code
claude plugin install /path/to/uk-tax-self-assessment
```

## What's Included

### 23 Skills (auto-activate based on context)

Skills load automatically when relevant to the conversation. They're organised into categories:

**Core**
| Skill | Covers |
|-------|--------|
| `sa-overview` | Who needs to file, registration, deadlines, penalties |
| `income-tax-bands` | Personal allowance, basic/higher/additional rates, income stacking |

**Income Types**
| Skill | Covers |
|-------|--------|
| `employment-paye` | P60, P45, P11D, tax codes, employment expenses |
| `self-employment-income` | Sole trader reporting, Class 2/4 NI, trading allowance |
| `dividend-income` | Dividend allowance, rates by band |
| `rental-income` | Property income, Section 24 mortgage interest restriction |
| `savings-interest` | PSA, starting rate for savings, NS&I, Premium Bonds |

**Investments & Capital Gains**
| Skill | Covers |
|-------|--------|
| `capital-gains-tax` | Annual exempt amount, rates, reliefs, mid-year rate change (30 Oct 2024) |
| `crypto-tax` | Disposals, token swaps, staking, DeFi, share pooling, record-keeping |
| `share-schemes-sip` | SIP free/partnership/matching shares, SAYE, the 3-tier holding period |
| `isa-tax` | ISA types, annual allowance, bed and ISA strategy |

**Reliefs & Deductions**
| Skill | Covers |
|-------|--------|
| `pension-tax-relief` | Relief at source, salary sacrifice, annual allowance, carry forward, the 60% trap |
| `marriage-allowance` | Eligibility, transfer amount, how to claim |
| `charitable-giving` | Gift Aid, payroll giving, carry-back elections |

**NI, Student Loans & Family**
| Skill | Covers |
|-------|--------|
| `national-insurance` | Class 1/2/4, voluntary contributions, state pension |
| `student-loan-repayments` | Plan 1/2/4/5, postgraduate loans, thresholds |
| `hicbc` | High Income Child Benefit Charge, ANI calculation, strategies |

**Side Business (6 sub-skills)**
| Skill | Covers |
|-------|--------|
| `side-business-overview` | Running a business alongside employment |
| `side-business-expenses` | Allowable deductions, capital vs revenue |
| `side-business-wfh` | Flat rate vs actual costs for home working |
| `side-business-rent-costs` | Claiming rent and housing costs |
| `side-business-losses` | Sideways relief, early years relief, carry forward, cash basis restriction |
| `side-business-registration` | HMRC registration, UTR, deadlines, MTD |

### 3 Commands

| Command | What it does |
|---------|-------------|
| `/tax-calculate` | Step-by-step UK tax calculation with workings |
| `/tax-checklist` | Personalised SA filing checklist |
| `/tax-plan` | Multi-horizon tax minimisation strategy |

### 2 Agents

| Agent | What it does |
|-------|-------------|
| `tax-situation-analyzer` | Gathers your full tax picture through structured questions, then chains relevant skills |
| `tax-reviewer` | Reviews your figures for missed reliefs, allowances, and planning opportunities |

### Reference Files

Tax rates, thresholds, and allowances are centralised in `references/`:
- `2024-25-rates.md` — 6 Apr 2024 to 5 Apr 2025
- `2025-26-rates.md` — 6 Apr 2025 to 5 Apr 2026

## Usage Examples

**Just describe your situation:**

> "I earn £72,000, sold some bitcoin for a £4,500 gain, have SIP shares held for 3 years, and a Plan 2 student loan. What's my tax position?"

The plugin will activate the relevant skills (employment, crypto, SIP, student loans) and provide a comprehensive breakdown with calculations.

**Use commands for structured output:**

> `/tax-calculate £85,000 salary, £3,000 dividends, £1,200 savings interest`

> `/tax-checklist I'm employed with rental income and some crypto sales`

> `/tax-plan I earn £108,000 and want to reduce my tax bill`

**Multi-source scenarios work well:**

> "I'm a nurse earning £35,000 who started a tutoring side business that made a loss. Can I claim my rent? How do I register?"

## Architecture

The plugin uses a **micro-skill architecture** with skill chaining. Instead of one monolithic tax skill, 23 small focused skills are loaded on-demand based on the conversation context. This keeps context lean — only the relevant tax knowledge is loaded for each query.

```
uk-tax-self-assessment/
├── .claude-plugin/
│   └── plugin.json
├── skills/              # 23 auto-activating skills
├── commands/            # 3 slash commands
├── agents/              # 2 specialised agents
├── references/
│   ├── 2024-25-rates.md # Rates for 2024/25
│   └── 2025-26-rates.md # Rates for 2025/26
└── evals/
    └── evals.json       # 10 test cases for benchmarking
```

## Updating for a New Tax Year

1. Edit `references/2024-25-rates.md` with the new year's rates and thresholds
2. Rename the file to match the new tax year (e.g., `2025-26-rates.md`)
3. Update the `${CLAUDE_PLUGIN_ROOT}/references/` path references in skills if the filename changes
4. Test with the eval cases in `evals/evals.json`

## Benchmarks

Tested across 10 eval scenarios (simple to complex multi-source) comparing with-skill vs baseline Claude:

| | With Skill | Without Skill |
|--|-----------|---------------|
| Assertion Pass Rate | **100%** | 91.1% |
| Avg Response Time | 112s | 77s |
| Avg Tokens | 27,148 | 12,696 |

The skill advantage is most pronounced in complex planning scenarios — PA tapering strategy (+37.5%), early years loss relief, mid-year CGT rate changes, and SIP tiered holding periods.

## License

MIT

## Disclaimer

This plugin provides general tax information for educational purposes only. It is not a substitute for professional tax advice. Always consult HMRC guidance or a qualified tax adviser before making financial decisions. HMRC is the sole authority on UK tax matters.
