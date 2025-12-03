# Part 5: Workflow & Configuration Specifications

## 5.1 Primary Finance Workflow

**File:** `.claude/workflows/primary-workflow.md`

```markdown
# Primary Finance Workflow

## Finance Operations Cycle

Plan → Execute → Analyze → Report → Comply → Audit

### Phase 1: Plan
- Delegate to `budget-planner` for annual budget
- Delegate to `budget-planner` for rolling forecasts
- Use `budgeting-forecasting` skill
- Output: Approved budget, updated forecast

### Phase 2: Execute
- Delegate to `treasury-manager` for cash operations
- Monitor daily cash position
- Execute payments and collections
- Output: Cash managed, transactions processed

### Phase 3: Analyze
- Delegate to `financial-analyst` for variance analysis
- Delegate to `financial-analyst` for trend analysis
- Use `financial-analysis` skill
- Output: Insights, explanations, recommendations

### Phase 4: Report
- Delegate to `report-generator` for statements
- Delegate to `report-generator` for board package
- Use `financial-reporting` skill
- Output: Financial statements, management reports

### Phase 5: Comply
- Delegate to `compliance-monitor` for control testing
- Delegate to `compliance-monitor` for risk assessment
- Use `compliance-controls` skill
- Output: Compliance verified, risks mitigated

### Phase 6: Audit
- Delegate to `audit-assistant` for preparation
- Delegate to `audit-assistant` for evidence gathering
- Coordinate with external auditors
- Output: Clean audit, findings remediated
```

---

## 5.2 Finance Rules

**File:** `.claude/workflows/finance-rules.md`

```markdown
# Finance Rules

## Data Accuracy Standards
- Reconcile all accounts monthly
- Verify calculations with dual controls
- Document all manual adjustments
- Maintain audit trail for changes

## Reporting Standards
- Follow GAAP/IFRS consistently
- Apply materiality thresholds
- Include comparative periods
- Disclose significant items

## Control Standards
- Segregate incompatible duties
- Require appropriate approvals
- Document control procedures
- Test controls periodically

## Compliance Standards
- Meet all filing deadlines
- Maintain required documentation
- Respond to auditors promptly
- Escalate issues immediately

## Security Standards
- Protect confidential financial data
- Restrict system access appropriately
- Log all sensitive transactions
- Encrypt data in transit and at rest
```

---

## 5.3 Orchestration Protocol

**File:** `.claude/workflows/orchestration-protocol.md`

```markdown
# Finance Agent Orchestration

## Sequential Workflows

### Month-End Close Flow
financial-analyst → report-generator → compliance-monitor
1. Complete variance analysis
2. Generate financial statements
3. Run compliance checklist

### Annual Budget Flow
budget-planner → financial-analyst → report-generator
1. Build budget model
2. Validate assumptions
3. Create budget presentation

### Audit Preparation Flow
audit-assistant → compliance-monitor → financial-analyst
1. Gather PBC items
2. Verify control documentation
3. Prepare analytical support

## Parallel Workflows

### Quarterly Review
- financial-analyst: Variance and ratio analysis
- report-generator: Financial statements and board package
- budget-planner: Forecast update
→ Combined quarterly package

### Year-End Close
- financial-analyst: Annual analysis
- compliance-monitor: Year-end compliance checklist
- audit-assistant: Audit preparation
→ Ready for external audit

## Agent Handoffs

| Trigger | From | To |
|---------|------|-----|
| Month-end close started | treasury-manager | financial-analyst |
| Analysis complete | financial-analyst | report-generator |
| Reports issued | report-generator | compliance-monitor |
| Audit scheduled | compliance-monitor | audit-assistant |
| Budget cycle start | report-generator | budget-planner |
| Forecast variance | budget-planner | financial-analyst |
```

---

## 5.4 Configuration Files

### metadata.json

```json
{
  "version": "1.0.0",
  "name": "claudekit-finance",
  "description": "AI-powered finance operations kit with specialized agents for financial analysis, reporting, budgeting, compliance, treasury, and audit support.",
  "buildDate": "2025-12-03T00:00:00.000Z",
  "repository": {
    "type": "git",
    "url": "https://github.com/claudekit/claudekit-finance.git"
  }
}
```

### CLAUDE.md

```markdown
# CLAUDE.md

## Role & Responsibilities

Your role is to assist finance professionals with analysis, reporting, budgeting, compliance, and treasury operations while maintaining accuracy, timeliness, and regulatory compliance.

## Workflows

- Primary workflow: `./.claude/workflows/primary-workflow.md`
- Finance rules: `./.claude/workflows/finance-rules.md`
- Orchestration: `./.claude/workflows/orchestration-protocol.md`

## Finance Agents

- `financial-analyst` - Analysis & modeling
- `report-generator` - Financial reporting
- `budget-planner` - Budgeting & forecasting
- `compliance-monitor` - Regulatory & controls
- `treasury-manager` - Cash & banking
- `audit-assistant` - Audit support

## Skills Catalog

- `financial-analysis` - Variance, ratios, trends
- `financial-reporting` - GAAP, statements
- `budgeting-forecasting` - Budgets, forecasts
- `compliance-controls` - SOX, controls, risk
- `treasury-operations` - Cash, FX, banking
```

### .mcp.json.example

```json
{
  "mcpServers": {
    "quickbooks": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-quickbooks"],
      "env": { "QB_ACCESS_TOKEN": "YOUR_TOKEN" }
    },
    "netsuite": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-netsuite"],
      "env": { "NS_ACCOUNT_ID": "YOUR_ID", "NS_TOKEN": "YOUR_TOKEN" }
    },
    "xero": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-xero"],
      "env": { "XERO_CLIENT_ID": "YOUR_ID", "XERO_CLIENT_SECRET": "YOUR_SECRET" }
    },
    "plaid": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-plaid"],
      "env": { "PLAID_CLIENT_ID": "YOUR_ID", "PLAID_SECRET": "YOUR_SECRET" }
    },
    "stripe": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-stripe"],
      "env": { "STRIPE_API_KEY": "YOUR_KEY" }
    },
    "bill-com": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-bill"],
      "env": { "BILL_API_KEY": "YOUR_KEY" }
    },
    "excel": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-excel"],
      "env": {}
    },
    "google-sheets": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-google-sheets"],
      "env": { "GOOGLE_CREDENTIALS": "YOUR_CREDS" }
    },
    "snowflake": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-snowflake"],
      "env": { "SNOWFLAKE_ACCOUNT": "YOUR_ACCOUNT", "SNOWFLAKE_USER": "YOUR_USER" }
    },
    "tableau": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-tableau"],
      "env": { "TABLEAU_TOKEN": "YOUR_TOKEN" }
    },
    "slack": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-slack"],
      "env": { "SLACK_BOT_TOKEN": "YOUR_TOKEN" }
    },
    "gmail": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-gmail"],
      "env": { "GMAIL_CREDENTIALS": "YOUR_CREDS" }
    }
  }
}
```

---

## 5.5 MCP Integration Summary

| Integration | Purpose | Priority |
|-------------|---------|----------|
| QuickBooks | SMB accounting | HIGH |
| NetSuite | Mid-market ERP | HIGH |
| Xero | Cloud accounting | HIGH |
| Plaid | Bank connectivity | HIGH |
| Stripe | Payment data | MEDIUM |
| Bill.com | AP automation | MEDIUM |
| Excel | Spreadsheet I/O | HIGH |
| Google Sheets | Cloud spreadsheets | MEDIUM |
| Snowflake | Data warehouse | LOW |
| Tableau | BI/visualization | LOW |
| Slack | Notifications | LOW |
| Gmail | Email reports | LOW |
