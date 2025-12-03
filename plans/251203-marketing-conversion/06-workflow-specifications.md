# Part 6: Workflow & Configuration Specifications

## 6.1 Primary Marketing Workflow

**File:** `.claude/workflows/primary-workflow.md`

```markdown
# Primary Marketing Workflow

## Marketing Automation Pipeline

Research → Insights → Creative → Plan → Create → Edit → Publish → Measure

### Phase 1: Research
- Delegate to `researcher` agent for market analysis
- Delegate to `attraction-specialist` for competitor intel
- Use `research` skill for methodology
- Output: Research reports in `./research/` directory

### Phase 2: Insights
- Delegate to `lead-qualifier` for audience analysis
- Synthesize research findings
- Identify opportunities and gaps
- Output: Insights summary

### Phase 3: Creative
- Delegate to `brainstormer` for ideation
- Delegate to `copywriter` for messaging concepts
- Use `content-strategy` skill
- Output: Creative brief

### Phase 4: Plan
- Delegate to `planner` agent for campaign planning
- Create content calendar
- Define KPIs and success metrics
- Output: Campaign plan in `./plans/`

### Phase 5: Create
- Delegate to `copywriter` for content creation
- Delegate to `email-wizard` for email sequences
- Delegate to `sales-enabler` for sales collateral
- Use `ai-multimodal` for visual content
- Output: Content assets

### Phase 6: Edit
- Review and optimize content
- A/B variant creation
- CRO optimization
- Output: Optimized content

### Phase 7: Publish
- Use MCP integrations for distribution
- Schedule across channels
- Coordinate launch timing
- Output: Published content

### Phase 8: Measure
- Gather performance data
- Delegate to analytics agents
- Calculate ROI and attribution
- Output: Performance reports

### Feedback Loop
- Insights from Measure feed back to Research
- Continuous optimization cycle
- Document learnings in `./docs/`
```

---

## 6.2 Marketing Rules

**File:** `.claude/workflows/marketing-rules.md`

```markdown
# Marketing Rules

## Content Quality Standards
- All copy must pass readability test (Grade 6-8 level)
- Headlines must follow 4-U formula (Useful, Unique, Urgent, Ultra-specific)
- CTAs must be action-oriented and specific
- No corporate jargon without purpose

## Brand Consistency
- Always check brand voice guidelines before writing
- Maintain consistent tone across channels
- Use approved brand assets only

## Compliance
- Include required disclaimers for regulated industries
- Follow platform-specific ad policies
- Respect data privacy regulations (GDPR, CCPA)

## Performance Standards
- Set measurable KPIs for all campaigns
- Track attribution across touchpoints
- Document learnings from all tests
```

---

## 6.3 Orchestration Protocol Updates

**File:** `.claude/workflows/orchestration-protocol.md`

```markdown
# Orchestration Protocol

## Sequential Chaining (Marketing)
- **Research → Insights → Creative**: Market understanding
- **Plan → Create → Edit**: Content production
- **Publish → Measure → Optimize**: Performance loop

## Parallel Execution (Marketing)
- **Multi-channel content**: Same message, platform-adapted
- **A/B variants**: Test versions created simultaneously
- **Campaign assets**: Copy + visuals + emails in parallel

## Agent Handoffs
| From | To | Trigger |
|------|-----|---------|
| researcher | attraction-specialist | SEO insights needed |
| attraction-specialist | copywriter | Content creation |
| copywriter | email-wizard | Email sequences |
| lead-qualifier | sales-enabler | MQL to SQL handoff |
| continuity-specialist | upsell-maximizer | Expansion ready |
```

---

## 6.4 Configuration Updates

### metadata.json
```json
{
  "version": "1.0.0",
  "name": "claudekit-marketing",
  "description": "AI-powered marketing automation kit with 6 specialized funnel-stage agents for lead generation, email campaigns, sales enablement, customer retention, and revenue optimization.",
  "buildDate": "2025-12-03T00:00:00.000Z",
  "repository": {
    "type": "git",
    "url": "https://github.com/claudekit/claudekit-marketing.git"
  }
}
```

### CLAUDE.md Updates

```markdown
# CLAUDE.md

## Role & Responsibilities

Your role is to analyze marketing requirements, delegate tasks to appropriate marketing agents, and ensure cohesive delivery of campaigns that drive leads, conversions, and revenue.

## Workflows

- Primary workflow: `./.claude/workflows/primary-workflow.md`
- Marketing rules: `./.claude/workflows/marketing-rules.md`
- Orchestration protocols: `./.claude/workflows/orchestration-protocol.md`

## Marketing Agents

- `attraction-specialist` - Lead generation & TOFU
- `lead-qualifier` - Intent detection & scoring
- `email-wizard` - Email campaign orchestration
- `sales-enabler` - Sales collateral creation
- `continuity-specialist` - Retention & engagement
- `upsell-maximizer` - Revenue expansion

## Skills Catalog

Activate relevant skills during tasks:
- `marketing-fundamentals` - Core marketing concepts
- `seo-mastery` - Search optimization
- `social-media` - Social strategies
- `email-marketing` - Email automation
- `paid-advertising` - Ad platform strategies
- `content-strategy` - Content planning
- `analytics-attribution` - Performance measurement
- `brand-building` - Brand strategy
```

### .mcp.json.example

```json
{
  "mcpServers": {
    "meta-ads": {
      "command": "npx",
      "args": ["-y", "@anthropic/mcp-meta-ads"],
      "env": { "META_ACCESS_TOKEN": "YOUR_TOKEN" }
    },
    "google-ads": {
      "command": "npx",
      "args": ["-y", "@anthropic/mcp-google-ads"],
      "env": { "GOOGLE_ADS_DEVELOPER_TOKEN": "YOUR_TOKEN" }
    },
    "google-analytics": {
      "command": "npx",
      "args": ["-y", "@anthropic/mcp-ga4"],
      "env": { "GA_PROPERTY_ID": "YOUR_PROPERTY_ID" }
    },
    "search-console": {
      "command": "npx",
      "args": ["-y", "@anthropic/mcp-gsc"],
      "env": { "GSC_SITE_URL": "YOUR_SITE_URL" }
    },
    "discord": {
      "command": "npx",
      "args": ["-y", "@anthropic/mcp-discord"],
      "env": { "DISCORD_BOT_TOKEN": "YOUR_TOKEN" }
    },
    "slack": {
      "command": "npx",
      "args": ["-y", "@anthropic/mcp-slack"],
      "env": { "SLACK_BOT_TOKEN": "YOUR_TOKEN" }
    },
    "stripe": {
      "command": "npx",
      "args": ["-y", "@anthropic/mcp-stripe"],
      "env": { "STRIPE_SECRET_KEY": "YOUR_KEY" }
    },
    "tiktok": {
      "command": "npx",
      "args": ["-y", "@anthropic/mcp-tiktok"],
      "env": { "TIKTOK_ACCESS_TOKEN": "YOUR_TOKEN" }
    },
    "meme-generator": {
      "command": "npx",
      "args": ["-y", "@anthropic/mcp-meme-gen"]
    }
  }
}
```
