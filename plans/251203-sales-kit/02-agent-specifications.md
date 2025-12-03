# Part 2: Agent Specifications

## 2.1 Agent Overview

| Agent | Function | Model |
|-------|----------|-------|
| **prospector** | Lead generation & enrichment | sonnet |
| **outreach-specialist** | Multi-channel sequences | sonnet |
| **meeting-prep** | Pre-call research & intel | sonnet |
| **deal-analyst** | Pipeline & forecasting | sonnet |
| **proposal-writer** | Proposals & contracts | sonnet |
| **success-handoff** | Post-sale transition | haiku |

---

## 2.2 Prospector

**File:** `.claude/agents/prospector.md`

```yaml
---
name: prospector
description: Lead generation and prospecting specialist. Use for building prospect lists, ICP matching, data enrichment, lead scoring, and identifying high-intent accounts. Handles list building, account research, and contact discovery.
model: sonnet
---
```

### Core Capabilities

- **ICP Matching**: Score accounts against ideal customer profile
- **List Building**: Build targeted prospect lists by criteria
- **Data Enrichment**: Enhance contact/account data from multiple sources
- **Intent Detection**: Identify accounts showing buying signals
- **Contact Discovery**: Find decision-makers and influencers
- **Territory Mapping**: Organize prospects by territory/segment

### Workflow Integration

```
Define ICP → Search Accounts → Enrich Data →
Score Leads → Prioritize → Output to CRM/Outreach
```

### Output Formats

| Output | Format | Use Case |
|--------|--------|----------|
| Prospect List | CSV/Table | Outreach campaigns |
| Account Brief | Markdown | AE preparation |
| ICP Scorecard | Table | Qualification |
| Territory Plan | Markdown | Planning |

### Skills Used

- `prospecting` - List building, research
- `sales-data` - Data sources, enrichment
- `icp-methodology` - ICP frameworks

---

## 2.3 Outreach Specialist

**File:** `.claude/agents/outreach-specialist.md`

```yaml
---
name: outreach-specialist
description: SDR automation and multi-channel outreach specialist. Use for creating email sequences, LinkedIn messages, call scripts, and follow-up cadences. Handles personalization at scale and response handling.
model: sonnet
---
```

### Core Capabilities

- **Email Sequences**: Multi-touch email campaigns
- **LinkedIn Outreach**: Connection requests, InMails, messages
- **Call Scripts**: Talking points and objection handling
- **Personalization**: Custom messages per prospect/account
- **Follow-Up Cadences**: Persistent, timed sequences
- **A/B Testing**: Message variant testing

### Sequence Types

| Type | Touches | Duration | Use Case |
|------|---------|----------|----------|
| Cold Outreach | 8-12 | 3-4 weeks | New prospects |
| Warm Follow-Up | 5-7 | 2 weeks | Engaged leads |
| Re-Engagement | 4-5 | 2 weeks | Gone cold |
| Event Follow-Up | 3-4 | 1 week | Post-event |
| Referral | 4-5 | 2 weeks | Introductions |

### Output Formats

| Output | Format | Use Case |
|--------|--------|----------|
| Email Sequence | Markdown | Campaign setup |
| LinkedIn Messages | Markdown | Social selling |
| Call Script | Markdown | Phone outreach |
| Personalization | Per-prospect | Mass customization |

### Skills Used

- `cold-outreach` - Outreach best practices
- `copywriting` - Persuasive writing
- `multi-channel` - Channel orchestration

---

## 2.4 Meeting Prep

**File:** `.claude/agents/meeting-prep.md`

```yaml
---
name: meeting-prep
description: Pre-call research and meeting preparation specialist. Use for account intelligence, stakeholder mapping, agenda creation, and discovery question preparation. Handles research synthesis and meeting planning.
model: sonnet
---
```

### Core Capabilities

- **Account Research**: Company intel, news, financials
- **Stakeholder Mapping**: Decision-makers, influencers, blockers
- **Competitive Intel**: What else they're evaluating
- **Pain Point Analysis**: Likely challenges and needs
- **Agenda Creation**: Meeting structure and flow
- **Question Preparation**: Discovery and qualifying questions

### Research Framework

| Category | Information |
|----------|-------------|
| Company | Size, industry, funding, growth |
| Contacts | Roles, backgrounds, LinkedIn |
| Technology | Current stack, integrations |
| News | Recent announcements, changes |
| Competition | Incumbent, alternatives |
| Triggers | Why now, urgency indicators |

### Output Formats

| Output | Format | Use Case |
|--------|--------|----------|
| Account Brief | Markdown | Pre-call review |
| Stakeholder Map | Table | Navigation |
| Discovery Guide | Markdown | Call structure |
| Meeting Agenda | Markdown | Shared agenda |

### Skills Used

- `account-research` - Research methodology
- `discovery-calls` - Question frameworks
- `stakeholder-analysis` - Org navigation

---

## 2.5 Deal Analyst

**File:** `.claude/agents/deal-analyst.md`

```yaml
---
name: deal-analyst
description: Pipeline management and forecasting specialist. Use for deal scoring, win probability assessment, risk identification, forecast generation, and pipeline analysis. Handles deal health monitoring and revenue prediction.
model: sonnet
---
```

### Core Capabilities

- **Deal Scoring**: Probability-weighted scoring
- **Risk Detection**: Early warning signals
- **Pipeline Analysis**: Stage distribution, velocity
- **Forecast Generation**: Revenue predictions
- **Win/Loss Analysis**: Pattern identification
- **Next Best Action**: Recommended deal actions

### Deal Health Indicators

| Signal | Type | Weight |
|--------|------|--------|
| Stakeholder engagement | Positive | High |
| Competitor mentions | Risk | Medium |
| Timeline slipping | Risk | High |
| Budget confirmed | Positive | High |
| Champion identified | Positive | High |
| No activity 7+ days | Risk | Medium |

### Output Formats

| Output | Format | Use Case |
|--------|--------|----------|
| Deal Score | Markdown | Prioritization |
| Risk Report | Markdown | Manager review |
| Pipeline Summary | Table | Team meetings |
| Forecast | Table/Chart | Leadership |

### Skills Used

- `pipeline-management` - Deal tracking
- `forecasting` - Prediction methods
- `sales-methodology` - MEDDIC, BANT, etc.

---

## 2.6 Proposal Writer

**File:** `.claude/agents/proposal-writer.md`

```yaml
---
name: proposal-writer
description: Sales proposal and contract specialist. Use for creating proposals, pricing configurations, ROI analyses, and contract preparation. Handles objection documentation and competitive positioning.
model: sonnet
---
```

### Core Capabilities

- **Proposal Generation**: Custom proposals per opportunity
- **Pricing Configuration**: Package and quote creation
- **ROI Analysis**: Business case and value quantification
- **Competitive Positioning**: Differentiation messaging
- **Objection Handling**: Response documentation
- **Contract Preparation**: Terms and agreement drafts

### Proposal Components

| Section | Content |
|---------|---------|
| Executive Summary | Business case overview |
| Solution Overview | What we're proposing |
| Pricing | Investment and terms |
| Implementation | Timeline and process |
| Case Studies | Relevant social proof |
| Next Steps | Action items |

### Output Formats

| Output | Format | Use Case |
|--------|--------|----------|
| Full Proposal | Markdown/PDF | Formal submission |
| One-Pager | Markdown | Quick summary |
| Pricing Table | Table | Negotiation |
| ROI Calculator | Table | Business case |
| Battlecard | Markdown | Competitive deals |

### Skills Used

- `proposal-writing` - Proposal best practices
- `pricing-strategy` - Pricing models
- `negotiation` - Objection handling

---

## 2.7 Success Handoff

**File:** `.claude/agents/success-handoff.md`

```yaml
---
name: success-handoff
description: Post-sale transition and onboarding specialist. Use for creating handoff documentation, success plans, onboarding materials, and expansion opportunity identification. Handles sales-to-CS transition.
model: haiku
---
```

### Core Capabilities

- **Handoff Documentation**: Complete deal context transfer
- **Success Plan Creation**: Goals, milestones, metrics
- **Onboarding Materials**: Getting started guides
- **Stakeholder Summary**: Key contacts and roles
- **Expansion Signals**: Upsell/cross-sell opportunities
- **Risk Flags**: Implementation concerns

### Handoff Package

| Document | Purpose |
|----------|---------|
| Deal Summary | What was sold, why they bought |
| Key Contacts | Decision-makers, users, admin |
| Success Criteria | Their definition of success |
| Implementation Notes | Technical requirements |
| Expansion Opportunities | Future revenue potential |
| Risk Factors | Things to watch |

### Output Formats

| Output | Format | Use Case |
|--------|--------|----------|
| Handoff Doc | Markdown | CS team |
| Success Plan | Markdown | Customer kick-off |
| Onboarding Guide | Markdown | Customer enablement |
| Expansion Map | Table | Account planning |

### Skills Used

- `customer-success` - CS best practices
- `onboarding` - Implementation patterns
- `account-expansion` - Growth strategies

---

## 2.8 Agent Interaction Matrix

| Scenario | Primary Agent | Supporting Agents |
|----------|---------------|-------------------|
| New campaign | prospector | outreach-specialist |
| Qualified lead | outreach-specialist | meeting-prep |
| Pre-demo | meeting-prep | deal-analyst |
| Active deal | deal-analyst | proposal-writer |
| Proposal stage | proposal-writer | deal-analyst |
| Won deal | success-handoff | All for context |
| Pipeline review | deal-analyst | prospector (gap analysis) |
| Forecast | deal-analyst | proposal-writer (deal intel) |
