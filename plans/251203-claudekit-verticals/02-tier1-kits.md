# Part 2: Tier 1 Kits (High Priority)

## Priority Criteria

- Market size > $8B
- Adoption rate > 40%
- Clear agent architecture
- Existing demand signals

---

## 2.1 ClaudeKit Marketing ✅ (In Progress)

**Target:** Marketing teams, agencies, growth marketers
**TAM:** $15B+
**Status:** Plan complete, ready for implementation

### Agent Architecture

| Agent | Stage | Function |
|-------|-------|----------|
| attraction-specialist | TOFU | SEO, keywords, landing pages |
| lead-qualifier | MOFU | Scoring, segmentation |
| email-wizard | MOFU | Sequences, personalization |
| sales-enabler | BOFU | Collateral, pitches |
| continuity-specialist | Retention | Churn, re-engagement |
| upsell-maximizer | Expansion | Cross-sell, upsell |

### Key Commands

`/campaign:*`, `/seo:*`, `/content:*`, `/leads:*`, `/analytics:*`, `/social:*`

### MCP Integrations

Meta Ads, Google Ads, GA4, Search Console, Discord, Slack, Stripe, TikTok

---

## 2.2 ClaudeKit Legal

**Target:** Law firms, in-house legal, paralegals
**TAM:** $10.82B by 2030
**Competition:** Harvey ($100-500/user), Spellbook (4,000+ firms)

### Market Data

- 23% of lawyer tasks automatable now
- AI-first legal practice tipping point in 2025
- Multi-step, cross-app agents replacing single-task tools

### Agent Architecture

| Agent | Function | Key Tasks |
|-------|----------|-----------|
| **contract-analyst** | Contract review | Clause extraction, risk flagging, redlining |
| **legal-researcher** | Case research | Precedent search, citation analysis, memo drafting |
| **discovery-agent** | E-discovery | Document review, privilege detection, deposition prep |
| **compliance-monitor** | Regulatory | HIPAA/GDPR review, policy updates, audit prep |
| **billing-optimizer** | Practice mgmt | Time tracking, invoice review, matter budgeting |
| **client-communicator** | Client relations | Status updates, intake, scheduling |

### Key Commands

```
/contract:review [file]      - Review contract for risks
/contract:draft [type]       - Draft contract from template
/contract:compare [a] [b]    - Compare contract versions
/research:case [query]       - Research case law
/research:statute [topic]    - Research statutes/regulations
/discovery:review [docs]     - Review document batch
/discovery:privilege [docs]  - Privilege review
/compliance:audit [area]     - Compliance audit
/compliance:policy [type]    - Generate/update policy
/billing:review [matter]     - Review billing for matter
/client:intake [type]        - Client intake workflow
/client:update [matter]      - Generate client status update
```

### Skills

```
legal-fundamentals/
├── contract-law.md
├── litigation-process.md
├── legal-research.md
└── legal-writing.md

compliance/
├── hipaa.md
├── gdpr.md
├── sox.md
└── industry-regs.md

practice-management/
├── matter-management.md
├── billing-best-practices.md
└── client-relations.md
```

### MCP Integrations

- Westlaw/LexisNexis (research)
- Clio/MyCase (practice management)
- NetDocuments/iManage (document management)
- DocuSign (e-signatures)

---

## 2.3 ClaudeKit Finance

**Target:** CFOs, accountants, FP&A teams, bookkeepers
**TAM:** $8B+
**Competition:** Basis, Vic.ai, Truewind, Maximor

### Market Data

- Only 34% using AI agents in accounting/finance (huge gap!)
- 79% of executives adopting AI agents overall
- Month-end close reduced 50%+ with AI

### Agent Architecture

| Agent | Function | Key Tasks |
|-------|----------|-----------|
| **bookkeeper** | Transaction mgmt | Categorization, reconciliation, journal entries |
| **invoice-processor** | AP/AR | Invoice extraction, PO matching, payment scheduling |
| **financial-analyst** | Analysis | Variance analysis, forecasting, modeling |
| **budget-planner** | Planning | Budget creation, scenario modeling, allocation |
| **compliance-checker** | Audit/tax | GAAP compliance, audit prep, tax documentation |
| **cash-manager** | Treasury | Cash flow forecasting, position consolidation |

### Key Commands

```
/books:reconcile [account]   - Reconcile account
/books:categorize [txns]     - Categorize transactions
/books:close [period]        - Month-end close checklist
/invoice:process [file]      - Process invoice
/invoice:approve [id]        - Invoice approval workflow
/invoice:pay [batch]         - Payment batch processing
/analysis:variance [period]  - Variance analysis report
/analysis:forecast [metric]  - Financial forecast
/analysis:model [scenario]   - Financial modeling
/budget:create [period]      - Create budget
/budget:track [dept]         - Budget vs actual tracking
/compliance:audit-prep       - Audit preparation checklist
/compliance:tax-docs         - Tax documentation
/cash:forecast [period]      - Cash flow forecast
/cash:position               - Current cash position
```

### Skills

```
accounting-fundamentals/
├── gaap-principles.md
├── journal-entries.md
├── reconciliation.md
└── financial-statements.md

financial-analysis/
├── variance-analysis.md
├── forecasting-methods.md
├── financial-modeling.md
└── kpi-metrics.md

compliance-audit/
├── audit-preparation.md
├── internal-controls.md
├── tax-compliance.md
└── regulatory-reporting.md
```

### MCP Integrations

- QuickBooks/Xero (accounting)
- Stripe/Square (payments)
- Plaid (banking data)
- Ramp/Brex (expense management)

---

## 2.4 ClaudeKit Sales

**Target:** Sales teams, SDRs, AEs, sales managers
**TAM:** $12B+
**Competition:** Outreach, Salesloft, Gong, Apollo

### Market Data

- Sales enablement AI growing 40%+ annually
- SDR automation highest ROI use case
- Multi-channel outreach becoming standard

### Agent Architecture

| Agent | Function | Key Tasks |
|-------|----------|-----------|
| **prospector** | Lead gen | ICP matching, list building, enrichment |
| **outreach-specialist** | SDR tasks | Email sequences, call scripts, LinkedIn messages |
| **meeting-prep** | Pre-call | Account research, stakeholder mapping, agenda |
| **deal-analyst** | Pipeline | Deal scoring, forecast, risk identification |
| **proposal-writer** | Closing | Proposals, pricing, contracts |
| **success-handoff** | Post-sale | Onboarding docs, success plans, handoff notes |

### Key Commands

```
/prospect:build [icp]        - Build prospect list
/prospect:enrich [list]      - Enrich prospect data
/prospect:qualify [lead]     - Qualify lead against ICP
/outreach:sequence [persona] - Create outreach sequence
/outreach:email [context]    - Write personalized email
/outreach:linkedin [profile] - LinkedIn message
/outreach:call [account]     - Call script/talking points
/meeting:prep [account]      - Pre-meeting research
/meeting:agenda [type]       - Meeting agenda
/meeting:followup [notes]    - Post-meeting follow-up
/deal:score [opp]            - Score deal probability
/deal:forecast [pipeline]    - Pipeline forecast
/deal:risk [opp]             - Deal risk analysis
/proposal:create [opp]       - Create proposal
/proposal:pricing [config]   - Pricing configuration
/handoff:success [account]   - Success team handoff
/handoff:onboard [account]   - Onboarding documentation
```

### Skills

```
sales-fundamentals/
├── sales-methodology.md     # MEDDIC, BANT, Challenger
├── objection-handling.md
├── negotiation.md
└── closing-techniques.md

prospecting/
├── icp-definition.md
├── list-building.md
├── cold-outreach.md
└── social-selling.md

deal-management/
├── pipeline-management.md
├── forecasting.md
├── proposal-writing.md
└── contract-negotiation.md
```

### MCP Integrations

- Salesforce/HubSpot (CRM)
- Apollo/ZoomInfo (prospecting)
- Outreach/Salesloft (engagement)
- LinkedIn (social)
- Gong/Chorus (call intelligence)

---

## 2.5 Tier 1 Summary

| Kit | Agents | Commands | Skills | MCP Integrations |
|-----|--------|----------|--------|------------------|
| Marketing | 6 | 28 | 8 | 10 |
| Legal | 6 | 12 | 3 | 4 |
| Finance | 6 | 15 | 3 | 4 |
| Sales | 6 | 17 | 3 | 5 |

### Development Priority

1. **Marketing** - Already planned, implement first
2. **Sales** - Highest demand, clear architecture
3. **Finance** - Biggest adoption gap (34% vs 79%)
4. **Legal** - High TAM, premium pricing potential
