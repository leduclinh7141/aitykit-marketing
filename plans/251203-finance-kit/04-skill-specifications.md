# Part 4: Skill Specifications

## 4.1 Skill Structure

```
.claude/skills/
├── financial-analysis/
│   ├── SKILL.md
│   └── references/
│       ├── variance-analysis.md
│       ├── ratio-analysis.md
│       ├── trend-analysis.md
│       └── benchmarking.md
├── financial-reporting/
│   ├── SKILL.md
│   └── references/
│       ├── gaap-standards.md
│       ├── statement-formats.md
│       ├── consolidation.md
│       └── disclosures.md
├── budgeting-forecasting/
│   ├── SKILL.md
│   └── references/
│       ├── budget-methods.md
│       ├── forecasting-techniques.md
│       ├── scenario-planning.md
│       └── driver-models.md
├── compliance-controls/
│   ├── SKILL.md
│   └── references/
│       ├── sox-compliance.md
│       ├── internal-controls.md
│       ├── risk-assessment.md
│       └── policy-frameworks.md
└── treasury-operations/
    ├── SKILL.md
    └── references/
        ├── cash-management.md
        ├── bank-reconciliation.md
        ├── fx-management.md
        └── working-capital.md
```

---

## 4.2 Skill: financial-analysis

**Purpose:** Financial analysis methodologies and techniques

### SKILL.md Content

```markdown
# Financial Analysis

## Activation
Use when performing variance analysis, ratio calculations, trend analysis, or financial modeling.

## Core Concepts
- Variance analysis (budget vs actual, period comparisons)
- Ratio analysis (liquidity, profitability, efficiency, leverage)
- Trend analysis and seasonality detection
- Financial modeling and sensitivity analysis
- Benchmarking against industry standards
```

### Reference Files

**variance-analysis.md**
- Budget vs actual methodology
- Period-over-period analysis
- Materiality thresholds
- Variance explanation frameworks
- Root cause analysis techniques
- Favorable vs unfavorable classification

**ratio-analysis.md**
- Liquidity ratios (current, quick, cash)
- Profitability ratios (gross margin, EBITDA, ROE, ROA)
- Efficiency ratios (DSO, DPO, inventory turns)
- Leverage ratios (debt/equity, interest coverage)
- Growth metrics (revenue, customer, ARR growth)
- Industry benchmarks

**trend-analysis.md**
- Time series analysis
- Seasonality identification
- Moving averages
- Growth rate calculations
- Regression analysis basics
- Forecasting from trends

**benchmarking.md**
- Industry comparison sources
- Peer group selection
- Normalization techniques
- Performance gap analysis
- Best practice identification

---

## 4.3 Skill: financial-reporting

**Purpose:** Financial statement preparation and reporting standards

### SKILL.md Content

```markdown
# Financial Reporting

## Activation
Use when generating financial statements, management reports, or board presentations.

## Core Concepts
- GAAP/IFRS accounting standards
- Financial statement formats (P&L, balance sheet, cash flow)
- Consolidation procedures
- Disclosure requirements
- Management reporting best practices
```

### Reference Files

**gaap-standards.md**
- Revenue recognition (ASC 606)
- Lease accounting (ASC 842)
- Stock compensation (ASC 718)
- Impairment testing
- Fair value measurement
- Recent pronouncements

**statement-formats.md**
- Income statement formats (single-step, multi-step)
- Balance sheet classifications
- Cash flow statement (direct vs indirect)
- Statement of equity
- Footnote requirements
- Comparative presentations

**consolidation.md**
- Subsidiary accounting
- Intercompany eliminations
- Minority interest
- Currency translation
- Segment reporting
- Consolidation schedules

**disclosures.md**
- Required disclosures by topic
- Significant accounting policies
- Related party transactions
- Subsequent events
- Contingencies and commitments
- MD&A requirements

---

## 4.4 Skill: budgeting-forecasting

**Purpose:** Budget creation and forecasting methodologies

### SKILL.md Content

```markdown
# Budgeting & Forecasting

## Activation
Use when creating budgets, updating forecasts, or performing scenario analysis.

## Core Concepts
- Budget methodologies (top-down, bottom-up, zero-based)
- Rolling forecast techniques
- Driver-based planning
- Scenario and sensitivity analysis
- Headcount and capital planning
```

### Reference Files

**budget-methods.md**
- Top-down budgeting process
- Bottom-up budgeting process
- Zero-based budgeting (ZBB)
- Activity-based budgeting
- Incremental budgeting
- Budget calendar and timeline

**forecasting-techniques.md**
- Rolling forecast methodology
- Forecast vs budget distinction
- Reforecast triggers
- Accuracy measurement
- Bias detection and correction
- Continuous planning

**scenario-planning.md**
- Base/best/worst case definition
- Variable identification
- Sensitivity analysis
- Monte Carlo simulation basics
- Stress testing
- Contingency planning

**driver-models.md**
- Revenue driver identification
- Cost driver mapping
- Unit economics modeling
- Capacity planning
- Conversion funnel modeling
- SaaS metrics (ARR, churn, LTV)

---

## 4.5 Skill: compliance-controls

**Purpose:** Regulatory compliance and internal control frameworks

### SKILL.md Content

```markdown
# Compliance & Controls

## Activation
Use when documenting controls, assessing compliance, or managing risk.

## Core Concepts
- SOX compliance requirements
- Internal control frameworks (COSO)
- Risk assessment methodologies
- Policy development
- Control testing procedures
```

### Reference Files

**sox-compliance.md**
- SOX 302 certification requirements
- SOX 404 control documentation
- Material weakness vs significant deficiency
- Remediation procedures
- Management testing
- External auditor coordination

**internal-controls.md**
- COSO framework overview
- Control environment
- Risk assessment
- Control activities
- Information and communication
- Monitoring activities
- Control documentation standards

**risk-assessment.md**
- Risk identification techniques
- Likelihood and impact scoring
- Risk heat maps
- Control gap analysis
- Remediation prioritization
- Risk appetite and tolerance

**policy-frameworks.md**
- Policy structure and format
- Approval workflows
- Version control
- Training requirements
- Exception handling
- Policy review cycles

---

## 4.6 Skill: treasury-operations

**Purpose:** Cash management and treasury functions

### SKILL.md Content

```markdown
# Treasury Operations

## Activation
Use when managing cash, bank reconciliations, FX exposure, or working capital.

## Core Concepts
- Cash positioning and forecasting
- Bank account management
- Foreign exchange management
- Working capital optimization
- Investment and debt management
```

### Reference Files

**cash-management.md**
- Daily cash positioning
- Cash pooling structures
- Liquidity buffers
- Short-term investment policies
- Cash concentration
- Payment timing optimization

**bank-reconciliation.md**
- Reconciliation procedures
- Matching algorithms
- Outstanding items handling
- Cutoff procedures
- Reconciling item categories
- Automation opportunities

**fx-management.md**
- Currency exposure identification
- Natural hedging
- Forward contracts
- Options strategies
- Hedge accounting basics
- FX policy development

**working-capital.md**
- Accounts receivable optimization
- Accounts payable management
- Inventory optimization
- Cash conversion cycle
- Working capital metrics
- Financing options

---

## 4.7 Skills Summary

| Skill | References | Primary Agents |
|-------|------------|----------------|
| financial-analysis | 4 | financial-analyst |
| financial-reporting | 4 | report-generator |
| budgeting-forecasting | 4 | budget-planner |
| compliance-controls | 4 | compliance-monitor, audit-assistant |
| treasury-operations | 4 | treasury-manager |
| **Total** | **20** | - |
