---
description: Qualify a lead using BANT/MEDDIC frameworks
argument-hint: [lead-info-or-company]
---

## Language & Quality Standards

**CRITICAL**: Respond in the same language the user is using. If Vietnamese, respond in Vietnamese. If Spanish, respond in Spanish.

**Standards**: Token efficiency, sacrifice grammar for concision, list unresolved questions at end.

**Skills**: Activate `sales-workflow.md` and `marketing-fundamentals` skill.

---

## Mission
Qualify this lead using BANT (SMB) or MEDDIC (Enterprise) framework:
<lead>$ARGUMENTS</lead>

## Workflow

1. Use `researcher` agent to gather company information:
   - Company size, industry, location
   - Recent news and funding
   - Tech stack (if B2B SaaS)
   - Decision makers on LinkedIn

2. Use `lead-qualifier` agent to score using appropriate framework:

   **BANT (0-100) - For SMB/Mid-Market:**
   - Budget (0-25): Can they afford it?
   - Authority (0-25): Is this the decision maker?
   - Need (0-25): Do they have the problem we solve?
   - Timeline (0-25): When do they need a solution?

   **MEDDIC (0-100) - For Enterprise:**
   - Metrics (0-17): Quantifiable goals
   - Economic Buyer (0-17): Person with budget authority
   - Decision Criteria (0-17): Evaluation criteria
   - Decision Process (0-17): How they buy
   - Identify Pain (0-16): Core business problems
   - Champion (0-16): Internal advocate

3. Determine lead temperature (unified thresholds):
   - 70-100: 🔥 Hot - Immediate outreach (<5 min SLA)
   - 50-69: 🌡️ Warm - Priority follow-up (<1 hr SLA)
   - 30-49: ❄️ Cool - Accelerated nurture (<24 hr SLA)
   - 0-29: 🧊 Cold - Marketing nurture only

4. Generate output:
   - BANT/MEDDIC scorecard
   - Recommended next action
   - Talking points for outreach
   - Relevant case studies to share

## Output Format
```markdown
# Lead Qualification: [Company Name]

## Framework: [BANT/MEDDIC]
## Total Score: [X]/100

### BANT Scorecard (if SMB/Mid-Market)
| Criteria | Score | Evidence |
|----------|-------|----------|
| Budget | X/25 | [Notes] |
| Authority | X/25 | [Notes] |
| Need | X/25 | [Notes] |
| Timeline | X/25 | [Notes] |

### MEDDIC Scorecard (if Enterprise)
| Criteria | Score | Evidence |
|----------|-------|----------|
| Metrics | X/17 | [Notes] |
| Economic Buyer | X/17 | [Notes] |
| Decision Criteria | X/17 | [Notes] |
| Decision Process | X/17 | [Notes] |
| Identify Pain | X/16 | [Notes] |
| Champion | X/16 | [Notes] |

## Lead Temperature: [🔥 Hot / 🌡️ Warm / ❄️ Cool / 🧊 Cold]
## Response SLA: [<5 min / <1 hr / <24 hr / Standard]

## Recommended Action
[Specific next step with urgency level]

## Talking Points
1. [Point 1]
2. [Point 2]
3. [Point 3]

## Relevant Case Studies
- [Case study 1]
- [Case study 2]
```
