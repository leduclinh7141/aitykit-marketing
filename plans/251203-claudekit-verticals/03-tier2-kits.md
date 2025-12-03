# Part 3: Tier 2 Kits (Medium Priority)

## Priority Criteria

- Market size $4-8B
- Growing adoption (30-50%)
- Clear use cases
- Moderate competition

---

## 3.1 ClaudeKit HR

**Target:** HR teams, recruiters, people ops, talent acquisition
**TAM:** $5B+
**Competition:** Paradox, Phenom, Eightfold

### Market Data

- HR leaders plan to redeploy 25% of workforce as AI takes routine tasks
- 30% productivity boost expected per employee
- Recruitment lifecycle most automated function

### Agent Architecture

| Agent | Function | Key Tasks |
|-------|----------|-----------|
| **recruiter** | Talent acquisition | Job posts, sourcing, screening, scheduling |
| **interviewer-prep** | Interview support | Question banks, scorecards, feedback |
| **onboarder** | New hire | Onboarding checklists, documentation, training |
| **policy-advisor** | HR compliance | Policy questions, handbook updates, compliance |
| **performance-coach** | Development | Reviews, goals, feedback, PIPs |
| **culture-curator** | Engagement | Surveys, recognition, event planning |

### Key Commands

```
/recruit:job-post [role]     - Create job posting
/recruit:source [role]       - Sourcing strategy
/recruit:screen [resume]     - Resume screening
/recruit:schedule [candidate]- Interview scheduling
/interview:questions [role]  - Interview questions
/interview:scorecard [role]  - Evaluation scorecard
/interview:feedback [notes]  - Structure feedback
/onboard:checklist [role]    - Onboarding checklist
/onboard:docs [employee]     - Generate onboarding docs
/onboard:buddy [employee]    - Buddy program setup
/policy:answer [question]    - Policy Q&A
/policy:update [section]     - Policy update draft
/performance:review [emp]    - Performance review draft
/performance:goals [emp]     - Goal setting
/culture:survey [type]       - Create engagement survey
/culture:recognize [emp]     - Recognition message
```

### Skills

```
talent-acquisition/
├── job-posting.md
├── sourcing-strategies.md
├── screening-criteria.md
└── interview-best-practices.md

hr-operations/
├── onboarding-processes.md
├── policy-management.md
├── compliance-requirements.md
└── documentation-standards.md

people-development/
├── performance-management.md
├── goal-frameworks.md
├── feedback-models.md
└── career-development.md
```

### MCP Integrations

- Greenhouse/Lever (ATS)
- Workday/BambooHR (HRIS)
- LinkedIn Recruiter (sourcing)
- Lattice/Culture Amp (performance)

---

## 3.2 ClaudeKit Education

**Target:** Teachers, instructional designers, L&D teams, coaches
**TAM:** $6B+ (37.2% CAGR through 2032)
**Competition:** MagicSchool, Cogniti, Disco

### Market Data

- 87% of institutions integrated AI tools
- Students using AI platforms score 12.4% higher
- 58% of instructors use generative AI daily
- 71% never used AI with students (training gap!)

### Agent Architecture

| Agent | Function | Key Tasks |
|-------|----------|-----------|
| **curriculum-designer** | Course design | Learning objectives, lesson plans, assessments |
| **content-creator** | Materials | Slides, handouts, activities, videos |
| **assessment-builder** | Evaluation | Quizzes, rubrics, grading, feedback |
| **tutor** | Student support | Explanations, practice, Q&A |
| **progress-tracker** | Analytics | Student progress, intervention alerts |
| **admin-assistant** | Operations | Scheduling, communication, reports |

### Key Commands

```
/curriculum:objectives [topic] - Learning objectives
/curriculum:plan [course]      - Course/lesson plan
/curriculum:sequence [topic]   - Learning sequence
/content:slides [topic]        - Create presentation
/content:handout [topic]       - Create handout
/content:activity [objective]  - Design activity
/content:video-script [topic]  - Video script
/assess:quiz [topic]           - Generate quiz
/assess:rubric [assignment]    - Create rubric
/assess:grade [submission]     - Grade with feedback
/assess:feedback [work]        - Detailed feedback
/tutor:explain [concept]       - Explain concept
/tutor:practice [skill]        - Practice problems
/tutor:answer [question]       - Answer student Q
/progress:report [student]     - Progress report
/progress:intervention [alert] - Intervention plan
/admin:schedule [class]        - Class scheduling
/admin:communicate [audience]  - Parent/student comms
```

### Skills

```
instructional-design/
├── learning-objectives.md
├── blooms-taxonomy.md
├── backward-design.md
└── universal-design.md

assessment/
├── formative-assessment.md
├── summative-assessment.md
├── rubric-design.md
└── feedback-strategies.md

pedagogy/
├── active-learning.md
├── differentiation.md
├── scaffolding.md
└── engagement-strategies.md
```

### MCP Integrations

- Canvas/Blackboard (LMS)
- Google Classroom (K-12)
- Notion/Confluence (knowledge base)
- Loom/Screencastify (video)

---

## 3.3 ClaudeKit Creator

**Target:** Content creators, YouTubers, podcasters, agencies
**TAM:** $4B+
**Competition:** Jasper, Copy.ai, Descript, Runway

### Market Data

- 41% of businesses used AI for video production in 2025
- "100x more content with 0 new hires" via AI factories
- Marketing teams matching output of 10x larger teams

### Agent Architecture

| Agent | Function | Key Tasks |
|-------|----------|-----------|
| **content-strategist** | Planning | Content calendar, topics, formats |
| **script-writer** | Scripts | Video scripts, podcast outlines, hooks |
| **copy-machine** | Short-form | Social posts, captions, threads |
| **thumbnail-designer** | Visuals | Thumbnail concepts, A/B variants |
| **seo-optimizer** | Discovery | Titles, descriptions, tags, keywords |
| **repurposer** | Distribution | Long→short, video→audio, multi-platform |

### Key Commands

```
/strategy:calendar [period]   - Content calendar
/strategy:topics [niche]      - Topic ideation
/strategy:series [theme]      - Content series plan
/script:youtube [topic]       - YouTube script
/script:podcast [topic]       - Podcast outline
/script:short [topic]         - Short-form script
/script:hook [content]        - Hook variations
/copy:thread [topic]          - Twitter/X thread
/copy:linkedin [topic]        - LinkedIn post
/copy:caption [content]       - Social caption
/copy:newsletter [topic]      - Newsletter draft
/thumbnail:concepts [video]   - Thumbnail ideas
/thumbnail:text [concept]     - Thumbnail text
/seo:title [content]          - Title optimization
/seo:description [content]    - Description
/seo:tags [content]           - Tags/keywords
/repurpose:clips [video]      - Clip suggestions
/repurpose:blog [video]       - Video to blog
/repurpose:social [content]   - Multi-platform versions
```

### Skills

```
content-creation/
├── storytelling.md
├── hook-formulas.md
├── script-structures.md
└── engagement-tactics.md

platform-optimization/
├── youtube-algorithm.md
├── podcast-discovery.md
├── social-algorithms.md
└── newsletter-growth.md

production/
├── video-editing.md
├── thumbnail-design.md
├── audio-production.md
└── repurposing-workflows.md
```

### MCP Integrations

- YouTube Studio (analytics)
- TubeBuddy/VidIQ (optimization)
- Canva (design)
- Descript (editing)
- Buffer/Later (scheduling)

---

## 3.4 ClaudeKit E-commerce

**Target:** Online stores, D2C brands, Shopify merchants
**TAM:** $8B+
**Competition:** Naratix, Shopify AI, Klevu

### Market Data

- E-commerce AI growing 30%+ annually
- Product catalog management highest ROI
- Conversion optimization key focus

### Agent Architecture

| Agent | Function | Key Tasks |
|-------|----------|-----------|
| **catalog-manager** | Products | Descriptions, attributes, categorization |
| **merchandiser** | Display | Collections, recommendations, search |
| **conversion-optimizer** | CRO | A/B tests, copy optimization, UX |
| **customer-support** | Service | FAQ, returns, order status |
| **inventory-analyst** | Operations | Forecasting, reorder, dead stock |
| **marketing-automator** | Campaigns | Email flows, ads, abandoned cart |

### Key Commands

```
/catalog:description [product] - Product description
/catalog:attributes [product]  - Extract attributes
/catalog:categorize [products] - Auto-categorization
/catalog:seo [product]         - Product SEO
/merch:collection [theme]      - Create collection
/merch:recommend [context]     - Recommendation rules
/merch:search [query]          - Search optimization
/cro:analyze [page]            - CRO analysis
/cro:copy [element]            - Copy optimization
/cro:test [hypothesis]         - A/B test design
/support:faq [topic]           - FAQ content
/support:response [inquiry]    - Customer response
/support:return [order]        - Return processing
/inventory:forecast [sku]      - Demand forecast
/inventory:reorder [category]  - Reorder recommendations
/marketing:flow [trigger]      - Email flow design
/marketing:cart [segment]      - Abandoned cart sequence
/marketing:ad [product]        - Ad copy for product
```

### Skills

```
ecommerce-fundamentals/
├── product-copywriting.md
├── conversion-optimization.md
├── customer-psychology.md
└── pricing-strategies.md

merchandising/
├── collection-curation.md
├── search-relevance.md
├── recommendation-engines.md
└── visual-merchandising.md

operations/
├── inventory-management.md
├── fulfillment.md
├── returns-management.md
└── customer-service.md
```

### MCP Integrations

- Shopify/WooCommerce (platform)
- Klaviyo/Mailchimp (email)
- Google Merchant Center (shopping)
- Gorgias/Zendesk (support)

---

## 3.5 Tier 2 Summary

| Kit | Agents | Commands | Skills | Target User |
|-----|--------|----------|--------|-------------|
| HR | 6 | 16 | 3 | HR teams, recruiters |
| Education | 6 | 18 | 3 | Teachers, L&D |
| Creator | 6 | 19 | 3 | YouTubers, podcasters |
| E-commerce | 6 | 18 | 3 | Online stores |

### Development Priority

1. **Creator** - High demand, clear differentiation
2. **E-commerce** - Large TAM, Shopify ecosystem
3. **Education** - Growing market, training gap
4. **HR** - Enterprise demand, complex workflows
