# Part 4: Command Specifications

## 4.1 Command Structure

```
.claude/commands/
├── campaign/
│   ├── plan.md        # /campaign:plan
│   ├── brief.md       # /campaign:brief
│   ├── calendar.md    # /campaign:calendar
│   └── analyze.md     # /campaign:analyze
├── seo/
│   ├── audit.md       # /seo:audit
│   ├── keywords.md    # /seo:keywords
│   ├── competitor.md  # /seo:competitor
│   └── optimize.md    # /seo:optimize
├── leads/
│   ├── qualify.md     # /leads:qualify
│   ├── score.md       # /leads:score
│   └── nurture.md     # /leads:nurture
├── analytics/
│   ├── report.md      # /analytics:report
│   ├── funnel.md      # /analytics:funnel
│   └── roi.md         # /analytics:roi
├── brand/
│   ├── voice.md       # /brand:voice
│   ├── book.md        # /brand:book
│   └── assets.md      # /brand:assets
├── social/
│   ├── schedule.md    # /social:schedule
│   ├── engage.md      # /social:engage
│   └── viral.md       # /social:viral
├── research/
│   ├── market.md      # /research:market
│   ├── persona.md     # /research:persona
│   └── trend.md       # /research:trend
└── content/           # (existing, enhanced)
    ├── blog.md        # /content:blog (NEW)
    ├── social.md      # /content:social (NEW)
    ├── email.md       # /content:email (NEW)
    ├── landing.md     # /content:landing (NEW)
    ├── ads.md         # /content:ads (NEW)
    ├── cro.md         # /content:cro (KEEP)
    ├── enhance.md     # /content:enhance (KEEP)
    ├── fast.md        # /content:fast (KEEP)
    └── good.md        # /content:good (KEEP)
```

---

## 4.2 Campaign Commands

### /campaign:plan
```yaml
---
description: Create comprehensive marketing campaign plan
argument-hint: [campaign-objective]
---
```

**Workflow:**
1. Analyze objective and target audience
2. Research competitor campaigns
3. Define funnel stages and touchpoints
4. Create content requirements
5. Set KPIs and success metrics
6. Generate timeline and budget allocation

**Agents:** `planner`, `researcher`

---

### /campaign:brief
```yaml
---
description: Generate creative brief for campaign execution
argument-hint: [campaign-name]
---
```

**Workflow:**
1. Extract campaign objectives
2. Define target audience personas
3. Outline key messages and USPs
4. Specify deliverables and formats
5. Set brand guidelines compliance
6. Define success criteria

**Agents:** `copywriter`, `planner`

---

### /campaign:calendar
```yaml
---
description: Generate content calendar for campaign
argument-hint: [timeframe]
---
```

**Workflow:**
1. Map campaign phases to dates
2. Assign content types per channel
3. Set publishing frequencies
4. Align with key dates/events
5. Define review/approval milestones
6. Export to calendar format

**Agents:** `project-manager`

---

### /campaign:analyze
```yaml
---
description: Analyze campaign performance and provide insights
argument-hint: [campaign-name-or-url]
---
```

**Workflow:**
1. Gather performance data
2. Compare against benchmarks
3. Identify top/bottom performers
4. Calculate ROI metrics
5. Generate optimization recommendations
6. Create performance report

**Agents:** `researcher`, `upsell-maximizer`

---

## 4.3 SEO Commands

### /seo:audit
```yaml
---
description: Perform comprehensive SEO audit
argument-hint: [url-or-sitemap]
---
```

**Workflow:**
1. Crawl site structure
2. Analyze technical SEO factors
3. Evaluate on-page optimization
4. Assess content quality
5. Check backlink profile
6. Generate prioritized recommendations

**Agents:** `attraction-specialist`

---

### /seo:keywords
```yaml
---
description: Conduct keyword research for topic/niche
argument-hint: [topic-or-seed-keyword]
---
```

**Workflow:**
1. Expand seed keywords
2. Analyze search intent
3. Assess keyword difficulty
4. Identify content gaps
5. Group by topic clusters
6. Prioritize by opportunity

**Agents:** `attraction-specialist`, `researcher`

---

### /seo:competitor
```yaml
---
description: Analyze competitor SEO strategy
argument-hint: [competitor-url]
---
```

**Workflow:**
1. Identify top-ranking pages
2. Analyze keyword portfolio
3. Assess content strategy
4. Evaluate backlink sources
5. Find content gaps
6. Generate competitive playbook

**Agents:** `researcher`, `attraction-specialist`

---

### /seo:optimize
```yaml
---
description: Optimize content for target keywords
argument-hint: [content-file] [target-keyword]
---
```

**Workflow:**
1. Analyze current optimization
2. Check title/meta optimization
3. Evaluate heading structure
4. Assess keyword density
5. Check internal linking
6. Generate optimized version

**Agents:** `copywriter`, `attraction-specialist`

---

## 4.4 Leads Commands

### /leads:qualify
```yaml
---
description: Create lead qualification criteria
argument-hint: [product-or-service]
---
```

**Workflow:**
1. Define ICP characteristics
2. Create scoring dimensions
3. Set qualification thresholds
4. Design disqualification criteria
5. Build handoff protocols
6. Generate qualification playbook

**Agents:** `lead-qualifier`

---

### /leads:score
```yaml
---
description: Design lead scoring model
argument-hint: [business-context]
---
```

**Workflow:**
1. Identify scoring signals
2. Weight behavioral factors
3. Weight demographic factors
4. Define score thresholds
5. Map scores to actions
6. Create scoring documentation

**Agents:** `lead-qualifier`

---

### /leads:nurture
```yaml
---
description: Design lead nurture sequence
argument-hint: [segment-or-stage]
---
```

**Workflow:**
1. Map buyer journey stage
2. Identify content needs
3. Design email sequence
4. Set timing and triggers
5. Create content briefs
6. Generate sequence documentation

**Agents:** `email-wizard`, `lead-qualifier`

---

## 4.5 Analytics Commands

### /analytics:report
```yaml
---
description: Generate marketing performance report
argument-hint: [timeframe] [channels]
---
```

**Workflow:**
1. Gather channel metrics
2. Calculate key KPIs
3. Compare to benchmarks
4. Identify trends
5. Generate visualizations
6. Create executive summary

**Agents:** `researcher`

---

### /analytics:funnel
```yaml
---
description: Analyze conversion funnel performance
argument-hint: [funnel-name-or-url]
---
```

**Workflow:**
1. Map funnel stages
2. Calculate stage conversions
3. Identify drop-off points
4. Analyze user behavior
5. Generate optimization hypotheses
6. Create funnel report

**Agents:** `lead-qualifier`

---

### /analytics:roi
```yaml
---
description: Calculate campaign/channel ROI
argument-hint: [campaign-or-channel]
---
```

**Workflow:**
1. Gather cost data
2. Attribute revenue
3. Calculate ROAS
4. Compute CAC/LTV
5. Model scenarios
6. Generate ROI report

**Agents:** `upsell-maximizer`

---

## 4.6 Brand Commands

### /brand:voice
```yaml
---
description: Create brand voice guidelines
argument-hint: [brand-context]
---
```

**Workflow:**
1. Analyze brand positioning
2. Define voice attributes
3. Create tone variations
4. Develop do's and don'ts
5. Generate example copy
6. Create voice guide document

**Agents:** `copywriter`

---

### /brand:book
```yaml
---
description: Generate comprehensive brand book
argument-hint: [brand-name]
---
```

**Workflow:**
1. Define brand essence
2. Document visual identity
3. Create voice guidelines
4. Establish usage rules
5. Compile asset library
6. Generate brand book PDF

**Agents:** `copywriter`, `ui-ux-designer`

---

### /brand:assets
```yaml
---
description: Manage and organize brand assets
argument-hint: [action] [asset-type]
---
```

**Workflow:**
1. Inventory existing assets
2. Categorize by type
3. Tag with metadata
4. Generate usage guidelines
5. Create asset library index
6. Setup version control

**Agents:** `project-manager`

---

## 4.7 Social Commands

### /social:schedule
```yaml
---
description: Create social media posting schedule
argument-hint: [platforms] [timeframe]
---
```

**Workflow:**
1. Analyze optimal posting times
2. Map content to platforms
3. Create posting calendar
4. Set frequency per platform
5. Align with campaigns
6. Generate schedule document

**Agents:** `project-manager`

---

### /social:engage
```yaml
---
description: Develop social engagement strategy
argument-hint: [platform]
---
```

**Workflow:**
1. Analyze audience behavior
2. Identify engagement opportunities
3. Create response templates
4. Design community initiatives
5. Set engagement metrics
6. Generate engagement playbook

**Agents:** `continuity-specialist`

---

### /social:viral
```yaml
---
description: Create viral-potential content
argument-hint: [topic] [platform]
---
```

**Workflow:**
1. Analyze viral patterns
2. Identify trending formats
3. Apply viral frameworks
4. Create content variants
5. Optimize for algorithm
6. Generate viral content brief

**Agents:** `copywriter`

---

## 4.8 Research Commands

### /research:market
```yaml
---
description: Conduct market research analysis
argument-hint: [market-or-industry]
---
```

**Workflow:**
1. Define research scope
2. Gather market data
3. Analyze trends
4. Assess competition
5. Identify opportunities
6. Generate market report

**Agents:** `researcher`

---

### /research:persona
```yaml
---
description: Create detailed buyer persona
argument-hint: [product-or-segment]
---
```

**Workflow:**
1. Gather customer data
2. Identify patterns
3. Define demographics
4. Map psychographics
5. Document behaviors
6. Create persona profile

**Agents:** `lead-qualifier`, `researcher`

---

### /research:trend
```yaml
---
description: Analyze industry/market trends
argument-hint: [industry-or-topic]
---
```

**Workflow:**
1. Identify trend sources
2. Gather trend data
3. Analyze patterns
4. Predict trajectories
5. Assess implications
6. Generate trend report

**Agents:** `researcher`

---

## 4.9 Enhanced Content Commands

### /content:blog
```yaml
---
description: Create SEO-optimized blog post
argument-hint: [topic] [target-keyword]
---
```
**Agents:** `copywriter`, `attraction-specialist`

---

### /content:social
```yaml
---
description: Create platform-specific social content
argument-hint: [topic] [platform]
---
```
**Agents:** `copywriter`

---

### /content:email
```yaml
---
description: Create email copy with sequences
argument-hint: [email-type] [objective]
---
```
**Agents:** `email-wizard`

---

### /content:landing
```yaml
---
description: Create high-converting landing page copy
argument-hint: [offer] [audience]
---
```
**Agents:** `copywriter`, `attraction-specialist`

---

### /content:ads
```yaml
---
description: Create ad copy for paid campaigns
argument-hint: [platform] [objective]
---
```
**Agents:** `copywriter`

---

## 4.10 Command Quick Reference

| Command | Description | Primary Agent |
|---------|-------------|---------------|
| `/campaign:plan` | Campaign plan | planner |
| `/campaign:brief` | Creative brief | copywriter |
| `/campaign:calendar` | Content calendar | project-manager |
| `/campaign:analyze` | Performance analysis | researcher |
| `/seo:audit` | SEO audit | attraction-specialist |
| `/seo:keywords` | Keyword research | attraction-specialist |
| `/seo:competitor` | Competitor analysis | researcher |
| `/seo:optimize` | On-page optimization | copywriter |
| `/leads:qualify` | Lead qualification | lead-qualifier |
| `/leads:score` | Lead scoring | lead-qualifier |
| `/leads:nurture` | Nurture sequence | email-wizard |
| `/analytics:report` | Performance report | researcher |
| `/analytics:funnel` | Funnel analysis | lead-qualifier |
| `/analytics:roi` | ROI calculation | upsell-maximizer |
| `/brand:voice` | Voice guidelines | copywriter |
| `/brand:book` | Brand book | copywriter |
| `/brand:assets` | Asset management | project-manager |
| `/social:schedule` | Posting schedule | project-manager |
| `/social:engage` | Engagement strategy | continuity-specialist |
| `/social:viral` | Viral content | copywriter |
| `/research:market` | Market research | researcher |
| `/research:persona` | Buyer personas | lead-qualifier |
| `/research:trend` | Trend analysis | researcher |
| `/content:blog` | Blog posts | copywriter |
| `/content:social` | Social content | copywriter |
| `/content:email` | Email copy | email-wizard |
| `/content:landing` | Landing pages | copywriter |
| `/content:ads` | Ad copy | copywriter |
| `/content:cro` | CRO optimization | copywriter |
