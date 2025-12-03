# Phase 1: Missing Advertised Workflows

## Overview
Website advertises 3 workflows: Marketing, Sales, CRM. Only Marketing exists.

## 1.1 Sales Workflow

**File:** `.claude/workflows/sales-workflow.md`

**Content Structure:**
```
Sales Pipeline Workflow
├── Lead Qualification
│   ├── BANT scoring (Budget, Authority, Need, Timeline)
│   ├── Lead source tracking
│   └── Intent signal detection
├── Prospect Research
│   ├── Company research
│   ├── Decision maker identification
│   └── Pain point analysis
├── Outreach Sequences
│   ├── Cold outreach templates
│   ├── Follow-up cadences
│   └── Multi-touch sequences
├── Sales Enablement
│   ├── Pitch deck generation
│   ├── Case study matching
│   ├── Objection handling scripts
│   └── Competitive battlecards
├── Deal Management
│   ├── Pipeline stage tracking
│   ├── Deal value estimation
│   └── Close probability scoring
└── Handoff Protocols
    ├── Marketing to Sales (MQL → SQL)
    ├── Sales to Success (Won deals)
    └── Lost deal analysis
```

## 1.2 CRM Workflow

**File:** `.claude/workflows/crm-workflow.md`

**Content Structure:**
```
CRM Automation Workflow
├── Contact Management
│   ├── Data enrichment
│   ├── Duplicate detection
│   └── Segmentation rules
├── Lifecycle Stages
│   ├── Subscriber → Lead → MQL → SQL → Opportunity → Customer
│   ├── Stage transition triggers
│   └── Automated status updates
├── Activity Tracking
│   ├── Email opens/clicks
│   ├── Website visits
│   ├── Content downloads
│   └── Meeting attendance
├── Lead Scoring
│   ├── Demographic scoring
│   ├── Behavioral scoring
│   ├── Engagement scoring
│   └── Score decay rules
├── Automation Triggers
│   ├── Welcome sequences
│   ├── Re-engagement campaigns
│   ├── Birthday/anniversary messages
│   └── Milestone celebrations
└── Reporting
    ├── Pipeline velocity
    ├── Conversion rates by stage
    └── Source attribution
```

## Implementation Tasks

- [ ] Create `sales-workflow.md` with full content
- [ ] Create `crm-workflow.md` with full content
- [ ] Update CLAUDE.md to reference new workflows
- [ ] Create supporting commands for each workflow
