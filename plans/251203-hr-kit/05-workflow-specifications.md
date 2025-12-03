# Part 5: Workflow & Configuration Specifications

## 5.1 Primary HR Workflow

**File:** `.claude/workflows/primary-workflow.md`

```markdown
# Primary HR Workflow

## Employee Lifecycle Flow

Recruit → Interview → Hire → Onboard → Perform → Develop → Retain/Exit

### Phase 1: Recruit
- Delegate to `talent-sourcer` for job posting
- Delegate to `talent-sourcer` for sourcing
- Use `talent-acquisition` skill
- Output: Qualified candidate pipeline

### Phase 2: Interview
- Delegate to `interview-coordinator` for scheduling
- Delegate to `interview-coordinator` for prep
- Use `interviewing` skill
- Output: Evaluated candidates, recommendations

### Phase 3: Hire
- Delegate to `interview-coordinator` for offer
- Delegate to `compliance-officer` for documentation
- Output: Signed offer, start date confirmed

### Phase 4: Onboard
- Delegate to `onboarding-specialist` for setup
- Use `onboarding` skill
- Output: Productive new hire

### Phase 5: Perform
- Delegate to `hr-analyst` for metrics
- Track performance, goals
- Output: Performance data

### Phase 6: Support
- Delegate to `employee-support` for inquiries
- Delegate to `compliance-officer` for policies
- Output: Satisfied employees
```

---

## 5.2 HR Rules

**File:** `.claude/workflows/hr-rules.md`

```markdown
# HR Rules

## Recruiting Standards
- Write inclusive job descriptions
- Use structured screening criteria
- Document all candidate interactions
- Respond to applicants within 48 hours

## Interview Standards
- Use structured interviews with scorecards
- Train interviewers on bias reduction
- Provide consistent candidate experience
- Make data-driven hiring decisions

## Compliance Standards
- Maintain accurate employee records
- Follow all employment laws
- Document policy acknowledgments
- Conduct regular compliance audits

## Privacy Standards
- Protect employee personal data
- Limit access to sensitive information
- Follow GDPR/CCPA requirements
- Secure all HR systems

## Communication Standards
- Respond to employee inquiries within 24 hours
- Communicate policy changes proactively
- Maintain confidentiality
- Document sensitive conversations
```

---

## 5.3 Orchestration Protocol

**File:** `.claude/workflows/orchestration-protocol.md`

```markdown
# HR Agent Orchestration

## Sequential Workflows

### Hiring Flow
talent-sourcer → interview-coordinator → onboarding-specialist
1. Source and screen candidates
2. Coordinate interviews, extend offer
3. Onboard new hire

### Compliance Review Flow
compliance-officer → hr-analyst → employee-support
1. Audit compliance status
2. Generate compliance metrics
3. Update employee communications

## Parallel Workflows

### Quarterly HR Review
- hr-analyst: Headcount and turnover reports
- talent-sourcer: Pipeline health report
- compliance-officer: Compliance status
→ Combined HR dashboard

### Annual Planning
- hr-analyst: Workforce planning
- talent-sourcer: Recruiting capacity
- compliance-officer: Policy updates needed
→ Annual HR plan

## Agent Handoffs

| Trigger | From | To |
|---------|------|-----|
| Candidate screened | talent-sourcer | interview-coordinator |
| Offer accepted | interview-coordinator | onboarding-specialist |
| Day 1 complete | onboarding-specialist | employee-support |
| Policy question | employee-support | compliance-officer |
| Metrics request | compliance-officer | hr-analyst |
| Hiring need | hr-analyst | talent-sourcer |
```

---

## 5.4 Configuration Files

### metadata.json

```json
{
  "version": "1.0.0",
  "name": "claudekit-hr",
  "description": "AI-powered HR and recruiting kit with specialized agents for talent acquisition, interviewing, onboarding, analytics, compliance, and employee support.",
  "buildDate": "2025-12-03T00:00:00.000Z",
  "repository": {
    "type": "git",
    "url": "https://github.com/claudekit/claudekit-hr.git"
  }
}
```

### CLAUDE.md

```markdown
# CLAUDE.md

## Role & Responsibilities

Your role is to assist HR professionals with recruiting, onboarding, employee management, compliance, and analytics while maintaining confidentiality and legal compliance.

## Workflows

- Primary workflow: `./.claude/workflows/primary-workflow.md`
- HR rules: `./.claude/workflows/hr-rules.md`
- Orchestration: `./.claude/workflows/orchestration-protocol.md`

## HR Agents

- `talent-sourcer` - Recruiting & sourcing
- `interview-coordinator` - Interview management
- `onboarding-specialist` - New hire onboarding
- `hr-analyst` - People analytics
- `compliance-officer` - HR compliance
- `employee-support` - Employee self-service

## Skills Catalog

- `talent-acquisition` - Sourcing, screening
- `interviewing` - Assessment, evaluation
- `onboarding` - New hire integration
- `people-analytics` - HR metrics, reporting
- `hr-compliance` - Employment law, policies
```

### .mcp.json.example

```json
{
  "mcpServers": {
    "greenhouse": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-greenhouse"],
      "env": { "GREENHOUSE_API_KEY": "YOUR_KEY" }
    },
    "lever": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-lever"],
      "env": { "LEVER_API_KEY": "YOUR_KEY" }
    },
    "bamboohr": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-bamboohr"],
      "env": { "BAMBOO_API_KEY": "YOUR_KEY", "BAMBOO_SUBDOMAIN": "YOUR_SUBDOMAIN" }
    },
    "rippling": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-rippling"],
      "env": { "RIPPLING_API_KEY": "YOUR_KEY" }
    },
    "linkedin": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-linkedin"],
      "env": { "LINKEDIN_ACCESS_TOKEN": "YOUR_TOKEN" }
    },
    "indeed": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-indeed"],
      "env": { "INDEED_API_KEY": "YOUR_KEY" }
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
    "slack": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-slack"],
      "env": { "SLACK_BOT_TOKEN": "YOUR_TOKEN" }
    },
    "gmail": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-gmail"],
      "env": { "GMAIL_CREDENTIALS": "YOUR_CREDS" }
    },
    "notion": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-notion"],
      "env": { "NOTION_API_KEY": "YOUR_KEY" }
    },
    "gusto": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-gusto"],
      "env": { "GUSTO_API_KEY": "YOUR_KEY" }
    }
  }
}
```

---

## 5.5 MCP Integration Summary

| Integration | Purpose | Priority |
|-------------|---------|----------|
| Greenhouse | ATS | HIGH |
| Lever | ATS | HIGH |
| BambooHR | HRIS | HIGH |
| Rippling | HRIS/Payroll | HIGH |
| LinkedIn | Sourcing | HIGH |
| Indeed | Job posting | MEDIUM |
| Google Calendar | Scheduling | HIGH |
| Zoom | Video interviews | HIGH |
| Slack | Communication | MEDIUM |
| Gmail | Email | MEDIUM |
| Notion | Documentation | LOW |
| Gusto | Payroll/Benefits | MEDIUM |
