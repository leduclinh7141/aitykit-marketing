# Part 5: Workflow & Configuration Specifications

## 5.1 Primary Creator Workflow

**File:** `.claude/workflows/primary-workflow.md`

```markdown
# Primary Creator Workflow

## Content Creation Cycle

Plan → Write → Produce → Publish → Engage → Analyze → Monetize

### Phase 1: Plan
- Delegate to `content-planner` for strategy
- Use `content-strategy` skill
- Output: Content calendar, ideas

### Phase 2: Write
- Delegate to `scriptwriter` for content
- Use `creator-writing` skill
- Output: Scripts, captions, copy

### Phase 3: Produce
- Delegate to `video-producer` for video
- Use `video-production` skill
- Output: Video outlines, thumbnails, SEO

### Phase 4: Publish
- Delegate to `social-manager` for distribution
- Use `social-media` skill
- Output: Scheduled posts, hashtags

### Phase 5: Engage
- Delegate to `social-manager` for community
- Respond to comments, build relationships
- Output: Engaged community

### Phase 6: Analyze
- Delegate to `analytics-tracker` for insights
- Track performance, identify patterns
- Output: Performance reports

### Phase 7: Monetize
- Delegate to `brand-liaison` for partnerships
- Use `creator-business` skill
- Output: Brand deals, revenue
```

---

## 5.2 Creator Rules

**File:** `.claude/workflows/creator-rules.md`

```markdown
# Creator Rules

## Content Standards
- Maintain authentic voice and brand
- Disclose sponsored content (FTC)
- Respect copyright and fair use
- Create original, valuable content

## Platform Standards
- Follow community guidelines
- Optimize for each platform's format
- Post consistently
- Engage authentically

## Brand Partnership Standards
- Only partner with aligned brands
- Deliver on commitments
- Disclose all sponsorships
- Maintain creative control

## Audience Standards
- Prioritize audience value
- Respond to community
- Handle criticism professionally
- Protect audience trust

## Business Standards
- Track all income/expenses
- Honor contracts
- Diversify revenue streams
- Plan for sustainability
```

---

## 5.3 Orchestration Protocol

**File:** `.claude/workflows/orchestration-protocol.md`

```markdown
# Creator Agent Orchestration

## Sequential Workflows

### Content Production Flow
content-planner → scriptwriter → video-producer → social-manager
1. Plan content ideas and calendar
2. Write scripts and captions
3. Create production assets
4. Schedule and publish

### Brand Deal Flow
brand-liaison → scriptwriter → video-producer → analytics-tracker
1. Negotiate and plan campaign
2. Write branded content
3. Produce deliverables
4. Report on performance

## Parallel Workflows

### Weekly Content Batch
- content-planner: Week's content plan
- scriptwriter: All scripts for week
- video-producer: All thumbnails/outlines
→ Complete content package

### Monthly Review
- analytics-tracker: Performance analysis
- content-planner: Strategy adjustment
- brand-liaison: Partnership opportunities
→ Monthly strategy update

## Agent Handoffs

| Trigger | From | To |
|---------|------|-----|
| Ideas approved | content-planner | scriptwriter |
| Script complete | scriptwriter | video-producer |
| Video ready | video-producer | social-manager |
| Published | social-manager | analytics-tracker |
| Performance data | analytics-tracker | content-planner |
| Brand interest | analytics-tracker | brand-liaison |
```

---

## 5.4 Configuration Files

### metadata.json

```json
{
  "version": "1.0.0",
  "name": "claudekit-creator",
  "description": "AI-powered creator kit with specialized agents for content planning, scriptwriting, social media, video production, brand partnerships, and analytics.",
  "buildDate": "2025-12-03T00:00:00.000Z",
  "repository": {
    "type": "git",
    "url": "https://github.com/claudekit/claudekit-creator.git"
  }
}
```

### CLAUDE.md

```markdown
# CLAUDE.md

## Role & Responsibilities

Your role is to assist content creators with planning, writing, production, publishing, and monetization while maintaining authenticity and audience trust.

## Workflows

- Primary workflow: `./.claude/workflows/primary-workflow.md`
- Creator rules: `./.claude/workflows/creator-rules.md`
- Orchestration: `./.claude/workflows/orchestration-protocol.md`

## Creator Agents

- `content-planner` - Strategy & calendar
- `scriptwriter` - Scripts & copy
- `social-manager` - Social media
- `video-producer` - Video production
- `brand-liaison` - Partnerships
- `analytics-tracker` - Performance

## Skills Catalog

- `content-strategy` - Planning, pillars
- `creator-writing` - Scripts, captions
- `social-media` - Platforms, engagement
- `video-production` - Video, thumbnails
- `creator-business` - Monetization, brands
```

### .mcp.json.example

```json
{
  "mcpServers": {
    "youtube": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-youtube"],
      "env": { "YOUTUBE_API_KEY": "YOUR_KEY" }
    },
    "instagram": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-instagram"],
      "env": { "INSTAGRAM_ACCESS_TOKEN": "YOUR_TOKEN" }
    },
    "tiktok": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-tiktok"],
      "env": { "TIKTOK_ACCESS_TOKEN": "YOUR_TOKEN" }
    },
    "twitter": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-twitter"],
      "env": { "TWITTER_API_KEY": "YOUR_KEY" }
    },
    "linkedin": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-linkedin"],
      "env": { "LINKEDIN_ACCESS_TOKEN": "YOUR_TOKEN" }
    },
    "canva": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-canva"],
      "env": { "CANVA_API_KEY": "YOUR_KEY" }
    },
    "google-drive": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-google-drive"],
      "env": { "GOOGLE_CREDENTIALS": "YOUR_CREDS" }
    },
    "notion": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-notion"],
      "env": { "NOTION_API_KEY": "YOUR_KEY" }
    },
    "buffer": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-buffer"],
      "env": { "BUFFER_ACCESS_TOKEN": "YOUR_TOKEN" }
    },
    "discord": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-discord"],
      "env": { "DISCORD_BOT_TOKEN": "YOUR_TOKEN" }
    },
    "patreon": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-patreon"],
      "env": { "PATREON_ACCESS_TOKEN": "YOUR_TOKEN" }
    },
    "social-blade": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-socialblade"],
      "env": { "SOCIALBLADE_API_KEY": "YOUR_KEY" }
    },
    "descript": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-descript"],
      "env": { "DESCRIPT_API_KEY": "YOUR_KEY" }
    },
    "anchor": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-anchor"],
      "env": { "ANCHOR_API_KEY": "YOUR_KEY" }
    }
  }
}
```

---

## 5.5 MCP Integration Summary

| Integration | Purpose | Priority |
|-------------|---------|----------|
| YouTube | Video platform | HIGH |
| Instagram | Social platform | HIGH |
| TikTok | Short-form video | HIGH |
| Twitter/X | Social platform | MEDIUM |
| LinkedIn | Professional content | MEDIUM |
| Canva | Design | HIGH |
| Google Drive | Storage | HIGH |
| Notion | Planning | MEDIUM |
| Buffer | Scheduling | MEDIUM |
| Discord | Community | MEDIUM |
| Patreon | Monetization | LOW |
| Social Blade | Analytics | LOW |
| Descript | Video/podcast | MEDIUM |
| Anchor | Podcasting | LOW |
