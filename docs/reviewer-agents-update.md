# Reviewer Agents Update Summary

**Date:** 2025-12-14
**Status:** ✅ Complete

## What Was Updated

All 6 persona reviewer agents from the cc4.marketing integration have been updated to match the aitykit-marketing agent format.

### Updated Agents

**Specialist Reviewers:**
1. **brand-voice-guardian.md** - Brand consistency and voice validation
2. **conversion-optimizer.md** - Conversion rate optimization
3. **seo-specialist.md** - Search engine optimization

**Persona Reviewers:**
4. **manager-maria.md** - Marketing manager perspective (38yo, mid-size company)
5. **solo-steve.md** - Solopreneur perspective (32yo, freelance consultant)
6. **startup-sam.md** - Startup founder perspective (28yo, early-stage founder)

## Format Changes

### Before (Old Format)
```markdown
# Agent Name

## Role
[Description]

## Expertise
[List]
```

### After (New Format)
```markdown
---
name: agent-name
description: One-line description. Use for [purpose]. Examples: <example>...</example>
model: sonnet
---

You are [Agent Name], a [role] with [expertise]. Your role is to [mission].

**IMPORTANT**: [Key instructions]

## Your Expertise
[Detailed skills and knowledge]

## Review Criteria
[Structured evaluation framework]

## Review Process
[Step-by-step process]

## Output Format
[Structured output template]

## Example Review
[Concrete example]

## When to Use This Agent
[Integration points and use cases]

## Success Criteria
[What constitutes a passing review]
```

## Key Improvements

### 1. YAML Frontmatter
- **name**: Agent identifier for Claude Code integration
- **description**: Inline with use case examples for better discovery
- **model**: Specifies which Claude model to use (sonnet)

### 2. Enhanced Structure
- Clear "You are..." introduction establishing agent identity
- **IMPORTANT** callouts for critical instructions
- Structured review frameworks with rating systems
- Concrete output templates for consistency
- Real-world examples demonstrating each agent's approach

### 3. Integration Points
- Clear guidance on when to use each agent
- Slash command integration examples
- Workflow integration suggestions
- Success criteria for validation

### 4. Persona Depth

**Marketing Manager:**
- 38yo Marketing Director at mid-size company
- Manages 5-person team with $500K budget
- Focus: Team execution, ROI, scalability, enterprise needs

**Solopreneur:**
- 32yo freelance marketing consultant
- One-person business, $120K/year revenue
- Focus: Time efficiency, affordability, DIY implementation

**Startup Founder:**
- 28yo founder, pre-seed/seed stage
- 30 customers, $15K MRR, 14 months runway
- Focus: Growth velocity, scrappy execution, founder-led marketing

## How to Use

### Specialist Reviewers

**Brand Voice Guardian:**
```bash
# After creating content
/content:good "blog post topic"
# Then review with Brand Voice Guardian for consistency
```

**Conversion Optimizer:**
```bash
# For landing pages
/content:landing "offer" "audience"
# Optimize with Conversion Optimizer for CRO
```

**SEO Specialist:**
```bash
# For blog content
/content:blog "topic" "keyword"
# Review with SEO Specialist for search optimization
```

### Persona Reviewers

**Use in multi-perspective reviews:**
1. Create marketing content
2. Review with specialist (Brand, CRO, SEO)
3. Get persona feedback (Marketing Manager, Solopreneur, Startup Founder)
4. Iterate based on target audience perspective

**Example Workflow:**
```
1. Create campaign plan
2. Brand Voice Guardian → ensure consistency
3. Marketing Manager → validate team execution
4. Startup Founder → check scrappy feasibility
5. Iterate and finalize
```

## Benefits

### 1. Consistent Format
- All agents follow same structure
- Easier to understand and use
- Better integration with Claude Code

### 2. Actionable Frameworks
- Clear review criteria with rating systems
- Structured output templates
- Step-by-step review processes

### 3. Real-World Perspectives
- Persona agents provide specific, experience-based feedback
- Not generic marketing advice
- Practical constraints and considerations

### 4. Better Discovery
- Examples in agent descriptions
- Clear use cases and integration points
- When/why to use each agent

## File Locations

**Reviewer Agents:**
`.claude/agents/`
- brand-voice-guardian.md
- conversion-optimizer.md
- seo-specialist.md
- manager-maria.md
- solo-steve.md
- startup-sam.md

**Plugin Agents (Original Location):**
`plugins/campaign-manager/agents/`
- Contains original versions for reference

## Migration Notes

### What Changed
- Format: Markdown → YAML frontmatter + Markdown
- Structure: Simple sections → Comprehensive frameworks
- Examples: Generic → Concrete with templates
- Integration: Implicit → Explicit with commands

### What Stayed the Same
- Agent expertise and knowledge
- Core review criteria
- Persona characteristics and backgrounds
- Review philosophy and approach

### Removed Files
- Old files with `-reviewer.md` suffix removed
- New files use clean names (e.g., `manager-maria.md`)

## Usage Examples

### Multi-Perspective Content Review

```
Step 1: Create Content
/content:landing "Free Trial Offer" "Marketing Directors"

Step 2: Specialist Reviews
- Brand Voice Guardian → Tone and messaging
- Conversion Optimizer → CTA and persuasion
- SEO Specialist → Keywords and structure

Step 3: Persona Validation
- Marketing Manager → "Would I approve this for my team?"
- Solopreneur → "Can I implement this alone?"
- Startup Founder → "Will this drive growth fast?"

Step 4: Iterate
- Address concerns from each perspective
- Balance enterprise vs. solo vs. startup needs
- Finalize with comprehensive validation
```

### Campaign Planning Review

```
Step 1: Create Plan
/campaign:plan "Q1 Product Launch"

Step 2: Get Perspectives
- Marketing Manager → Team execution feasibility
- Startup Founder → Growth velocity potential
- Solopreneur → Resource constraints

Step 3: Adapt Plan
- Simplify for Solopreneur's one-person reality
- Scale up for Marketing Manager's team
- Add growth hacks for Startup Founder
- Provide multiple implementation paths
```

## Best Practices

### When to Use Specialist Reviewers
- **Brand Voice Guardian**: All external content before publication
- **Conversion Optimizer**: Landing pages, emails, ads, CTAs
- **SEO Specialist**: Blog posts, website pages, content marketing

### When to Use Persona Reviewers
- **Marketing Manager**: B2B mid-market content, team collaboration topics
- **Solopreneur**: Solopreneur content, DIY strategies, budget-conscious campaigns
- **Startup Founder**: Growth marketing, founder-led content, scrappy tactics

### Review Sequence
1. **Create content** with main agents (copywriter, planner, etc.)
2. **Specialist review** for technical optimization
3. **Persona feedback** for target audience validation
4. **Iterate** based on combined insights

## Integration with Existing Workflows

### Content Creation
```
Create → Brand Voice → CRO → SEO → Persona → Finalize
```

### Campaign Planning
```
Plan → Marketing Manager (feasibility) → Startup Founder (growth) → Execute
```

### Landing Page Optimization
```
Create → CRO Review → Brand Review → A/B Test → Launch
```

## Success Metrics

**Agent adoption:**
- All reviewers available in `.claude/agents/`
- Consistent format across all 6 agents
- Clear integration points with existing commands

**Quality improvements:**
- Structured review frameworks
- Actionable output templates
- Concrete examples for each agent

**Usability:**
- Easy to discover when to use each agent
- Clear guidance on integration
- Multi-perspective review workflows

---

## Next Steps

1. ✅ Reviewer agents updated
2. ✅ Old files cleaned up
3. Test agents with real content
4. Add to documentation (usage-guide.md)
5. Create workflow examples
6. Train team on multi-perspective reviews

---

**Update complete!** All 6 reviewer agents now match aitykit-marketing format with enhanced frameworks, clear integration points, and actionable review templates. 🎉
