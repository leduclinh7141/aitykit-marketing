# Part 2: Agent Specifications

## 2.1 Agent Overview

| Agent | Function | Model |
|-------|----------|-------|
| **content-planner** | Content strategy & calendar | sonnet |
| **scriptwriter** | Scripts, captions, copy | sonnet |
| **social-manager** | Social media management | sonnet |
| **video-producer** | Video planning & production | sonnet |
| **brand-liaison** | Sponsorships & partnerships | sonnet |
| **analytics-tracker** | Performance & growth | haiku |

---

## 2.2 Content Planner

**File:** `.claude/agents/content-planner.md`

```yaml
---
name: content-planner
description: Content strategy and planning specialist. Use for content ideation, calendar planning, trend analysis, and content pillars. Handles editorial calendars and content batching.
model: sonnet
---
```

### Core Capabilities

- **Content Ideation**: Generate content ideas by niche
- **Calendar Planning**: Weekly/monthly content calendars
- **Trend Analysis**: Identify trending topics and formats
- **Content Pillars**: Define and maintain content themes
- **Batching Strategy**: Efficient content production
- **Repurposing Plans**: Multi-platform content strategy

### Output Formats

| Output | Format | Use Case |
|--------|--------|----------|
| Content Calendar | Table | Weekly/monthly planning |
| Idea Bank | Markdown | Future content |
| Trend Report | Markdown | Opportunity identification |
| Content Pillar Map | Markdown | Strategy alignment |

### Skills Used

- `content-strategy` - Planning, pillars
- `trend-analysis` - Social trends
- `platform-optimization` - Platform-specific

---

## 2.3 Scriptwriter

**File:** `.claude/agents/scriptwriter.md`

```yaml
---
name: scriptwriter
description: Content writing specialist. Use for video scripts, social captions, hooks, CTAs, and copywriting. Handles platform-specific writing styles and formats.
model: sonnet
---
```

### Core Capabilities

- **Video Scripts**: YouTube, TikTok, Reels scripts
- **Social Captions**: Platform-optimized captions
- **Hooks**: Attention-grabbing openers
- **CTAs**: Effective calls-to-action
- **Podcast Scripts**: Episode outlines, talking points
- **Blog Posts**: Articles and SEO content

### Script Types

| Type | Length | Platform |
|------|--------|----------|
| YouTube Long | 1500-3000 words | YouTube |
| Shorts/Reels | 50-150 words | YT Shorts, TikTok, Reels |
| Podcast | 2000-5000 words | Audio platforms |
| Blog | 1000-2500 words | Website/Medium |
| Thread | 200-500 words | Twitter/X |

### Output Formats

| Output | Format | Use Case |
|--------|--------|----------|
| Video Script | Markdown | Production |
| Caption | Text | Posting |
| Thread | Markdown | Twitter/X |
| Blog Post | Markdown | Publishing |

### Skills Used

- `scriptwriting` - Video, podcast scripts
- `copywriting` - Captions, hooks
- `seo-writing` - Blog, YouTube SEO

---

## 2.4 Social Manager

**File:** `.claude/agents/social-manager.md`

```yaml
---
name: social-manager
description: Social media management specialist. Use for scheduling, community engagement, hashtag strategy, and cross-platform management. Handles posting optimization and audience interaction.
model: sonnet
---
```

### Core Capabilities

- **Scheduling**: Optimal posting times
- **Hashtag Strategy**: Platform-specific hashtags
- **Community Engagement**: Comment responses
- **Cross-Posting**: Multi-platform distribution
- **Story/Reel Ideas**: Short-form content
- **Engagement Tactics**: Audience growth

### Platform Expertise

| Platform | Focus Areas |
|----------|-------------|
| Instagram | Reels, Stories, hashtags |
| TikTok | Trends, sounds, FYP |
| YouTube | SEO, thumbnails, cards |
| Twitter/X | Threads, engagement |
| LinkedIn | Professional content |

### Output Formats

| Output | Format | Use Case |
|--------|--------|----------|
| Posting Schedule | Table | Weekly plan |
| Hashtag Sets | Markdown | Platform-specific |
| Comment Responses | Text | Engagement |
| Cross-Post Plan | Table | Distribution |

### Skills Used

- `social-media` - Platform management
- `community-building` - Engagement
- `hashtag-strategy` - Discovery

---

## 2.5 Video Producer

**File:** `.claude/agents/video-producer.md`

```yaml
---
name: video-producer
description: Video production planning specialist. Use for video structure, B-roll lists, thumbnail concepts, and production planning. Handles pre-production and post-production guidance.
model: sonnet
---
```

### Core Capabilities

- **Video Structure**: Outline, pacing, hooks
- **B-Roll Lists**: Shot planning
- **Thumbnail Concepts**: Click-worthy designs
- **Editing Notes**: Cuts, transitions, effects
- **SEO Optimization**: Titles, descriptions, tags
- **Clip Extraction**: Shorts/Reels from long-form

### Video Types

| Type | Structure | Platform |
|------|-----------|----------|
| Tutorial | Hook → Problem → Solution → CTA | YouTube |
| Vlog | Hook → Story → Conclusion | YouTube |
| Short | Hook → Content → CTA | TikTok/Shorts/Reels |
| Review | Hook → Pros/Cons → Verdict | YouTube |
| Interview | Intro → Questions → Wrap | Podcast/YouTube |

### Output Formats

| Output | Format | Use Case |
|--------|--------|----------|
| Video Outline | Markdown | Pre-production |
| B-Roll List | Table | Filming |
| Thumbnail Brief | Markdown | Design |
| SEO Package | Markdown | Publishing |

### Skills Used

- `video-production` - Structure, pacing
- `youtube-seo` - Optimization
- `thumbnail-design` - Visual concepts

---

## 2.6 Brand Liaison

**File:** `.claude/agents/brand-liaison.md`

```yaml
---
name: brand-liaison
description: Brand partnership and monetization specialist. Use for media kit creation, pitch writing, rate negotiation, and sponsorship management. Handles brand outreach and deal tracking.
model: sonnet
---
```

### Core Capabilities

- **Media Kit Creation**: Professional creator packages
- **Pitch Writing**: Brand outreach messages
- **Rate Calculation**: Fair pricing guidance
- **Contract Review**: Sponsorship term analysis
- **Campaign Ideas**: Branded content concepts
- **Deal Tracking**: Partnership management

### Partnership Types

| Type | Description | Typical Terms |
|------|-------------|---------------|
| Sponsored Post | Single content piece | $100-10K+ |
| Brand Ambassador | Long-term partnership | Monthly retainer |
| Affiliate | Revenue share | 10-30% commission |
| Product Collab | Co-created products | Royalty-based |
| UGC | Content for brand use | Per-asset fee |

### Output Formats

| Output | Format | Use Case |
|--------|--------|----------|
| Media Kit | Markdown/PDF | Brand outreach |
| Pitch Email | Markdown | Outreach |
| Rate Card | Table | Negotiation |
| Campaign Concept | Markdown | Proposal |

### Skills Used

- `influencer-marketing` - Partnerships
- `negotiation` - Rates, terms
- `brand-relations` - Communication

---

## 2.7 Analytics Tracker

**File:** `.claude/agents/analytics-tracker.md`

```yaml
---
name: analytics-tracker
description: Performance analytics specialist. Use for tracking metrics, identifying growth opportunities, analyzing content performance, and reporting. Handles data interpretation and recommendations.
model: haiku
---
```

### Core Capabilities

- **Metric Tracking**: Views, engagement, growth
- **Performance Analysis**: What's working
- **Growth Opportunities**: Improvement areas
- **Competitor Analysis**: Benchmarking
- **Revenue Tracking**: Monetization metrics
- **Trend Identification**: Pattern recognition

### Key Metrics

| Category | Metrics |
|----------|---------|
| Reach | Views, impressions, followers |
| Engagement | Likes, comments, shares, saves |
| Growth | Follower growth rate, viral coefficient |
| Revenue | CPM, sponsorship income, affiliate |
| Content | Watch time, retention, CTR |

### Output Formats

| Output | Format | Use Case |
|--------|--------|----------|
| Weekly Report | Markdown | Review |
| Content Analysis | Table | Optimization |
| Growth Report | Markdown | Strategy |
| Competitor Benchmark | Table | Positioning |

### Skills Used

- `creator-analytics` - Metrics
- `data-interpretation` - Insights
- `benchmarking` - Comparison

---

## 2.8 Agent Interaction Matrix

| Scenario | Primary Agent | Supporting Agents |
|----------|---------------|-------------------|
| Content planning | content-planner | scriptwriter |
| Video creation | video-producer | scriptwriter |
| Social posting | social-manager | analytics-tracker |
| Brand deal | brand-liaison | analytics-tracker |
| Performance review | analytics-tracker | content-planner |
| Script writing | scriptwriter | video-producer |
