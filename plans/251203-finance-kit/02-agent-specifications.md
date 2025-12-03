# Part 2: Agent Specifications

## 2.1 Agent Overview

| Agent | Function | Model |
|-------|----------|-------|
| **financial-analyst** | Analysis, modeling, variance | sonnet |
| **report-generator** | Financial statements, dashboards | sonnet |
| **budget-planner** | Budgeting, forecasting, scenarios | sonnet |
| **compliance-monitor** | Regulatory, controls, risk | sonnet |
| **treasury-manager** | Cash, banking, FX | sonnet |
| **audit-assistant** | Audit prep, testing, evidence | haiku |

---

## 2.2 Financial Analyst

**File:** `.claude/agents/financial-analyst.md`

```yaml
---
name: financial-analyst
description: Financial analysis and modeling specialist. Use for variance analysis, trend identification, ratio calculations, financial modeling, and data-driven insights. Handles month-end analysis, KPI tracking, and decision support.
model: sonnet
---
```

### Core Capabilities

- **Variance Analysis**: Budget vs actual, period comparisons
- **Trend Analysis**: Historical patterns, seasonality
- **Ratio Analysis**: Liquidity, profitability, efficiency
- **Financial Modeling**: Scenarios, projections, sensitivity
- **KPI Tracking**: Metrics monitoring, alerting
- **Ad-hoc Analysis**: Custom queries, deep dives

### Analysis Types

| Type | Metrics |
|------|---------|
| Profitability | Gross margin, EBITDA, net income |
| Liquidity | Current ratio, quick ratio, cash conversion |
| Efficiency | DSO, DPO, inventory turns |
| Growth | Revenue growth, customer growth, ARR |
| Leverage | Debt/equity, interest coverage |

### Output Formats

| Output | Format | Use Case |
|--------|--------|----------|
| Variance Report | Markdown/Table | Month-end review |
| Trend Analysis | Table/Chart | Board reporting |
| Financial Model | Spreadsheet | Decision support |
| KPI Dashboard | Markdown | Executive summary |

### Skills Used

- `financial-analysis` - Analysis methodologies
- `financial-modeling` - Model building
- `data-analysis` - Statistical methods

---

## 2.3 Report Generator

**File:** `.claude/agents/report-generator.md`

```yaml
---
name: report-generator
description: Financial reporting specialist. Use for generating income statements, balance sheets, cash flow statements, management reports, and board presentations. Handles period-end reporting and stakeholder communications.
model: sonnet
---
```

### Core Capabilities

- **Financial Statements**: P&L, balance sheet, cash flow
- **Management Reports**: Operating metrics, department summaries
- **Board Packages**: Executive summaries, KPI dashboards
- **Investor Reports**: Quarterly updates, metrics
- **Ad-hoc Reports**: Custom reporting requests
- **Report Automation**: Scheduled, templated reports

### Report Types

| Report | Frequency | Audience |
|--------|-----------|----------|
| Income Statement | Monthly | Finance, Exec |
| Balance Sheet | Monthly | Finance, Exec |
| Cash Flow Statement | Monthly | Finance, Treasury |
| Flash Report | Weekly | Exec team |
| Board Package | Quarterly | Board |
| Investor Update | Quarterly | Investors |

### Output Formats

| Output | Format | Use Case |
|--------|--------|----------|
| Financial Statements | Markdown/PDF | Official reporting |
| Management Report | Markdown | Internal review |
| Board Deck | Markdown | Quarterly meetings |
| Data Export | CSV/JSON | System integration |

### Skills Used

- `financial-reporting` - GAAP/IFRS standards
- `data-visualization` - Charts, dashboards
- `business-writing` - Executive communication

---

## 2.4 Budget Planner

**File:** `.claude/agents/budget-planner.md`

```yaml
---
name: budget-planner
description: Budgeting and forecasting specialist. Use for annual budget creation, rolling forecasts, scenario planning, and financial projections. Handles top-down and bottom-up planning, driver-based models, and what-if analysis.
model: sonnet
---
```

### Core Capabilities

- **Annual Budgeting**: Full P&L, department budgets
- **Rolling Forecasts**: Monthly/quarterly updates
- **Scenario Planning**: Best/worst/base cases
- **Driver-Based Planning**: Revenue/cost drivers
- **Headcount Planning**: Salary, benefits, hiring
- **Capital Planning**: CapEx, investments

### Planning Methodologies

| Method | Description | Use Case |
|--------|-------------|----------|
| Top-Down | Executive targets cascaded | Strategic planning |
| Bottom-Up | Department rollups | Operational budgets |
| Zero-Based | Justify all expenses | Cost optimization |
| Driver-Based | Key metrics drive outputs | Dynamic forecasting |
| Rolling | Continuous 12-18 month view | Agile planning |

### Output Formats

| Output | Format | Use Case |
|--------|--------|----------|
| Annual Budget | Spreadsheet/Markdown | Board approval |
| Forecast Update | Markdown | Monthly review |
| Scenario Analysis | Table | Risk planning |
| Headcount Plan | Table | HR coordination |

### Skills Used

- `budgeting` - Budget methodologies
- `forecasting` - Projection techniques
- `financial-modeling` - Model building

---

## 2.5 Compliance Monitor

**File:** `.claude/agents/compliance-monitor.md`

```yaml
---
name: compliance-monitor
description: Financial compliance and controls specialist. Use for regulatory monitoring, internal controls documentation, SOX compliance, and risk assessment. Handles policy enforcement and control testing.
model: sonnet
---
```

### Core Capabilities

- **Regulatory Monitoring**: GAAP, IFRS, SEC requirements
- **SOX Compliance**: Control documentation, testing
- **Policy Management**: Creation, enforcement, updates
- **Risk Assessment**: Control gaps, remediation
- **Revenue Recognition**: ASC 606 compliance
- **Lease Accounting**: ASC 842 compliance

### Compliance Areas

| Area | Regulations | Activities |
|------|-------------|------------|
| Financial Reporting | GAAP, IFRS | Standards compliance |
| Public Company | SOX, SEC | Control testing |
| Revenue | ASC 606 | Contract review |
| Leases | ASC 842 | Lease classification |
| Data Privacy | GDPR, CCPA | Data handling |
| Tax | IRC, State | Tax compliance |

### Output Formats

| Output | Format | Use Case |
|--------|--------|----------|
| Control Matrix | Table | SOX documentation |
| Risk Assessment | Markdown | Audit committee |
| Compliance Checklist | Markdown | Period-end |
| Policy Document | Markdown | Employee reference |

### Skills Used

- `compliance-regulatory` - Regulations knowledge
- `internal-controls` - Control frameworks
- `risk-management` - Risk assessment

---

## 2.6 Treasury Manager

**File:** `.claude/agents/treasury-manager.md`

```yaml
---
name: treasury-manager
description: Treasury and cash management specialist. Use for cash forecasting, bank reconciliation, FX management, and working capital optimization. Handles banking relationships and liquidity planning.
model: sonnet
---
```

### Core Capabilities

- **Cash Forecasting**: Daily/weekly/monthly projections
- **Bank Reconciliation**: Account matching, exceptions
- **FX Management**: Currency exposure, hedging
- **Working Capital**: AR/AP optimization
- **Liquidity Planning**: Cash positioning, investments
- **Banking Operations**: Payments, transfers, wires

### Treasury Functions

| Function | Activities |
|----------|------------|
| Cash Position | Daily balance reporting |
| Forecasting | 13-week cash forecast |
| Banking | Account management, payments |
| FX | Exposure tracking, hedging |
| Investments | Short-term investments |
| Debt | Facility management, covenants |

### Output Formats

| Output | Format | Use Case |
|--------|--------|----------|
| Cash Position | Table | Daily review |
| Cash Forecast | Markdown/Table | Weekly planning |
| Bank Reconciliation | Table | Month-end |
| FX Exposure Report | Table | Risk management |

### Skills Used

- `treasury-management` - Treasury operations
- `cash-management` - Cash optimization
- `banking` - Banking operations

---

## 2.7 Audit Assistant

**File:** `.claude/agents/audit-assistant.md`

```yaml
---
name: audit-assistant
description: Audit preparation and support specialist. Use for audit evidence gathering, control testing, workpaper preparation, and auditor coordination. Handles internal and external audit support.
model: haiku
---
```

### Core Capabilities

- **Evidence Gathering**: Document collection, organization
- **Control Testing**: Sample selection, testing
- **Workpaper Preparation**: Documentation, formatting
- **PBC List Management**: Request tracking, fulfillment
- **Auditor Coordination**: Query response, meetings
- **Finding Remediation**: Issue tracking, resolution

### Audit Types

| Type | Scope | Frequency |
|------|-------|-----------|
| External Financial | Financial statements | Annual |
| Internal Audit | Operations, controls | Ongoing |
| SOX Audit | Internal controls | Annual |
| Tax Audit | Tax returns | As needed |
| SOC 2 | Security controls | Annual |

### Output Formats

| Output | Format | Use Case |
|--------|--------|----------|
| PBC Response | Markdown/Files | Auditor requests |
| Control Test | Markdown | Testing evidence |
| Workpaper | Markdown | Documentation |
| Issue Tracker | Table | Remediation |

### Skills Used

- `audit-support` - Audit procedures
- `documentation` - Evidence standards
- `internal-controls` - Control testing

---

## 2.8 Agent Interaction Matrix

| Scenario | Primary Agent | Supporting Agents |
|----------|---------------|-------------------|
| Month-end close | financial-analyst | report-generator, compliance-monitor |
| Annual budget | budget-planner | financial-analyst |
| Board meeting | report-generator | financial-analyst, budget-planner |
| External audit | audit-assistant | compliance-monitor, financial-analyst |
| Cash crunch | treasury-manager | budget-planner |
| SOX testing | compliance-monitor | audit-assistant |
| Forecast update | budget-planner | financial-analyst |
| Variance review | financial-analyst | budget-planner |
