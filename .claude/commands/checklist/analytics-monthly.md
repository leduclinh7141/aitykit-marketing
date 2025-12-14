---
description: Monthly analytics review and insights template
argument-hint: [month-year] [client-or-brand]
---

## Language & Quality Standards

**CRITICAL**: Respond in the same language the user is using. If Vietnamese, respond in Vietnamese. If Spanish, respond in Spanish.

**Standards**: Token efficiency, sacrifice grammar for concision, list unresolved questions at end.

**Skills**: Activate `analytics-attribution`, `marketing-fundamentals`, `crm-workflow.md`, `sales-workflow.md` skills.

---

## Mission
Generate monthly analytics review:
<context>$ARGUMENTS</context>

## Agent Delegation
| Task | Agent | Trigger |
|------|-------|---------|
| Data compilation | `researcher` | Monthly review |
| Funnel analysis | `lead-qualifier` | Conversion review |
| Insights narrative | `copywriter` | Report writing |
| Recommendations | `planner` | Strategy planning |

## Output Format
```markdown
# Monthly Analytics Review: [Month Year]

## Review Checklist

### Data Collection (Day 1-2)

**Traffic & Acquisition**
- [ ] Export Google Analytics data
- [ ] Pull Search Console metrics
- [ ] Compile paid ads data (all platforms)
- [ ] Gather social media analytics
- [ ] Export email campaign metrics
- [ ] Pull CRM/lead data

**Revenue & Conversion**
- [ ] Export sales/revenue data
- [ ] Pull conversion data by channel
- [ ] Calculate attribution by source
- [ ] Compile customer acquisition data

---

## Analysis Framework

### 1. Traffic Analysis

| Source | Sessions | % Total | MoM | YoY |
|--------|----------|---------|-----|-----|
| Organic Search | | | | |
| Direct | | | | |
| Paid Search | | | | |
| Social | | | | |
| Email | | | | |
| Referral | | | | |
| **Total** | | | | |

**Key Questions:**
- [ ] Which channels grew/declined most?
- [ ] What drove the changes?
- [ ] Are we hitting traffic targets?
- [ ] Where should we invest more/less?

### 2. Engagement Analysis

| Metric | This Month | Last Month | Benchmark |
|--------|------------|------------|-----------|
| Bounce Rate | | | <50% |
| Pages/Session | | | >2.5 |
| Avg Session Duration | | | >2:00 |
| New vs Returning | | | 60/40 |

**Key Questions:**
- [ ] Is content engaging visitors?
- [ ] Are users finding what they need?
- [ ] Which pages have high bounce rates?
- [ ] What content keeps users engaged?

### 3. Conversion Analysis

| Stage | Volume | Rate | MoM | Benchmark |
|-------|--------|------|-----|-----------|
| Visitors | | - | | |
| Leads | | % | | 3% |
| MQLs | | % | | 20% |
| SQLs | | % | | 30% |
| Customers | | % | | 25% |

**Conversion by Channel:**
| Channel | Leads | Conv Rate | CAC | Quality |
|---------|-------|-----------|-----|---------|
| Organic | | | | |
| Paid | | | | |
| Social | | | | |
| Email | | | | |
| Referral | | | | |

**Key Questions:**
- [ ] Which channels convert best?
- [ ] Where are funnel drop-offs?
- [ ] Is lead quality improving?
- [ ] Are we hitting conversion targets?

### 4. Content Performance

**Top 10 Pages by Traffic:**
| Page | Sessions | Conv | Bounce | Avg Time |
|------|----------|------|--------|----------|
| 1. | | | | |
| 2. | | | | |
| 3. | | | | |

**Content by Type:**
| Type | Pieces | Views | Leads | Best Performer |
|------|--------|-------|-------|----------------|
| Blog | | | | |
| Landing | | | | |
| Video | | | | |
| Download | | | | |

**Key Questions:**
- [ ] What content drives conversions?
- [ ] What topics resonate most?
- [ ] Where are content gaps?
- [ ] What should we create more of?

### 5. Campaign Performance

| Campaign | Spend | Impressions | Clicks | Conv | CPA | ROAS |
|----------|-------|-------------|--------|------|-----|------|
| | | | | | | |

**Key Questions:**
- [ ] Which campaigns hit targets?
- [ ] Where should we reallocate budget?
- [ ] What creative/messaging worked?
- [ ] What tests should we run?

### 6. Email Performance

| Metric | This Month | Last Month | Benchmark |
|--------|------------|------------|-----------|
| List Size | | | Growth >3% |
| Open Rate | | | >25% |
| Click Rate | | | >3% |
| Unsubscribe | | | <0.5% |
| Revenue | | | |

**Key Questions:**
- [ ] Is list growing healthily?
- [ ] Are engagement rates improving?
- [ ] Which emails performed best?
- [ ] What subject lines worked?

### 7. Social Media Performance

| Platform | Followers | Engagement | Reach | Traffic |
|----------|-----------|------------|-------|---------|
| LinkedIn | | | | |
| Twitter | | | | |
| Instagram | | | | |
| Facebook | | | | |

**Key Questions:**
- [ ] Which platform drives most value?
- [ ] What content gets engagement?
- [ ] Is social driving conversions?
- [ ] Where should we focus?

---

## Insights & Actions

### Top 3 Wins
1. **[Win]:** [Data + Impact]
2. **[Win]:** [Data + Impact]
3. **[Win]:** [Data + Impact]

### Top 3 Challenges
1. **[Challenge]:** [Data] → Action: [Fix]
2. **[Challenge]:** [Data] → Action: [Fix]
3. **[Challenge]:** [Data] → Action: [Fix]

### Key Learnings
- [Learning 1]
- [Learning 2]
- [Learning 3]

### Next Month Priorities
1. [Priority + Target metric]
2. [Priority + Target metric]
3. [Priority + Target metric]

---

## Scorecard

| KPI | Target | Actual | Status | Trend |
|-----|--------|--------|--------|-------|
| Traffic | | | 🟢/🟡/🔴 | ↑/↓/→ |
| Leads | | | 🟢/🟡/🔴 | ↑/↓/→ |
| MQLs | | | 🟢/🟡/🔴 | ↑/↓/→ |
| Revenue | | | 🟢/🟡/🔴 | ↑/↓/→ |
| CAC | | | 🟢/🟡/🔴 | ↑/↓/→ |
| ROAS | | | 🟢/🟡/🔴 | ↑/↓/→ |
```
