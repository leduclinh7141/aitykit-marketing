---
description: Generate client-ready weekly marketing report
argument-hint: [client-or-project] [week-dates]
---

## Language & Quality Standards

**CRITICAL**: Respond in the same language the user is using. If Vietnamese, respond in Vietnamese. If Spanish, respond in Spanish.

**Standards**: Token efficiency, sacrifice grammar for concision, list unresolved questions at end.

**Skills**: Activate `marketing-fundamentals`, `analytics-attribution`, `crm-workflow.md` skills.

---

## Mission
Generate professional client-ready weekly report:
<context>$ARGUMENTS</context>

## Workflow

1. Use `researcher` agent to compile metrics:
   - Traffic and acquisition data
   - Campaign performance
   - Lead generation stats
   - Engagement metrics

2. Use `lead-qualifier` agent to analyze:
   - Funnel performance vs CRM benchmarks
   - Lead quality and SLA compliance
   - Conversion trends

3. Use `copywriter` agent to:
   - Write executive summary
   - Highlight wins and insights
   - Frame challenges constructively

4. Format for client presentation

## Agent Delegation
| Task | Agent | Trigger |
|------|-------|---------|
| Data compilation | `researcher` | Report generation |
| Funnel analysis | `lead-qualifier` | Lead metrics |
| Executive summary | `copywriter` | Report narrative |
| Recommendations | `planner` | Next steps |

## Report Structure

### Executive Summary
[2-3 sentences: What happened, what it means, what's next]

### Key Performance Indicators
Dashboard-style metrics with targets and status indicators.

### Campaign Highlights
Top performing content and campaigns with insights.

### Recommendations
Actionable next steps based on data.

## Output Format
```markdown
# Weekly Marketing Report
**Client:** [Client Name]
**Period:** [Start Date] - [End Date]
**Prepared by:** [Agency/Name]

---

## Executive Summary

This week we [achieved/saw] [key result]. [Main insight]. Next week we'll focus on [priority].

---

## Key Metrics Dashboard

| Metric | This Week | Last Week | Change | Target | Status |
|--------|-----------|-----------|--------|--------|--------|
| Website Sessions | X | X | +X% | X | 🟢 |
| New Leads | X | X | +X% | X | 🟢 |
| Email Open Rate | X% | X% | +X% | 25% | 🟡 |
| Social Engagement | X | X | +X% | X | 🟢 |
| Ad Spend | $X | $X | +X% | $X | 🟢 |
| Conversions | X | X | +X% | X | 🟢 |

---

## Traffic Analysis

### Sessions by Source
| Source | Sessions | % of Total | Trend |
|--------|----------|------------|-------|
| Organic Search | X | X% | ↑ |
| Direct | X | X% | → |
| Social | X | X% | ↑ |
| Paid | X | X% | ↓ |
| Email | X | X% | ↑ |
| Referral | X | X% | → |

### Top Landing Pages
1. [Page URL] - X sessions - X% conversion
2. [Page URL] - X sessions - X% conversion
3. [Page URL] - X sessions - X% conversion

---

## Campaign Performance

### Active Campaigns
| Campaign | Impressions | Clicks | CTR | Conversions | CPA |
|----------|-------------|--------|-----|-------------|-----|
| [Campaign 1] | X | X | X% | X | $X |
| [Campaign 2] | X | X | X% | X | $X |

### Email Campaigns
| Campaign | Sent | Opens | Clicks | Conversions |
|----------|------|-------|--------|-------------|
| [Email 1] | X | X% | X% | X |
| [Email 2] | X | X% | X% | X |

---

## Content Performance

### Top Performing Content
| Content | Views | Engagement | Leads |
|---------|-------|------------|-------|
| [Content 1] | X | X% | X |
| [Content 2] | X | X% | X |

### Social Media Highlights
- **Best Post:** [Description] - X engagement
- **Reach:** X (↑X% from last week)
- **New Followers:** X

---

## Lead Generation

### Funnel Overview
- **New Leads:** X
- **Marketing Qualified:** X
- **Sales Qualified:** X
- **Opportunities:** X

### Lead Sources
| Source | Leads | % of Total | Quality Score |
|--------|-------|------------|---------------|
| [Source 1] | X | X% | High/Med/Low |
| [Source 2] | X | X% | High/Med/Low |

---

## Wins & Insights

### This Week's Wins
1. **[Win 1]**: [Brief description with data]
2. **[Win 2]**: [Brief description with data]

### Key Insights
- [Insight 1 - actionable observation]
- [Insight 2 - actionable observation]

---

## Challenges & Actions

| Challenge | Impact | Action Taken/Planned |
|-----------|--------|---------------------|
| [Challenge 1] | [Impact] | [Action] |
| [Challenge 2] | [Impact] | [Action] |

---

## Next Week Focus

### Priorities
1. [Priority 1]
2. [Priority 2]
3. [Priority 3]

### Upcoming Content
| Date | Content | Channel | Goal |
|------|---------|---------|------|
| [Date] | [Content] | [Channel] | [Goal] |

### Campaigns Launching
- [Campaign details]

---

## Appendix

### Definitions
- **MQL**: Marketing Qualified Lead (score 50+)
- **SQL**: Sales Qualified Lead (BANT/MEDDIC verified)

### Data Sources
- Google Analytics
- [CRM Name]
- [Email Platform]
- [Social Platforms]
```
