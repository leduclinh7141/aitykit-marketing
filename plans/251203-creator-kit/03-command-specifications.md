# Part 3: Command Specifications

## 3.1 Command Structure

```
.claude/commands/
├── plan/
│   ├── ideas.md           # /plan:ideas
│   ├── calendar.md        # /plan:calendar
│   ├── trends.md          # /plan:trends
│   ├── pillars.md         # /plan:pillars
│   └── repurpose.md       # /plan:repurpose
├── write/
│   ├── script.md          # /write:script
│   ├── caption.md         # /write:caption
│   ├── hook.md            # /write:hook
│   ├── thread.md          # /write:thread
│   └── blog.md            # /write:blog
├── social/
│   ├── schedule.md        # /social:schedule
│   ├── hashtags.md        # /social:hashtags
│   ├── engage.md          # /social:engage
│   └── crosspost.md       # /social:crosspost
├── video/
│   ├── outline.md         # /video:outline
│   ├── thumbnail.md       # /video:thumbnail
│   ├── seo.md             # /video:seo
│   └── clips.md           # /video:clips
├── brand/
│   ├── mediakit.md        # /brand:mediakit
│   ├── pitch.md           # /brand:pitch
│   ├── rates.md           # /brand:rates
│   └── campaign.md        # /brand:campaign
└── analytics/
    ├── report.md          # /analytics:report
    ├── content.md         # /analytics:content
    ├── growth.md          # /analytics:growth
    └── compare.md         # /analytics:compare
```

---

## 3.2 Plan Commands

### /plan:ideas
```yaml
---
description: Generate content ideas for niche/topic
argument-hint: [niche] [platform] [quantity]
---
```

**Workflow:**
1. Analyze niche and audience
2. Research trending topics
3. Generate diverse ideas
4. Categorize by content type
5. Output idea bank

**Agent:** `content-planner`

---

### /plan:calendar
```yaml
---
description: Create content calendar
argument-hint: [period] [platforms] [frequency]
---
```

**Workflow:**
1. Define posting frequency
2. Map content pillars
3. Assign content types
4. Set optimal times
5. Output calendar

**Agent:** `content-planner`

---

### /plan:trends
```yaml
---
description: Analyze current trends for platform
argument-hint: [platform] [niche]
---
```

**Workflow:**
1. Scan platform trends
2. Identify relevant opportunities
3. Suggest content angles
4. Note timing urgency
5. Output trend report

**Agent:** `content-planner`

---

### /plan:pillars
```yaml
---
description: Define content pillars for brand
argument-hint: [niche] [goals]
---
```

**Workflow:**
1. Analyze brand/niche
2. Identify core themes
3. Define pillar categories
4. Create content ratios
5. Output pillar strategy

**Agent:** `content-planner`

---

### /plan:repurpose
```yaml
---
description: Create repurposing plan for content
argument-hint: [original-content] [target-platforms]
---
```

**Workflow:**
1. Analyze original content
2. Identify repurpose opportunities
3. Adapt for each platform
4. Create production checklist
5. Output repurpose plan

**Agent:** `content-planner`

---

## 3.3 Write Commands

### /write:script
```yaml
---
description: Write video/podcast script
argument-hint: [topic] [format] [duration]
---
```

**Workflow:**
1. Research topic
2. Structure content
3. Write hook
4. Develop body
5. Add CTA
6. Output script

**Agent:** `scriptwriter`

---

### /write:caption
```yaml
---
description: Write social media caption
argument-hint: [platform] [content-description]
---
```

**Workflow:**
1. Understand content context
2. Apply platform style
3. Write engaging copy
4. Add CTA
5. Output caption + hashtags

**Agent:** `scriptwriter`

---

### /write:hook
```yaml
---
description: Generate hooks/openers for content
argument-hint: [topic] [platform] [quantity]
---
```

**Workflow:**
1. Analyze topic angle
2. Apply hook formulas
3. Generate variations
4. Rank by impact
5. Output hook options

**Agent:** `scriptwriter`

---

### /write:thread
```yaml
---
description: Write Twitter/X thread
argument-hint: [topic] [angle]
---
```

**Workflow:**
1. Outline key points
2. Write hook tweet
3. Develop thread
4. Add engagement CTA
5. Output thread

**Agent:** `scriptwriter`

---

### /write:blog
```yaml
---
description: Write blog post/article
argument-hint: [topic] [keywords] [length]
---
```

**Workflow:**
1. Research topic
2. Structure outline
3. Write SEO-optimized content
4. Add headers, formatting
5. Output article

**Agent:** `scriptwriter`

---

## 3.4 Social Commands

### /social:schedule
```yaml
---
description: Create optimal posting schedule
argument-hint: [platforms] [content-types]
---
```

**Workflow:**
1. Analyze audience activity
2. Determine optimal times
3. Balance content types
4. Create weekly schedule
5. Output posting plan

**Agent:** `social-manager`

---

### /social:hashtags
```yaml
---
description: Generate hashtag strategy
argument-hint: [platform] [content-topic]
---
```

**Workflow:**
1. Research relevant hashtags
2. Mix reach levels
3. Check competitiveness
4. Create hashtag sets
5. Output hashtag strategy

**Agent:** `social-manager`

---

### /social:engage
```yaml
---
description: Generate engagement responses
argument-hint: [comment-type] [context]
---
```

**Workflow:**
1. Analyze comment context
2. Determine response type
3. Write authentic reply
4. Add engagement hook
5. Output response

**Agent:** `social-manager`

---

### /social:crosspost
```yaml
---
description: Adapt content for cross-posting
argument-hint: [original-content] [target-platform]
---
```

**Workflow:**
1. Analyze original content
2. Adapt for platform specs
3. Adjust caption/format
4. Optimize for platform
5. Output adapted content

**Agent:** `social-manager`

---

## 3.5 Video Commands

### /video:outline
```yaml
---
description: Create video structure/outline
argument-hint: [topic] [format] [duration]
---
```

**Workflow:**
1. Define video goal
2. Structure hook
3. Plan content beats
4. Include B-roll notes
5. Output outline

**Agent:** `video-producer`

---

### /video:thumbnail
```yaml
---
description: Generate thumbnail concepts
argument-hint: [video-topic] [style]
---
```

**Workflow:**
1. Analyze successful thumbnails
2. Generate concept ideas
3. Write text overlays
4. Suggest visual elements
5. Output thumbnail briefs

**Agent:** `video-producer`

---

### /video:seo
```yaml
---
description: Optimize video SEO (title, description, tags)
argument-hint: [video-topic] [keywords]
---
```

**Workflow:**
1. Research keywords
2. Write optimized title
3. Create description
4. Generate tags
5. Output SEO package

**Agent:** `video-producer`

---

### /video:clips
```yaml
---
description: Identify clip opportunities from long-form
argument-hint: [video-content] [target-platforms]
---
```

**Workflow:**
1. Analyze video content
2. Identify highlight moments
3. Suggest timestamps
4. Create clip hooks
5. Output clip plan

**Agent:** `video-producer`

---

## 3.6 Brand Commands

### /brand:mediakit
```yaml
---
description: Create/update media kit
argument-hint: [creator-info] [metrics]
---
```

**Workflow:**
1. Compile creator stats
2. Highlight achievements
3. Define audience
4. List offerings
5. Output media kit

**Agent:** `brand-liaison`

---

### /brand:pitch
```yaml
---
description: Write brand pitch/outreach
argument-hint: [brand] [partnership-type]
---
```

**Workflow:**
1. Research brand
2. Identify alignment
3. Craft pitch angle
4. Write outreach
5. Output pitch email

**Agent:** `brand-liaison`

---

### /brand:rates
```yaml
---
description: Calculate sponsorship rates
argument-hint: [metrics] [deliverables]
---
```

**Workflow:**
1. Analyze metrics
2. Research market rates
3. Calculate base rates
4. Adjust for factors
5. Output rate card

**Agent:** `brand-liaison`

---

### /brand:campaign
```yaml
---
description: Create branded content campaign concept
argument-hint: [brand] [product] [goals]
---
```

**Workflow:**
1. Understand brand goals
2. Develop creative concept
3. Plan content pieces
4. Define deliverables
5. Output campaign proposal

**Agent:** `brand-liaison`

---

## 3.7 Analytics Commands

### /analytics:report
```yaml
---
description: Generate performance report
argument-hint: [period] [platforms]
---
```

**Workflow:**
1. Gather metrics
2. Calculate trends
3. Identify highlights
4. Note areas to improve
5. Output report

**Agent:** `analytics-tracker`

---

### /analytics:content
```yaml
---
description: Analyze content performance
argument-hint: [content-set] [metrics]
---
```

**Workflow:**
1. Pull content metrics
2. Rank by performance
3. Identify patterns
4. Suggest optimizations
5. Output analysis

**Agent:** `analytics-tracker`

---

### /analytics:growth
```yaml
---
description: Analyze growth and opportunities
argument-hint: [platform] [period]
---
```

**Workflow:**
1. Track growth metrics
2. Identify growth drivers
3. Find opportunities
4. Recommend actions
5. Output growth report

**Agent:** `analytics-tracker`

---

### /analytics:compare
```yaml
---
description: Benchmark against competitors
argument-hint: [competitors] [metrics]
---
```

**Workflow:**
1. Gather competitor data
2. Compare metrics
3. Identify gaps
4. Note strengths
5. Output comparison

**Agent:** `analytics-tracker`

---

## 3.8 Command Quick Reference

| Command | Description | Agent |
|---------|-------------|-------|
| `/plan:ideas` | Content ideas | content-planner |
| `/plan:calendar` | Content calendar | content-planner |
| `/plan:trends` | Trend analysis | content-planner |
| `/plan:pillars` | Content pillars | content-planner |
| `/plan:repurpose` | Repurposing plan | content-planner |
| `/write:script` | Video/podcast script | scriptwriter |
| `/write:caption` | Social caption | scriptwriter |
| `/write:hook` | Hooks/openers | scriptwriter |
| `/write:thread` | Twitter thread | scriptwriter |
| `/write:blog` | Blog post | scriptwriter |
| `/social:schedule` | Posting schedule | social-manager |
| `/social:hashtags` | Hashtag strategy | social-manager |
| `/social:engage` | Engagement responses | social-manager |
| `/social:crosspost` | Cross-platform adapt | social-manager |
| `/video:outline` | Video structure | video-producer |
| `/video:thumbnail` | Thumbnail concepts | video-producer |
| `/video:seo` | Video SEO | video-producer |
| `/video:clips` | Clip extraction | video-producer |
| `/brand:mediakit` | Media kit | brand-liaison |
| `/brand:pitch` | Brand pitch | brand-liaison |
| `/brand:rates` | Rate calculation | brand-liaison |
| `/brand:campaign` | Campaign concept | brand-liaison |
| `/analytics:report` | Performance report | analytics-tracker |
| `/analytics:content` | Content analysis | analytics-tracker |
| `/analytics:growth` | Growth analysis | analytics-tracker |
| `/analytics:compare` | Competitor benchmark | analytics-tracker |
