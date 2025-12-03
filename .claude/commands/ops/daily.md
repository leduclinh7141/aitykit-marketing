---
description: Daily marketing tasks checklist and review
argument-hint: [focus-area]
---

Activate `marketing-fundamentals`, `social-media`, `sales-workflow.md`, `crm-workflow.md` skills.

## Mission
Generate daily marketing checklist and review:
<focus>$ARGUMENTS</focus>

## Workflow

1. Use `project-manager` agent to compile daily tasks:
   - Urgent items from previous day
   - Scheduled content for today
   - Engagement responses needed
   - Lead follow-ups due

2. Use `lead-qualifier` agent to check (per unified thresholds):
   - 🔥 Hot leads (70-100): Immediate response (<5 min SLA)
   - 🌡️ Warm leads (50-69): Priority follow-up (<1 hr SLA)
   - ❄️ Cool leads (30-49): Accelerated nurture (<24 hr SLA)
   - MQL notifications from overnight
   - Lead score changes

3. Review and prioritize by impact and SLA

## Agent Delegation
| Task | Agent | Trigger |
|------|-------|---------|
| Daily task compilation | `project-manager` | Morning routine |
| Lead scoring review | `lead-qualifier` | New leads/score changes |
| Content scheduling | `copywriter` | Content calendar |
| Social engagement | `brainstormer` | Engagement strategy |

## Daily Marketing Checklist

### Morning Routine (First 30 min)

**Inbox & Alerts (10 min)**
- [ ] Check hot lead alerts (respond <5 min)
- [ ] Review email campaign performance
- [ ] Check for urgent client requests
- [ ] Review overnight mentions/DMs

**Content & Social (15 min)**
- [ ] Publish scheduled social posts
- [ ] Respond to comments/mentions
- [ ] Engage with 5-10 relevant posts
- [ ] Share/retweet industry content

**Analytics Quick Check (5 min)**
- [ ] Website traffic anomalies
- [ ] Email deliverability issues
- [ ] Ad spend pacing

### Midday Check (15 min)

**Engagement**
- [ ] Respond to new comments
- [ ] Follow up on morning posts
- [ ] Check email replies

**Lead Management**
- [ ] Process new leads
- [ ] Update CRM notes
- [ ] Send promised follow-ups

### End of Day (15 min)

**Wrap-up**
- [ ] Log completed tasks
- [ ] Note blockers for tomorrow
- [ ] Schedule tomorrow's content
- [ ] Update campaign status

**Reporting**
- [ ] Daily metrics snapshot
- [ ] Flag any issues for team

## Output Format
```markdown
# Daily Marketing Review: [Date]

## Priority Tasks (Do First)
| Task | Priority | Owner | Due |
|------|----------|-------|-----|
| [Task 1] | 🔴 High | [Name] | [Time] |
| [Task 2] | 🟡 Medium | [Name] | [Time] |

## Leads Requiring Response (by SLA)

### 🔥 Hot Leads (70-100) - Respond <5 min
| Lead | Score | Action Needed | Time Remaining |
|------|-------|---------------|----------------|
| [Name] | [X] | [Action] | [X min] |

### 🌡️ Warm Leads (50-69) - Respond <1 hr
| Lead | Score | Action Needed | Time Remaining |
|------|-------|---------------|----------------|
| [Name] | [X] | [Action] | [X min] |

## Today's Content Schedule
| Time | Platform | Content | Status |
|------|----------|---------|--------|
| [Time] | [Platform] | [Description] | Ready/Draft |

## Yesterday's Performance
- Email open rate: X% (target: 25%)
- Social engagement: X (vs avg)
- New leads: X
- Website traffic: X

## Blockers & Escalations
- [Issue 1]
- [Issue 2]

## Tomorrow Preview
- [Key task 1]
- [Key task 2]
```
