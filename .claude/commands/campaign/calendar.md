---
description: Generate content calendar for campaign
argument-hint: [timeframe]
---

# Content Calendar Generation

## Objective
Generate a comprehensive content calendar for the specified timeframe.

## Workflow

1. **Phase Mapping**
   - Align campaign phases with dates
   - Identify key milestones
   - Map dependencies

2. **Content Assignment**
   - Assign content types per channel
   - Map content to audience segments
   - Balance content mix

3. **Publishing Schedule**
   - Set optimal posting frequencies
   - Define publishing times per platform
   - Schedule content bursts for launches

4. **Event Alignment**
   - Integrate industry events
   - Include seasonal opportunities
   - Add company milestones

5. **Workflow Integration**
   - Set review/approval deadlines
   - Define handoff points
   - Create production milestones

## Output Format
```markdown
| Date | Channel | Content Type | Topic | CTA | Owner | Status |
|------|---------|--------------|-------|-----|-------|--------|
```

## Output
- Content calendar in Markdown/CSV format
- Saved to `./plans/calendars/`

## Agents
Primary: `project-manager`

$ARGUMENTS
