---
description: Generate client-ready monthly marketing report
argument-hint: [client-or-project] [month-year]
---

Activate `marketing-fundamentals`, `analytics-attribution`, `sales-workflow.md`, `crm-workflow.md` skills.

## Mission
Generate comprehensive client-ready monthly report:
<context>$ARGUMENTS</context>

## Workflow

1. Use `researcher` agent to compile:
   - Full month metrics with MoM/YoY
   - Campaign ROI analysis
   - Competitive landscape

2. Use `lead-qualifier` agent to analyze:
   - Funnel performance vs CRM benchmarks
   - Lead quality and velocity
   - Attribution data
   - SLA compliance review

3. Use `copywriter` agent to:
   - Craft executive narrative
   - Present insights clearly
   - Frame strategic recommendations

4. Use `planner` agent for:
   - Next month recommendations
   - Budget optimization suggestions

## Agent Delegation
| Task | Agent | Trigger |
|------|-------|---------|
| Data compilation | `researcher` | Report generation |
| Funnel analysis | `lead-qualifier` | Performance review |
| Competitive intel | `researcher` | Market analysis |
| Executive narrative | `copywriter` | Report writing |
| Strategy recommendations | `planner` | Next month planning |
| Retention metrics | `continuity-specialist` | Customer analysis |

## Output Format
```markdown
# Monthly Marketing Report
**Client:** [Client Name]
**Period:** [Month Year]
**Prepared by:** [Agency/Name]
**Date:** [Report Date]

---

## Executive Summary

### The Bottom Line
[1-2 sentences on revenue impact and business results]

### Month Highlights
- [Highlight 1 with metric]
- [Highlight 2 with metric]
- [Highlight 3 with metric]

### Strategic Insight
[Key learning that should inform future strategy]

---

## Business Impact

### Revenue Attribution
| Metric | This Month | Last Month | MoM | YoY |
|--------|------------|------------|-----|-----|
| Marketing Revenue | $X | $X | +X% | +X% |
| Pipeline Generated | $X | $X | +X% | +X% |
| New Customers | X | X | +X% | +X% |
| Customer LTV | $X | $X | +X% | +X% |

### ROI Summary
| Channel | Investment | Revenue | ROI |
|---------|------------|---------|-----|
| Paid Search | $X | $X | X% |
| Paid Social | $X | $X | X% |
| Content | $X | $X | X% |
| Email | $X | $X | X% |
| **Total** | $X | $X | X% |

---

## Funnel Performance

### Full Funnel View
```
Visitors: X (+X% MoM)
    ↓ X% conversion
Leads: X (+X% MoM)
    ↓ X% conversion
MQLs: X (+X% MoM)
    ↓ X% conversion
SQLs: X (+X% MoM)
    ↓ X% conversion
Customers: X (+X% MoM)
```

### Stage Analysis
| Stage | Volume | Rate | Benchmark | Gap |
|-------|--------|------|-----------|-----|
| Visitor → Lead | X% | X% | 3% | +/-X% |
| Lead → MQL | X% | X% | 20% | +/-X% |
| MQL → SQL | X% | X% | 30% | +/-X% |
| SQL → Customer | X% | X% | 25% | +/-X% |

### Velocity Metrics
- Avg time to MQL: X days
- Avg time to SQL: X days
- Avg sales cycle: X days

---

## Channel Deep Dive

### Organic Search
| Metric | Actual | Target | Status |
|--------|--------|--------|--------|
| Organic Sessions | X | X | 🟢 |
| Keywords in Top 10 | X | X | 🟢 |
| Organic Leads | X | X | 🟡 |

**Top Ranking Improvements:**
- [Keyword 1]: Position X → X
- [Keyword 2]: Position X → X

### Paid Advertising
| Platform | Spend | Impressions | Clicks | Conv | CPA | ROAS |
|----------|-------|-------------|--------|------|-----|------|
| Google Ads | $X | X | X | X | $X | X |
| Meta Ads | $X | X | X | X | $X | X |
| LinkedIn | $X | X | X | X | $X | X |
| **Total** | $X | X | X | X | $X | X |

### Email Marketing
| Metric | Actual | Benchmark | Status |
|--------|--------|-----------|--------|
| List Size | X | - | ↑X% |
| Avg Open Rate | X% | 25% | 🟢/🔴 |
| Avg Click Rate | X% | 3% | 🟢/🔴 |
| Unsubscribe Rate | X% | <0.5% | 🟢/🔴 |
| Revenue | $X | - | ↑X% |

### Social Media
| Platform | Followers | Reach | Engagement | Traffic |
|----------|-----------|-------|------------|---------|
| LinkedIn | X (+X) | X | X% | X |
| Twitter/X | X (+X) | X | X% | X |
| Instagram | X (+X) | X | X% | X |
| Facebook | X (+X) | X | X% | X |

---

## Content Performance

### Top Performing Content
| Content | Type | Views | Time on Page | Leads |
|---------|------|-------|--------------|-------|
| [Title 1] | Blog | X | Xm Xs | X |
| [Title 2] | Video | X | Xm Xs | X |
| [Title 3] | Guide | X | Xm Xs | X |

### Content by Funnel Stage
| Stage | Pieces | Views | Conversions |
|-------|--------|-------|-------------|
| TOFU | X | X | X |
| MOFU | X | X | X |
| BOFU | X | X | X |

---

## Campaign Analysis

### Campaign Performance Summary
| Campaign | Objective | Spend | Results | CPA | Status |
|----------|-----------|-------|---------|-----|--------|
| [Campaign 1] | [Goal] | $X | X | $X | 🟢 |
| [Campaign 2] | [Goal] | $X | X | $X | 🟡 |

### A/B Test Results
| Test | Variable | Winner | Lift | Significance |
|------|----------|--------|------|--------------|
| [Test 1] | [Variable] | A/B | +X% | 95% |

---

## Competitive Landscape

### Share of Voice
| Competitor | This Month | Last Month | Trend |
|------------|------------|------------|-------|
| Us | X% | X% | ↑ |
| [Comp 1] | X% | X% | → |
| [Comp 2] | X% | X% | ↓ |

### Notable Competitor Activity
- [Competitor 1]: [Activity and potential impact]
- [Competitor 2]: [Activity and potential impact]

---

## Budget Analysis

### Spend vs Budget
| Category | Budget | Actual | Variance | Notes |
|----------|--------|--------|----------|-------|
| Paid Media | $X | $X | +$X | [Note] |
| Content | $X | $X | -$X | [Note] |
| Tools | $X | $X | $0 | On budget |
| **Total** | $X | $X | +/-$X | |

### Efficiency Metrics
- CAC: $X (target: $X)
- LTV:CAC: X:1 (target: 3:1)
- Marketing % of Revenue: X%

---

## Key Wins

1. **[Win 1]**
   [Description with specific metrics and business impact]

2. **[Win 2]**
   [Description with specific metrics and business impact]

3. **[Win 3]**
   [Description with specific metrics and business impact]

---

## Challenges & Learnings

| Challenge | Root Cause | Solution | Impact |
|-----------|------------|----------|--------|
| [Challenge 1] | [Cause] | [Solution] | [Expected result] |
| [Challenge 2] | [Cause] | [Solution] | [Expected result] |

---

## Next Month Recommendations

### Strategic Priorities
1. **[Priority 1]**: [Rationale and expected impact]
2. **[Priority 2]**: [Rationale and expected impact]
3. **[Priority 3]**: [Rationale and expected impact]

### Campaign Roadmap
| Week | Campaign | Channel | Budget | Goal |
|------|----------|---------|--------|------|
| 1 | [Campaign] | [Channel] | $X | [Goal] |
| 2 | [Campaign] | [Channel] | $X | [Goal] |
| 3 | [Campaign] | [Channel] | $X | [Goal] |
| 4 | [Campaign] | [Channel] | $X | [Goal] |

### Budget Recommendations
[Specific reallocation suggestions based on performance data]

### Tests to Run
- [Test 1]: [Hypothesis]
- [Test 2]: [Hypothesis]

---

## Appendix

### Methodology
- Attribution Model: [First-touch/Last-touch/Multi-touch]
- Data Sources: [List]
- Reporting Period: [Dates]

### Glossary
- CAC: Customer Acquisition Cost
- LTV: Lifetime Value
- ROAS: Return on Ad Spend
- MQL: Marketing Qualified Lead (score 50+)
- SQL: Sales Qualified Lead
```
