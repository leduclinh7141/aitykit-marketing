# Part 3: Command Specifications

## 3.1 Command Structure

```
.claude/commands/
├── prospect/
│   ├── build.md          # /prospect:build
│   ├── enrich.md         # /prospect:enrich
│   ├── score.md          # /prospect:score
│   ├── icp.md            # /prospect:icp
│   └── territory.md      # /prospect:territory
├── outreach/
│   ├── sequence.md       # /outreach:sequence
│   ├── email.md          # /outreach:email
│   ├── linkedin.md       # /outreach:linkedin
│   ├── call.md           # /outreach:call
│   └── followup.md       # /outreach:followup
├── meeting/
│   ├── prep.md           # /meeting:prep
│   ├── agenda.md         # /meeting:agenda
│   ├── questions.md      # /meeting:questions
│   └── followup.md       # /meeting:followup
├── deal/
│   ├── score.md          # /deal:score
│   ├── risk.md           # /deal:risk
│   ├── forecast.md       # /deal:forecast
│   ├── pipeline.md       # /deal:pipeline
│   └── action.md         # /deal:action
├── proposal/
│   ├── create.md         # /proposal:create
│   ├── pricing.md        # /proposal:pricing
│   ├── roi.md            # /proposal:roi
│   └── battlecard.md     # /proposal:battlecard
└── handoff/
    ├── create.md         # /handoff:create
    ├── success.md        # /handoff:success
    └── expansion.md      # /handoff:expansion
```

---

## 3.2 Prospect Commands

### /prospect:build
```yaml
---
description: Build targeted prospect list based on criteria
argument-hint: [icp-criteria] [quantity]
---
```

**Workflow:**
1. Parse ICP criteria (industry, size, tech, etc.)
2. Search available data sources
3. Filter by criteria match
4. Score against ICP
5. Deduplicate and validate
6. Output prioritized list

**Agent:** `prospector`

**Output:** Prospect list with scores, sorted by priority

---

### /prospect:enrich
```yaml
---
description: Enrich prospect/account data from multiple sources
argument-hint: [prospect-list-or-account]
---
```

**Workflow:**
1. Identify data gaps
2. Query enrichment sources
3. Validate and merge data
4. Calculate completeness score
5. Output enriched records

**Agent:** `prospector`

---

### /prospect:score
```yaml
---
description: Score prospects against ICP criteria
argument-hint: [prospect-list] [icp-definition]
---
```

**Workflow:**
1. Load ICP definition
2. Evaluate each prospect
3. Score on each dimension
4. Calculate weighted total
5. Rank and segment

**Agent:** `prospector`

---

### /prospect:icp
```yaml
---
description: Define or refine ideal customer profile
argument-hint: [product-or-segment]
---
```

**Workflow:**
1. Analyze best customers (if data available)
2. Identify common characteristics
3. Define firmographic criteria
4. Define technographic criteria
5. Define behavioral signals
6. Output ICP document

**Agent:** `prospector`

---

### /prospect:territory
```yaml
---
description: Create territory plan and account allocation
argument-hint: [accounts] [reps]
---
```

**Workflow:**
1. Analyze account distribution
2. Calculate territory potential
3. Balance workload
4. Assign accounts to reps
5. Output territory plan

**Agent:** `prospector`

---

## 3.3 Outreach Commands

### /outreach:sequence
```yaml
---
description: Create multi-channel outreach sequence
argument-hint: [persona] [objective]
---
```

**Workflow:**
1. Define target persona
2. Select channels (email, LinkedIn, phone)
3. Create touch cadence
4. Write message templates
5. Add personalization tokens
6. Output complete sequence

**Agent:** `outreach-specialist`

**Output:** Full sequence with all touches, timing, templates

---

### /outreach:email
```yaml
---
description: Write personalized email for prospect
argument-hint: [prospect-info] [context]
---
```

**Workflow:**
1. Research prospect/account
2. Identify relevant hook
3. Craft personalized message
4. Apply best practices
5. Output email with subject line

**Agent:** `outreach-specialist`

---

### /outreach:linkedin
```yaml
---
description: Create LinkedIn message or connection request
argument-hint: [profile-url] [context]
---
```

**Workflow:**
1. Analyze LinkedIn profile
2. Find common ground
3. Craft appropriate message
4. Keep within character limits
5. Output message

**Agent:** `outreach-specialist`

**Types:** Connection request, InMail, direct message

---

### /outreach:call
```yaml
---
description: Generate call script and talking points
argument-hint: [prospect-info] [objective]
---
```

**Workflow:**
1. Research prospect/account
2. Define call objective
3. Create opening hook
4. Prepare key questions
5. Anticipate objections
6. Output call script

**Agent:** `outreach-specialist`

---

### /outreach:followup
```yaml
---
description: Create follow-up message after interaction
argument-hint: [interaction-type] [notes]
---
```

**Workflow:**
1. Parse interaction context
2. Identify key points to reinforce
3. Add value (resource, insight)
4. Include clear next step
5. Output follow-up message

**Agent:** `outreach-specialist`

---

## 3.4 Meeting Commands

### /meeting:prep
```yaml
---
description: Generate pre-meeting research brief
argument-hint: [account-or-contact] [meeting-type]
---
```

**Workflow:**
1. Research company thoroughly
2. Research attendees
3. Identify likely pain points
4. Gather competitive intel
5. Compile recent news/triggers
6. Output comprehensive brief

**Agent:** `meeting-prep`

---

### /meeting:agenda
```yaml
---
description: Create meeting agenda
argument-hint: [meeting-type] [objectives]
---
```

**Workflow:**
1. Define meeting objectives
2. Structure time blocks
3. Assign topics
4. Include discovery questions
5. Plan next steps discussion
6. Output shareable agenda

**Agent:** `meeting-prep`

**Types:** Discovery, demo, proposal review, negotiation, kick-off

---

### /meeting:questions
```yaml
---
description: Generate discovery questions for meeting
argument-hint: [context] [methodology]
---
```

**Workflow:**
1. Apply sales methodology (MEDDIC, BANT, etc.)
2. Customize for context
3. Prioritize questions
4. Add follow-up probes
5. Output question guide

**Agent:** `meeting-prep`

**Methodologies:** MEDDIC, BANT, SPIN, Challenger, GPCTBA/C&I

---

### /meeting:followup
```yaml
---
description: Create meeting follow-up and recap
argument-hint: [meeting-notes]
---
```

**Workflow:**
1. Summarize key discussion points
2. Document action items
3. Confirm next steps
4. Add relevant resources
5. Output follow-up email

**Agent:** `meeting-prep`

---

## 3.5 Deal Commands

### /deal:score
```yaml
---
description: Score deal and assess win probability
argument-hint: [opportunity-info]
---
```

**Workflow:**
1. Evaluate against methodology criteria
2. Assess stakeholder engagement
3. Check timeline/urgency
4. Review competitive position
5. Calculate probability score
6. Output score with rationale

**Agent:** `deal-analyst`

---

### /deal:risk
```yaml
---
description: Identify deal risks and mitigation strategies
argument-hint: [opportunity-info]
---
```

**Workflow:**
1. Analyze deal signals
2. Identify risk factors
3. Assess impact/likelihood
4. Recommend mitigations
5. Output risk report

**Agent:** `deal-analyst`

---

### /deal:forecast
```yaml
---
description: Generate pipeline forecast
argument-hint: [pipeline-data] [period]
---
```

**Workflow:**
1. Analyze pipeline by stage
2. Apply probability weights
3. Assess deal velocity
4. Factor historical conversion
5. Generate forecast ranges
6. Output forecast report

**Agent:** `deal-analyst`

---

### /deal:pipeline
```yaml
---
description: Analyze pipeline health and coverage
argument-hint: [pipeline-data]
---
```

**Workflow:**
1. Segment by stage
2. Calculate coverage ratio
3. Identify gaps
4. Analyze velocity
5. Output health report

**Agent:** `deal-analyst`

---

### /deal:action
```yaml
---
description: Recommend next best actions for deal
argument-hint: [opportunity-info]
---
```

**Workflow:**
1. Assess current deal state
2. Identify blockers
3. Determine optimal next steps
4. Prioritize actions
5. Output action plan

**Agent:** `deal-analyst`

---

## 3.6 Proposal Commands

### /proposal:create
```yaml
---
description: Generate sales proposal
argument-hint: [opportunity-info] [template]
---
```

**Workflow:**
1. Gather deal context
2. Select appropriate template
3. Customize value proposition
4. Include relevant case studies
5. Add pricing section
6. Output complete proposal

**Agent:** `proposal-writer`

---

### /proposal:pricing
```yaml
---
description: Create pricing configuration
argument-hint: [products] [requirements]
---
```

**Workflow:**
1. Identify required products/tiers
2. Apply discount rules
3. Calculate total investment
4. Structure payment terms
5. Output pricing table

**Agent:** `proposal-writer`

---

### /proposal:roi
```yaml
---
description: Create ROI analysis and business case
argument-hint: [customer-metrics] [solution]
---
```

**Workflow:**
1. Gather current state metrics
2. Project improvements
3. Calculate savings/revenue impact
4. Determine payback period
5. Output ROI document

**Agent:** `proposal-writer`

---

### /proposal:battlecard
```yaml
---
description: Generate competitive battlecard
argument-hint: [competitor] [context]
---
```

**Workflow:**
1. Research competitor
2. Identify key differentiators
3. Document common objections
4. Prepare counter-positioning
5. Output battlecard

**Agent:** `proposal-writer`

---

## 3.7 Handoff Commands

### /handoff:create
```yaml
---
description: Create sales-to-success handoff document
argument-hint: [opportunity-info]
---
```

**Workflow:**
1. Compile deal history
2. Document key stakeholders
3. Summarize success criteria
4. Note implementation requirements
5. Flag risks and opportunities
6. Output handoff package

**Agent:** `success-handoff`

---

### /handoff:success
```yaml
---
description: Create customer success plan
argument-hint: [customer-info] [goals]
---
```

**Workflow:**
1. Define success metrics
2. Set milestones
3. Assign responsibilities
4. Create check-in cadence
5. Output success plan

**Agent:** `success-handoff`

---

### /handoff:expansion
```yaml
---
description: Identify expansion opportunities
argument-hint: [account-info]
---
```

**Workflow:**
1. Analyze current usage/adoption
2. Identify whitespace
3. Map expansion triggers
4. Recommend approach
5. Output expansion plan

**Agent:** `success-handoff`

---

## 3.8 Command Quick Reference

| Command | Description | Agent |
|---------|-------------|-------|
| `/prospect:build` | Build prospect list | prospector |
| `/prospect:enrich` | Enrich data | prospector |
| `/prospect:score` | Score against ICP | prospector |
| `/prospect:icp` | Define ICP | prospector |
| `/prospect:territory` | Territory planning | prospector |
| `/outreach:sequence` | Create sequence | outreach-specialist |
| `/outreach:email` | Write email | outreach-specialist |
| `/outreach:linkedin` | LinkedIn message | outreach-specialist |
| `/outreach:call` | Call script | outreach-specialist |
| `/outreach:followup` | Follow-up message | outreach-specialist |
| `/meeting:prep` | Pre-meeting research | meeting-prep |
| `/meeting:agenda` | Meeting agenda | meeting-prep |
| `/meeting:questions` | Discovery questions | meeting-prep |
| `/meeting:followup` | Meeting recap | meeting-prep |
| `/deal:score` | Deal scoring | deal-analyst |
| `/deal:risk` | Risk analysis | deal-analyst |
| `/deal:forecast` | Pipeline forecast | deal-analyst |
| `/deal:pipeline` | Pipeline health | deal-analyst |
| `/deal:action` | Next best action | deal-analyst |
| `/proposal:create` | Create proposal | proposal-writer |
| `/proposal:pricing` | Pricing config | proposal-writer |
| `/proposal:roi` | ROI analysis | proposal-writer |
| `/proposal:battlecard` | Competitive battlecard | proposal-writer |
| `/handoff:create` | Handoff document | success-handoff |
| `/handoff:success` | Success plan | success-handoff |
| `/handoff:expansion` | Expansion plan | success-handoff |
