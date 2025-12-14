---
description: Content approval workflow for team collaboration
argument-hint: [content-type] [approvers]
---

## Language & Quality Standards

**CRITICAL**: Respond in the same language the user is using. If Vietnamese, respond in Vietnamese. If Spanish, respond in Spanish.

**Standards**: Token efficiency, sacrifice grammar for concision, list unresolved questions at end.

**Skills**: Activate `content-strategy`, `marketing-fundamentals`, `crm-workflow.md`, `sales-workflow.md` skills.

---

## Mission
Generate content approval workflow:
<context>$ARGUMENTS</context>

## Agent Delegation
| Task | Agent | Trigger |
|------|-------|---------|
| Content creation | `copywriter` | Draft stage |
| SEO review | `attraction-specialist` | Optimization |
| Quality check | `researcher` | Fact verification |
| Final polish | `copywriter` | Revisions |

## Output Format
```markdown
# Content Approval Workflow

## Workflow Stages

```
Draft → Review → Revisions → Approval → Schedule → Publish
```

| Stage | Owner | SLA | Exit Criteria |
|-------|-------|-----|---------------|
| Draft | Creator | 2-3 days | First draft complete |
| Review | Reviewer | 24 hours | Feedback provided |
| Revisions | Creator | 24 hours | Changes implemented |
| Approval | Approver | 24 hours | Sign-off received |
| Schedule | Publisher | Same day | Content queued |
| Publish | System | Scheduled | Live and verified |

---

## Stage 1: Draft Creation

### Creator Checklist
- [ ] Brief reviewed and understood
- [ ] Target audience defined
- [ ] Key messages included
- [ ] SEO keywords incorporated
- [ ] CTA clear and compelling
- [ ] Sources cited (if applicable)
- [ ] Images/media selected
- [ ] Internal links added
- [ ] Word count meets target
- [ ] Self-review complete

### Draft Requirements
| Element | Requirement | Check |
|---------|-------------|-------|
| Title | Compelling, includes keyword | ☐ |
| Meta description | 150-160 chars, includes CTA | ☐ |
| Introduction | Hook + value promise | ☐ |
| Body | Structured, scannable | ☐ |
| Conclusion | Summary + CTA | ☐ |
| Images | Relevant, optimized | ☐ |

---

## Stage 2: Review Process

### Reviewer Roles

**Content Reviewer (Required)**
- [ ] Accuracy and factual correctness
- [ ] Brand voice consistency
- [ ] Message clarity
- [ ] Grammar and spelling
- [ ] Logical flow
- [ ] Value delivery

**SEO Reviewer (Required for blogs/pages)**
- [ ] Primary keyword placement
- [ ] Secondary keywords included
- [ ] Header structure (H1, H2, H3)
- [ ] Internal linking
- [ ] Meta tags optimized
- [ ] Image alt text

**Legal/Compliance (If needed)**
- [ ] Claims substantiated
- [ ] Disclaimers included
- [ ] Copyright clearance
- [ ] Privacy compliance
- [ ] Industry regulations met

**Subject Matter Expert (If needed)**
- [ ] Technical accuracy
- [ ] Industry terminology
- [ ] Best practices reflected

### Feedback Format
```
## Review: [Content Title]
**Reviewer:** [Name]
**Date:** [Date]
**Status:** Approved / Needs Revisions

### Must Fix (Blocking)
1. [Issue + suggested fix]
2. [Issue + suggested fix]

### Should Fix (Important)
1. [Suggestion]
2. [Suggestion]

### Nice to Have (Optional)
1. [Enhancement idea]

### What Works Well
- [Positive feedback]
```

---

## Stage 3: Revisions

### Creator Actions
- [ ] Address all "Must Fix" items
- [ ] Consider "Should Fix" suggestions
- [ ] Note any disagreements with rationale
- [ ] Update version number
- [ ] Request re-review if major changes

### Version Control
| Version | Date | Changes | Status |
|---------|------|---------|--------|
| v1.0 | | Initial draft | Review |
| v1.1 | | Revisions | Review |
| v2.0 | | Final | Approved |

---

## Stage 4: Final Approval

### Approver Checklist
- [ ] All feedback addressed
- [ ] Brand guidelines followed
- [ ] Quality standards met
- [ ] Legal requirements satisfied
- [ ] Ready for publication

### Approval Record
```
Content: [Title]
Approved by: [Name]
Date: [Date]
Publication date: [Date]
Notes: [Any conditions]
```

---

## Stage 5: Scheduling & Publishing

### Pre-Publish Checklist
- [ ] Final proofread complete
- [ ] All links tested
- [ ] Images uploaded correctly
- [ ] SEO fields populated
- [ ] Categories/tags assigned
- [ ] Author assigned
- [ ] Publish date/time set
- [ ] Social sharing enabled
- [ ] Email notification configured

### Post-Publish Verification
- [ ] Page loads correctly
- [ ] Mobile display verified
- [ ] Links working
- [ ] Forms functional
- [ ] Analytics tracking
- [ ] Social sharing works

---

## Content Types & Requirements

| Type | Reviewers | Approval | SLA |
|------|-----------|----------|-----|
| Blog Post | Content + SEO | Marketing Lead | 3 days |
| Social Post | Content | Social Manager | Same day |
| Email | Content + Legal | Email Manager | 2 days |
| Landing Page | Content + SEO + Legal | Marketing Lead | 5 days |
| Case Study | Content + SME + Legal | Director | 7 days |
| Press Release | Content + Legal + Exec | CEO/CMO | 5 days |
| Ad Copy | Content + Legal | Ads Manager | 2 days |

---

## Escalation Process

| Situation | Action | Escalate To |
|-----------|--------|-------------|
| Missed SLA | Notify stakeholders | Team Lead |
| Disagreement | Document + discuss | Manager |
| Urgent content | Fast-track process | Director |
| Legal concern | Hold publication | Legal Team |
| Brand risk | Stop and review | CMO |

---

## Quality Standards

### Writing Quality
- Clear, concise language
- Active voice preferred
- No jargon (unless audience-appropriate)
- Proper grammar and punctuation
- Consistent formatting

### Brand Alignment
- Tone matches brand voice
- Visual style consistent
- Messaging on-brand
- Values reflected

### SEO Standards
- Target keyword density 1-2%
- Minimum 300 words (ideally 1500+)
- Proper heading hierarchy
- Internal links (3-5 minimum)
- External links to authority sources
```
