# Part 3: Command Specifications

## 3.1 Command Structure

```
.claude/commands/
├── contract/
│   ├── review.md         # /contract:review
│   ├── draft.md          # /contract:draft
│   ├── compare.md        # /contract:compare
│   ├── extract.md        # /contract:extract
│   └── redline.md        # /contract:redline
├── research/
│   ├── case.md           # /research:case
│   ├── statute.md        # /research:statute
│   ├── memo.md           # /research:memo
│   └── cite.md           # /research:cite
├── discovery/
│   ├── review.md         # /discovery:review
│   ├── privilege.md      # /discovery:privilege
│   ├── search.md         # /discovery:search
│   └── summary.md        # /discovery:summary
├── compliance/
│   ├── audit.md          # /compliance:audit
│   ├── policy.md         # /compliance:policy
│   ├── gap.md            # /compliance:gap
│   └── track.md          # /compliance:track
├── draft/
│   ├── document.md       # /draft:document
│   ├── brief.md          # /draft:brief
│   ├── motion.md         # /draft:motion
│   └── letter.md         # /draft:letter
└── matter/
    ├── status.md         # /matter:status
    ├── budget.md         # /matter:budget
    ├── billing.md        # /matter:billing
    └── deadline.md       # /matter:deadline
```

---

## 3.2 Contract Commands

### /contract:review
```yaml
---
description: Review contract for risks, key terms, and deviations
argument-hint: [file-path] [playbook-type]
---
```

**Workflow:**
1. Parse contract document
2. Extract key terms and clauses
3. Compare against playbook (if specified)
4. Identify risks and deviations
5. Generate risk score
6. Produce review report

**Agent:** `contract-analyst`

**Output:** Risk report with flagged clauses, recommendations

---

### /contract:draft
```yaml
---
description: Draft contract from template
argument-hint: [contract-type] [party-info]
---
```

**Workflow:**
1. Select appropriate template
2. Gather party information
3. Insert standard clauses
4. Customize terms
5. Apply firm style
6. Generate draft

**Agent:** `drafting-assistant`, `contract-analyst`

**Supported Types:** NDA, MSA, SOW, Employment, License, Purchase

---

### /contract:compare
```yaml
---
description: Compare two contract versions
argument-hint: [file-a] [file-b]
---
```

**Workflow:**
1. Parse both documents
2. Identify differences
3. Categorize changes (material vs. non-material)
4. Generate comparison report
5. Highlight risk changes

**Agent:** `contract-analyst`

---

### /contract:extract
```yaml
---
description: Extract key terms from contract
argument-hint: [file-path] [term-types]
---
```

**Workflow:**
1. Parse document
2. Identify clause boundaries
3. Extract specified terms
4. Structure output
5. Generate term sheet

**Term Types:** `dates`, `parties`, `payment`, `termination`, `ip`, `confidentiality`, `liability`, `all`

---

### /contract:redline
```yaml
---
description: Generate redline with suggested changes
argument-hint: [file-path] [playbook]
---
```

**Workflow:**
1. Review contract
2. Apply playbook standards
3. Generate suggested changes
4. Create redlined version
5. Add negotiation notes

**Agent:** `contract-analyst`, `drafting-assistant`

---

## 3.3 Research Commands

### /research:case
```yaml
---
description: Research case law on legal issue
argument-hint: [legal-issue] [jurisdiction]
---
```

**Workflow:**
1. Parse legal issue
2. Identify relevant search terms
3. Search case databases
4. Rank by relevance and authority
5. Summarize key holdings
6. Generate case list with citations

**Agent:** `legal-researcher`

---

### /research:statute
```yaml
---
description: Research statutes and regulations
argument-hint: [topic] [jurisdiction]
---
```

**Workflow:**
1. Identify relevant statutes
2. Gather regulatory guidance
3. Analyze requirements
4. Check for recent amendments
5. Generate statutory summary

**Agent:** `legal-researcher`

---

### /research:memo
```yaml
---
description: Generate legal research memo
argument-hint: [question-presented] [jurisdiction]
---
```

**Workflow:**
1. Frame legal question
2. Conduct case research
3. Conduct statutory research
4. Analyze and synthesize
5. Draft memo with IRAC structure
6. Add citations

**Agent:** `legal-researcher`

**Structure:** Question Presented → Brief Answer → Facts → Discussion → Conclusion

---

### /research:cite
```yaml
---
description: Validate and format citations
argument-hint: [citation-list] [format]
---
```

**Workflow:**
1. Parse citations
2. Validate each citation
3. Check currency (overruled, distinguished)
4. Format per style guide
5. Generate validation report

**Formats:** `bluebook`, `alwd`, `chicago`, `firm-style`

---

## 3.4 Discovery Commands

### /discovery:review
```yaml
---
description: Review document batch for relevance
argument-hint: [document-set] [issues]
---
```

**Workflow:**
1. Process document set
2. Apply issue coding
3. Score relevance
4. Categorize documents
5. Generate review summary

**Agent:** `discovery-agent`

---

### /discovery:privilege
```yaml
---
description: Review for privilege and work product
argument-hint: [document-set]
---
```

**Workflow:**
1. Identify attorney communications
2. Check work product indicators
3. Flag potential privilege
4. Generate privilege log entries
5. Create review report

**Agent:** `discovery-agent`

---

### /discovery:search
```yaml
---
description: Search documents with natural language
argument-hint: [query] [document-set]
---
```

**Workflow:**
1. Parse natural language query
2. Execute semantic search
3. Rank results
4. Generate hit report
5. Provide context snippets

**Agent:** `discovery-agent`

---

### /discovery:summary
```yaml
---
description: Summarize document or document set
argument-hint: [document-or-set]
---
```

**Workflow:**
1. Process document(s)
2. Extract key information
3. Identify important facts
4. Generate summary
5. Note relevance to issues

**Agent:** `discovery-agent`

---

## 3.5 Compliance Commands

### /compliance:audit
```yaml
---
description: Prepare compliance audit documentation
argument-hint: [regulation] [scope]
---
```

**Workflow:**
1. Identify audit requirements
2. Gather relevant policies
3. Create audit checklist
4. Assess current compliance
5. Generate audit report

**Agent:** `compliance-monitor`

---

### /compliance:policy
```yaml
---
description: Draft or update compliance policy
argument-hint: [policy-type] [regulation]
---
```

**Workflow:**
1. Review regulatory requirements
2. Analyze current policy (if exists)
3. Draft updated policy
4. Include required elements
5. Format for approval

**Agent:** `compliance-monitor`, `drafting-assistant`

---

### /compliance:gap
```yaml
---
description: Analyze compliance gaps
argument-hint: [regulation] [current-state]
---
```

**Workflow:**
1. Map regulatory requirements
2. Document current state
3. Identify gaps
4. Prioritize by risk
5. Recommend remediation

**Agent:** `compliance-monitor`

---

### /compliance:track
```yaml
---
description: Track regulatory changes
argument-hint: [regulations] [jurisdictions]
---
```

**Workflow:**
1. Monitor specified regulations
2. Identify recent changes
3. Assess impact
4. Generate change summary
5. Recommend actions

**Agent:** `compliance-monitor`

---

## 3.6 Drafting Commands

### /draft:document
```yaml
---
description: Draft legal document from template
argument-hint: [document-type] [parameters]
---
```

**Agent:** `drafting-assistant`

**Document Types:** Corporate resolutions, bylaws, consents, amendments

---

### /draft:brief
```yaml
---
description: Draft litigation brief
argument-hint: [brief-type] [matter-info]
---
```

**Brief Types:** Motion to dismiss, summary judgment, opposition, reply

**Agent:** `drafting-assistant`, `legal-researcher`

---

### /draft:motion
```yaml
---
description: Draft motion
argument-hint: [motion-type] [matter-info]
---
```

**Motion Types:** Discovery, compel, protective order, extension

**Agent:** `drafting-assistant`

---

### /draft:letter
```yaml
---
description: Draft legal correspondence
argument-hint: [letter-type] [recipient-info]
---
```

**Letter Types:** Demand, opinion, engagement, status update

**Agent:** `drafting-assistant`

---

## 3.7 Matter Commands

### /matter:status
```yaml
---
description: Generate matter status report
argument-hint: [matter-id]
---
```

**Agent:** `practice-manager`

---

### /matter:budget
```yaml
---
description: Review and forecast matter budget
argument-hint: [matter-id]
---
```

**Agent:** `practice-manager`

---

### /matter:billing
```yaml
---
description: Review time entries and prepare billing
argument-hint: [matter-id] [period]
---
```

**Agent:** `practice-manager`

---

### /matter:deadline
```yaml
---
description: Track and manage matter deadlines
argument-hint: [matter-id]
---
```

**Agent:** `practice-manager`

---

## 3.8 Command Quick Reference

| Command | Description | Agent |
|---------|-------------|-------|
| `/contract:review` | Review contract risks | contract-analyst |
| `/contract:draft` | Draft from template | drafting-assistant |
| `/contract:compare` | Compare versions | contract-analyst |
| `/contract:extract` | Extract key terms | contract-analyst |
| `/contract:redline` | Generate redlines | contract-analyst |
| `/research:case` | Case law research | legal-researcher |
| `/research:statute` | Statutory research | legal-researcher |
| `/research:memo` | Research memo | legal-researcher |
| `/research:cite` | Validate citations | legal-researcher |
| `/discovery:review` | Document review | discovery-agent |
| `/discovery:privilege` | Privilege review | discovery-agent |
| `/discovery:search` | Natural language search | discovery-agent |
| `/discovery:summary` | Document summary | discovery-agent |
| `/compliance:audit` | Audit preparation | compliance-monitor |
| `/compliance:policy` | Policy drafting | compliance-monitor |
| `/compliance:gap` | Gap analysis | compliance-monitor |
| `/compliance:track` | Regulatory tracking | compliance-monitor |
| `/draft:document` | Legal documents | drafting-assistant |
| `/draft:brief` | Litigation briefs | drafting-assistant |
| `/draft:motion` | Court motions | drafting-assistant |
| `/draft:letter` | Legal letters | drafting-assistant |
| `/matter:status` | Status report | practice-manager |
| `/matter:budget` | Budget tracking | practice-manager |
| `/matter:billing` | Billing review | practice-manager |
| `/matter:deadline` | Deadline tracking | practice-manager |
