---
description: Create welcome email sequence for new subscribers
argument-hint: [brand-or-product] [audience]
---

## Language & Quality Standards

**CRITICAL**: Respond in the same language the user is using. If Vietnamese, respond in Vietnamese. If Spanish, respond in Spanish.

**Standards**: Token efficiency, sacrifice grammar for concision, list unresolved questions at end.

**Skills**: Activate `email-marketing`, `marketing-fundamentals`, `crm-workflow.md` skills.

---

## Mission
Create a high-converting welcome email sequence:
<context>$ARGUMENTS</context>

## Workflow

1. Use `email-wizard` agent to design sequence:
   - Timing and triggers
   - Subject line variants (A/B)
   - Email structure

2. Use `copywriter` agent to write:
   - Compelling subject lines
   - Engaging body copy
   - Clear CTAs

3. Use `lead-qualifier` agent to define:
   - Segment triggers
   - Exit conditions
   - Success metrics

## Best Practices
- Complete within 7 days (engagement peaks early)
- First email: immediate (<5 min SLA per speed-to-lead research)
- Progressive value delivery
- Single CTA per email
- Mobile-first design

## Agent Delegation
| Task | Agent | Trigger |
|------|-------|---------|
| Sequence design | `email-wizard` | New sequence request |
| Copy writing | `copywriter` | Email content needed |
| Segment definition | `lead-qualifier` | Entry/exit criteria |
| A/B testing | `email-wizard` | Subject line variants |

## Output Format
```markdown
# Welcome Sequence: [Brand/Product]

## Overview
- **Trigger:** New email signup
- **Goal:** Build trust, deliver value, drive first action
- **Duration:** 7 days (5 emails)
- **Target:** New subscribers

---

## Email 1: Welcome (Immediately)

**Subject A:** Welcome to [Brand]! Here's your [promised value]
**Subject B:** You're in! [Immediate benefit] inside
**Preview:** [First 40 chars of preview text]

**From:** [Name] from [Brand]

**Body:**
```
Hey {{first_name}},

Welcome to [Brand]!

[1 sentence about what they signed up for]

As promised, here's [your lead magnet/promised value]:
[BUTTON: Get Your [Resource]]

Here's what to expect from us:
- [Benefit 1]
- [Benefit 2]
- [Benefit 3]

Talk soon,
[Signature]

P.S. [Curiosity hook for next email]
```

**CTA:** [Primary action button]

---

## Email 2: Quick Win (Day 1)

**Subject A:** [Quick win they can achieve today]
**Subject B:** Try this [timeframe] [topic] tip
**Preview:** [Preview text]

**Body:**
```
Hey {{first_name}},

Quick tip that'll take you 5 minutes:

[Actionable tip with specific steps]

1. [Step 1]
2. [Step 2]
3. [Step 3]

[Why this matters - 1 sentence]

Try it now and hit reply to let me know how it goes.

[Signature]
```

**CTA:** [Action they should take]

---

## Email 3: Brand Story (Day 3)

**Subject A:** Why I started [Brand]
**Subject B:** The story behind [Brand]
**Preview:** [Preview text]

**Body:**
```
Hey {{first_name}},

I want to share something personal with you.

[Origin story - problem you experienced]

[How you solved it]

[Why you're sharing this with them]

That's why [Brand] exists - to help [audience] achieve [outcome].

And that's exactly what I want to help you do.

[Signature]

P.S. Tomorrow I'm sharing [tease next email content]
```

**CTA:** [Optional soft CTA - reply, follow, etc.]

---

## Email 4: Social Proof (Day 5)

**Subject A:** How [Customer] achieved [result]
**Subject B:** "[Quote from testimonial]"
**Preview:** [Preview text]

**Body:**
```
Hey {{first_name}},

Meet [Customer Name].

[Brief backstory - their situation before]

Then they [action they took with your product/service].

The result?
- [Result 1]
- [Result 2]
- [Result 3]

"[Testimonial quote]" - [Customer Name], [Title]

Ready to get similar results?

[BUTTON: [CTA related to customer journey]]

[Signature]
```

**CTA:** [Primary conversion action]

---

## Email 5: Engagement (Day 7)

**Subject A:** Quick question, {{first_name}}
**Subject B:** I'd love your input
**Preview:** [Preview text]

**Body:**
```
Hey {{first_name}},

I want to make sure I'm sending you stuff you actually care about.

Quick question - what's your biggest challenge with [topic]?

[ ] [Option 1]
[ ] [Option 2]
[ ] [Option 3]
[ ] Something else: ___

[BUTTON: Tell Me]

Your answer helps me send you more relevant content.

Thanks!
[Signature]
```

**CTA:** Survey/preference center link

---

## Exit Conditions
- **Goal achieved:** Subscriber takes primary action (purchase, demo, trial)
- **Unsubscribe:** Remove from sequence, add to suppression
- **No engagement after email 5:** Move to re-engagement sequence after 14 days

## Success Metrics
| Metric | Target | Alert If |
|--------|--------|----------|
| Email 1 Open Rate | 60%+ | <40% |
| Sequence Open Rate | 40%+ | <25% |
| Click Rate | 5%+ | <2% |
| Unsubscribe Rate | <1% | >2% |
| Conversion to [Goal] | 10%+ | <5% |

## Automation Logic
```
ON signup:
  → Send Email 1 (immediate)
  → Wait 1 day
  → IF opened Email 1:
      → Send Email 2
    ELSE:
      → Resend Email 1 with Subject B
      → Wait 1 day → Send Email 2
  → Wait 2 days → Send Email 3
  → Wait 2 days → Send Email 4
  → Wait 2 days → Send Email 5

ON conversion at any point:
  → Exit sequence
  → Move to [next appropriate sequence]
```
```
