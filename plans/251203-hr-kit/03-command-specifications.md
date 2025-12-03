# Part 3: Command Specifications

## 3.1 Command Structure

```
.claude/commands/
├── recruit/
│   ├── job.md             # /recruit:job
│   ├── source.md          # /recruit:source
│   ├── screen.md          # /recruit:screen
│   ├── outreach.md        # /recruit:outreach
│   └── pipeline.md        # /recruit:pipeline
├── interview/
│   ├── schedule.md        # /interview:schedule
│   ├── prep.md            # /interview:prep
│   ├── questions.md       # /interview:questions
│   ├── feedback.md        # /interview:feedback
│   └── offer.md           # /interview:offer
├── onboard/
│   ├── checklist.md       # /onboard:checklist
│   ├── training.md        # /onboard:training
│   ├── plan.md            # /onboard:plan
│   └── docs.md            # /onboard:docs
├── analytics/
│   ├── headcount.md       # /analytics:headcount
│   ├── turnover.md        # /analytics:turnover
│   ├── recruiting.md      # /analytics:recruiting
│   └── compensation.md    # /analytics:compensation
├── compliance/
│   ├── policy.md          # /compliance:policy
│   ├── audit.md           # /compliance:audit
│   ├── handbook.md        # /compliance:handbook
│   └── report.md          # /compliance:report
└── support/
    ├── faq.md             # /support:faq
    ├── benefits.md        # /support:benefits
    ├── pto.md             # /support:pto
    └── ticket.md          # /support:ticket
```

---

## 3.2 Recruit Commands

### /recruit:job
```yaml
---
description: Create or optimize job description
argument-hint: [role-title] [requirements]
---
```

**Workflow:**
1. Gather role requirements
2. Research market comparables
3. Write compelling job description
4. Optimize for SEO/searchability
5. Add inclusive language
6. Output job posting

**Agent:** `talent-sourcer`

---

### /recruit:source
```yaml
---
description: Source candidates for open role
argument-hint: [job-id] [sources]
---
```

**Workflow:**
1. Parse job requirements
2. Build Boolean search strings
3. Search specified sources
4. Deduplicate candidates
5. Initial scoring
6. Output candidate list

**Agent:** `talent-sourcer`

---

### /recruit:screen
```yaml
---
description: Screen candidates against requirements
argument-hint: [candidates] [criteria]
---
```

**Workflow:**
1. Parse resumes/profiles
2. Extract skills and experience
3. Match against requirements
4. Score and rank candidates
5. Generate screening notes
6. Output ranked list

**Agent:** `talent-sourcer`

---

### /recruit:outreach
```yaml
---
description: Create recruiting outreach message
argument-hint: [candidate-info] [role]
---
```

**Workflow:**
1. Research candidate background
2. Identify personalization hooks
3. Craft compelling message
4. Include role highlights
5. Output outreach message

**Agent:** `talent-sourcer`

---

### /recruit:pipeline
```yaml
---
description: Generate pipeline status report
argument-hint: [role-or-all] [period]
---
```

**Workflow:**
1. Pull pipeline data
2. Segment by stage
3. Calculate conversion rates
4. Identify bottlenecks
5. Output pipeline report

**Agent:** `talent-sourcer`

---

## 3.3 Interview Commands

### /interview:schedule
```yaml
---
description: Schedule interview with candidate
argument-hint: [candidate] [interviewers] [type]
---
```

**Workflow:**
1. Check interviewer availability
2. Check candidate availability
3. Find optimal slot
4. Send calendar invites
5. Output confirmation

**Agent:** `interview-coordinator`

---

### /interview:prep
```yaml
---
description: Prepare interviewer for candidate
argument-hint: [candidate] [interviewer] [interview-type]
---
```

**Workflow:**
1. Compile candidate background
2. Review job requirements
3. Generate focus areas
4. Create scorecard
5. Output prep package

**Agent:** `interview-coordinator`

---

### /interview:questions
```yaml
---
description: Generate interview questions
argument-hint: [role] [interview-type] [competencies]
---
```

**Workflow:**
1. Identify key competencies
2. Select question framework
3. Generate role-specific questions
4. Add follow-up probes
5. Output question guide

**Agent:** `interview-coordinator`

**Types:** behavioral, technical, situational, culture-fit

---

### /interview:feedback
```yaml
---
description: Collect and summarize interview feedback
argument-hint: [candidate] [interview-round]
---
```

**Workflow:**
1. Gather interviewer feedback
2. Synthesize scores and notes
3. Identify consensus/concerns
4. Generate recommendation
5. Output feedback summary

**Agent:** `interview-coordinator`

---

### /interview:offer
```yaml
---
description: Generate offer letter
argument-hint: [candidate] [compensation] [terms]
---
```

**Workflow:**
1. Pull candidate details
2. Apply compensation package
3. Include benefits summary
4. Add contingencies
5. Output offer letter

**Agent:** `interview-coordinator`

---

## 3.4 Onboard Commands

### /onboard:checklist
```yaml
---
description: Create onboarding checklist for new hire
argument-hint: [new-hire] [role] [start-date]
---
```

**Workflow:**
1. Identify role requirements
2. Generate preboarding tasks
3. Create day 1 checklist
4. Add week 1 activities
5. Output full checklist

**Agent:** `onboarding-specialist`

---

### /onboard:training
```yaml
---
description: Create training plan for new hire
argument-hint: [role] [level]
---
```

**Workflow:**
1. Identify required skills
2. Map to training resources
3. Create learning path
4. Set milestones
5. Output training plan

**Agent:** `onboarding-specialist`

---

### /onboard:plan
```yaml
---
description: Create 30-60-90 day plan
argument-hint: [role] [goals]
---
```

**Workflow:**
1. Define 30-day goals (learn)
2. Define 60-day goals (contribute)
3. Define 90-day goals (own)
4. Add success metrics
5. Output 30-60-90 plan

**Agent:** `onboarding-specialist`

---

### /onboard:docs
```yaml
---
description: Generate onboarding documentation request
argument-hint: [new-hire] [requirements]
---
```

**Workflow:**
1. Identify required documents
2. Generate collection checklist
3. Create submission instructions
4. Track completion status
5. Output document request

**Agent:** `onboarding-specialist`

---

## 3.5 Analytics Commands

### /analytics:headcount
```yaml
---
description: Generate headcount report
argument-hint: [scope] [period]
---
```

**Workflow:**
1. Pull headcount data
2. Segment by department/location
3. Calculate growth rates
4. Compare to plan
5. Output headcount report

**Agent:** `hr-analyst`

---

### /analytics:turnover
```yaml
---
description: Analyze turnover and retention
argument-hint: [period] [segments]
---
```

**Workflow:**
1. Calculate turnover rates
2. Segment by type (vol/invol)
3. Identify risk factors
4. Benchmark against industry
5. Output turnover analysis

**Agent:** `hr-analyst`

---

### /analytics:recruiting
```yaml
---
description: Generate recruiting metrics report
argument-hint: [period] [roles]
---
```

**Workflow:**
1. Pull recruiting funnel data
2. Calculate key metrics
3. Analyze source effectiveness
4. Identify bottlenecks
5. Output recruiting report

**Agent:** `hr-analyst`

---

### /analytics:compensation
```yaml
---
description: Analyze compensation and pay equity
argument-hint: [scope] [benchmarks]
---
```

**Workflow:**
1. Pull compensation data
2. Calculate compa-ratios
3. Analyze pay equity
4. Compare to market
5. Output comp analysis

**Agent:** `hr-analyst`

---

## 3.6 Compliance Commands

### /compliance:policy
```yaml
---
description: Create or update HR policy
argument-hint: [policy-type] [requirements]
---
```

**Workflow:**
1. Research requirements
2. Draft policy content
3. Add procedures
4. Include acknowledgment
5. Output policy document

**Agent:** `compliance-officer`

---

### /compliance:audit
```yaml
---
description: Conduct HR compliance audit
argument-hint: [audit-type] [scope]
---
```

**Workflow:**
1. Define audit scope
2. Pull relevant records
3. Check against requirements
4. Identify gaps
5. Output audit report

**Agent:** `compliance-officer`

---

### /compliance:handbook
```yaml
---
description: Update employee handbook section
argument-hint: [section] [changes]
---
```

**Workflow:**
1. Review current content
2. Apply required updates
3. Ensure legal compliance
4. Version control
5. Output updated section

**Agent:** `compliance-officer`

---

### /compliance:report
```yaml
---
description: Generate compliance report (EEO-1, etc.)
argument-hint: [report-type] [period]
---
```

**Workflow:**
1. Pull employee data
2. Categorize per requirements
3. Calculate statistics
4. Format for submission
5. Output compliance report

**Agent:** `compliance-officer`

---

## 3.7 Support Commands

### /support:faq
```yaml
---
description: Answer employee HR question
argument-hint: [question]
---
```

**Workflow:**
1. Parse employee question
2. Search knowledge base
3. Find relevant policy
4. Generate clear answer
5. Output response

**Agent:** `employee-support`

---

### /support:benefits
```yaml
---
description: Provide benefits information
argument-hint: [benefit-type] [question]
---
```

**Workflow:**
1. Identify benefit plan
2. Pull plan details
3. Answer specific question
4. Include enrollment info
5. Output benefits response

**Agent:** `employee-support`

---

### /support:pto
```yaml
---
description: Handle PTO inquiry or request
argument-hint: [employee] [action]
---
```

**Workflow:**
1. Pull employee PTO data
2. Check balance/accruals
3. Process request if applicable
4. Check policy compliance
5. Output PTO response

**Agent:** `employee-support`

---

### /support:ticket
```yaml
---
description: Create HR support ticket
argument-hint: [issue] [priority]
---
```

**Workflow:**
1. Categorize issue
2. Assess priority
3. Route to appropriate team
4. Create ticket
5. Output confirmation

**Agent:** `employee-support`

---

## 3.8 Command Quick Reference

| Command | Description | Agent |
|---------|-------------|-------|
| `/recruit:job` | Create job description | talent-sourcer |
| `/recruit:source` | Source candidates | talent-sourcer |
| `/recruit:screen` | Screen candidates | talent-sourcer |
| `/recruit:outreach` | Recruiting outreach | talent-sourcer |
| `/recruit:pipeline` | Pipeline report | talent-sourcer |
| `/interview:schedule` | Schedule interview | interview-coordinator |
| `/interview:prep` | Interviewer prep | interview-coordinator |
| `/interview:questions` | Interview questions | interview-coordinator |
| `/interview:feedback` | Feedback summary | interview-coordinator |
| `/interview:offer` | Generate offer | interview-coordinator |
| `/onboard:checklist` | Onboarding checklist | onboarding-specialist |
| `/onboard:training` | Training plan | onboarding-specialist |
| `/onboard:plan` | 30-60-90 plan | onboarding-specialist |
| `/onboard:docs` | Document collection | onboarding-specialist |
| `/analytics:headcount` | Headcount report | hr-analyst |
| `/analytics:turnover` | Turnover analysis | hr-analyst |
| `/analytics:recruiting` | Recruiting metrics | hr-analyst |
| `/analytics:compensation` | Comp analysis | hr-analyst |
| `/compliance:policy` | Policy creation | compliance-officer |
| `/compliance:audit` | Compliance audit | compliance-officer |
| `/compliance:handbook` | Handbook update | compliance-officer |
| `/compliance:report` | Compliance report | compliance-officer |
| `/support:faq` | Answer HR question | employee-support |
| `/support:benefits` | Benefits info | employee-support |
| `/support:pto` | PTO inquiry | employee-support |
| `/support:ticket` | Create HR ticket | employee-support |
