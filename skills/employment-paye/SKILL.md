---
name: employment-paye
description: "Covers UK employment income and PAYE for Self Assessment purposes. Make sure to use this skill whenever the user mentions employment income, P60, P45, P11D, benefits in kind, tax codes, emergency tax, why employed people need to file Self Assessment, or anything about their salary and tax — even if they just say 'I'm employed and need to do my tax return'."
---

> **DISCLAIMER**: This skill provides general tax information only. It is NOT professional tax advice. Tax situations vary — always verify with HMRC guidance or a qualified accountant before making decisions. HMRC is the sole authority on UK tax matters.

## Purpose

This skill covers employment income within Self Assessment. Most employees have tax handled entirely through PAYE, but certain circumstances require filing SA. Explain when and how employed individuals report employment income, claim expenses, and resolve tax code issues.

## When PAYE Employees Must File Self Assessment

Ask the user whether any of these situations apply:

- Total income exceeds the high-income SA filing threshold (check `${CLAUDE_PLUGIN_ROOT}/references/2024-25-rates.md`)
- Untaxed income from other sources (rental, freelance, investments) above relevant thresholds
- High Income Child Benefit Charge applies (check `${CLAUDE_PLUGIN_ROOT}/references/2024-25-rates.md` for the HICBC threshold)
- Benefits in kind not taxed through payroll
- Employment with two or more employers causing incorrect PAYE collection
- Foreign income or overseas employment duties
- HMRC has issued a notice to file

If none apply, advise the user they likely do not need SA for employment income alone — PAYE should handle everything.

## Key Employment Forms

Explain the purpose of each form and when to expect them:

- **P60**: End-of-year certificate from the employer showing total pay and tax deducted. Issued by 31 May after the tax year ends. The user needs this to complete their SA return.
- **P45**: Issued when leaving a job. Shows pay and tax for the period of employment. Needed if the user changed jobs during the tax year.
- **P11D**: Reports benefits in kind and expenses provided by the employer (company car, private medical insurance, interest-free loans, etc.). Issued by 6 July.
- **P11D(b)**: Reports Class 1A NIC on benefits — relevant to the employer but the amounts feed into the employee's SA return.

Ask the user to gather these documents before starting the employment pages of their return.

## Benefits in Kind

Common taxable benefits to ask the user about:

- Company car and fuel benefit (reference data file for CO2-based percentages)
- Private medical insurance
- Interest-free or low-interest loans above the threshold in the data file
- Living accommodation provided by the employer
- Employer-paid subscriptions not on the HMRC approved list

If benefits are "payrolled" (taxed through PAYE in real time), they do not need separate reporting on SA. Check whether the P11D shows the benefit or whether the employer has opted into payrolling.

## Tax Codes

Help the user understand their tax code:

- The numeric portion represents the tax-free amount (multiply by 10). Check the data file for the standard code.
- Common suffixes: L (standard allowance), M/N (marriage allowance), BR (basic rate, no allowance), D0 (higher rate on all income), K (negative allowance — deductions exceed allowance).
- Emergency tax codes (W1/M1) mean PAYE is calculated non-cumulatively — the user may be owed a refund or may underpay.

If the user suspects their tax code is wrong, advise contacting HMRC or checking their Personal Tax Account online. Incorrect codes are a common reason for underpayment.

## Claiming Employment Expenses

Explain the rules for deductible employment expenses:

- Expenses must be incurred "wholly, exclusively, and necessarily" in the performance of duties — this is a strict test.
- **Flat rate deductions**: HMRC publishes fixed amounts for specific industries (e.g. nurses' uniforms, tools for mechanics). Check if the user's occupation qualifies.
- **Professional subscriptions**: Fees to HMRC-approved professional bodies are deductible. Direct the user to the HMRC list (List 3).
- **Uniform and clothing allowance**: Available if the user must wear a uniform or protective clothing and washes it themselves.
- **Working from home**: A flat rate deduction is available if the employer requires home working — check data file for the current amount.

Expenses are claimed on the SA return (employment pages) or via form P87 if the user does not otherwise need to file SA.

## Practical Steps

1. Collect P60, P45 (if applicable), and P11D.
2. Check the tax code on the final payslip against the data file's standard code.
3. Identify any benefits in kind not payrolled.
4. List any allowable expenses to claim.
5. Enter figures into the SA100 employment pages (or SA102 supplementary pages if multiple employments).

Chain to **income-tax-bands** for understanding how employment income is taxed across bands, or to **sa-overview** for the broader filing process.
