---
name: tax-checklist
description: "Generate a personalized Self Assessment filing checklist"
argument-hint: "[optional: brief description of your situation]"
allowed-tools:
  - Read
  - AskUserQuestion
---

> **DISCLAIMER**: This checklist is for guidance only. It is NOT professional tax advice. Always verify requirements with HMRC.

Generate a personalized Self Assessment filing checklist for 2024/25.

Read rates and deadlines from `${CLAUDE_PLUGIN_ROOT}/references/2024-25-rates.md`.

Ask the user about their situation (employment, self-employment, investments, property, etc.) using AskUserQuestion, then generate a checklist with:

**Documents to gather:**
- [ ] P60 from employer(s)
- [ ] P11D for benefits in kind
- [ ] Bank/building society interest certificates
- [ ] Dividend vouchers
- [ ] Records of crypto/share disposals
- [ ] Self-employment income and expense records
- [ ] Rental income and expense records
- [ ] Pension contribution statements
- [ ] Gift Aid donation records
- [ ] Student loan statements
- [ ] Child Benefit statements (if HICBC applies)
(Only include relevant items based on user's situation)

**SA form pages needed:**
- SA100 (main return) — always
- SA102 (employment) — if employed
- SA103 (self-employment) — if self-employed
- SA105 (property) — if rental income
- SA108 (capital gains) — if disposals above exempt amount
- SA101 (additional information) — if needed

**Key deadlines:**
- List relevant deadlines from reference file

**Common mistakes to avoid:**
- Tailored to their situation
