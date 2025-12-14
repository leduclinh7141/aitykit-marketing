---
description: Comprehensive marketing audit across all channels
argument-hint: [brand-or-website]
---

## Language & Quality Standards

**CRITICAL**: Respond in the same language the user is using. If Vietnamese, respond in Vietnamese. If Spanish, respond in Spanish.

**Standards**: Token efficiency, sacrifice grammar for concision, list unresolved questions at end.

**Skills**: Activate `marketing-fundamentals`, `seo-mastery`, `analytics-attribution` skills.

---

## Mission
Conduct full marketing audit:
<target>$ARGUMENTS</target>

## Workflow

1. Use `researcher` agent to audit:
   - Website & SEO
   - Content marketing
   - Social presence
   - Competitive positioning

2. Use `attraction-specialist` agent for:
   - SEO technical audit
   - Content gap analysis
   - Lead gen assessment

3. Use `lead-qualifier` agent for:
   - Funnel analysis
   - Conversion optimization
   - Lead scoring review

4. Use `email-wizard` agent for:
   - Email program audit
   - Deliverability check
   - Automation review

## Agent Delegation
| Task | Agent | Trigger |
|------|-------|---------|
| Website/SEO audit | `attraction-specialist` | Technical review |
| Content analysis | `researcher` | Content inventory |
| Funnel analysis | `lead-qualifier` | Conversion review |
| Email audit | `email-wizard` | Email program |
| Social audit | `researcher` | Social presence |
| Competitive context | `researcher` | Market position |

## Output Format
```markdown
# Marketing Audit: [Brand/Website]
**Date:** [Date]
**Auditor:** [Name/Tool]

---

## Executive Summary

### Overall Health Score: [X]/100

| Area | Score | Priority |
|------|-------|----------|
| Website & UX | X/100 | 🔴/🟡/🟢 |
| SEO | X/100 | 🔴/🟡/🟢 |
| Content | X/100 | 🔴/🟡/🟢 |
| Social Media | X/100 | 🔴/🟡/🟢 |
| Email Marketing | X/100 | 🔴/🟡/🟢 |
| Lead Generation | X/100 | 🔴/🟡/🟢 |
| Analytics | X/100 | 🔴/🟡/🟢 |

### Top 3 Urgent Issues
1. [Issue 1] - Impact: [High/Med]
2. [Issue 2] - Impact: [High/Med]
3. [Issue 3] - Impact: [High/Med]

### Top 3 Quick Wins
1. [Win 1] - Effort: [Low] - Impact: [High]
2. [Win 2] - Effort: [Low] - Impact: [High]
3. [Win 3] - Effort: [Low] - Impact: [Med]

---

## Website & UX Audit

### Technical Health
| Check | Status | Issue |
|-------|--------|-------|
| Mobile responsive | ✅/❌ | [Details] |
| Page speed (mobile) | X sec | Target: <3s |
| Page speed (desktop) | X sec | Target: <2s |
| SSL certificate | ✅/❌ | |
| Core Web Vitals | Pass/Fail | [Details] |
| 404 errors | X found | [List] |
| Broken links | X found | [List] |

### UX Assessment
| Element | Rating | Notes |
|---------|--------|-------|
| Navigation | 1-5 | [Notes] |
| CTA clarity | 1-5 | [Notes] |
| Value proposition | 1-5 | [Notes] |
| Trust signals | 1-5 | [Notes] |
| Mobile experience | 1-5 | [Notes] |

### Recommendations
- [ ] [Recommendation 1]
- [ ] [Recommendation 2]

---

## SEO Audit

### Technical SEO
| Factor | Status | Action |
|--------|--------|--------|
| Sitemap | ✅/❌ | [Action] |
| Robots.txt | ✅/❌ | [Action] |
| Schema markup | ✅/❌ | [Action] |
| Canonical tags | ✅/❌ | [Action] |
| Meta titles | X% optimized | [Action] |
| Meta descriptions | X% optimized | [Action] |
| H1 tags | X% present | [Action] |
| Image alt text | X% present | [Action] |

### Keyword Performance
| Keyword | Position | Volume | Opportunity |
|---------|----------|--------|-------------|
| [Keyword 1] | X | X/mo | [Notes] |
| [Keyword 2] | X | X/mo | [Notes] |

### Backlink Profile
- Domain Authority: X
- Total backlinks: X
- Referring domains: X
- Toxic links: X (disavow needed?)

### Recommendations
- [ ] [SEO recommendation 1]
- [ ] [SEO recommendation 2]

---

## Content Audit

### Content Inventory
| Type | Count | Avg Performance | Gap |
|------|-------|-----------------|-----|
| Blog posts | X | X views | [Gap] |
| Landing pages | X | X% conv | [Gap] |
| Case studies | X | X downloads | [Gap] |
| Videos | X | X views | [Gap] |
| Lead magnets | X | X downloads | [Gap] |

### Content Quality
| Metric | Score | Benchmark |
|--------|-------|-----------|
| Avg word count | X | 1500+ |
| Readability | Grade X | Grade 8 |
| Freshness (avg age) | X months | <12 mo |
| Internal linking | X avg | 3-5 |

### Content Gaps
- [Topic gap 1]
- [Topic gap 2]
- [Funnel stage gap]

### Recommendations
- [ ] [Content recommendation 1]
- [ ] [Content recommendation 2]

---

## Social Media Audit

### Presence Overview
| Platform | Followers | Engagement | Posting Freq |
|----------|-----------|------------|--------------|
| LinkedIn | X | X% | X/week |
| Twitter/X | X | X% | X/week |
| Instagram | X | X% | X/week |
| Facebook | X | X% | X/week |

### Profile Optimization
| Platform | Bio | Link | CTA | Branding |
|----------|-----|------|-----|----------|
| LinkedIn | ✅/❌ | ✅/❌ | ✅/❌ | ✅/❌ |
| Twitter/X | ✅/❌ | ✅/❌ | ✅/❌ | ✅/❌ |

### Content Performance
- Best performing content type: [Type]
- Best posting time: [Day/Time]
- Engagement vs competitors: [Above/Below avg]

### Recommendations
- [ ] [Social recommendation 1]
- [ ] [Social recommendation 2]

---

## Email Marketing Audit

### List Health
| Metric | Value | Benchmark |
|--------|-------|-----------|
| List size | X | - |
| Growth rate | X%/mo | 3-5% |
| Bounce rate | X% | <2% |
| Unsubscribe rate | X% | <0.5% |
| Inactive % | X% | <30% |

### Performance
| Metric | Actual | Benchmark |
|--------|--------|-----------|
| Open rate | X% | 25% |
| Click rate | X% | 3% |
| Conversion rate | X% | 1% |

### Automation
| Sequence | Exists | Performance |
|----------|--------|-------------|
| Welcome | ✅/❌ | [Metrics] |
| Nurture | ✅/❌ | [Metrics] |
| Re-engagement | ✅/❌ | [Metrics] |
| Onboarding | ✅/❌ | [Metrics] |

### Recommendations
- [ ] [Email recommendation 1]
- [ ] [Email recommendation 2]

---

## Lead Generation Audit

### Funnel Analysis
| Stage | Volume | Conv Rate | Benchmark |
|-------|--------|-----------|-----------|
| Visitors | X | - | - |
| Leads | X | X% | 3% |
| MQLs | X | X% | 20% |
| SQLs | X | X% | 30% |
| Customers | X | X% | 25% |

### Lead Capture
| Element | Present | Quality |
|---------|---------|---------|
| Lead magnets | ✅/❌ | [Score] |
| Forms | ✅/❌ | [Score] |
| CTAs | ✅/❌ | [Score] |
| Pop-ups | ✅/❌ | [Score] |
| Chat | ✅/❌ | [Score] |

### Recommendations
- [ ] [Lead gen recommendation 1]
- [ ] [Lead gen recommendation 2]

---

## Analytics Audit

### Tracking Setup
| Tool | Installed | Configured |
|------|-----------|------------|
| Google Analytics | ✅/❌ | ✅/❌ |
| Tag Manager | ✅/❌ | ✅/❌ |
| Conversion tracking | ✅/❌ | ✅/❌ |
| UTM usage | ✅/❌ | ✅/❌ |
| CRM integration | ✅/❌ | ✅/❌ |

### Data Quality
- [ ] Goals configured
- [ ] Events tracking
- [ ] E-commerce tracking
- [ ] Cross-domain tracking

---

## Priority Action Plan

### Immediate (Week 1)
1. [Critical fix 1]
2. [Critical fix 2]

### Short-term (Month 1)
1. [Priority 1]
2. [Priority 2]
3. [Priority 3]

### Medium-term (Quarter 1)
1. [Strategic initiative 1]
2. [Strategic initiative 2]

### Resource Needs
- [Resource 1]
- [Resource 2]
```
