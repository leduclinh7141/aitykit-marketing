# Part 5: Workflow & Configuration Specifications

## 5.1 Primary Sales Workflow

**File:** `.claude/workflows/primary-workflow.md`

```markdown
# Primary Sales Workflow

## Sales Pipeline Flow

Prospect → Outreach → Qualify → Demo → Propose → Negotiate → Close → Handoff

### Phase 1: Prospect
- Delegate to `prospector` for list building
- Use `prospecting` skill for ICP matching
- Output: Qualified prospect list

### Phase 2: Outreach
- Delegate to `outreach-specialist` for sequences
- Use `sales-outreach` skill for messaging
- Output: Engaged prospects, meetings booked

### Phase 3: Qualify
- Delegate to `meeting-prep` for research
- Delegate to `deal-analyst` for scoring
- Use `sales-methodology` skill
- Output: Qualified opportunities

### Phase 4: Demo
- Delegate to `meeting-prep` for preparation
- Use discovery and demo best practices
- Output: Demo completed, next steps confirmed

### Phase 5: Propose
- Delegate to `proposal-writer` for proposal
- Use `sales-enablement` skill
- Output: Proposal delivered

### Phase 6: Negotiate
- Delegate to `proposal-writer` for terms
- Delegate to `deal-analyst` for risk assessment
- Use `deal-management` skill
- Output: Terms agreed

### Phase 7: Close
- Delegate to `deal-analyst` for close planning
- Execute mutual action plan
- Output: Deal closed, contract signed

### Phase 8: Handoff
- Delegate to `success-handoff` for transition
- Create success plan
- Output: Customer onboarding initiated
```

---

## 5.2 Sales Rules

**File:** `.claude/workflows/sales-rules.md`

```markdown
# Sales Rules

## Outreach Standards
- Personalize every message with specific research
- Respect opt-out requests immediately
- Follow up persistently but not annoyingly
- Multi-channel but coordinated timing

## Qualification Standards
- Apply consistent methodology (MEDDIC/BANT)
- Document all discovery findings
- Score objectively against criteria
- Disqualify early when fit is poor

## Deal Management Standards
- Update CRM after every interaction
- Maintain accurate close dates
- Flag risks proactively
- Create mutual action plans for commits

## Communication Standards
- Respond to prospects within 24 hours
- Send meeting agendas in advance
- Follow up same day after meetings
- Keep internal teams informed

## Ethical Standards
- Be honest about capabilities
- Don't disparage competitors unfairly
- Honor pricing commitments
- Protect customer information
```

---

## 5.3 Orchestration Protocol

**File:** `.claude/workflows/orchestration-protocol.md`

```markdown
# Sales Agent Orchestration

## Sequential Workflows

### New Campaign Flow
prospector → outreach-specialist → meeting-prep
1. Build targeted list
2. Create personalized sequences
3. Prepare for booked meetings

### Deal Progression Flow
meeting-prep → deal-analyst → proposal-writer → success-handoff
1. Research and prepare
2. Score and track deal
3. Create proposal
4. Hand off to success

## Parallel Workflows

### Pipeline Review
- prospector: Assess list quality and gaps
- deal-analyst: Score all active deals
- proposal-writer: Update pending proposals
→ Combined pipeline health report

### Account Planning
- prospector: Research expansion targets
- meeting-prep: Map stakeholders
- success-handoff: Identify expansion signals
→ Comprehensive account plan

## Agent Handoffs

| Trigger | From | To |
|---------|------|-----|
| Meeting booked | outreach-specialist | meeting-prep |
| Demo completed | meeting-prep | deal-analyst |
| Proposal requested | deal-analyst | proposal-writer |
| Deal won | deal-analyst | success-handoff |
| Expansion signal | success-handoff | prospector |
```

---

## 5.4 Configuration Files

### metadata.json

```json
{
  "version": "1.0.0",
  "name": "claudekit-sales",
  "description": "AI-powered sales automation kit with specialized agents for prospecting, outreach, deal management, proposals, and customer success handoff.",
  "buildDate": "2025-12-03T00:00:00.000Z",
  "repository": {
    "type": "git",
    "url": "https://github.com/claudekit/claudekit-sales.git"
  }
}
```

### CLAUDE.md

```markdown
# CLAUDE.md

## Role & Responsibilities

Your role is to assist sales professionals with prospecting, outreach, deal management, and closing while maintaining ethical sales practices and accurate pipeline data.

## Workflows

- Primary workflow: `./.claude/workflows/primary-workflow.md`
- Sales rules: `./.claude/workflows/sales-rules.md`
- Orchestration: `./.claude/workflows/orchestration-protocol.md`

## Sales Agents

- `prospector` - Lead generation & list building
- `outreach-specialist` - Multi-channel sequences
- `meeting-prep` - Pre-call research & intel
- `deal-analyst` - Pipeline & forecasting
- `proposal-writer` - Proposals & battlecards
- `success-handoff` - Post-sale transition

## Skills Catalog

- `prospecting` - ICP, list building, scoring
- `sales-outreach` - Email, LinkedIn, calling
- `sales-methodology` - MEDDIC, BANT, SPIN
- `deal-management` - Pipeline, forecasting
- `sales-enablement` - Proposals, objections
```

### .mcp.json.example

```json
{
  "mcpServers": {
    "salesforce": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-salesforce"],
      "env": { "SF_ACCESS_TOKEN": "YOUR_TOKEN" }
    },
    "hubspot": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-hubspot"],
      "env": { "HUBSPOT_API_KEY": "YOUR_KEY" }
    },
    "apollo": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-apollo"],
      "env": { "APOLLO_API_KEY": "YOUR_KEY" }
    },
    "linkedin": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-linkedin"],
      "env": { "LINKEDIN_ACCESS_TOKEN": "YOUR_TOKEN" }
    },
    "outreach": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-outreach"],
      "env": { "OUTREACH_API_KEY": "YOUR_KEY" }
    },
    "gmail": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-gmail"],
      "env": { "GMAIL_CREDENTIALS": "YOUR_CREDS" }
    },
    "calendar": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-google-calendar"],
      "env": { "GOOGLE_CALENDAR_CREDS": "YOUR_CREDS" }
    },
    "zoom": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-zoom"],
      "env": { "ZOOM_API_KEY": "YOUR_KEY" }
    },
    "gong": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-gong"],
      "env": { "GONG_API_KEY": "YOUR_KEY" }
    },
    "slack": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-slack"],
      "env": { "SLACK_BOT_TOKEN": "YOUR_TOKEN" }
    }
  }
}
```

---

## 5.5 MCP Integration Summary

| Integration | Purpose | Priority |
|-------------|---------|----------|
| Salesforce | CRM | HIGH |
| HubSpot | CRM | HIGH |
| Apollo | Prospecting data | HIGH |
| LinkedIn | Social selling | HIGH |
| Outreach/Salesloft | Sequences | MEDIUM |
| Gmail/Outlook | Email | HIGH |
| Calendar | Scheduling | HIGH |
| Zoom/Teams | Meetings | MEDIUM |
| Gong/Chorus | Call intelligence | LOW |
| Slack | Communication | LOW |
