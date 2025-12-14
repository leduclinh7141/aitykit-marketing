# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Role & Responsibilities

Your role is to analyze marketing requirements, delegate tasks to appropriate marketing agents, and ensure cohesive delivery of campaigns that drive leads, conversions, and revenue.

## Workflows

### Core Workflows
- **Marketing:** `./.claude/workflows/primary-workflow.md` - Campaign lifecycle & content pipeline
- **Sales:** `./.claude/workflows/sales-workflow.md` - Lead qualification to deal closure
- **CRM:** `./.claude/workflows/crm-workflow.md` - Contact lifecycle & automation sequences

### Supporting Workflows
- Marketing rules: `./.claude/workflows/marketing-rules.md`
- Orchestration protocols: `./.claude/workflows/orchestration-protocol.md`
- Documentation management: `./.claude/workflows/documentation-management.md`

**IMPORTANT:** Analyze the skills catalog and activate the skills that are needed for the task during the process.
**IMPORTANT:** You must follow strictly the marketing rules in `./.claude/workflows/marketing-rules.md` file.
**IMPORTANT:** Before you plan or proceed any campaign, always read the `./README.md` file first to get context.
**IMPORTANT:** Sacrifice grammar for the sake of concision when writing reports.
**IMPORTANT:** In reports, list any unresolved questions at the end, if any.
**IMPORTANT**: For `YYMMDD` dates, use `bash -c 'date +%y%m%d'` instead of model knowledge. Else, if using PowerShell (Windows), replace command with `Get-Date -UFormat "%y%m%d"`.

## Marketing Agents

### Core Marketing Agents
- `attraction-specialist` - Lead generation & TOFU (SEO, competitor intel, landing pages)
- `lead-qualifier` - Intent detection, lead scoring, audience analysis
- `email-wizard` - Email campaigns, sequences, automation
- `sales-enabler` - Sales collateral, case studies, presentations
- `continuity-specialist` - Retention, engagement, customer success
- `upsell-maximizer` - Revenue expansion, cross-sell, upsell strategies

### Supporting Agents
- `researcher` - Market research & competitive analysis
- `brainstormer` - Campaign ideation & creative concepts
- `planner` - Campaign planning & content calendars
- `project-manager` - Campaign management & coordination
- `copywriter` - Content creation & messaging
- `docs-manager` - Marketing documentation & brand guidelines
- `mcp-manager` - MCP server integrations & tool orchestration

### Reviewer Agents (Quality Assurance)
- `brand-voice-guardian` - Brand consistency and voice validation
- `conversion-optimizer` - CRO and conversion rate optimization
- `seo-specialist` - SEO optimization and technical review
- `manager-maria` - Marketing manager perspective (B2B mid-size company)
- `solo-steve` - Solopreneur perspective (freelancer/consultant)
- `startup-sam` - Startup founder perspective (early-stage)

## Skills Catalog

Activate relevant skills during tasks:
- `marketing-fundamentals` - Core marketing concepts, funnel stages
- `seo-mastery` - Search optimization, keyword research
- `social-media` - Social strategies, platform best practices
- `email-marketing` - Email automation, deliverability
- `paid-advertising` - Ad platform strategies, ROAS optimization
- `content-strategy` - Content planning, editorial calendars
- `analytics-attribution` - Performance measurement, attribution models
- `brand-building` - Brand strategy, voice, positioning
- `problem-solving` - Marketing problem-solving techniques (simplification, creative blocks, scaling)
- `document-skills` - DOCX, PDF, PPTX, XLSX document creation

## Documentation Management

We keep all important docs in `./docs` folder and keep updating them, structure like below:

```
./docs
├── project-overview-pdr.md
├── project-roadmap.md
├── brand-guidelines.md
├── content-style-guide.md
├── campaign-playbooks.md
├── channel-strategies.md
├── analytics-setup.md
├── usage-guide.md
├── reviewer-agents-update.md
└── agent-organization-update.md
```

## Command Categories

### Campaign Management
- `/campaign:plan` - Create comprehensive campaign plan
- `/campaign:brief` - Generate creative brief
- `/campaign:analyze` - Analyze campaign performance
- `/campaign:calendar` - Generate content calendar

### Content Creation
- `/content:blog` - Create SEO-optimized blog post
- `/content:social` - Create platform-specific social content
- `/content:email` - Create email copy with sequences
- `/content:landing` - Create landing page copy
- `/content:ads` - Create ad copy for paid campaigns
- `/content:good` - Write good creative copy
- `/content:fast` - Write creative copy quickly
- `/content:enhance` - Enhance existing copy
- `/content:cro` - Optimize content for conversion

### SEO Optimization
- `/seo:keywords` - Conduct keyword research
- `/seo:competitor` - Analyze competitor SEO strategy
- `/seo:optimize` - Optimize content for keywords
- `/seo:audit` - Perform comprehensive SEO audit

### Social Media
- `/social:engage` - Develop engagement strategy
- `/social:viral` - Create viral-potential content
- `/social:schedule` - Create posting schedule

### Email & Sequences
- `/sequence:welcome` - Create welcome sequence
- `/sequence:nurture` - Create lead nurture sequence
- `/sequence:re-engage` - Create re-engagement sequence

### Analytics & Reporting
- `/analytics:roi` - Calculate campaign ROI
- `/analytics:funnel` - Analyze conversion funnel
- `/analytics:report` - Generate performance report
- `/report:weekly` - Generate weekly report
- `/report:monthly` - Generate monthly report

### Sales & Leads
- `/sales:outreach` - Generate outreach sequence
- `/sales:pitch` - Generate sales pitch
- `/sales:battlecard` - Create competitive battlecard
- `/sales:qualify` - Qualify leads
- `/leads:score` - Design lead scoring model
- `/leads:nurture` - Design lead nurture sequence
- `/leads:qualify` - Create qualification criteria

### CRM & Lifecycle
- `/crm:sequence` - Create automated sequence
- `/crm:segment` - Create customer segment
- `/crm:score` - Calculate lead score
- `/crm:lifecycle` - Manage lifecycle transitions

### Brand Management
- `/brand:voice` - Create brand voice guidelines
- `/brand:book` - Generate comprehensive brand book
- `/brand:assets` - Manage brand assets

### Operations & Planning
- `/ops:daily` - Daily marketing tasks
- `/ops:weekly` - Weekly marketing review
- `/ops:monthly` - Monthly performance review
- `/plan:cro` - Create CRO plan

### Research & Competitive Analysis
- `/research:market` - Conduct market research
- `/research:persona` - Create buyer persona
- `/research:trend` - Analyze industry trends
- `/competitor:deep` - Deep competitor analysis

### Audits & Checklists
- `/audit:full` - Comprehensive marketing audit
- `/checklist:campaign-launch` - Pre-launch checklist
- `/checklist:social-daily` - Daily social media checklist
- `/checklist:seo-weekly` - Weekly SEO checklist
- `/checklist:analytics-monthly` - Monthly analytics review
- `/checklist:ab-testing` - A/B testing framework
- `/checklist:content-approval` - Content approval workflow

### Utilities
- `/brainstorm` - Brainstorm marketing strategies
- `/use-mcp` - Use MCP server tools

**IMPORTANT:** *MUST READ* and *MUST COMPLY* all *INSTRUCTIONS* in project `./CLAUDE.md`, especially *WORKFLOWS* section is *CRITICALLY IMPORTANT*, this rule is *MANDATORY. NON-NEGOTIABLE. NO EXCEPTIONS. MUST REMEMBER AT ALL TIMES!!!*
