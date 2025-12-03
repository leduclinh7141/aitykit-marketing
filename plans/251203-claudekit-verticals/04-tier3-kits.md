# Part 4: Tier 3 Kits (Lower Priority)

## Priority Criteria

- Market size $2-4B
- Emerging adoption (<30%)
- Niche use cases
- Less competition

---

## 4.1 ClaudeKit Healthcare

**Target:** Clinics, medical practices, health admin
**TAM:** $7B+
**Note:** Compliance-heavy, requires careful implementation

### Agent Architecture

| Agent | Function |
|-------|----------|
| **documentation-assistant** | Clinical notes, visit summaries |
| **scheduling-optimizer** | Appointment optimization |
| **billing-coder** | Medical coding, claims |
| **patient-communicator** | Reminders, follow-ups |
| **compliance-monitor** | HIPAA, regulations |

### Key Commands

`/docs:visit-note`, `/docs:referral`, `/schedule:optimize`, `/billing:code`, `/patient:reminder`, `/compliance:check`

### Considerations

- HIPAA compliance critical
- Medical accuracy requirements
- Integration with EHR systems
- Liability concerns

---

## 4.2 ClaudeKit Real Estate

**Target:** Agents, brokers, property managers
**TAM:** $3B+

### Agent Architecture

| Agent | Function |
|-------|----------|
| **listing-writer** | Property descriptions, MLS |
| **market-analyst** | Comps, valuations, trends |
| **lead-nurturer** | Buyer/seller follow-up |
| **transaction-coordinator** | Docs, deadlines, checklists |
| **property-manager** | Tenant comms, maintenance |

### Key Commands

`/listing:write`, `/listing:photos`, `/market:comps`, `/market:value`, `/lead:nurture`, `/transaction:checklist`, `/property:lease`

---

## 4.3 ClaudeKit Consulting

**Target:** Consultants, freelancers, coaches
**TAM:** $2B+

### Agent Architecture

| Agent | Function |
|-------|----------|
| **proposal-writer** | Proposals, SOWs, contracts |
| **research-analyst** | Industry research, benchmarks |
| **deliverable-creator** | Reports, presentations, frameworks |
| **client-manager** | Status updates, scheduling |
| **knowledge-builder** | Templates, playbooks, IP |

### Key Commands

`/proposal:create`, `/proposal:scope`, `/research:industry`, `/research:benchmark`, `/deliverable:report`, `/deliverable:deck`, `/client:update`

---

## 4.4 ClaudeKit Operations

**Target:** Ops teams, SMBs, startups
**TAM:** $4B+

### Agent Architecture

| Agent | Function |
|-------|----------|
| **process-documenter** | SOPs, workflows, runbooks |
| **project-tracker** | Status, dependencies, risks |
| **meeting-assistant** | Agendas, notes, action items |
| **vendor-manager** | Contracts, negotiations, reviews |
| **data-analyst** | Reports, dashboards, insights |

### Key Commands

`/ops:sop`, `/ops:workflow`, `/project:status`, `/project:risk`, `/meeting:agenda`, `/meeting:notes`, `/vendor:review`, `/data:report`

---

## 4.5 ClaudeKit Customer Success

**Target:** CS teams, account managers
**TAM:** $3B+

### Agent Architecture

| Agent | Function |
|-------|----------|
| **health-monitor** | Account health scoring |
| **qbr-preparer** | Business reviews |
| **renewal-manager** | Renewal playbooks |
| **expansion-finder** | Upsell opportunities |
| **advocate-builder** | References, case studies |

### Key Commands

`/health:score`, `/health:alert`, `/qbr:prep`, `/qbr:deck`, `/renewal:plan`, `/expansion:identify`, `/advocate:request`

---

## 4.6 ClaudeKit Product

**Target:** Product managers, product teams
**TAM:** $2B+

### Agent Architecture

| Agent | Function |
|-------|----------|
| **prd-writer** | Requirements, specs |
| **user-researcher** | Interview guides, synthesis |
| **roadmap-planner** | Prioritization, planning |
| **release-manager** | Release notes, comms |
| **metrics-analyst** | Product analytics |

### Key Commands

`/prd:write`, `/prd:spec`, `/research:interview`, `/research:synthesis`, `/roadmap:plan`, `/roadmap:prioritize`, `/release:notes`

---

## 4.7 Tier 3 Summary

| Kit | Agents | Primary Use Case |
|-----|--------|------------------|
| Healthcare | 5 | Clinical documentation |
| Real Estate | 5 | Listings & transactions |
| Consulting | 5 | Proposals & deliverables |
| Operations | 5 | SOPs & project tracking |
| Customer Success | 5 | Health monitoring & QBRs |
| Product | 5 | PRDs & roadmaps |

### Development Notes

- Lower priority due to smaller TAM or complexity
- Can be developed based on demand signals
- Healthcare requires compliance expertise
- May combine some kits (Ops + Product)
