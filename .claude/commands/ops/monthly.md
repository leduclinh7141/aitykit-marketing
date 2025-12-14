---
description: Monthly marketing performance review and strategy adjustment
argument-hint: [month-year]
---

## Language & Quality Standards

**CRITICAL**: Respond in the same language the user is using. If Vietnamese, respond in Vietnamese. If Spanish, respond in Spanish.

**Standards**: Token efficiency, sacrifice grammar for concision, list unresolved questions at end.

**Skills**: Activate `marketing-fundamentals`, `analytics-attribution`, `sales-workflow.md`, `crm-workflow.md` skills.

---

## Mission
Generate comprehensive monthly marketing review:
<month>$ARGUMENTS</month>

## Workflow

1. Use `researcher` agent to compile:
   - Full month metrics
   - YoY and MoM comparisons
   - Industry benchmarks

2. Use `lead-qualifier` agent to analyze:
   - Funnel performance (per CRM workflow benchmarks)
   - Lead quality trends
   - Conversion patterns
   - SLA compliance metrics

3. Use `planner` agent for:
   - Next month strategy
   - Budget allocation
   - Campaign planning

4. Use `continuity-specialist` agent for:
   - Retention metrics
   - Churn analysis
   - Customer health review

## Agent Delegation
| Task | Agent | Trigger |
|------|-------|---------|
| Metrics compilation | `researcher` | Monthly review |
| Funnel analysis | `lead-qualifier` | Performance review |
| Strategy planning | `planner` | Next month prep |
| Retention analysis | `continuity-specialist` | Customer review |
| Upsell opportunities | `upsell-maximizer` | Revenue expansion |
| Competitive intel | `researcher` | Market analysis |

## Monthly Review Framework

### Executive Dashboard

**Revenue Impact**
- Marketing-attributed revenue: $[X]
- Pipeline generated: $[X]
- CAC: $[X]
- LTV:CAC ratio: [X]:1

**Funnel Performance**
| Stage | Count | Rate | MoM Change |
|-------|-------|------|------------|
| Visitors | X | - | +/-% |
| Leads | X | X% | +/-% |
| MQLs | X | X% | +/-% |
| SQLs | X | X% | +/-% |
| Opportunities | X | X% | +/-% |
| Customers | X | X% | +/-% |

### Channel Performance

**Organic Search**
- Sessions: [X] (MoM: +/-%)
- Keywords ranking: [X]
- Top landing pages
- Technical issues

**Paid Advertising**
- Total spend: $[X]
- ROAS: [X]
- CAC by channel
- Top campaigns

**Email Marketing**
- List size: [X] (growth: +/-%)
- Avg open rate: [X%]
- Avg click rate: [X%]
- Revenue attributed: $[X]

**Social Media**
- Total followers: [X] (growth: +/-%)
- Engagement rate: [X%]
- Reach: [X]
- Referral traffic: [X]

**Content Marketing**
- Posts published: [X]
- Total views: [X]
- Avg time on page: [X]
- Content leads: [X]

### Campaign Analysis

| Campaign | Objective | Result | ROI | Status |
|----------|-----------|--------|-----|--------|
| [Campaign 1] | [Goal] | [Outcome] | [X%] | Success/Fail |

### A/B Test Results

| Test | Hypothesis | Winner | Lift | Implement? |
|------|------------|--------|------|------------|
| [Test 1] | [H] | A/B | +X% | Yes/No |

### Competitor Activity

- [Competitor 1]: [Notable activity]
- [Competitor 2]: [Notable activity]

### Budget Analysis

| Category | Budget | Actual | Variance |
|----------|--------|--------|----------|
| Paid Ads | $X | $X | +/-$X |
| Content | $X | $X | +/-$X |
| Tools | $X | $X | +/-$X |
| Events | $X | $X | +/-$X |
| **Total** | $X | $X | +/-$X |

## Next Month Strategy

### Goals
1. [SMART Goal 1]
2. [SMART Goal 2]
3. [SMART Goal 3]

### Campaigns Planned
- [Campaign 1]: [Brief description]
- [Campaign 2]: [Brief description]

### Budget Allocation
- [Channel 1]: $X (X%)
- [Channel 2]: $X (X%)

### Key Initiatives
- [Initiative 1]
- [Initiative 2]

## Output Format
```markdown
# Monthly Marketing Report: [Month Year]

## Executive Summary
[3-5 sentences summarizing the month]

### Key Results
| Metric | Actual | Target | YoY | Status |
|--------|--------|--------|-----|--------|
| Revenue Attributed | $X | $X | +X% | 🟢/🔴 |
| New Customers | X | X | +X% | 🟢/🔴 |
| MQLs Generated | X | X | +X% | 🟢/🔴 |
| CAC | $X | $X | -X% | 🟢/🔴 |
| ROAS | X | X | +X% | 🟢/🔴 |

## Funnel Analysis
[Visualization of funnel with conversion rates]

## Channel Performance Matrix
| Channel | Traffic | Leads | CAC | ROAS | Trend |
|---------|---------|-------|-----|------|-------|
| Organic | X | X | $X | N/A | ↑/↓ |
| Paid Search | X | X | $X | X | ↑/↓ |
| Social | X | X | $X | X | ↑/↓ |
| Email | X | X | $X | X | ↑/↓ |
| Referral | X | X | $X | N/A | ↑/↓ |

## Top Wins
1. [Win 1 with data and impact]
2. [Win 2 with data and impact]
3. [Win 3 with data and impact]

## Challenges & Solutions
| Challenge | Impact | Solution | Owner |
|-----------|--------|----------|-------|
| [Challenge 1] | [Impact] | [Solution] | [Name] |

## Content Performance
### Top Performing Content
1. [Content 1] - [X views, X leads]
2. [Content 2] - [X views, X leads]

### Underperforming Content
- [Content] - Issue: [X] - Action: [Y]

## Next Month Plan

### Priority Goals
1. [Goal 1]: Target [X] by [Date]
2. [Goal 2]: Target [X] by [Date]
3. [Goal 3]: Target [X] by [Date]

### Campaign Calendar
| Week | Campaign | Channel | Budget |
|------|----------|---------|--------|
| 1 | [Campaign] | [Channel] | $X |
| 2 | [Campaign] | [Channel] | $X |
| 3 | [Campaign] | [Channel] | $X |
| 4 | [Campaign] | [Channel] | $X |

### Budget Recommendation
[Recommended adjustments based on performance]

### Risks & Mitigation
- [Risk 1]: Mitigation [X]
- [Risk 2]: Mitigation [X]
```
