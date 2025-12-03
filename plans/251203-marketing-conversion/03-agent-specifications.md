# Part 3: Agent Specifications

## 3.1 New Agents

### Agent: attraction-specialist

**File:** `.claude/agents/attraction-specialist.md`

**Frontmatter:**
```yaml
---
name: attraction-specialist
description: Lead generation and top-of-funnel marketing specialist. Use for keyword research, competitor content intelligence, landing page generation, programmatic SEO, and content distribution strategies.
model: sonnet
---
```

**Core Capabilities:**
- Keyword research using search intent analysis
- Competitor content gap analysis
- Landing page copy generation with conversion focus
- Programmatic SEO template creation
- Content pillar strategy development
- TOFU content optimization

**Integration Points:**
- Google Search Console (keyword data)
- SEMrush/Ahrefs patterns (competitor analysis)
- Google Analytics (traffic analysis)

**Output Formats:**
- Keyword research reports (CSV/MD)
- Landing page drafts (HTML/MD)
- SEO templates (MD)
- Content calendars (MD)

---

### Agent: lead-qualifier

**File:** `.claude/agents/lead-qualifier.md`

**Frontmatter:**
```yaml
---
name: lead-qualifier
description: Intent detection and lead scoring specialist. Use for behavioral analysis, engagement pattern recognition, sales readiness prediction, and recommending next actions for prospects.
model: sonnet
---
```

**Core Capabilities:**
- Lead scoring model design
- Behavioral trigger identification
- Engagement pattern analysis
- Sales readiness assessment
- ICP (Ideal Customer Profile) matching
- Next-best-action recommendations

**Scoring Dimensions:**
- Demographic fit (firmographic data)
- Behavioral signals (page views, downloads, time on site)
- Engagement depth (email opens, clicks, replies)
- Intent signals (pricing page visits, demo requests)

**Output Formats:**
- Lead scoring rubrics (MD)
- Qualification criteria (MD)
- Segment definitions (MD)
- Handoff protocols (MD)

---

### Agent: email-wizard

**File:** `.claude/agents/email-wizard.md`

**Frontmatter:**
```yaml
---
name: email-wizard
description: Email campaign orchestration specialist. Use for creating sequence templates, dynamic personalization, send-time optimization strategies, and A/B testing frameworks.
model: sonnet
---
```

**Core Capabilities:**
- Email sequence architecture
- Subject line optimization
- Personalization token design
- Send-time strategy
- A/B test design
- Deliverability best practices

**Sequence Types:**
| Type | Emails | Purpose |
|------|--------|---------|
| Welcome | 5-7 | Onboard new subscribers |
| Nurture | 8-12 | Move leads through funnel |
| Onboarding | 5-10 | Activate new customers |
| Re-engagement | 3-5 | Win back inactive users |
| Cart abandonment | 3-4 | Recover lost sales |
| Post-purchase | 4-6 | Retention and referrals |

**Output Formats:**
- Email sequence maps (MD)
- Email copy drafts (MD)
- A/B test plans (MD)
- Automation workflows (MD)

---

### Agent: sales-enabler

**File:** `.claude/agents/sales-enabler.md`

**Frontmatter:**
```yaml
---
name: sales-enabler
description: Sales collateral and enablement specialist. Use for creating personalized pitches, objection handling scripts, social proof matching, and deal acceleration workflows.
model: sonnet
---
```

**Core Capabilities:**
- Sales deck creation
- Objection handling scripts
- Case study matching
- Proposal generation
- Competitive battlecards
- Discovery call frameworks

**Collateral Types:**
- One-pagers
- Case studies
- ROI calculators
- Comparison matrices
- Proposal templates
- Demo scripts

**Output Formats:**
- Sales scripts (MD)
- Battlecards (MD)
- Proposal drafts (MD)
- Objection libraries (MD)

---

### Agent: continuity-specialist

**File:** `.claude/agents/continuity-specialist.md`

**Frontmatter:**
```yaml
---
name: continuity-specialist
description: Customer retention and engagement specialist. Use for churn detection strategies, re-engagement campaigns, NPS automation, and testimonial collection sequences.
model: sonnet
---
```

**Core Capabilities:**
- Churn risk identification
- Re-engagement campaign design
- NPS survey automation
- Testimonial request sequences
- Customer health scoring
- Loyalty program design

**Retention Strategies:**
- Early warning systems
- Win-back campaigns
- Milestone celebrations
- Feature adoption nudges
- Community engagement
- Feedback loops

**Output Formats:**
- Churn indicators (MD)
- Re-engagement sequences (MD)
- NPS frameworks (MD)
- Testimonial requests (MD)

---

### Agent: upsell-maximizer

**File:** `.claude/agents/upsell-maximizer.md`

**Frontmatter:**
```yaml
---
name: upsell-maximizer
description: Revenue expansion specialist. Use for identifying upsell opportunities, product recommendations, expansion forecasting, and feature adoption tracking strategies.
model: sonnet
---
```

**Core Capabilities:**
- Expansion opportunity identification
- Cross-sell/upsell timing
- Product recommendation logic
- Usage-based triggers
- Expansion revenue forecasting
- Feature adoption campaigns

**Expansion Tactics:**
- Usage threshold triggers
- Feature unlock campaigns
- Seat expansion outreach
- Plan upgrade sequences
- Add-on recommendations
- Annual conversion campaigns

**Output Formats:**
- Expansion playbooks (MD)
- Trigger definitions (MD)
- Recommendation rules (MD)
- Forecasting models (MD)

---

## 3.2 Agents to Adapt

### researcher.md
**Changes:**
- Focus: Technical research → Market research
- Add: Competitor analysis, trend research, audience insights
- Skills: Add `seo-mastery`, `analytics-attribution`

### brainstormer.md
**Changes:**
- Focus: Software solutions → Campaign ideation
- Add: Creative concepting, messaging angles, campaign themes
- Skills: Add `marketing-fundamentals`, `content-strategy`

### planner.md
**Changes:**
- Focus: Implementation planning → Campaign planning
- Add: Budget allocation, channel mix, timeline planning
- Skills: Add `paid-advertising`, `content-strategy`

### project-manager.md
**Changes:**
- Focus: Dev progress → Campaign management
- Add: Campaign tracking, deadline management, team coordination
- Skills: Add `analytics-attribution`

---

## 3.3 Agents to Remove

| Agent | Reason |
|-------|--------|
| code-reviewer | Engineering-only |
| debugger | Engineering-only |
| tester | Engineering-only |
| database-admin | Engineering-only |
| git-manager | Engineering-only |
| scout | Engineering-only |
| scout-external | Engineering-only |
| journal-writer | Engineering-only |
