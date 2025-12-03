---
description: Create re-engagement sequence for inactive contacts
argument-hint: [brand-or-product] [inactive-criteria]
---

Activate `email-marketing`, `crm-workflow.md` skills.

## Mission
Create win-back sequence for inactive contacts:
<context>$ARGUMENTS</context>

## Workflow

1. Use `continuity-specialist` agent to:
   - Define inactivity criteria
   - Segment by last engagement
   - Plan win-back strategy

2. Use `email-wizard` agent to design:
   - 21-day re-engagement cadence
   - Escalating urgency
   - Breakup email

3. Use `copywriter` agent for:
   - Attention-grabbing subject lines
   - Emotional reconnection copy
   - Clear value proposition

## Re-engagement Philosophy
- Lead with value, not guilt
- Remind them why they subscribed
- Give easy way to re-engage or leave
- Clean list if no response (GDPR compliant)

## Agent Delegation
| Task | Agent | Trigger |
|------|-------|---------|
| Inactivity criteria | `continuity-specialist` | Segment definition |
| Sequence design | `email-wizard` | Win-back campaign |
| Win-back copy | `copywriter` | Emotional reconnection |
| Offer strategy | `upsell-maximizer` | Incentive design |
| List hygiene | `lead-qualifier` | Post-sequence cleanup |

## Output Format
```markdown
# Re-engagement Sequence: [Brand/Product]

## Overview
- **Trigger:** No email engagement for 30+ days
- **Goal:** Win back or clean list
- **Duration:** 21 days (5 emails)
- **Target:** Inactive subscribers

## Entry Criteria
- No email opens: 30+ days
- No website visits: 30+ days
- No purchases: 90+ days (if applicable)
- Previously engaged at least once

---

## Email 1: We Miss You (Day 0)

**Subject A:** We miss you, {{first_name}}
**Subject B:** It's been a while...
**Subject C:** 👋 Hey stranger

**Preview:** We noticed you've been quiet lately

**Body:**
```
Hey {{first_name}},

We noticed it's been a while since we've heard from you.

Life gets busy - we get it.

But we've been working on some things we think you'll love:

- [New feature/content 1]
- [New feature/content 2]
- [New feature/content 3]

Want to catch up?

[BUTTON: See What's New]

If your interests have changed, no hard feelings - you can update your preferences anytime.

[LINK: Update Preferences]

[Signature]
```

---

## Email 2: Best Content (Day 3)

**Subject A:** You might have missed this
**Subject B:** Our most popular [content type] this month
**Subject C:** [X] people loved this - you might too

**Preview:** Top content you haven't seen yet

**Body:**
```
Hey {{first_name}},

While you were away, here's what people loved most:

**#1 Most Popular:**
[Content title with brief description]
[LINK: Read/Watch/Listen]

**#2 Reader Favorite:**
[Content title with brief description]
[LINK: Read/Watch/Listen]

**#3 Most Shared:**
[Content title with brief description]
[LINK: Read/Watch/Listen]

Any of these catch your eye?

[Signature]
```

---

## Email 3: Special Offer (Day 7)

**Subject A:** A little something for you, {{first_name}}
**Subject B:** We'd love you back (here's why)
**Subject C:** [X% off / Free gift] - just for you

**Preview:** Exclusive offer for returning subscribers

**Body:**
```
Hey {{first_name}},

We want to make it easy to reconnect.

Here's an exclusive offer just for you:

[OFFER BOX]
[Discount / Free trial / Bonus content]
Code: WELCOME BACK
Expires: [Date]
[/OFFER BOX]

[BUTTON: Claim Your Offer]

No strings attached - just our way of saying we'd love to have you back.

[Signature]
```

---

## Email 4: Feedback Request (Day 14)

**Subject A:** Quick question, {{first_name}}
**Subject B:** Did we do something wrong?
**Subject C:** 30 seconds of your time?

**Preview:** We'd love your honest feedback

**Body:**
```
Hey {{first_name}},

I'll be honest - I'm wondering if we've been sending you the wrong stuff.

Mind helping me out with one quick question?

**Why haven't you been opening our emails?**

[ ] Too many emails
[ ] Content isn't relevant
[ ] I'm just busy right now
[ ] I'm no longer interested in [topic]
[ ] Other: ___

[BUTTON: Tell Us (30 sec)]

Your answer helps us do better - for you and everyone else.

Thanks,
[Signature]
```

---

## Email 5: Breakup (Day 21)

**Subject A:** Should we stop emailing you?
**Subject B:** This is goodbye (unless...)
**Subject C:** Last email from us?

**Preview:** We'll remove you unless you want to stay

**Body:**
```
Hey {{first_name}},

I don't want to be that brand that clutters your inbox.

Since we haven't heard from you, I'm going to remove you from our list.

**But if you want to stay:**

[BUTTON: Yes, Keep Me Subscribed]

No action needed if you'd like to go - we'll remove you automatically in 7 days.

Either way, no hard feelings. Thanks for being part of our community.

[Signature]

P.S. You can always come back anytime at [website].
```

---

## Post-Sequence Actions

**If re-engaged (opened/clicked):**
- Reset engagement score
- Move to appropriate nurture sequence
- Tag as "re-engaged"

**If no response after breakup:**
- Wait 7 days
- Move to "Inactive" segment
- Suppress from all campaigns
- Keep for transactional emails only

**If clicked "Keep Me Subscribed":**
- Reset engagement score
- Send "Welcome Back" confirmation
- Move to main nurture sequence

## Success Metrics
| Metric | Target |
|--------|--------|
| Re-engagement rate | 10-15% |
| Open rate (this sequence) | 15%+ |
| Preference updates | 5%+ |
| Clean unsubscribes | 20-30% |
| List hygiene improvement | Remove 20%+ inactive |

## Segmentation Tips
| Inactive Period | Treatment |
|-----------------|-----------|
| 30-60 days | Standard re-engagement |
| 60-90 days | Aggressive offer |
| 90+ days | Direct to breakup |
| Never engaged | Remove immediately |
```
