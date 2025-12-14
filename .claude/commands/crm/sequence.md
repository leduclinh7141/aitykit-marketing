---
description: Create automated email sequence
argument-hint: [sequence-type] [target-segment]
---

## Language & Quality Standards

**CRITICAL**: Respond in the same language the user is using. If Vietnamese, respond in Vietnamese. If Spanish, respond in Spanish.

**Standards**: Token efficiency, sacrifice grammar for concision, list unresolved questions at end.

**Skills**: Activate `crm-workflow.md` and `email-marketing` skill.

---

## Mission
Create an automated email sequence:
<context>$ARGUMENTS</context>

## Sequence Types
- `welcome` - New subscriber onboarding
- `nurture` - Lead nurturing to MQL
- `onboarding` - New customer success
- `re-engage` - Win back inactive contacts
- `upsell` - Expansion opportunities

## Workflow

1. Identify sequence type and goal
2. Use `email-wizard` agent to design sequence:
   - Email timing and triggers
   - Subject lines (A/B variants)
   - Body copy with personalization
   - CTAs for each stage

3. Use `copywriter` agent to refine:
   - Compelling hooks
   - Value-focused content
   - Clear next steps

## Output Format
```markdown
# [Sequence Type] Sequence

## Overview
- **Trigger:** [What starts this sequence]
- **Goal:** [Desired outcome]
- **Duration:** [X days/emails]
- **Target:** [Segment criteria]

## Sequence Flow

### Email 1: [Name] (Day 0)
**Trigger:** [Trigger event]
**Subject A:** [Subject line]
**Subject B:** [A/B variant]
**Preview:** [Preview text]

**Body:**
[Full email copy with {{personalization}} tokens]

**CTA:** [Button text and action]

---

### Email 2: [Name] (Day X)
**Trigger:** [Time/action trigger]
**Subject A:** [Subject line]
**Subject B:** [A/B variant]

**Body:**
[Full email copy]

**CTA:** [Button text and action]

---

[Continue for all emails...]

## Exit Conditions
- [Condition 1]: Move to [next sequence/segment]
- [Condition 2]: Mark as [status]

## Success Metrics
- Open rate target: X%
- Click rate target: X%
- Conversion goal: [Specific action]
```
