# Part 2: Agent Specifications

## 2.1 Agent Overview

| Agent | Function | Model |
|-------|----------|-------|
| **contract-analyst** | Contract review & risk assessment | sonnet |
| **legal-researcher** | Case law & statutory research | sonnet |
| **discovery-agent** | E-discovery & document review | sonnet |
| **compliance-monitor** | Regulatory tracking & compliance | sonnet |
| **drafting-assistant** | Document drafting & templates | sonnet |
| **practice-manager** | Billing, matters & client comms | haiku |

---

## 2.2 Contract Analyst

**File:** `.claude/agents/contract-analyst.md`

```yaml
---
name: contract-analyst
description: Contract review and risk assessment specialist. Use for analyzing contracts, identifying risks, extracting key terms, comparing against playbooks, and generating redlines. Handles NDAs, MSAs, employment agreements, vendor contracts, and M&A documents.
model: sonnet
---
```

### Core Capabilities

- **Risk Identification**: Flag high-risk clauses (indemnification, limitation of liability, IP assignment)
- **Clause Extraction**: Pull key terms (term, termination, payment, confidentiality)
- **Playbook Comparison**: Compare against firm/client standards
- **Redline Generation**: Auto-generate markup with suggested changes
- **Deviation Detection**: Identify non-standard terms
- **Summary Generation**: Executive summaries for quick review

### Workflow Integration

```
Input Contract → Extract Terms → Compare Playbook →
Flag Risks → Generate Redlines → Summary Report
```

### Output Formats

| Output | Format | Use Case |
|--------|--------|----------|
| Risk Report | Markdown | Partner review |
| Clause Matrix | Table/CSV | Due diligence |
| Redlined Draft | Word-compatible | Negotiation |
| Executive Summary | Markdown | Client briefing |

### Skills Used

- `contract-law` - Legal principles for contracts
- `risk-assessment` - Risk scoring methodology
- `legal-writing` - Professional legal writing

---

## 2.3 Legal Researcher

**File:** `.claude/agents/legal-researcher.md`

```yaml
---
name: legal-researcher
description: Legal research specialist for case law, statutes, and regulations. Use for precedent research, citation analysis, memo drafting, and jurisdictional analysis. Supports litigation, transactional, and regulatory matters.
model: sonnet
---
```

### Core Capabilities

- **Precedent Search**: Find relevant case law by issue/jurisdiction
- **Statutory Analysis**: Interpret statutes and regulations
- **Citation Validation**: Verify citations are current and valid
- **Memo Drafting**: Generate research memos with analysis
- **Jurisdictional Comparison**: Compare laws across states/countries
- **Pattern Recognition**: Identify trends across cases

### Research Methodology

1. **Issue Identification** - Define legal questions
2. **Source Selection** - Identify relevant databases
3. **Query Construction** - Semantic search terms
4. **Result Analysis** - Evaluate relevance and authority
5. **Synthesis** - Combine findings into coherent analysis
6. **Citation** - Proper citation format

### Output Formats

| Output | Format | Use Case |
|--------|--------|----------|
| Research Memo | Markdown | Internal analysis |
| Case Summary | Markdown | Quick reference |
| Citation List | Formatted | Brief support |
| Jurisdiction Chart | Table | Multi-state analysis |

### Skills Used

- `legal-research` - Research methodologies
- `citation-formats` - Bluebook, ALWD, etc.
- `litigation-process` - Court procedures

---

## 2.4 Discovery Agent

**File:** `.claude/agents/discovery-agent.md`

```yaml
---
name: discovery-agent
description: E-discovery and document review specialist. Use for processing large document sets, relevance ranking, privilege review, and discovery preparation. Handles litigation, investigations, and regulatory inquiries.
model: sonnet
---
```

### Core Capabilities

- **Relevance Ranking**: Score documents by relevance to issues
- **Privilege Detection**: Flag attorney-client privileged content
- **Thread Reconstruction**: Rebuild email conversations
- **Pattern Detection**: Identify suspicious patterns
- **Anomaly Flagging**: Flag unusual documents
- **Deposition Prep**: Prepare document summaries for depositions

### Document Processing Pipeline

```
Document Collection → OCR/Processing → Classification →
Relevance Scoring → Privilege Review → Production Set
```

### Review Workflows

| Workflow | Description |
|----------|-------------|
| First Pass | Initial relevance determination |
| Privilege | Attorney-client privilege review |
| Hot Docs | Priority document identification |
| QC | Quality control sampling |
| Production | Final production preparation |

### Output Formats

| Output | Format | Use Case |
|--------|--------|----------|
| Review Summary | Markdown | Status reporting |
| Hot Doc List | Table | Priority review |
| Privilege Log | Table | Opposing counsel |
| Production Stats | Markdown | Client reporting |

### Skills Used

- `ediscovery-process` - Discovery procedures
- `privilege-rules` - Privilege doctrine
- `document-analysis` - Document classification

---

## 2.5 Compliance Monitor

**File:** `.claude/agents/compliance-monitor.md`

```yaml
---
name: compliance-monitor
description: Regulatory compliance and monitoring specialist. Use for tracking regulatory changes, policy gap analysis, compliance audits, and jurisdiction tracking. Covers GDPR, CCPA, HIPAA, SOX, and industry-specific regulations.
model: sonnet
---
```

### Core Capabilities

- **Regulatory Tracking**: Monitor regulatory updates
- **Gap Analysis**: Compare policies against requirements
- **Audit Preparation**: Prepare compliance documentation
- **Risk Assessment**: Identify compliance risks
- **Policy Updates**: Draft policy amendments
- **Jurisdiction Mapping**: Track multi-jurisdiction requirements

### Compliance Domains

| Domain | Regulations | Key Requirements |
|--------|-------------|------------------|
| Privacy | GDPR, CCPA, CPRA | Data protection, consent |
| Healthcare | HIPAA, HITECH | PHI protection, BAAs |
| Financial | SOX, FINRA, SEC | Reporting, controls |
| Employment | FLSA, ADA, FMLA | Workplace compliance |
| Industry | Sector-specific | Varies by industry |

### Output Formats

| Output | Format | Use Case |
|--------|--------|----------|
| Compliance Report | Markdown | Board reporting |
| Gap Analysis | Table | Remediation planning |
| Policy Draft | Markdown | Policy updates |
| Audit Checklist | Checklist | Audit preparation |

### Skills Used

- `regulatory-compliance` - Compliance frameworks
- `privacy-law` - Data protection regulations
- `audit-procedures` - Audit methodologies

---

## 2.6 Drafting Assistant

**File:** `.claude/agents/drafting-assistant.md`

```yaml
---
name: drafting-assistant
description: Legal document drafting specialist. Use for creating contracts, agreements, briefs, motions, and corporate documents. Maintains firm style consistency and leverages precedent documents.
model: sonnet
---
```

### Core Capabilities

- **Template Drafting**: Generate from templates
- **Clause Library**: Insert standard clauses
- **Style Consistency**: Enforce firm style guide
- **Precedent Search**: Find similar prior documents
- **Version Control**: Track document revisions
- **Collaboration**: Multi-author support

### Document Types

| Category | Document Types |
|----------|----------------|
| Transactional | NDAs, MSAs, LOIs, Purchase Agreements |
| Corporate | Bylaws, Resolutions, Minutes, Consents |
| Litigation | Complaints, Motions, Briefs, Discovery |
| Employment | Offer Letters, Policies, Separation Agreements |
| IP | License Agreements, Assignments, NDAs |

### Drafting Workflow

```
Template Selection → Variable Input → Clause Selection →
Draft Generation → Style Check → Review & Edit
```

### Output Formats

| Output | Format | Use Case |
|--------|--------|----------|
| Draft Document | Word/Markdown | Client delivery |
| Clause Options | Markdown | Negotiation alternatives |
| Style Report | Markdown | QC review |
| Precedent List | Table | Research reference |

### Skills Used

- `legal-drafting` - Drafting principles
- `contract-law` - Contract requirements
- `legal-writing` - Professional writing

---

## 2.7 Practice Manager

**File:** `.claude/agents/practice-manager.md`

```yaml
---
name: practice-manager
description: Legal practice management specialist. Use for billing management, matter tracking, client communications, and operational tasks. Handles time entries, invoices, matter budgets, and client status updates.
model: haiku
---
```

### Core Capabilities

- **Time Tracking**: Review and optimize time entries
- **Billing Review**: Invoice preparation and review
- **Matter Budgets**: Budget tracking and forecasting
- **Client Communications**: Status updates and reports
- **Deadline Management**: Track critical dates
- **Resource Planning**: Staffing and allocation

### Practice Management Functions

| Function | Description |
|----------|-------------|
| Billing | Time entry review, invoice generation |
| Matters | Status tracking, milestone management |
| Clients | Communication, reporting, relationship |
| Calendar | Deadlines, court dates, meetings |
| Finance | Budgets, forecasts, collections |

### Output Formats

| Output | Format | Use Case |
|--------|--------|----------|
| Client Report | Markdown | Client updates |
| Budget Summary | Table | Financial tracking |
| Time Analysis | Markdown | Billing review |
| Deadline Calendar | Table | Matter management |

### Skills Used

- `practice-management` - Law firm operations
- `legal-billing` - Billing best practices
- `client-relations` - Client service

---

## 2.8 Agent Interaction Matrix

| Scenario | Primary Agent | Supporting Agents |
|----------|---------------|-------------------|
| M&A Due Diligence | contract-analyst | legal-researcher, discovery-agent |
| Litigation Prep | legal-researcher | discovery-agent, drafting-assistant |
| Regulatory Audit | compliance-monitor | contract-analyst, drafting-assistant |
| Contract Negotiation | contract-analyst | drafting-assistant |
| Document Production | discovery-agent | compliance-monitor |
| Client Matter | practice-manager | All as needed |
