# AityKit Marketing

**AI-Powered Marketing Automation Framework for Claude Code**

A comprehensive marketing kit that brings systematic, efficient marketing workflows to Claude Code. Plan campaigns, generate content, analyze competitors, and automate marketing operations—all powered by 18 specialized AI agents, 76 slash commands, and the Compounding Marketing philosophy.

**System Overview:**
- **18 Marketing Agents** - Core, Supporting, and Reviewer agents
- **76 Slash Commands** - Organized by category (campaign, content, SEO, analytics, etc.)
- **9 Marketing Skills** - Domain expertise modules
- **3 Core Workflows** - Marketing Pipeline, Sales Pipeline, CRM Lifecycle
- **19 Training Lessons** - Interactive hands-on learning

## What is Claude Code?

**Claude Code** is Anthropic's official CLI tool that brings AI-powered development assistance directly to your terminal. It enables natural language interaction with your codebase and provides intelligent automation for common development tasks.

- [Claude Code](https://claude.com/product/claude-code)
- [Docs](https://docs.claude.com/en/docs/claude-code/overview)

**Open Code CLI Coding Agents** extend Claude Code with specialized AI agents that handle specific aspects of software development - from planning and research to testing and documentation. This creates a collaborative AI development team that works alongside human developers.

- [Open Code](https://opencode.ai/)
- [Docs](https://opencode.ai/docs)

## Related Projects & Directories

- `aitykit` - Website of AityKit
  - Directory: `../aitykit`
  - Repo: https://github.com/leduclinh7141/aitykit
- `aitykit-marketing` - Marketing Kit repository
  - Directory: `../aitykit-marketing`
  - Repo: https://github.com/leduclinh7141/aitykit-marketing
- `aitykit-cli` - CLI tool for quick project setup
  - Directory: `../aitykit-cli`
  - Repo: https://github.com/mrgoonie/aitykit-cli
- `aitykit-docs` - Public documentation repository: https://docs.aitykit.cc
  - Directory: `../aitykit-docs`
  - Repo: https://github.com/leduclinh7141/aitykit-docs

## Key Benefits

### 🚀 Accelerated Marketing
- **AI-Powered Campaign Planning**: Automated campaign strategy and content calendars
- **Intelligent Content Generation**: Context-aware copy creation and optimization
- **Automated SEO**: Comprehensive keyword research and on-page optimization
- **Multi-Channel Orchestration**: Coordinated campaigns across email, social, ads

### 🎯 Enhanced Performance
- **Multi-Perspective Review**: Specialized reviewers for brand, SEO, conversion, personas
- **Data-Driven Optimization**: Continuous testing and performance tracking
- **Best Practices Enforcement**: Built-in adherence to marketing frameworks
- **Conversion-First Approach**: Every asset optimized for leads and revenue

### 🏗️ Structured Workflow
- **Agent Orchestration**: Coordinated AI agents for research, planning, execution
- **Campaign Management**: Automated progress tracking and deliverable monitoring
- **Documentation Sync**: Always up-to-date brand guidelines and playbooks
- **Quality Assurance**: Multi-stage review before content publication

## Documentation

### 📚 Core Documentation
- **[Usage Guide](./docs/usage-guide.md)** - Complete command reference and workflows
- **[Project Overview & PDR](./docs/project-overview-pdr.md)** - Project goals, features, and requirements
- **[Project Roadmap](./docs/project-roadmap.md)** - Development timeline and milestones
- **[Training Guide](./training/README.md)** - Interactive learning path
- **[Plugin Guide](./plugins/README.md)** - Plugin system overview

### 📖 Additional Resources
- **[CLAUDE.md](./CLAUDE.md)** - Marketing workflows and agent instructions
- **[CHANGELOG.md](./CHANGELOG.md)** - Version history and release notes
- **[Reviewer Agents](./docs/reviewer-agents-update.md)** - Persona reviewers documentation
- **[Agent Organization](./docs/agent-organization-update.md)** - Agent structure documentation

## Quick Start

### For New Users (Start with Training)

Learn marketing automation through hands-on practice:

```bash
# Navigate to project
cd aitykit-marketing

# Launch Claude Code
claude

# Begin interactive training
/training:start-0-0
```

**Time:** 4-6 hours for complete training
**What You'll Build:** Campaign briefs, content library, brand guidelines
**Practice Project:** Markit agency for Planerio client

### For Experienced Users (Jump to Production)

Start using marketing automation immediately:

```bash
# Plan a campaign
/campaign:plan "Q1 Product Launch"

# Generate content
/content:good "Blog post about our new feature"

# SEO research
/seo:keywords "your topic"

# Competitor analysis
/competitor:deep "competitor-url.com"

# Create email sequence
/sequence:welcome "your-product" "trial users"
```

### Installation

**Prerequisites:**
- [Claude Code](https://code.claude.com/docs/en/setup) installed and configured
- Git for version control

**Clone Repository:**
```bash
git clone https://github.com/leduclinh7141/aitykit-marketing.git
cd aitykit-marketing
claude
```

📖 **Complete Documentation:**
- **[Usage Guide](./docs/usage-guide.md)** - Complete command reference and workflows
- **[Training Guide](./training/README.md)** - Interactive learning path
- **[Plugin Guide](./plugins/README.md)** - Plugin system overview
- **[CC4 Integration Summary](./docs/cc4-integration-summary.md)** - What's new details
- **[Commands Reference](./guide/COMMANDS.md)** - All slash commands
- **[Skills Catalog](./guide/SKILLS.md)** - Available marketing skills

## What's New 🎉

### Enterprise-Grade Marketing System (December 2024)

✅ **18 Specialized Marketing Agents**
- 6 Core agents (Attraction, Lead Qualifier, Email Wizard, Sales Enabler, Continuity, Upsell)
- 6 Supporting agents (Researcher, Brainstormer, Planner, Copywriter, Project Manager, Docs Manager)
- 6 Reviewer agents (Brand Voice, CRO, SEO, Manager Maria, Solo Steve, Startup Sam)

✅ **76 Slash Commands**
- Campaign management (`/campaign:*`)
- Content creation (`/content:*`)
- SEO optimization (`/seo:*`)
- Analytics & reporting (`/analytics:*`, `/report:*`)
- Sales & leads (`/sales:*`, `/leads:*`)
- Email sequences (`/sequence:*`)
- And more...

✅ **3 Core Workflows**
- Marketing Pipeline: TOFU → MOFU → BOFU → Retention
- Sales Pipeline: Lead → MQL → SQL → Opportunity → Customer
- CRM Lifecycle: Contact management and automation

✅ **19 Interactive Training Lessons**
- Module 0: Getting Started (3 lessons)
- Module 1: Core Concepts (7 lessons)
- Module 2: Advanced Applications (6 lessons)
- Bonus content: Pattern Library, 10x Marketer Framework

✅ **Multi-Language Support**
- All agents and commands respond in user's language
- Enterprise-grade quality standards

## Project Structure

```
├── .claude/                 # Claude Code configuration
│   ├── agents/             # Marketing agents + persona reviewers
│   │   ├── reviewers/      # Quality assurance persona agents
│   │   └── *.md           # Core marketing agents
│   ├── commands/           # Slash commands (76 marketing commands)
│   │   ├── training/       # Interactive training lessons
│   │   └── */             # Organized by category (campaign, content, seo, etc.)
│   ├── hooks/              # Discord/Telegram notification hooks
│   ├── skills/             # Marketing domain skills
│   │   ├── marketing-fundamentals/
│   │   ├── seo-mastery/
│   │   ├── social-media/
│   │   ├── email-marketing/
│   │   ├── paid-advertising/
│   │   ├── content-strategy/
│   │   ├── analytics-attribution/
│   │   ├── brand-building/
│   │   └── document-skills/
│   └── workflows/          # Core marketing workflows
├── plugins/                # Plugin extensions
│   ├── content-factory/    # High-volume content generation
│   └── campaign-manager/   # Campaign planning & review
├── training/               # Interactive training modules
│   ├── exercises/markit/   # Practice agency project (Planerio client)
│   └── README.md          # Training guide
├── docs/                   # Marketing documentation
│   ├── usage-guide.md      # Complete command reference
│   ├── project-overview-pdr.md
│   ├── project-roadmap.md
│   └── *.md               # Various guides and updates
├── CLAUDE.md              # Marketing workflows and agent instructions
└── README.md              # This file
```

## The AI Marketing Team

Specialized AI agents that work together to deliver high-performance marketing campaigns:

### 🎯 Core Marketing Agents

#### **Attraction Specialist**
- Lead generation and TOFU strategy (SEO, landing pages, competitor intel)
- Keyword research and content gap analysis
- Programmatic SEO and organic traffic growth
- Landing page optimization and A/B testing

#### **Lead Qualifier**
- Intent detection and behavioral analysis
- Lead scoring model design
- Audience segmentation and persona development
- Sales readiness prediction

#### **Email Wizard**
- Email sequence design and automation
- Deliverability optimization
- Personalization and dynamic content
- A/B testing and performance analysis

#### **Sales Enabler**
- Sales collateral and case studies
- Competitive battlecards
- Pitch deck creation
- Objection handling scripts

#### **Continuity Specialist**
- Customer retention and re-engagement
- NPS automation and feedback loops
- Lifecycle marketing campaigns
- Customer success content

#### **Upsell Maximizer**
- Revenue expansion strategies
- Cross-sell and upsell campaigns
- Usage-based triggers
- Feature adoption tracking

### 🔍 Supporting Agents

#### **Researcher**
- Market research and competitive analysis
- Audience insights and trend analysis
- Industry best practices
- Data-driven recommendations

#### **Brainstormer**
- Campaign ideation and creative concepts
- Strategy workshops and planning sessions
- Multi-approach evaluation
- Creative problem-solving

#### **Planner**
- Campaign planning and content calendars
- Budget allocation and resource planning
- Timeline and milestone management
- Channel mix strategy

#### **Copywriter**
- High-converting copy creation
- Brand voice consistency
- Messaging frameworks
- Content optimization

#### **Project Manager**
- Campaign coordination and tracking
- Deadline management
- Status reporting
- Cross-functional alignment

#### **Docs Manager**
- Brand guidelines management
- Marketing documentation
- Playbook creation
- Knowledge base maintenance

### ⭐ Reviewer Agents (Quality Assurance)

#### **Brand Voice Guardian**
- Brand consistency validation
- Voice and tone review
- Messaging alignment
- Emotional impact assessment

#### **Conversion Optimizer**
- CRO best practices application
- Persuasion psychology review
- Friction analysis
- CTA optimization

#### **SEO Specialist**
- On-page SEO optimization
- Keyword usage validation
- Technical SEO review
- SERP feature potential

#### **Manager Maria** (Marketing Manager Persona)
- Team execution feasibility
- ROI and budget alignment
- Enterprise/mid-market fit
- Resource requirements

#### **Solo Steve** (Solopreneur Persona)
- Self-service ease
- Time efficiency
- Budget sensitivity
- DIY implementation

#### **Startup Sam** (Startup Founder Persona)
- Growth potential and virality
- Speed to market
- Scrappy execution
- Founder-market fit

## Marketing Workflow Examples

### 1. Campaign Launch
```bash
# Start with research and planning
/research:market "SaaS productivity tools"
/competitor:deep "competitor-url.com"

# Create campaign plan
/campaign:plan "Q1 Product Launch"

# Generate content assets
/content:landing "new feature" "target audience"
/content:email "product launch" "trial users"
/content:social "product announcement" "linkedin"

# SEO optimization
/seo:keywords "product category"
/seo:optimize "landing-page.md" "target keyword"

# Review with personas
# Brand voice guardian reviews messaging
# Conversion optimizer reviews CTAs
# SEO specialist reviews optimization

# Schedule and track
/social:schedule "linkedin, twitter" "2 weeks"
/ops:weekly "2024-01-15"
```

### 2. Content Creation Pipeline
```bash
# Research and ideation
/research:persona "target customer segment"
/brainstorm "content ideas for blog"

# Create content
/content:blog "topic" "target keyword"

# Optimize for conversion
/content:cro "blog-post.md"

# Multi-channel repurposing
/content:social "blog summary" "twitter"
/content:email "blog announcement" "newsletter"

# Quality review
# Brand voice validation
# SEO optimization check
```

### 3. Lead Nurture Campaign
```bash
# Design lead scoring
/leads:score "SaaS B2B product"

# Create nurture sequence
/sequence:nurture "product" "MQL segment"

# Build email automation
/crm:sequence "lead nurture" "30-day drip"

# Sales enablement
/sales:battlecard "main competitor"
/sales:pitch "enterprise prospect" "use case"

# Track and optimize
/analytics:funnel "lead-to-customer"
/analytics:roi "nurture campaign"
```

### 4. SEO Content Strategy
```bash
# Keyword research
/seo:keywords "industry topic"

# Competitor analysis
/seo:competitor "competitor-blog.com"

# Content creation
/content:blog "target keyword topic" "primary keyword"

# On-page optimization
/seo:optimize "blog-post.md" "primary keyword"

# Technical audit
/seo:audit "website-url.com"

# Performance tracking
/analytics:report "organic traffic" "monthly"
```

## Configuration Files

### CLAUDE.md
Marketing-specific instructions for Claude Code. Defines:
- Marketing workflows and campaign lifecycle
- Agent coordination protocols
- Brand guidelines and messaging standards
- Marketing automation workflows

### .claude/agents/*.md
Individual marketing agent configurations defining:
- Agent expertise (SEO, email, content, etc.)
- Interaction patterns with other agents
- Output formats (campaigns, copy, reports)
- Quality standards and review criteria

### .claude/skills/*/
Marketing domain knowledge including:
- SEO mastery and keyword research
- Social media platform best practices
- Email marketing and deliverability
- Paid advertising strategies
- Content strategy frameworks
- Analytics and attribution models
- Brand building principles

## Best Practices

### Marketing Principles
- **Customer-First**: Always prioritize customer needs and pain points
- **Data-Driven**: Base decisions on metrics, analytics, and testing
- **Test & Learn**: Continuous experimentation and optimization
- **Brand Consistency**: Maintain voice, tone, and messaging alignment

### Content Quality
- All content goes through multi-perspective review (brand, SEO, conversion, personas)
- Comprehensive audience research before creation
- Brand voice and messaging consistency enforced
- Conversion optimization is built-in

### Campaign Management
- Clear goals and KPIs defined upfront
- Regular performance tracking and reporting
- A/B testing for continuous improvement
- Documentation of learnings and insights

### Documentation Standards
- Brand guidelines kept up-to-date
- Campaign playbooks maintained
- Marketing processes documented
- Knowledge shared across team

## Advanced Features

### Multi-Brand Support
- Manage multiple brands/clients simultaneously
- Shared marketing frameworks across brands
- Consistent campaign quality standards

### Custom Agent Creation
- Define brand-specific reviewer personas
- Extend existing marketing agent capabilities
- Create industry-specific expertise

### Integration Capabilities
- Discord/Telegram notifications for campaign updates
- Marketing automation platform integration
- Analytics and reporting dashboards

## Customization Guide

### 1. Brand Setup
- Update `CLAUDE.md` with brand specifics and workflows
- Create brand guidelines in `docs/brand-guidelines.md`
- Customize reviewer personas for your audience

### 2. Agent Specialization
- Add industry-specific knowledge to agents
- Create custom agents for unique marketing needs
- Configure multi-brand workflows

### 3. Workflow Optimization
- Define brand-specific slash commands
- Create shortcuts for recurring campaigns
- Establish content review standards

## Contributing

1. Fork this repository
2. Create a feature branch (`git checkout -b feature/marketing-enhancement`)
3. Follow marketing best practices and agent workflows
4. Ensure all content passes quality review (brand, SEO, conversion)
5. Update documentation and create a Pull Request

## License

This project is proprietary software. A commercial license is required for use. See the [LICENSE](LICENSE) file for details.

For licensing inquiries: [aitykit.cc](https://aitykit.cc)

## Learn More

### AityKit Resources
- [AityKit Website](https://aitykit.cc)
- [AityKit Documentation](https://docs.aitykit.cc)
- [AityKit CLI](https://github.com/mrgoonie/aitykit-cli)

### Claude Code Resources
- [Claude Code Documentation](https://claude.ai/code)
- [Claude Code Setup Guide](https://code.claude.com/docs/en/setup)
- [Model Context Protocol (MCP)](https://modelcontextprotocol.io)

### Community & Support
- [GitHub Issues](https://github.com/leduclinh7141/aitykit-marketing/issues)
- [GitHub Discussions](https://github.com/leduclinh7141/aitykit-marketing/discussions)
- [AityKit Blog](https://faafospecialist.substack.com)

---

**Start building AI-powered marketing campaigns today!**

This framework provides everything you need to create professional marketing campaigns with intelligent agent assistance.

---

*Copyright 2024-2025 AityKit Team. All Rights Reserved.*