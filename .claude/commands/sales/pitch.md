---
description: Generate customized sales pitch
argument-hint: [prospect-company] [use-case]
---

## Language & Quality Standards

**CRITICAL**: Respond in the same language the user is using. If Vietnamese, respond in Vietnamese. If Spanish, respond in Spanish.

**Standards**: Token efficiency, sacrifice grammar for concision, list unresolved questions at end.

**Skills**: Activate `sales-workflow.md` skill.

---

## Mission
Create a customized sales pitch for:
<context>$ARGUMENTS</context>

## Workflow

1. Use `researcher` agent to understand prospect:
   - Industry challenges
   - Company-specific pain points
   - Decision maker priorities
   - Budget indicators

2. Use `sales-enabler` agent to create pitch:
   - Problem statement (their world)
   - Solution overview (our approach)
   - Proof points (relevant results)
   - Differentiation (why us)
   - Call to action (next step)

3. Use `copywriter` agent to polish:
   - Compelling narrative
   - Clear value proposition
   - Memorable hooks

## Output Format
```markdown
# Sales Pitch: [Prospect Company]

## Opening Hook (30 seconds)
[Attention-grabbing statement about their pain]

## Problem Statement (1 minute)
[Describe their current situation and challenges]

## Solution Overview (2 minutes)
[How we solve this problem]

### Key Benefits
1. [Benefit 1 + metric]
2. [Benefit 2 + metric]
3. [Benefit 3 + metric]

## Social Proof (1 minute)
[Relevant case study summary]

> "[Quote from similar customer]"
> Results: [Specific metrics achieved]

## Why Us (1 minute)
[Key differentiators for this prospect]

## Investment Overview
[Pricing context without hard numbers if unknown]

## Call to Action
[Specific next step with timeline]

---

## Appendix: Objection Responses

**If they say "[Objection 1]":**
> [Response]

**If they say "[Objection 2]":**
> [Response]

## Questions to Ask
1. [Discovery question 1]
2. [Discovery question 2]
3. [Qualifying question]
```
