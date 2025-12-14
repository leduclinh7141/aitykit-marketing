---
description: Design lead scoring model
argument-hint: [business-context]
---

## Language & Quality Standards

**CRITICAL**: Respond in the same language the user is using. If Vietnamese, respond in Vietnamese. If Spanish, respond in Spanish.

**Standards**: Token efficiency, sacrifice grammar for concision, list unresolved questions at end.

---

# Lead Scoring Model Design

## Objective
Design a comprehensive lead scoring model tailored to your business.

## Workflow

1. **Identify Scoring Signals**
   - Website behavior signals
   - Email engagement signals
   - Content consumption patterns
   - Social engagement
   - Direct interactions

2. **Weight Behavioral Factors**
   - Page visits (which pages, frequency)
   - Content downloads
   - Form submissions
   - Email interactions
   - Trial/demo activity

3. **Weight Demographic Factors**
   - Job title/role
   - Company size
   - Industry fit
   - Geographic location
   - Tech stack fit

4. **Define Score Thresholds**
   - Cold lead (0-20)
   - Warm lead (21-50)
   - MQL (51-75)
   - SQL (76-100)

5. **Map Scores to Actions**
   - Score triggers for nurture
   - Score triggers for outreach
   - Score alerts for sales
   - Re-engagement triggers

## Output Format
```markdown
| Signal | Category | Points | Trigger |
|--------|----------|--------|---------|
| Pricing page visit | Behavioral | +15 | Intent |
| Demo request | Behavioral | +30 | High intent |
| Director+ title | Demographic | +10 | Authority |
```

## Output
- Complete scoring model documentation
- Implementation specifications

## Agents
Primary: `lead-qualifier`

$ARGUMENTS
