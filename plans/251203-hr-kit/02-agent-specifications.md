# Part 2: Agent Specifications

## 2.1 Agent Overview

| Agent | Function | Model |
|-------|----------|-------|
| **talent-sourcer** | Candidate sourcing & screening | sonnet |
| **interview-coordinator** | Interview scheduling & prep | sonnet |
| **onboarding-specialist** | New hire onboarding | sonnet |
| **hr-analyst** | People analytics & reporting | sonnet |
| **compliance-officer** | HR compliance & policies | sonnet |
| **employee-support** | Employee inquiries & self-service | haiku |

---

## 2.2 Talent Sourcer

**File:** `.claude/agents/talent-sourcer.md`

```yaml
---
name: talent-sourcer
description: Recruiting and talent acquisition specialist. Use for job posting optimization, candidate sourcing, resume screening, skills matching, and pipeline management. Handles Boolean searches, outreach sequences, and candidate scoring.
model: sonnet
---
```

### Core Capabilities

- **Job Posting**: Write and optimize job descriptions
- **Candidate Sourcing**: Search LinkedIn, databases, job boards
- **Resume Screening**: Parse, match, and score candidates
- **Skills Matching**: Map candidates to requirements
- **Outreach**: Personalized recruiting messages
- **Pipeline Management**: Track and nurture candidates

### Output Formats

| Output | Format | Use Case |
|--------|--------|----------|
| Job Description | Markdown | Posting |
| Candidate List | Table | Review |
| Screening Report | Markdown | Hiring manager |
| Outreach Sequence | Markdown | Recruiting |

### Skills Used

- `talent-acquisition` - Recruiting strategies
- `sourcing` - Boolean, LinkedIn, databases
- `screening` - Resume parsing, scoring

---

## 2.3 Interview Coordinator

**File:** `.claude/agents/interview-coordinator.md`

```yaml
---
name: interview-coordinator
description: Interview management specialist. Use for interview scheduling, interviewer preparation, question generation, feedback collection, and offer coordination. Handles interview logistics and candidate experience.
model: sonnet
---
```

### Core Capabilities

- **Scheduling**: Coordinate interviews, manage calendars
- **Interview Prep**: Prepare interviewers, scorecards
- **Question Generation**: Role-specific interview questions
- **Feedback Collection**: Gather and synthesize feedback
- **Offer Management**: Generate offers, track acceptance
- **Candidate Communication**: Status updates, logistics

### Interview Types

| Type | Duration | Focus |
|------|----------|-------|
| Phone Screen | 30 min | Initial qualification |
| Technical | 45-60 min | Skills assessment |
| Behavioral | 45 min | Culture fit |
| Panel | 60 min | Cross-functional |
| Executive | 45 min | Leadership alignment |

### Output Formats

| Output | Format | Use Case |
|--------|--------|----------|
| Interview Schedule | Table | Logistics |
| Interview Guide | Markdown | Interviewer prep |
| Scorecard | Template | Evaluation |
| Offer Letter | Markdown | Candidate |

### Skills Used

- `interviewing` - Question frameworks
- `assessment` - Evaluation methods
- `candidate-experience` - Communication

---

## 2.4 Onboarding Specialist

**File:** `.claude/agents/onboarding-specialist.md`

```yaml
---
name: onboarding-specialist
description: New hire onboarding specialist. Use for preboarding tasks, first-day setup, training schedules, documentation collection, and 30-60-90 day plans. Handles new employee integration and early success.
model: sonnet
---
```

### Core Capabilities

- **Preboarding**: Pre-start tasks, equipment, access
- **Documentation**: I-9, W-4, policy acknowledgments
- **Training Plans**: Role-specific learning paths
- **Buddy Programs**: Mentor matching, check-ins
- **30-60-90 Plans**: Goal setting, milestones
- **New Hire Support**: Questions, resources

### Onboarding Timeline

| Phase | Timing | Activities |
|-------|--------|------------|
| Preboarding | -7 to 0 days | Paperwork, equipment, access |
| Day 1 | Day 1 | Welcome, setup, orientation |
| Week 1 | Days 1-5 | Team intros, training start |
| Month 1 | Days 1-30 | Role training, first projects |
| Month 2-3 | Days 31-90 | Independence, performance |

### Output Formats

| Output | Format | Use Case |
|--------|--------|----------|
| Onboarding Checklist | Markdown | New hire |
| Training Plan | Table | Learning path |
| 30-60-90 Plan | Markdown | Goals |
| Welcome Package | Markdown | Day 1 |

### Skills Used

- `onboarding` - New hire integration
- `training` - Learning programs
- `compliance` - Documentation

---

## 2.5 HR Analyst

**File:** `.claude/agents/hr-analyst.md`

```yaml
---
name: hr-analyst
description: People analytics and HR reporting specialist. Use for workforce analytics, headcount reporting, turnover analysis, compensation benchmarking, and HR dashboards. Handles data-driven HR insights.
model: sonnet
---
```

### Core Capabilities

- **Workforce Analytics**: Headcount, demographics, trends
- **Turnover Analysis**: Attrition rates, retention risks
- **Compensation Analysis**: Benchmarking, equity audits
- **Performance Metrics**: Review cycles, ratings
- **Recruiting Analytics**: Funnel, time-to-hire, quality
- **HR Dashboards**: Executive reporting

### Key Metrics

| Category | Metrics |
|----------|---------|
| Headcount | Total, by dept, growth rate |
| Turnover | Voluntary, involuntary, regrettable |
| Recruiting | Time-to-fill, cost-per-hire, quality |
| Compensation | Compa-ratio, pay equity |
| Engagement | eNPS, survey scores |
| Performance | Rating distribution, calibration |

### Output Formats

| Output | Format | Use Case |
|--------|--------|----------|
| HR Dashboard | Markdown/Table | Executive |
| Turnover Report | Markdown | Leadership |
| Comp Analysis | Table | HR/Finance |
| Recruiting Metrics | Table | TA team |

### Skills Used

- `people-analytics` - HR metrics
- `data-analysis` - Statistical methods
- `compensation` - Benchmarking

---

## 2.6 Compliance Officer

**File:** `.claude/agents/compliance-officer.md`

```yaml
---
name: compliance-officer
description: HR compliance and policy specialist. Use for policy creation, compliance audits, EEOC reporting, handbook updates, and regulatory monitoring. Handles employment law and workplace compliance.
model: sonnet
---
```

### Core Capabilities

- **Policy Management**: Create, update, publish policies
- **Compliance Audits**: I-9, EEO, OFCCP audits
- **Regulatory Monitoring**: Track law changes
- **Handbook Management**: Employee handbook updates
- **Training Compliance**: Required training tracking
- **Investigations**: Complaint handling support

### Compliance Areas

| Area | Regulations | Activities |
|------|-------------|------------|
| Hiring | EEO, OFCCP | Adverse impact analysis |
| Workplace | OSHA, ADA | Safety, accommodation |
| Wages | FLSA, state laws | Overtime, minimum wage |
| Leave | FMLA, state | Leave administration |
| Privacy | GDPR, CCPA | Data protection |
| Records | Retention laws | Document management |

### Output Formats

| Output | Format | Use Case |
|--------|--------|----------|
| Policy Document | Markdown | Employee reference |
| Audit Report | Markdown | Compliance review |
| EEO-1 Report | Structured | Government filing |
| Training Matrix | Table | Compliance tracking |

### Skills Used

- `hr-compliance` - Employment law
- `policy-management` - Policy frameworks
- `risk-management` - HR risk

---

## 2.7 Employee Support

**File:** `.claude/agents/employee-support.md`

```yaml
---
name: employee-support
description: Employee self-service and HR support specialist. Use for answering employee questions, benefits inquiries, PTO requests, policy clarification, and HR ticket routing. Handles first-line employee support.
model: haiku
---
```

### Core Capabilities

- **FAQ Responses**: Common HR questions
- **Benefits Information**: Plan details, enrollment
- **PTO Management**: Balance checks, requests
- **Policy Lookup**: Find relevant policies
- **Ticket Routing**: Escalate complex issues
- **Document Requests**: Paystubs, letters

### Common Inquiries

| Category | Examples |
|----------|----------|
| Benefits | Health plan options, FSA, 401k |
| Time Off | PTO balance, holiday schedule |
| Payroll | Pay dates, direct deposit |
| Policies | Dress code, remote work |
| Documents | Employment verification |

### Output Formats

| Output | Format | Use Case |
|--------|--------|----------|
| FAQ Response | Markdown | Quick answer |
| Policy Summary | Markdown | Reference |
| Benefits Guide | Markdown | Enrollment |
| Ticket | Structured | Escalation |

### Skills Used

- `employee-relations` - Support
- `benefits` - Plan knowledge
- `hr-policies` - Policy lookup

---

## 2.8 Agent Interaction Matrix

| Scenario | Primary Agent | Supporting Agents |
|----------|---------------|-------------------|
| New requisition | talent-sourcer | interview-coordinator |
| Interview process | interview-coordinator | talent-sourcer |
| New hire start | onboarding-specialist | employee-support |
| Quarterly review | hr-analyst | compliance-officer |
| Policy update | compliance-officer | employee-support |
| Employee question | employee-support | compliance-officer |
| Turnover spike | hr-analyst | talent-sourcer |
| Compliance audit | compliance-officer | hr-analyst |
