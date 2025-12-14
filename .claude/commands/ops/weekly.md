---
description: Weekly marketing review and planning
argument-hint: [week-ending-date]
---

## Language & Quality Standards

**CRITICAL**: Respond in the same language the user is using. If Vietnamese, respond in Vietnamese. If Spanish, respond in Spanish.

**Standards**: Token efficiency, sacrifice grammar for concision, list unresolved questions at end.

**Skills**: Activate `marketing-fundamentals`, `analytics-attribution`, `sales-workflow.md`, `crm-workflow.md` skills.

---

## Mission
Generate weekly marketing review and next week planning:
<week>$ARGUMENTS</week>

## Workflow

1. Use `researcher` agent to compile metrics:
   - Traffic, leads, conversions
   - Email performance
   - Social engagement
   - Ad performance

2. Use `project-manager` agent to:
   - Review completed vs planned
   - Identify blockers
   - Plan next week

3. Use `planner` agent for:
   - Content calendar update
   - Campaign adjustments
   - Resource allocation

4. Use `lead-qualifier` agent for:
   - Funnel conversion analysis (per CRM workflow benchmarks)
   - Lead quality trends
   - SLA compliance review

## Agent Delegation
| Task | Agent | Trigger |
|------|-------|---------|
| Metrics compilation | `researcher` | Weekly review |
| Progress tracking | `project-manager` | Status update |
| Content planning | `planner` | Next week prep |
| Funnel analysis | `lead-qualifier` | Conversion review |
| Copy review | `copywriter` | Content assessment |

## Weekly Review Framework

### Performance Metrics

**Traffic & Acquisition**
- Total sessions: [X] (vs last week: +/-%)
- New vs returning: [X%] / [X%]
- Top traffic sources
- Bounce rate changes

**Lead Generation**
- New leads: [X]
- MQLs: [X]
- SQLs: [X]
- Conversion rates by source

**Email Marketing**
- Campaigns sent: [X]
- Avg open rate: [X%]
- Avg click rate: [X%]
- Unsubscribes: [X]
- List growth: [X]

**Social Media**
- Total reach: [X]
- Engagement rate: [X%]
- Followers gained: [X]
- Top performing posts

**Paid Advertising**
- Spend: $[X]
- Impressions: [X]
- Clicks: [X]
- CPC: $[X]
- Conversions: [X]
- ROAS: [X]

### Content Performance

| Content | Views | Engagement | Conversions |
|---------|-------|------------|-------------|
| [Post 1] | X | X% | X |
| [Post 2] | X | X% | X |

### Campaign Status

| Campaign | Status | Progress | Issues |
|----------|--------|----------|--------|
| [Campaign 1] | On Track/At Risk | X% | [Notes] |

### Wins & Learnings

**What Worked**
- [Win 1]
- [Win 2]

**What Didn't Work**
- [Issue 1] - Learning: [Insight]

**Test Results**
- [A/B test]: Winner was [X] with [X%] improvement

## Next Week Planning

### Priority Tasks
1. [Task 1] - Owner: [X] - Due: [Date]
2. [Task 2] - Owner: [X] - Due: [Date]

### Content Calendar
| Day | Platform | Content | Owner |
|-----|----------|---------|-------|
| Mon | | | |
| Tue | | | |
| Wed | | | |
| Thu | | | |
| Fri | | | |

### Campaigns to Launch/Continue
- [Campaign details]

### Goals for Next Week
- [ ] [Goal 1 with metric]
- [ ] [Goal 2 with metric]

## Output Format
```markdown
# Weekly Marketing Review: Week of [Date]

## Executive Summary
[2-3 sentences on overall performance]

## Key Metrics vs Targets
| Metric | Actual | Target | Status |
|--------|--------|--------|--------|
| Traffic | X | X | 🟢/🟡/🔴 |
| Leads | X | X | 🟢/🟡/🔴 |
| MQLs | X | X | 🟢/🟡/🔴 |
| Email Open Rate | X% | 25% | 🟢/🟡/🔴 |
| Social Engagement | X% | X% | 🟢/🟡/🔴 |

## Top 3 Wins
1. [Win with data]
2. [Win with data]
3. [Win with data]

## Top 3 Challenges
1. [Challenge] - Action: [Solution]
2. [Challenge] - Action: [Solution]
3. [Challenge] - Action: [Solution]

## Content Performance
| Top Content | Metric | Why It Worked |
|-------------|--------|---------------|
| [Content 1] | [X] | [Reason] |
| [Content 2] | [X] | [Reason] |

## Next Week Priorities
1. [Priority 1]
2. [Priority 2]
3. [Priority 3]

## Resource Needs
- [Resource 1]
- [Resource 2]
```
