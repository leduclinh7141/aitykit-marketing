---
description: Calculate lead score with demographic and behavioral factors
argument-hint: [lead-data]
---

Activate `crm-workflow.md` and `marketing-fundamentals` skill.

## Mission
Calculate comprehensive lead score for:
<lead>$ARGUMENTS</lead>

## Workflow

1. Use `lead-qualifier` agent to analyze:

   **Demographic Score (0-50):**
   - Job title level
   - Company size
   - Industry fit
   - Geographic location

   **Behavioral Score (0-50):**
   - Website visits
   - Content downloads
   - Email engagement
   - Event attendance

2. Apply scoring model from `crm-workflow.md`

3. Determine segment and recommended action

## Output Format
```markdown
# Lead Score: [Contact Name]

## Total Score: [X]/100

### Demographic Score: [X]/50
| Factor | Value | Points |
|--------|-------|--------|
| Job Title | [Title] | X/20 |
| Company Size | [Size] | X/15 |
| Industry | [Industry] | X/10 |
| Location | [Location] | X/5 |

### Behavioral Score: [X]/50
| Action | Details | Points |
|--------|---------|--------|
| Page Visits | [Count] | X/10 |
| Content Downloads | [List] | X/15 |
| Email Engagement | [Rate] | X/10 |
| Recent Activity | [Days] | X/15 |

## Lead Temperature
[🔥 Hot / 🌡️ Warm / ❄️ Cool / 🧊 Cold]

## Recommended Action
[Specific next step]

## Segment Assignment
[Segment name and nurture track]
```
