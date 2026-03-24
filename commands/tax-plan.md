---
name: tax-plan
description: "Create a personalized tax minimization plan for current and future years"
argument-hint: "[optional: current salary or brief situation]"
allowed-tools:
  - Read
  - AskUserQuestion
  - Bash
---

> **DISCLAIMER**: This plan provides general tax planning suggestions only. It is NOT professional tax advice. Always consult a qualified accountant before making financial decisions based on tax planning.

Create a personalized tax planning strategy. Read rates from `${CLAUDE_PLUGIN_ROOT}/references/2024-25-rates.md`.

Gather the user's current situation via AskUserQuestion:
- Current gross salary and any expected changes
- Existing pension contributions (% or £)
- ISA usage
- Any share schemes available (SIP, SAYE)
- Family situation (married, children, partner's income)
- Any investments outside ISAs
- Side business income if any
- Student loans
- Planned major events (property sale, large bonus, retirement)

Then create a plan covering:

**Immediate actions (this tax year):**
- Pension top-up opportunities before 5 April
- ISA contributions before allowance resets
- Capital gains harvesting (using annual exempt amount)
- Gift Aid timing

**Next tax year planning:**
- Optimal pension contribution strategy
- Salary sacrifice opportunities
- ISA strategy (stocks & shares vs cash vs LISA)
- SIP maximization if available
- HICBC mitigation if applicable
- Personal allowance recovery if near £100k

**Longer term (2-3 years):**
- CGT planning for planned disposals
- Pension carry forward strategy
- Marriage Allowance optimization
- Side business structuring

Present as actionable steps with estimated tax savings where possible. Prioritize by impact.
