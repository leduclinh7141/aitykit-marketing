---
description: Create competitive battlecard
argument-hint: [competitor-name-or-url]
---

## Language & Quality Standards

**CRITICAL**: Respond in the same language the user is using. If Vietnamese, respond in Vietnamese. If Spanish, respond in Spanish.

**Standards**: Token efficiency, sacrifice grammar for concision, list unresolved questions at end.

**Skills**: Activate `sales-workflow.md` and `marketing-fundamentals` skill.

---

## Mission
Create a competitive battlecard for:
<competitor>$ARGUMENTS</competitor>

## Workflow

1. Use `researcher` agent to analyze competitor:
   - Product features and pricing
   - Target market and positioning
   - Strengths and weaknesses
   - Customer reviews and complaints
   - Recent news and updates

2. Use `sales-enabler` agent to create battlecard:
   - Side-by-side comparison
   - Win/loss scenarios
   - Objection handling
   - Trap questions
   - Customer quotes

3. Format for sales team use

## Output Format
```markdown
# Competitive Battlecard: [Competitor Name]

## Quick Facts
| Aspect | Us | [Competitor] |
|--------|-----|--------------|
| Pricing | $ | $ |
| Target Market | X | Y |
| Key Differentiator | X | Y |

## Their Strengths
- [Strength 1] - How to counter: [Counter]
- [Strength 2] - How to counter: [Counter]

## Their Weaknesses
- [Weakness 1] - How to exploit: [Approach]
- [Weakness 2] - How to exploit: [Approach]

## Our Advantages
- [Advantage 1] - Proof point: [Evidence]
- [Advantage 2] - Proof point: [Evidence]

## When We Win
- [Scenario 1]
- [Scenario 2]

## When We Lose
- [Scenario 1] - Mitigation: [Approach]
- [Scenario 2] - Mitigation: [Approach]

## Trap Questions
Ask these to expose their weaknesses:
1. "[Question 1]"
2. "[Question 2]"
3. "[Question 3]"

## Objection Handling

**"[Competitor] is cheaper"**
> [Response script]

**"[Competitor] has [feature]"**
> [Response script]

## Customer Quotes
> "[Quote from customer who switched]" - [Customer Name], [Company]
```
