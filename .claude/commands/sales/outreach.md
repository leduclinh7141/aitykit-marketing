---
description: Generate personalized outreach sequence
argument-hint: [prospect-info] [sequence-type]
---

## Language & Quality Standards

**CRITICAL**: Respond in the same language the user is using. If Vietnamese, respond in Vietnamese. If Spanish, respond in Spanish.

**Standards**: Token efficiency, sacrifice grammar for concision, list unresolved questions at end.

**Skills**: Activate `sales-workflow.md` and `email-marketing` skill.

---

## Mission
Create a personalized outreach sequence for:
<prospect>$ARGUMENTS</prospect>

## Workflow

1. Use `researcher` agent to research the prospect:
   - Recent company news
   - LinkedIn activity
   - Pain points in their industry
   - Mutual connections

2. Determine sequence type:
   - **Cold:** No prior engagement (7 touches, 21 days)
   - **Warm:** Some engagement (5 touches, 14 days)
   - **Hot:** High intent shown (3 touches, 7 days)

3. Use `sales-enabler` agent to create sequence:
   - Personalized subject lines
   - Value-focused email copy
   - Strategic follow-ups
   - LinkedIn touchpoints
   - Breakup email

4. Use `copywriter` agent to refine messaging:
   - Hook optimization
   - CTA clarity
   - Personalization tokens

## Output Format
```markdown
# Outreach Sequence: [Prospect Name] @ [Company]

## Prospect Research
- Company: [Details]
- Role: [Details]
- Pain Points: [Identified]
- Personalization Hook: [What to reference]

## Sequence Type: [Cold/Warm/Hot]

### Day 1: Initial Email
**Subject:** [Subject line]
**Body:**
[Full email copy]

### Day 3: Follow-up
**Subject:** [Subject line]
**Body:**
[Full email copy]

### Day 5: LinkedIn
**Action:** [Connect/Message/Engage]
**Message:**
[Message copy]

[Continue for full sequence...]

### Final: Breakup Email
**Subject:** [Subject line]
**Body:**
[Full email copy]
```
