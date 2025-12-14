---
description: Pre-launch campaign checklist to ensure nothing is missed
argument-hint: [campaign-name] [launch-date]
---

## Language & Quality Standards

**CRITICAL**: Respond in the same language the user is using. If Vietnamese, respond in Vietnamese. If Spanish, respond in Spanish.

**Standards**: Token efficiency, sacrifice grammar for concision, list unresolved questions at end.

**Skills**: Activate `marketing-fundamentals`, `analytics-attribution`, `sales-workflow.md` skills.

---

## Mission
Generate campaign launch checklist:
<context>$ARGUMENTS</context>

## Agent Delegation
| Task | Agent | Trigger |
|------|-------|---------|
| Copy review | `copywriter` | Content QA |
| Landing page | `attraction-specialist` | Page optimization |
| Lead routing | `lead-qualifier` | CRM setup |
| Sales alignment | `sales-enabler` | Handoff prep |

## Output Format
```markdown
# Campaign Launch Checklist: [Campaign Name]
**Launch Date:** [Date]
**Owner:** [Name]

---

## T-14 Days: Strategy & Planning

### Campaign Foundation
- [ ] Campaign objective clearly defined (SMART goal)
- [ ] Target audience documented
- [ ] Key messages finalized
- [ ] Unique value proposition clear
- [ ] Budget approved and allocated
- [ ] Timeline and milestones set
- [ ] Success metrics defined (KPIs)
- [ ] Stakeholders aligned and briefed

### Competitive Check
- [ ] Competitor campaigns reviewed
- [ ] Differentiation points confirmed
- [ ] Timing conflicts checked
- [ ] Market positioning validated

---

## T-7 Days: Content & Creative

### Landing Page
- [ ] Page live and loading fast (<3s)
- [ ] Mobile responsive (test on devices)
- [ ] Form working correctly
- [ ] Thank you page/confirmation set up
- [ ] CTA buttons visible and compelling
- [ ] Trust signals present (testimonials, logos)
- [ ] Legal/privacy policy linked
- [ ] UTM parameters ready

### Copy & Messaging
- [ ] Headlines tested for clarity
- [ ] Body copy proofread (no typos)
- [ ] CTA text action-oriented
- [ ] Brand voice consistent
- [ ] Legal disclaimers included (if needed)
- [ ] Accessibility checked (alt text, contrast)

### Visual Assets
- [ ] Images optimized for web
- [ ] Videos uploaded and tested
- [ ] Ad creatives in all required sizes
- [ ] Brand guidelines followed
- [ ] File naming conventions correct

---

## T-3 Days: Technical Setup

### Tracking & Analytics
- [ ] Google Analytics goals configured
- [ ] Conversion tracking pixels installed
- [ ] UTM parameters tested
- [ ] Attribution model confirmed
- [ ] Dashboard/reporting ready
- [ ] Baseline metrics documented

### CRM & Lead Flow
- [ ] Form submissions routing to CRM
- [ ] Lead scoring rules updated
- [ ] Auto-assignment rules set (hot leads <5 min SLA)
- [ ] Notification triggers active
- [ ] Lead source tracking working
- [ ] Duplicate handling configured

### Email Automation
- [ ] Welcome/confirmation email ready
- [ ] Nurture sequence activated
- [ ] Email templates tested (all devices)
- [ ] Sender reputation verified
- [ ] Unsubscribe working
- [ ] SPF/DKIM configured

### Paid Ads (if applicable)
- [ ] Ad accounts funded
- [ ] Campaigns built and reviewed
- [ ] Targeting parameters set
- [ ] Bid strategy configured
- [ ] Ad schedule set
- [ ] Negative keywords added
- [ ] Audience lists uploaded

---

## T-1 Day: Final QA

### Technical Testing
- [ ] Complete user journey tested
- [ ] Form submission tested (receive in CRM?)
- [ ] Email delivery tested (check spam)
- [ ] All links verified working
- [ ] Page speed acceptable
- [ ] Cross-browser testing complete
- [ ] Mobile experience verified

### Stakeholder Alignment
- [ ] Sales team briefed on campaign
- [ ] Lead handoff process confirmed
- [ ] Talking points shared
- [ ] FAQ document ready
- [ ] Escalation path defined
- [ ] Support team notified

### Backup Plans
- [ ] Know how to pause if issues arise
- [ ] Emergency contacts documented
- [ ] Rollback plan ready (if needed)

---

## Launch Day (T-0)

### Pre-Launch (Morning)
- [ ] Final systems check
- [ ] Team on standby
- [ ] Monitoring dashboards open
- [ ] Communication channels ready

### Go Live
- [ ] Activate campaigns
- [ ] Publish content
- [ ] Send announcement emails
- [ ] Post on social media
- [ ] Enable paid ads

### Post-Launch Monitoring (First 2 hours)
- [ ] Confirm ads serving
- [ ] Check form submissions flowing
- [ ] Monitor for errors/issues
- [ ] Watch initial metrics
- [ ] Respond to early engagement

---

## T+1 Day: Early Performance

### Quick Health Check
- [ ] Review overnight performance
- [ ] Check lead quality
- [ ] Verify sales received leads
- [ ] Address any issues
- [ ] Optimize based on data

### Metrics to Check
| Metric | Expected | Actual | Status |
|--------|----------|--------|--------|
| Impressions | | | |
| Clicks | | | |
| CTR | | | |
| Conversions | | | |
| CPA | | | |
| Lead Quality | | | |

---

## T+7 Days: Week 1 Review

### Performance Assessment
- [ ] Compare to targets
- [ ] Identify top performers
- [ ] Note underperformers
- [ ] Gather learnings
- [ ] Plan optimizations

### Optimization Actions
- [ ] Pause underperforming ads
- [ ] Scale winning creatives
- [ ] Refine targeting
- [ ] Adjust bids/budgets
- [ ] Update messaging if needed

---

## Sign-Off Checklist

| Area | Owner | Approved | Date |
|------|-------|----------|------|
| Strategy | | ☐ | |
| Creative | | ☐ | |
| Copy | | ☐ | |
| Technical | | ☐ | |
| Legal | | ☐ | |
| Sales | | ☐ | |
| **Final Go** | | ☐ | |

---

## Emergency Contacts

| Role | Name | Contact |
|------|------|---------|
| Campaign Owner | | |
| Tech Lead | | |
| Sales Lead | | |
| Executive Sponsor | | |
```
