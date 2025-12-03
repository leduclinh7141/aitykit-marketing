# Phase 2: Real-World Marketing Commands

## Overview
Based on research, marketers need daily operations support, not just campaign creation.

## 2.1 Daily Operations Commands

### `/daily` - Daily Marketing Checklist
```yaml
Tasks:
  Social Media:
    - Check mentions and DMs (all platforms)
    - Respond to comments within 1 hour
    - Monitor brand mentions
    - Engage with industry content

  Email:
    - Review bounce rates
    - Check spam complaints
    - Monitor key sequences

  Analytics:
    - Quick traffic check
    - Campaign performance snapshot
    - Anomaly detection

  Content:
    - Review scheduled posts
    - Check content calendar gaps
```

### `/weekly` - Weekly Marketing Review
```yaml
Tasks:
  Performance Review:
    - Traffic vs last week
    - Conversion rates
    - Top performing content
    - Underperforming campaigns

  Content Planning:
    - Schedule next week's content
    - Review content pipeline
    - Assign tasks to team

  SEO Check:
    - Ranking changes
    - New backlinks
    - Technical issues

  Team Sync:
    - Campaign updates
    - Blockers and solutions
    - Next week priorities
```

### `/monthly` - Monthly Performance Review
```yaml
Tasks:
  Analytics Deep Dive:
    - Traffic trends
    - Goal completions
    - Revenue attribution
    - Channel performance

  Content Audit:
    - Top performers
    - Content gaps
    - Update schedule

  Competitive Analysis:
    - Competitor content
    - Market positioning
    - Opportunity gaps

  Planning:
    - Next month's calendar
    - Campaign roadmap
    - Budget allocation
```

## 2.2 Sequence Commands

### `/welcome-sequence [product/service]`
Creates 5-7 email welcome sequence:
- Email 1: Welcome + value prop
- Email 2: Quick win/getting started
- Email 3: Feature highlight
- Email 4: Social proof/case study
- Email 5: Engagement ask
- Email 6: Offer/CTA
- Email 7: Feedback request

### `/nurture-sequence [segment] [goal]`
Creates lead nurturing sequence based on:
- Segment characteristics
- Buying stage
- Content preferences
- Conversion goal

### `/re-engage [segment]`
Creates win-back campaign:
- Identify inactive criteria
- Re-engagement email series
- Special offer strategy
- Final break-up email

## 2.3 Reporting Commands

### `/report:weekly [date-range]`
Generates weekly report with:
- Traffic summary
- Top content
- Conversion metrics
- Key wins
- Action items

### `/report:monthly [month]`
Generates comprehensive monthly report:
- Executive summary
- Channel performance
- Campaign results
- ROI analysis
- Recommendations

## 2.4 Audit Commands

### `/audit:full`
Complete marketing audit:
- Website audit
- SEO audit
- Content audit
- Social media audit
- Email audit
- Competitive audit

### `/competitor:deep [competitor-url]`
Deep competitor analysis:
- Traffic analysis
- Content strategy
- Keyword gaps
- Backlink profile
- Social presence
- Ad strategy

## Implementation Priority

1. `/daily` - Most used
2. `/weekly` - Weekly ritual
3. `/monthly` - Monthly reporting
4. `/welcome-sequence` - High impact automation
5. `/nurture-sequence` - Lead conversion
6. `/report:weekly` - Client deliverable
7. `/report:monthly` - Client deliverable
8. `/audit:full` - Strategic planning
9. `/re-engage` - Revenue recovery
10. `/competitor:deep` - Competitive intel
