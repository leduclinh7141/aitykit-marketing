# AityKit Marketing Usage Guide

Complete guide to using aitykit-marketing for production marketing workflows and learning.

## Quick Start

### For New Users (Learning Mode)

Start with interactive training:
```bash
cd /path/to/aitykit-marketing
claude
/training:start-0-0
```

Complete all training modules (4-6 hours) to master the system.

### For Experienced Users (Production Mode)

Jump straight into production workflows:
```bash
# Plan a campaign
/campaign:plan "Q1 Product Launch"

# Generate content
/content:good "Blog post about new feature"

# Analyze competitors
/competitor:deep "competitor-url.com"

# Create SEO strategy
/seo:keywords "your topic"
```

---

## Project Structure

```
aitykit-marketing/
├── .claude/
│   ├── agents/              # 12 specialized marketing agents
│   │   ├── reviewers/       # 6 persona-based reviewers (from cc4)
│   │   └── *.md            # Core marketing agents
│   ├── commands/            # 30+ slash commands
│   │   └── training/        # 19 training lesson commands (from cc4)
│   ├── skills/              # Marketing domain skills
│   └── workflows/           # Core workflows and protocols
├── docs/                    # Documentation
├── plugins/                 # Plugin extensions (from cc4)
│   ├── content-factory/     # High-volume content generation
│   └── campaign-manager/    # Campaign planning & review
├── training/                # Interactive training modules (from cc4)
│   ├── exercises/markit/    # Practice project
│   └── modules/            # Learning modules
└── guide/                   # Command & skills reference
```

---

## Core Workflows

### 1. Campaign Planning & Execution

**Plan Campaign:**
```bash
/campaign:plan "Campaign Name"
```
Creates comprehensive brief with objectives, audience, channels, budget, metrics.

**Create Campaign Brief:**
```bash
/campaign:brief "Campaign Name"
```
Generates creative brief for execution.

**Analyze Campaign:**
```bash
/campaign:analyze "campaign-name-or-url"
```
Reviews performance and provides insights.

**Generate Calendar:**
```bash
/campaign:calendar "timeframe"
```
Creates content distribution calendar.

---

### 2. Content Creation

#### High-Quality Content (Production)

**Fast Mode (Good Quality):**
```bash
/content:fast "LinkedIn post about productivity tips"
```
Quick turnaround, good quality for social and short-form.

**Good Mode (High Quality):**
```bash
/content:good "Blog post: 10 ways to improve team collaboration"
```
Thorough research, high quality for blogs and important content.

**Landing Pages:**
```bash
/content:landing "offer" "audience"
```
High-converting landing page copy.

**Email Campaigns:**
```bash
/content:email "email-type" "objective"
```
Creates email copy with sequences.

**Social Media:**
```bash
/content:social "topic" "platform"
```
Platform-specific social content.

**Blog Posts:**
```bash
/content:blog "topic" "target-keyword"
```
SEO-optimized long-form content.

#### Content Optimization

**Conversion Rate Optimization:**
```bash
/content:cro "current-content-issues"
```
Analyzes and optimizes for conversions.

**Content Enhancement:**
```bash
/content:enhance "issues"
```
Improves existing copy.

**Ad Copy:**
```bash
/content:ads "platform" "objective"
```
Creates ad copy for paid campaigns.

---

### 3. SEO & Competitive Intelligence

**Keyword Research:**
```bash
/seo:keywords "topic-or-seed-keyword"
```
Comprehensive keyword research with volume and difficulty.

**Competitor Analysis:**
```bash
/seo:competitor "competitor-url"
```
Analyzes competitor SEO strategy.

**Content Optimization:**
```bash
/seo:optimize "content-file" "target-keyword"
```
Optimizes existing content for SEO.

**SEO Audit:**
```bash
/seo:audit "url-or-sitemap"
```
Complete technical and content SEO audit.

**Deep Competitor Analysis:**
```bash
/competitor:deep "competitor-url"
```
Comprehensive competitive intelligence.

---

### 4. Email Marketing & Sequences

**Welcome Sequence:**
```bash
/sequence:welcome "brand-or-product" "audience"
```
Creates onboarding email sequence.

**Nurture Sequence:**
```bash
/sequence:nurture "product-or-service" "target-segment"
```
Converts leads to MQL/SQL.

**Re-engagement:**
```bash
/sequence:re-engage "brand-or-product" "inactive-criteria"
```
Wins back inactive contacts.

---

### 5. Lead Generation & Qualification

**Lead Scoring:**
```bash
/leads:score "business-context"
```
Designs lead scoring model.

**Lead Nurturing:**
```bash
/leads:nurture "segment-or-stage"
```
Creates nurture sequence strategy.

**Lead Qualification:**
```bash
/leads:qualify "product-or-service"
```
Establishes qualification criteria.

---

### 6. Social Media Management

**Engagement Strategy:**
```bash
/social:engage "platform"
```
Develops platform-specific engagement.

**Viral Content:**
```bash
/social:viral "topic" "platform"
```
Creates high-engagement content.

**Content Schedule:**
```bash
/social:schedule "platforms" "timeframe"
```
Plans posting calendar.

---

### 7. Sales Enablement

**Sales Pitch:**
```bash
/sales:pitch "prospect-company" "use-case"
```
Customized pitch deck content.

**Outreach Sequence:**
```bash
/sales:outreach "prospect-info" "sequence-type"
```
Personalized outreach messaging.

**Competitive Battlecard:**
```bash
/sales:battlecard "competitor-name-or-url"
```
Competitive positioning document.

**Lead Qualification:**
```bash
/sales:qualify "lead-info-or-company"
```
BANT/MEDDIC qualification analysis.

---

### 8. CRM & Lifecycle Management

**Customer Segmentation:**
```bash
/crm:segment "segment-criteria-or-name"
```
Creates customer segments.

**Lead Scoring:**
```bash
/crm:score "lead-data"
```
Calculates lead score.

**Lifecycle Management:**
```bash
/crm:lifecycle "contact-or-segment" "action"
```
Manages stage transitions.

**Automated Sequence:**
```bash
/crm:sequence "sequence-type" "target-segment"
```
Creates CRM automation.

---

### 9. Analytics & Reporting

**ROI Calculation:**
```bash
/analytics:roi "campaign-or-channel"
```
Calculates marketing ROI.

**Funnel Analysis:**
```bash
/analytics:funnel "funnel-name-or-url"
```
Analyzes conversion paths.

**Performance Report:**
```bash
/analytics:report "timeframe" "channels"
```
Generates comprehensive report.

**Weekly Report:**
```bash
/report:weekly "client-or-project" "week-dates"
```
Client-ready weekly summary.

**Monthly Report:**
```bash
/report:monthly "client-or-project" "month-year"
```
Comprehensive monthly review.

---

### 10. Brand & Documentation

**Brand Voice:**
```bash
/brand:voice "brand-context"
```
Creates voice guidelines.

**Brand Book:**
```bash
/brand:book "brand-name"
```
Comprehensive brand documentation.

**Asset Management:**
```bash
/brand:assets "action" "asset-type"
```
Organizes brand assets.

---

## Using Plugins

### Content Factory Plugin

High-volume content generation with templates.

**Location:** `./plugins/content-factory/`

**Use Cases:**
- Product launch content blitz (blog, email, social, ads)
- Content repurposing across formats
- Monthly content calendar automation

**Integration:** Templates available via `/content:*` commands

**Templates:**
- Blog templates (how-to, listicle, case study)
- Social media templates (LinkedIn, Twitter, Instagram)
- Video script templates
- Email templates (welcome, nurture, promotional)

---

### Campaign Manager Plugin

Systematic campaign planning with specialized reviewers.

**Location:** `./plugins/campaign-manager/`

**Use Cases:**
- Campaign planning with research frameworks
- Multi-perspective content review
- Brand consistency validation

**Persona Reviewers (in `.claude/agents/`):**
- **Brand Voice Guardian** - Ensures brand consistency
- **Conversion Optimizer** - Maximizes conversion rates
- **SEO Specialist** - Search optimization
- **Startup Founder** - Founder perspective (28yo)
- **Marketing Manager** - Manager perspective (38yo)
- **Solopreneur** - Solopreneur perspective (32yo)

**Integration:** Use with `/campaign:*` commands

---

## Agent System

### Core Marketing Agents

**Attraction Specialist** - TOFU lead generation
- SEO, competitor intelligence, landing pages
- Use for: Traffic generation, awareness campaigns

**Lead Qualifier** - Intent detection & scoring
- Behavioral analysis, lead scoring
- Use for: Lead prioritization, segmentation

**Email Wizard** - Email campaigns & automation
- Sequences, personalization, optimization
- Use for: Email marketing, drip campaigns

**Sales Enabler** - Sales collateral & enablement
- Pitches, case studies, battlecards
- Use for: Sales support, deal acceleration

**Continuity Specialist** - Customer retention
- Churn detection, re-engagement, NPS
- Use for: Retention, customer success

**Upsell Maximizer** - Revenue expansion
- Cross-sell, upsell, feature adoption
- Use for: Account expansion, growth

### Supporting Agents

**Researcher** - Market research & analysis
**Brainstormer** - Campaign ideation
**Planner** - Strategic planning
**Project Manager** - Campaign coordination
**Copywriter** - Content creation
**UI/UX Designer** - Landing page design
**Docs Manager** - Documentation management

### Persona Reviewers (from Plugins)

**Brand Voice Guardian** - Brand consistency
**Conversion Optimizer** - CRO expert
**SEO Specialist** - Search optimization
**Startup Founder** - Founder perspective
**Marketing Manager** - Manager perspective
**Solopreneur** - Solopreneur perspective

---

## Checklists & Operations

### Daily Operations

```bash
/ops:daily "focus-area"
```
Daily task checklist and priorities.

### Weekly Operations

```bash
/ops:weekly "week-ending-date"
```
Weekly review and planning.

### Monthly Operations

```bash
/ops:monthly "month-year"
```
Monthly performance review.

### Specialized Checklists

**A/B Testing:**
```bash
/checklist:ab-testing "test-type" "element"
```

**SEO Maintenance:**
```bash
/checklist:seo-weekly "website"
```

**Social Media:**
```bash
/checklist:social-daily "platforms" "brand"
```

**Campaign Launch:**
```bash
/checklist:campaign-launch "campaign-name" "launch-date"
```

**Content Approval:**
```bash
/checklist:content-approval "content-type" "approvers"
```

**Analytics Review:**
```bash
/checklist:analytics-monthly "month-year" "client"
```

---

## Planning & Research

### Research Commands

**Market Research:**
```bash
/research:market "market-or-industry"
```

**Buyer Persona:**
```bash
/research:persona "product-or-segment"
```

**Trend Analysis:**
```bash
/research:trend "industry-or-topic"
```

### Planning Commands

**Fast Planning:**
```bash
/plan:fast "task"
```
Quick implementation plan without deep research.

**Thorough Planning:**
```bash
/plan:hard "task"
```
Comprehensive research and analysis.

**Two Approaches:**
```bash
/plan:two "task"
```
Compare two strategic approaches.

**CRO Planning:**
```bash
/plan:cro "issues"
```
Conversion optimization strategy.

---

## Training Mode

### Interactive Learning

Start training:
```bash
/training:start-0-0
```

**Module 0: Getting Started**
- `/training:start-0-0` - Introduction
- `/training:start-0-1` - Setup
- `/training:start-0-2` - First task

**Module 1: Core Concepts**
- `/training:start-1-1` to `/training:start-1-7`
- Learn: Campaign briefs, agents, project memory

**Module 2: Advanced Workflows**
- `/training:start-2-1` to `/training:start-2-6`
- Build: Content library, analytics, SEO plans

**Bonus Content:**
- `/training:bonus-secret` - 10x Marketer Framework
- `/training:bonus-patterns` - Pattern library
- `/training:help` - Training help

**Practice Project:** Markit agency for Planerio client
**Location:** `./training/exercises/markit/`

---

## Best Practices

### The Compounding Philosophy

Each campaign makes the next one easier:

**Campaign 1:** 40 hours
- Build foundation
- Create templates
- Document patterns

**Campaign 5:** 15 hours (62% faster)
- Leverage templates
- Automated workflows
- Pattern recognition

**Campaign 10:** 10 hours (75% faster)
- Fully systematized
- Rich library
- Strategic focus

### Building Your Marketing Library

1. **Start with Training** - Complete modules
2. **Customize Templates** - Adapt for your brand
3. **Document Patterns** - What works for you
4. **Create Personas** - Your specific audience
5. **Build Sequences** - Reusable email flows
6. **Refine Voice** - Brand consistency

### Workflow Optimization

**For Each Campaign:**
1. Plan: `/campaign:plan`
2. Research: `/seo:keywords`, `/competitor:deep`
3. Create: `/content:*` commands
4. Optimize: `/content:cro`, `/seo:optimize`
5. Review: Use persona reviewers
6. Report: `/report:weekly`

**Reuse & Refine:**
- Save successful campaigns as templates
- Document what worked
- Build pattern library
- Compound efficiency

---

## Advanced Features

### Agent Orchestration

**Delegate to specialized agents:**
- Use Task tool for complex multi-step work
- Agents work in parallel when possible
- Context preserved across agent handoffs

**When to delegate:**
- Complex research: researcher agent
- Strategic planning: planner agent
- Content review: copywriter + persona reviewers
- Multi-channel campaigns: project-manager agent

### Plugin Development

Create custom plugins:
```
plugins/
└── your-plugin/
    ├── README.md
    ├── commands/
    ├── agents/
    ├── templates/
    └── workflows/
```

See `./plugins/README.md` for details.

### Custom Slash Commands

Add to `.claude/commands/`:
- Follow existing patterns
- Use markdown format
- Document clearly
- Test thoroughly

---

## Integration Examples

### Full Campaign Workflow

```bash
# 1. Planning Phase
/campaign:plan "Q2 Product Launch"
/research:market "productivity software"
/competitor:deep "competitor.com"
/research:persona "remote team managers"

# 2. Strategy Phase
/seo:keywords "team productivity"
/plan:hard "content marketing strategy"
/campaign:calendar "6 weeks"

# 3. Content Creation
/content:blog "10 ways to improve team focus" "team productivity"
/content:email "welcome" "trial users"
/content:social "productivity tips" "linkedin"
/content:landing "free trial offer" "team managers"
/content:ads "linkedin" "awareness"

# 4. Optimization
/seo:optimize "blog-post.md" "team productivity"
/content:cro "landing page copy"

# 5. Enablement
/sales:pitch "enterprise prospect" "team collaboration"
/sales:battlecard "competitor.com"

# 6. Execution
/sequence:welcome "product" "trial users"
/social:schedule "linkedin,twitter" "6 weeks"

# 7. Tracking
/analytics:funnel "trial signup funnel"
/report:weekly "Q2 Launch" "Week 1"
```

---

## Troubleshooting

### Command Not Found

**Issue:** Slash command doesn't work
**Solution:**
- Check spelling: `/campaign:plan` not `/campaignplan`
- Training commands need prefix: `/training:start-0-0`
- See `/guide/COMMANDS.md` for full list

### Agent Not Responding

**Issue:** Agent doesn't activate
**Solution:**
- Check `.claude/agents/` directory
- Verify agent file exists
- Review CLAUDE.md for agent coordination

### Templates Not Loading

**Issue:** Can't find templates
**Solution:**
- Check `.claude/skills/marketing-fundamentals/templates/`
- Check `./plugins/*/templates/`
- Verify file paths in commands

---

## Support & Resources

### Documentation

- **This Guide** - Complete usage reference
- **Commands Reference** - `./guide/COMMANDS.md`
- **Skills Catalog** - `./guide/SKILLS.md`
- **Plugin Docs** - `./plugins/README.md`
- **Training Guide** - `./training/README.md`
- **Merge Strategy** - `./docs/cc4-marketing-merge-strategy.md`

### Project Files

- **Main README** - `./README.md`
- **CLAUDE.md** - Agent instructions and workflows
- **Workflows** - `./.claude/workflows/`

### Community

- GitHub Issues - Bug reports
- GitHub Discussions - Questions and ideas
- Contributions - PRs welcome

---

## What's New (CC4 Integration)

### Added from cc4.marketing

✅ **Plugins:**
- Content Factory - Batch content generation
- Campaign Manager - Systematic planning

✅ **Training Modules:**
- 19 interactive lessons
- Practice project (Markit/Planerio)
- Bonus frameworks

✅ **Persona Reviewers:**
- 6 specialized reviewer agents
- Multi-perspective validation

✅ **Templates:**
- Enhanced content templates
- Campaign planning frameworks
- Email sequence templates

### Enhanced Existing Features

✅ Content creation commands
✅ Campaign planning workflows
✅ Multi-agent review capabilities
✅ Template library expansion

---

**Start creating better marketing, faster.** 🚀
