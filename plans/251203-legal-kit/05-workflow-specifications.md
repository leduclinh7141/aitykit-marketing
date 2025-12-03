# Part 5: Workflow & Configuration Specifications

## 5.1 Primary Legal Workflow

**File:** `.claude/workflows/primary-workflow.md`

```markdown
# Primary Legal Workflow

## Legal Matter Pipeline

Intake → Research → Analysis → Drafting → Review → Delivery → Close

### Phase 1: Intake
- Receive matter/document
- Identify matter type and requirements
- Delegate to appropriate agent
- Output: Matter scope definition

### Phase 2: Research
- Delegate to `legal-researcher` for case/statutory research
- Delegate to `compliance-monitor` for regulatory context
- Use `legal-research` skill
- Output: Research findings

### Phase 3: Analysis
- Delegate to `contract-analyst` for contract matters
- Delegate to `discovery-agent` for discovery matters
- Apply relevant skills
- Output: Analysis report

### Phase 4: Drafting
- Delegate to `drafting-assistant` for document creation
- Apply firm style and templates
- Use `contract-law` or `litigation` skills
- Output: Draft documents

### Phase 5: Review
- Quality check against requirements
- Verify citations and accuracy
- Ensure compliance with ethics rules
- Output: Reviewed documents

### Phase 6: Delivery
- Format for client/court
- Prepare supporting materials
- Update matter status
- Output: Final deliverables

### Phase 7: Close
- Delegate to `practice-manager` for billing
- Document lessons learned
- Archive matter materials
- Output: Closed matter
```

---

## 5.2 Legal Practice Rules

**File:** `.claude/workflows/legal-rules.md`

```markdown
# Legal Practice Rules

## Professional Standards
- All work product must be reviewed by licensed attorney
- Maintain attorney-client privilege at all times
- Follow applicable ethics rules (jurisdiction-specific)
- Document all research and analysis methodology

## Quality Standards
- Verify all citations before delivery
- Check for conflicts before engagement
- Apply firm style guide consistently
- Maintain version control on all documents

## Security Requirements
- No client data in prompts without authorization
- Follow firm data classification policies
- Encrypt sensitive communications
- Maintain audit trail for all actions

## Compliance Requirements
- Track regulatory deadlines
- Document compliance decisions
- Escalate potential violations
- Maintain required records
```

---

## 5.3 Orchestration Protocol

**File:** `.claude/workflows/orchestration-protocol.md`

```markdown
# Legal Agent Orchestration

## Sequential Workflows

### Contract Review Flow
contract-analyst → drafting-assistant → practice-manager
1. Analyze contract risks
2. Generate redlines/edits
3. Track time and billing

### Litigation Research Flow
legal-researcher → drafting-assistant → practice-manager
1. Conduct legal research
2. Draft memo/brief
3. Update matter status

### Compliance Audit Flow
compliance-monitor → contract-analyst → drafting-assistant
1. Identify requirements
2. Review relevant contracts
3. Draft policies/updates

## Parallel Workflows

### Due Diligence
- contract-analyst: Review target contracts
- legal-researcher: Research regulatory issues
- compliance-monitor: Compliance assessment
→ Combine findings in DD report

### Litigation Preparation
- discovery-agent: Document review
- legal-researcher: Case research
- drafting-assistant: Brief preparation
→ Coordinate on case strategy
```

---

## 5.4 Configuration Files

### metadata.json

```json
{
  "version": "1.0.0",
  "name": "claudekit-legal",
  "description": "AI-powered legal automation kit with specialized agents for contract review, legal research, e-discovery, compliance monitoring, and practice management.",
  "buildDate": "2025-12-03T00:00:00.000Z",
  "repository": {
    "type": "git",
    "url": "https://github.com/claudekit/claudekit-legal.git"
  }
}
```

### CLAUDE.md

```markdown
# CLAUDE.md

## Role & Responsibilities

Your role is to assist legal professionals with contract review, legal research, document drafting, compliance monitoring, and practice management while maintaining professional standards and ethical obligations.

## Important Disclaimers

- All output requires review by licensed attorney
- Not a substitute for legal advice
- Maintain attorney-client privilege
- Follow jurisdiction-specific rules

## Workflows

- Primary workflow: `./.claude/workflows/primary-workflow.md`
- Legal rules: `./.claude/workflows/legal-rules.md`
- Orchestration: `./.claude/workflows/orchestration-protocol.md`

## Legal Agents

- `contract-analyst` - Contract review & risk assessment
- `legal-researcher` - Case law & statutory research
- `discovery-agent` - E-discovery & document review
- `compliance-monitor` - Regulatory compliance
- `drafting-assistant` - Document drafting
- `practice-manager` - Billing & matter management

## Skills Catalog

- `contract-law` - Contract principles & clauses
- `legal-research` - Research methodology & citation
- `litigation` - Procedure, discovery, brief writing
- `compliance-regulatory` - GDPR, HIPAA, SOX, etc.
- `practice-management` - Billing, ethics, operations
```

### .mcp.json.example

```json
{
  "mcpServers": {
    "clio": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-clio"],
      "env": { "CLIO_API_KEY": "YOUR_API_KEY" }
    },
    "netdocuments": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-netdocuments"],
      "env": { "NETDOCS_API_KEY": "YOUR_API_KEY" }
    },
    "docusign": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-docusign"],
      "env": { "DOCUSIGN_API_KEY": "YOUR_API_KEY" }
    },
    "westlaw": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-westlaw"],
      "env": { "WESTLAW_API_KEY": "YOUR_API_KEY" }
    },
    "lexisnexis": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-lexisnexis"],
      "env": { "LEXIS_API_KEY": "YOUR_API_KEY" }
    },
    "google-workspace": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-google-workspace"],
      "env": { "GOOGLE_SERVICE_ACCOUNT": "YOUR_SERVICE_ACCOUNT" }
    },
    "microsoft365": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-microsoft365"],
      "env": { "MS365_CLIENT_ID": "YOUR_CLIENT_ID" }
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
| Clio/MyCase | Practice management | HIGH |
| NetDocuments/iManage | Document management | HIGH |
| DocuSign | E-signatures | MEDIUM |
| Westlaw/LexisNexis | Legal research | HIGH |
| Google Workspace | Productivity | MEDIUM |
| Microsoft 365 | Word, Outlook | HIGH |
| Slack/Teams | Communication | LOW |
