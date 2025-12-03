# Part 3: Command Specifications

## 3.1 Command Structure

```
.claude/commands/
├── analysis/
│   ├── variance.md        # /analysis:variance
│   ├── trend.md           # /analysis:trend
│   ├── ratio.md           # /analysis:ratio
│   └── model.md           # /analysis:model
├── report/
│   ├── income.md          # /report:income
│   ├── balance.md         # /report:balance
│   ├── cashflow.md        # /report:cashflow
│   └── board.md           # /report:board
├── budget/
│   ├── create.md          # /budget:create
│   ├── forecast.md        # /budget:forecast
│   ├── scenario.md        # /budget:scenario
│   └── headcount.md       # /budget:headcount
├── compliance/
│   ├── check.md           # /compliance:check
│   ├── control.md         # /compliance:control
│   ├── risk.md            # /compliance:risk
│   └── policy.md          # /compliance:policy
├── treasury/
│   ├── cash.md            # /treasury:cash
│   ├── forecast.md        # /treasury:forecast
│   ├── reconcile.md       # /treasury:reconcile
│   └── fx.md              # /treasury:fx
└── audit/
    ├── prep.md            # /audit:prep
    ├── test.md            # /audit:test
    ├── evidence.md        # /audit:evidence
    └── respond.md         # /audit:respond
```

---

## 3.2 Analysis Commands

### /analysis:variance
```yaml
---
description: Perform variance analysis comparing actual vs budget/forecast
argument-hint: [period] [comparison-type]
---
```

**Workflow:**
1. Load actual data for period
2. Load budget/forecast/prior period
3. Calculate variances ($ and %)
4. Identify significant variances
5. Generate explanations
6. Output variance report

**Agent:** `financial-analyst`

**Output:** Variance report with explanations, sorted by materiality

---

### /analysis:trend
```yaml
---
description: Analyze trends across multiple periods
argument-hint: [metric] [period-range]
---
```

**Workflow:**
1. Extract historical data
2. Calculate period-over-period changes
3. Identify patterns and seasonality
4. Project future trend
5. Output trend analysis

**Agent:** `financial-analyst`

---

### /analysis:ratio
```yaml
---
description: Calculate and analyze financial ratios
argument-hint: [ratio-category] [period]
---
```

**Workflow:**
1. Gather financial data
2. Calculate requested ratios
3. Compare to benchmarks/prior periods
4. Identify concerns/improvements
5. Output ratio analysis

**Agent:** `financial-analyst`

**Categories:** liquidity, profitability, efficiency, leverage, growth

---

### /analysis:model
```yaml
---
description: Build or update financial model
argument-hint: [model-type] [assumptions]
---
```

**Workflow:**
1. Define model structure
2. Input assumptions
3. Build calculations
4. Run scenarios
5. Output model with sensitivities

**Agent:** `financial-analyst`

---

## 3.3 Report Commands

### /report:income
```yaml
---
description: Generate income statement
argument-hint: [period] [format]
---
```

**Workflow:**
1. Extract revenue data
2. Extract expense data
3. Calculate subtotals (gross profit, EBITDA, etc.)
4. Format per GAAP/company standards
5. Output income statement

**Agent:** `report-generator`

**Output:** Formatted P&L with comparisons

---

### /report:balance
```yaml
---
description: Generate balance sheet
argument-hint: [as-of-date] [format]
---
```

**Workflow:**
1. Extract asset balances
2. Extract liability balances
3. Calculate equity
4. Verify balance (A = L + E)
5. Output balance sheet

**Agent:** `report-generator`

---

### /report:cashflow
```yaml
---
description: Generate cash flow statement
argument-hint: [period] [method]
---
```

**Workflow:**
1. Start with net income
2. Calculate operating adjustments
3. Calculate investing activities
4. Calculate financing activities
5. Reconcile to cash change
6. Output cash flow statement

**Agent:** `report-generator`

**Methods:** indirect, direct

---

### /report:board
```yaml
---
description: Generate board reporting package
argument-hint: [period] [sections]
---
```

**Workflow:**
1. Compile financial highlights
2. Add KPI dashboard
3. Include variance analysis
4. Add forecast update
5. Append supporting schedules
6. Output board package

**Agent:** `report-generator`

---

## 3.4 Budget Commands

### /budget:create
```yaml
---
description: Create annual budget or department budget
argument-hint: [fiscal-year] [scope]
---
```

**Workflow:**
1. Gather historical data
2. Apply growth assumptions
3. Build revenue projections
4. Build expense projections
5. Consolidate and validate
6. Output budget

**Agent:** `budget-planner`

**Output:** Complete budget with assumptions documented

---

### /budget:forecast
```yaml
---
description: Update rolling forecast
argument-hint: [forecast-period] [actuals-through]
---
```

**Workflow:**
1. Lock in actuals
2. Update remaining period projections
3. Apply latest assumptions
4. Calculate variance to budget
5. Output updated forecast

**Agent:** `budget-planner`

---

### /budget:scenario
```yaml
---
description: Create scenario analysis
argument-hint: [scenario-type] [variables]
---
```

**Workflow:**
1. Define base case
2. Define scenario parameters
3. Model impact on financials
4. Compare scenarios
5. Output scenario analysis

**Agent:** `budget-planner`

**Types:** best-case, worst-case, custom

---

### /budget:headcount
```yaml
---
description: Create or update headcount plan
argument-hint: [department] [period]
---
```

**Workflow:**
1. List current headcount
2. Add planned hires
3. Calculate fully-loaded costs
4. Project by period
5. Output headcount plan

**Agent:** `budget-planner`

---

## 3.5 Compliance Commands

### /compliance:check
```yaml
---
description: Run compliance checklist for period-end
argument-hint: [period] [checklist-type]
---
```

**Workflow:**
1. Load compliance checklist
2. Check each requirement
3. Flag gaps or issues
4. Generate remediation steps
5. Output compliance report

**Agent:** `compliance-monitor`

---

### /compliance:control
```yaml
---
description: Document or test internal control
argument-hint: [control-id] [action]
---
```

**Workflow:**
1. Identify control
2. Document control description
3. Define test procedures
4. Execute or plan testing
5. Output control documentation

**Agent:** `compliance-monitor`

**Actions:** document, test, update

---

### /compliance:risk
```yaml
---
description: Assess financial or compliance risk
argument-hint: [risk-area]
---
```

**Workflow:**
1. Identify risk factors
2. Assess likelihood and impact
3. Evaluate existing controls
4. Recommend mitigations
5. Output risk assessment

**Agent:** `compliance-monitor`

---

### /compliance:policy
```yaml
---
description: Create or update financial policy
argument-hint: [policy-type]
---
```

**Workflow:**
1. Research best practices
2. Draft policy content
3. Define procedures
4. Add approval workflow
5. Output policy document

**Agent:** `compliance-monitor`

**Types:** expense, travel, procurement, revenue-recognition

---

## 3.6 Treasury Commands

### /treasury:cash
```yaml
---
description: Generate cash position report
argument-hint: [as-of-date]
---
```

**Workflow:**
1. Pull bank balances
2. Add pending transactions
3. Calculate available cash
4. Identify restricted cash
5. Output cash position

**Agent:** `treasury-manager`

---

### /treasury:forecast
```yaml
---
description: Create cash flow forecast
argument-hint: [horizon] [granularity]
---
```

**Workflow:**
1. Start with current cash
2. Project receipts (AR, other)
3. Project disbursements (AP, payroll, other)
4. Calculate weekly/daily positions
5. Identify funding needs
6. Output cash forecast

**Agent:** `treasury-manager`

**Horizons:** 13-week, 6-month, annual

---

### /treasury:reconcile
```yaml
---
description: Perform bank reconciliation
argument-hint: [account] [period]
---
```

**Workflow:**
1. Load bank statement
2. Load book transactions
3. Match transactions
4. Identify reconciling items
5. Output reconciliation

**Agent:** `treasury-manager`

---

### /treasury:fx
```yaml
---
description: Analyze FX exposure and hedging
argument-hint: [currency] [period]
---
```

**Workflow:**
1. Identify currency exposures
2. Calculate net position
3. Assess hedge coverage
4. Recommend hedging actions
5. Output FX report

**Agent:** `treasury-manager`

---

## 3.7 Audit Commands

### /audit:prep
```yaml
---
description: Prepare for upcoming audit
argument-hint: [audit-type] [period]
---
```

**Workflow:**
1. Identify audit requirements
2. Create PBC list
3. Gather initial documents
4. Schedule key meetings
5. Output audit prep plan

**Agent:** `audit-assistant`

---

### /audit:test
```yaml
---
description: Perform control or substantive test
argument-hint: [test-type] [area]
---
```

**Workflow:**
1. Define test objective
2. Select sample
3. Execute test procedures
4. Document results
5. Output test workpaper

**Agent:** `audit-assistant`

---

### /audit:evidence
```yaml
---
description: Gather and organize audit evidence
argument-hint: [request-id] [evidence-type]
---
```

**Workflow:**
1. Parse auditor request
2. Locate relevant documents
3. Organize and format
4. Add context/explanations
5. Output evidence package

**Agent:** `audit-assistant`

---

### /audit:respond
```yaml
---
description: Draft response to audit inquiry
argument-hint: [inquiry]
---
```

**Workflow:**
1. Analyze inquiry
2. Research relevant facts
3. Gather supporting data
4. Draft clear response
5. Output response

**Agent:** `audit-assistant`

---

## 3.8 Command Quick Reference

| Command | Description | Agent |
|---------|-------------|-------|
| `/analysis:variance` | Variance analysis | financial-analyst |
| `/analysis:trend` | Trend analysis | financial-analyst |
| `/analysis:ratio` | Ratio analysis | financial-analyst |
| `/analysis:model` | Financial modeling | financial-analyst |
| `/report:income` | Income statement | report-generator |
| `/report:balance` | Balance sheet | report-generator |
| `/report:cashflow` | Cash flow statement | report-generator |
| `/report:board` | Board package | report-generator |
| `/budget:create` | Create budget | budget-planner |
| `/budget:forecast` | Rolling forecast | budget-planner |
| `/budget:scenario` | Scenario analysis | budget-planner |
| `/budget:headcount` | Headcount planning | budget-planner |
| `/compliance:check` | Compliance checklist | compliance-monitor |
| `/compliance:control` | Control documentation | compliance-monitor |
| `/compliance:risk` | Risk assessment | compliance-monitor |
| `/compliance:policy` | Policy creation | compliance-monitor |
| `/treasury:cash` | Cash position | treasury-manager |
| `/treasury:forecast` | Cash forecast | treasury-manager |
| `/treasury:reconcile` | Bank reconciliation | treasury-manager |
| `/treasury:fx` | FX analysis | treasury-manager |
| `/audit:prep` | Audit preparation | audit-assistant |
| `/audit:test` | Control/substantive testing | audit-assistant |
| `/audit:evidence` | Evidence gathering | audit-assistant |
| `/audit:respond` | Inquiry response | audit-assistant |
