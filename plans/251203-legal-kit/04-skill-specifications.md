# Part 4: Skill Specifications

## 4.1 Skill Structure

```
.claude/skills/
├── contract-law/
│   ├── SKILL.md
│   └── references/
│       ├── contract-basics.md
│       ├── common-clauses.md
│       ├── risk-assessment.md
│       └── negotiation-tactics.md
├── legal-research/
│   ├── SKILL.md
│   └── references/
│       ├── research-methodology.md
│       ├── citation-formats.md
│       ├── case-analysis.md
│       └── statutory-interpretation.md
├── litigation/
│   ├── SKILL.md
│   └── references/
│       ├── civil-procedure.md
│       ├── discovery-rules.md
│       ├── brief-writing.md
│       └── evidence-rules.md
├── compliance-regulatory/
│   ├── SKILL.md
│   └── references/
│       ├── gdpr.md
│       ├── ccpa-cpra.md
│       ├── hipaa.md
│       ├── sox-finra.md
│       └── audit-procedures.md
└── practice-management/
    ├── SKILL.md
    └── references/
        ├── billing-practices.md
        ├── matter-management.md
        ├── client-relations.md
        └── ethics-rules.md
```

---

## 4.2 Skill: contract-law

**Purpose:** Contract drafting, review, and negotiation expertise

### SKILL.md Content

```markdown
# Contract Law

## Activation
Use when reviewing, drafting, or negotiating contracts.

## Core Concepts
- Contract formation (offer, acceptance, consideration)
- Conditions and covenants
- Representations and warranties
- Risk allocation mechanisms
- Remedies and damages
```

### Reference Files

**contract-basics.md**
- Elements of a valid contract
- Types of contracts (bilateral, unilateral)
- Statute of frauds requirements
- Parol evidence rule
- Contract interpretation principles

**common-clauses.md**
- Indemnification (types, caps, baskets)
- Limitation of liability (consequential, cap)
- Confidentiality (definition, exceptions, term)
- IP ownership and licensing
- Termination (for cause, convenience)
- Force majeure
- Assignment and delegation
- Governing law and dispute resolution

**risk-assessment.md**
- Risk scoring methodology
- High-risk clause indicators
- Industry-specific risks
- Counterparty risk factors
- Deal-breaker identification

**negotiation-tactics.md**
- Prioritization frameworks
- Alternative clause options
- Fallback positions
- Market standard arguments
- Leverage assessment

---

## 4.3 Skill: legal-research

**Purpose:** Legal research methodology and citation

### SKILL.md Content

```markdown
# Legal Research

## Activation
Use when conducting legal research or drafting research memos.

## Core Concepts
- Primary vs. secondary sources
- Binding vs. persuasive authority
- Jurisdictional hierarchy
- Citation validation
- Research memo structure
```

### Reference Files

**research-methodology.md**
- Issue identification and framing
- Search strategy development
- Database selection (Westlaw, Lexis, free sources)
- Boolean vs. natural language search
- Results evaluation criteria
- Research trail documentation

**citation-formats.md**
- Bluebook citation format
- ALWD citation format
- Short form citations
- Signals (e.g., See, Cf., But see)
- Parentheticals
- String citations

**case-analysis.md**
- Case briefing methodology
- Holding vs. dicta
- Distinguishing cases
- Synthesizing case law
- Identifying trends

**statutory-interpretation.md**
- Textualism vs. purposivism
- Canons of construction
- Legislative history
- Agency deference (Chevron)
- Regulatory interpretation

---

## 4.4 Skill: litigation

**Purpose:** Litigation process, discovery, and brief writing

### SKILL.md Content

```markdown
# Litigation

## Activation
Use when working on litigation matters, discovery, or court filings.

## Core Concepts
- Civil procedure stages
- Discovery scope and limits
- Motion practice
- Brief writing
- Evidence rules
```

### Reference Files

**civil-procedure.md**
- Federal vs. state procedure
- Pleading standards (Twombly/Iqbal)
- Motion to dismiss (12(b)(6))
- Summary judgment (Rule 56)
- Class actions
- Appeals process

**discovery-rules.md**
- Scope of discovery (Rule 26)
- Initial disclosures
- Interrogatories
- Requests for production
- Depositions
- Requests for admission
- E-discovery protocols
- Privilege and work product

**brief-writing.md**
- Brief structure and components
- Statement of facts (persuasive)
- Argument organization
- Standard of review
- Headings and roadmaps
- Conclusion and prayer for relief

**evidence-rules.md**
- Relevance (FRE 401-403)
- Hearsay and exceptions
- Authentication
- Best evidence rule
- Privilege rules
- Expert testimony (Daubert)

---

## 4.5 Skill: compliance-regulatory

**Purpose:** Regulatory compliance across jurisdictions

### SKILL.md Content

```markdown
# Compliance & Regulatory

## Activation
Use when addressing compliance issues or regulatory requirements.

## Core Concepts
- Privacy regulations
- Healthcare compliance
- Financial regulations
- Industry-specific rules
- Audit and monitoring
```

### Reference Files

**gdpr.md**
- Territorial scope
- Lawful bases for processing
- Data subject rights
- Controller/processor obligations
- Data protection impact assessments
- Cross-border transfers
- Enforcement and penalties

**ccpa-cpra.md**
- Covered businesses
- Consumer rights
- Opt-out requirements
- Service provider obligations
- CPRA amendments
- Enforcement

**hipaa.md**
- Covered entities and BAs
- PHI definition and handling
- Privacy Rule requirements
- Security Rule requirements
- Breach notification
- Business associate agreements

**sox-finra.md**
- SOX compliance requirements
- Internal controls
- FINRA member obligations
- Broker-dealer requirements
- SEC reporting
- Whistleblower protections

**audit-procedures.md**
- Audit planning
- Control testing
- Documentation requirements
- Gap remediation
- Audit reporting
- Continuous monitoring

---

## 4.6 Skill: practice-management

**Purpose:** Law firm operations and client service

### SKILL.md Content

```markdown
# Practice Management

## Activation
Use when handling billing, matter management, or client communications.

## Core Concepts
- Legal billing practices
- Matter lifecycle
- Client relationships
- Professional responsibility
- Firm operations
```

### Reference Files

**billing-practices.md**
- Time entry best practices
- Billing rate structures
- Alternative fee arrangements
- Invoice preparation
- Collections
- Outside counsel guidelines

**matter-management.md**
- Matter intake
- Conflict checking
- Staffing and budgeting
- Milestone tracking
- Matter closure
- Knowledge management

**client-relations.md**
- Client communication standards
- Status reporting
- Expectation management
- Client feedback
- Business development
- Relationship management

**ethics-rules.md**
- ABA Model Rules overview
- Competence (Rule 1.1)
- Confidentiality (Rule 1.6)
- Conflicts of interest (Rules 1.7-1.10)
- Fees (Rule 1.5)
- Technology competence
- Supervision obligations

---

## 4.7 Skills to Keep from Base Kit

| Skill | Use in Legal Kit |
|-------|------------------|
| ai-multimodal | Document image analysis |
| document-skills | PDF/Word processing |
| research | Research methodology base |

---

## 4.8 Summary

| Skill | References | Primary Agents |
|-------|------------|----------------|
| contract-law | 4 | contract-analyst, drafting-assistant |
| legal-research | 4 | legal-researcher |
| litigation | 4 | discovery-agent, drafting-assistant |
| compliance-regulatory | 5 | compliance-monitor |
| practice-management | 4 | practice-manager |
| **Total** | **21** | - |
