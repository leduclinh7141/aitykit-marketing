---
description: Create lead nurturing sequence to convert leads to MQL/SQL
argument-hint: [product-or-service] [target-segment]
---

## Language & Quality Standards

**CRITICAL**: Respond in the same language the user is using. If Vietnamese, respond in Vietnamese. If Spanish, respond in Spanish.

**Standards**: Token efficiency, sacrifice grammar for concision, list unresolved questions at end.

**Skills**: Activate `email-marketing`, `crm-workflow.md`, `sales-workflow.md` skills.

---

## Mission
Create lead nurturing sequence to move leads through funnel:
<context>$ARGUMENTS</context>

## Workflow

1. Use `lead-qualifier` agent to define:
   - Entry criteria (lead score, behavior)
   - Stage progression triggers
   - Exit conditions

2. Use `email-wizard` agent to design:
   - 6-week nurture cadence
   - Content progression (TOFU → MOFU → BOFU)
   - Behavioral triggers

3. Use `copywriter` agent for:
   - Educational content
   - Case study narratives
   - Conversion copy

## Nurture Philosophy
- Lead with value, not pitch
- Match content to buyer journey stage
- Use behavioral triggers, not just time
- Personalize based on engagement

## Agent Delegation
| Task | Agent | Trigger |
|------|-------|---------|
| Entry criteria | `lead-qualifier` | Segment definition |
| Sequence design | `email-wizard` | Nurture campaign |
| Educational content | `copywriter` | Content creation |
| Case studies | `sales-enabler` | Social proof emails |
| Conversion copy | `copywriter` | BOFU content |

## Output Format
```markdown
# Lead Nurture Sequence: [Product/Service]

## Overview
- **Trigger:** Lead score reaches 30+ (Cool threshold) OR [specific action]
- **Goal:** Progress Cool leads (30-49) to MQL (50+) to SQL (70+)
- **Duration:** 6 weeks
- **Target:** [Segment definition]

## Entry Criteria
- Lead score: 30-49 (Cool leads needing nurture to become MQL)
- Has engaged with: [Content type]
- Not yet: Reached MQL threshold (50+)

---

## Week 1: Problem Awareness

### Email 1.1 (Day 0)
**Subject A:** The hidden cost of [problem]
**Subject B:** Why [audience] struggle with [problem]

**Content Focus:** Industry pain points with data

**Body:**
```
Hey {{first_name}},

Did you know that [shocking statistic about problem]?

Most [audience type] face these challenges:
- [Challenge 1]
- [Challenge 2]
- [Challenge 3]

We've put together a guide that breaks down exactly why this happens and what you can do about it.

[BUTTON: Read the Guide]

[Signature]
```

### Email 1.2 (Day 3) - If opened 1.1
**Subject:** [Follow-up on problem topic]
**Content:** Deeper dive into one specific pain point

---

## Week 2: Solution Education

### Email 2.1 (Day 7)
**Subject A:** How to solve [problem] (step-by-step)
**Subject B:** The [X]-step framework for [outcome]

**Content Focus:** Educational how-to content

**Body:**
```
Hey {{first_name}},

Last week we talked about [problem].

Today, let's fix it.

Here's our proven [X]-step framework:

**Step 1: [Step name]**
[Brief explanation]

**Step 2: [Step name]**
[Brief explanation]

**Step 3: [Step name]**
[Brief explanation]

Want the full breakdown with examples?

[BUTTON: Get the Full Guide]

[Signature]
```

---

## Week 3: Social Proof

### Email 3.1 (Day 14)
**Subject A:** How [Company] achieved [specific result]
**Subject B:** "[Result metric]" - See how they did it

**Content Focus:** Case study with metrics

**Body:**
```
Hey {{first_name}},

[Company Name] was struggling with [problem you solve].

Sound familiar?

Here's what happened when they [took action]:

**Before:**
- [Pain point 1]
- [Pain point 2]

**After:**
- [Result 1 with metric]
- [Result 2 with metric]

"[Testimonial quote]"
- [Name], [Title] at [Company]

[BUTTON: Read the Full Case Study]

[Signature]
```

---

## Week 4: Product Introduction

### Email 4.1 (Day 21)
**Subject A:** There's an easier way to [outcome]
**Subject B:** What if [desired outcome] took half the time?

**Content Focus:** Soft product introduction

**Body:**
```
Hey {{first_name}},

Over the past few weeks, we've covered:
- [Topic 1]
- [Topic 2]
- [Topic 3]

Now I want to show you how to put it all together.

[Product Name] helps [audience] [achieve outcome] by:

✓ [Benefit 1]
✓ [Benefit 2]
✓ [Benefit 3]

Curious how it works?

[BUTTON: See How It Works]

[Signature]
```

---

## Week 5: Comparison/Evaluation

### Email 5.1 (Day 28)
**Subject A:** [Your solution] vs [alternative approaches]
**Subject B:** Which [solution type] is right for you?

**Content Focus:** Comparison content, buying guide

**Body:**
```
Hey {{first_name}},

When evaluating [solution type], you have options:

**Option 1: [Alternative 1]**
- Pro: [X]
- Con: [X]

**Option 2: [Alternative 2]**
- Pro: [X]
- Con: [X]

**Option 3: [Your solution]**
- Pro: [Key differentiator]
- Pro: [Key differentiator]

Not sure which is right for you?

[BUTTON: Take the Assessment] or [BUTTON: Talk to an Expert]

[Signature]
```

---

## Week 6: Decision/Offer

### Email 6.1 (Day 35)
**Subject A:** Ready to [achieve outcome]?
**Subject B:** Your next step to [outcome]

**Content Focus:** Clear CTA with offer

**Body:**
```
Hey {{first_name}},

You've been learning about [topic] for a few weeks now.

If you're ready to [achieve outcome], here's your next step:

[OFFER: Free consultation / Demo / Trial]

What you'll get:
- [Benefit 1]
- [Benefit 2]
- [Benefit 3]

No pressure, no commitment - just a conversation about your goals.

[BUTTON: Book Your [Offer]]

[Signature]

P.S. [Urgency element if applicable]
```

### Email 6.2 (Day 38) - If no action
**Subject:** Last chance: [Offer]
**Content:** Final push with deadline/scarcity

---

## Behavioral Triggers

| Trigger | Action |
|---------|--------|
| Visits pricing page | Skip to Week 5, alert sales |
| Downloads case study | Send related case studies |
| High email engagement | Accelerate sequence |
| No opens for 2 weeks | Move to re-engagement |
| Score reaches 50+ | Alert sales, MQL workflow |
| Score reaches 70+ | Immediate sales outreach |

## Exit Conditions
- **Converts:** Books demo/trial/purchase → Exit, move to onboarding
- **Becomes MQL (50+):** Sales handoff, pause marketing emails
- **Unsubscribes:** Remove, add to suppression
- **No engagement:** After week 6, move to re-engagement

## Success Metrics
| Metric | Target |
|--------|--------|
| Open rate | 30%+ |
| Click rate | 3%+ |
| Lead → MQL conversion | 20%+ |
| MQL → SQL conversion | 30%+ |
| Sequence completion | 60%+ |
```
