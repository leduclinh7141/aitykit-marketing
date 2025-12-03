---
description: Manage contact lifecycle stage transitions
argument-hint: [contact-or-segment] [action]
---

Activate `crm-workflow.md` skill.

## Mission
Manage lifecycle stage for:
<context>$ARGUMENTS</context>

## Lifecycle Stages
```
Subscriber → Lead → MQL → SQL → Opportunity → Customer → Advocate
```

## Workflow

1. Identify current stage and transition criteria
2. Use `lead-qualifier` agent to validate transition:
   - Score thresholds met
   - Required actions completed
   - Time requirements satisfied

3. Define automation triggers and actions

## Output Format
```markdown
# Lifecycle Management: [Contact/Segment]

## Current State
- **Stage:** [Current stage]
- **Time in stage:** [Duration]
- **Score:** [Current score]

## Stage Transition Analysis

### Criteria for Next Stage ([Next Stage Name])
| Requirement | Status | Gap |
|-------------|--------|-----|
| [Criteria 1] | ✅/❌ | [What's needed] |
| [Criteria 2] | ✅/❌ | [What's needed] |
| [Criteria 3] | ✅/❌ | [What's needed] |

### Readiness Score: [X]%

## Recommended Actions

### To Progress to [Next Stage]:
1. [Action 1] - [Expected impact]
2. [Action 2] - [Expected impact]
3. [Action 3] - [Expected impact]

### Automation Triggers to Set:
- **When:** [Trigger condition]
- **Then:** [Automated action]

## Stage-Specific Playbook

### [Current Stage] Best Practices:
- [Practice 1]
- [Practice 2]
- [Practice 3]

### Content to Deliver:
- [Content 1] - [Purpose]
- [Content 2] - [Purpose]

### Touchpoint Cadence:
- Email: [Frequency]
- Phone: [Frequency]
- Social: [Frequency]
```
