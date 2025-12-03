---
description: Create or analyze customer segment
argument-hint: [segment-criteria-or-name]
---

Activate `crm-workflow.md` skill.

## Mission
Create or analyze customer segment:
<segment>$ARGUMENTS</segment>

## Workflow

1. Use `lead-qualifier` agent to define segment:
   - Demographic criteria
   - Behavioral criteria
   - Engagement criteria
   - Lifecycle stage

2. Analyze segment characteristics:
   - Size estimation
   - Value potential
   - Engagement patterns
   - Conversion likelihood

3. Recommend segment strategy

## Output Format
```markdown
# Segment: [Segment Name]

## Definition
**Description:** [What this segment represents]

### Inclusion Criteria
| Type | Criteria | Value |
|------|----------|-------|
| Demographic | [Field] | [Condition] |
| Behavioral | [Action] | [Threshold] |
| Engagement | [Metric] | [Threshold] |
| Lifecycle | [Stage] | [Value] |

### Exclusion Criteria
- [Exclusion 1]
- [Exclusion 2]

## Segment Analysis

### Size & Value
- Estimated contacts: [Number]
- Avg. lead score: [Score]
- Revenue potential: [Estimate]

### Engagement Profile
- Avg. email open rate: [%]
- Avg. click rate: [%]
- Most engaged content: [Type]
- Peak engagement time: [Day/Time]

### Conversion Patterns
- Avg. time to conversion: [Days]
- Top conversion paths: [List]
- Common drop-off points: [List]

## Recommended Strategy

### Content Focus
- [Content type 1]
- [Content type 2]

### Channel Priority
1. [Channel 1] - [Reason]
2. [Channel 2] - [Reason]

### Automation Sequence
[Recommended sequence name]

### Personalization Approach
- [Personalization 1]
- [Personalization 2]
```
